# Comparing `tmp/whitecloak-0.2.1.tar.gz` & `tmp/whitecloak-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitecloak-0.2.1.tar", max compression
+gzip compressed data, was "whitecloak-0.3.1.tar", max compression
```

## Comparing `whitecloak-0.2.1.tar` & `whitecloak-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       16 2024-04-19 00:23:31.429374 whitecloak-0.2.1/README.md
--rw-r--r--   0        0        0      500 2024-04-22 21:13:49.927979 whitecloak-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 00:18:15.153562 whitecloak-0.2.1/whitecloak/__init__.py
--rw-r--r--   0        0        0       51 2024-04-19 00:30:27.087597 whitecloak-0.2.1/whitecloak/__main__.py
--rw-r--r--   0        0        0     4870 2024-04-22 21:14:04.947349 whitecloak-0.2.1/whitecloak/main.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 whitecloak-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-19 00:23:31.429374 whitecloak-0.3.1/README.md
+-rw-r--r--   0        0        0      500 2024-04-22 21:55:17.523153 whitecloak-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 00:18:15.153562 whitecloak-0.3.1/whitecloak/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-19 00:30:27.087597 whitecloak-0.3.1/whitecloak/__main__.py
+-rw-r--r--   0        0        0     4971 2024-04-22 21:54:10.191344 whitecloak-0.3.1/whitecloak/main.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 whitecloak-0.3.1/PKG-INFO
```

### Comparing `whitecloak-0.2.1/whitecloak/main.py` & `whitecloak-0.3.1/whitecloak/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 import httpx
 import typer
 from rich.console import Console
 from rich.table import Table
 from rich.progress import track
-from pydantic import BaseModel, TypeAdapter
+from pydantic import BaseModel, TypeAdapter, Field
 
 err_console = Console(stderr=True)
 console = Console()
 
 
 app = typer.Typer(no_args_is_help=True)
 
@@ -38,25 +38,30 @@
 
     error: StepResponseError | None = None
 
 
 class StepRun(BaseModel):
     id: str
     step_id: str
+    step_version: int
+    plugin_id: str
 
+    step_input: dict
     execute_response: StepResponse
     execute_duration_ms: float
 
     started_at_ms: float
     ended_at_ms: float
 
 
 class Step(BaseModel):
     id: str
-    slug: str
+    version: int = Field(ge=0)
+
+    slug: str = Field(pattern=r"^[a-zA-Z0-9-]+$")
     plugin_id: str
     input: dict[str, T.Any]
 
 
 class Plugin(BaseModel):
     input_schema: dict[str, T.Any]
     execute_url: str
@@ -95,35 +100,31 @@
         err_console.print(
             "[bold red]Error:[/bold red] Please provide either [green]--json_file[/green] or [green]--json_string[/green], not both."
         )
         return
     if json_file:
         path = Path(json_file)
         if path.exists():
-            with path.open("r") as f:
-                json_string = f.read()
+            json_string = path.read_bytes()
         else:
             err_console.print(
                 f"[bold red]Error:[/bold red] No file found at {json_file}"
             )
             return
     steps_input = StepsInput.model_validate_json(json_string)
     runs: list[StepRun] = []
     for step in track(steps_input.steps, description="Running steps..."):
         console.log(f"running step {step.id}")
         step_started_at_ms = time.time() * 1_000
-        # confirm the input types conform to the plugins inputSchema
-        input = step.input
         plugin = steps_input.plugins[step.plugin_id]
-        input_schema = plugin.input_schema
-        valid_input(schema=input_schema, input=input)
+        valid_input(schema=plugin.input_schema, input=step.input)  # TODO
         run_id = f"run_{uuid.uuid4()}"
         r = httpx.post(
             url=plugin.execute_url,
-            json=input,
+            json=step.input,
             headers={
                 "x-whitecloak-run-id": str(run_id),
                 "x-whitecloak-step-id": step.id,
             },
             timeout=60,
         )
         step_ended_at_ms = time.time() * 1_000
@@ -135,35 +136,38 @@
                 headers=None,
                 error=StepResponseError(exception_log=str(e), raw_response_text=r.text),
             )
         runs.append(
             StepRun(
                 id=run_id,
                 step_id=step.id,
+                step_version=step.version,
+                plugin_id=step.plugin_id,
+                step_input=step.input,
                 execute_response=step_response,
                 execute_duration_ms=r.elapsed.total_seconds() * 1_000,
                 started_at_ms=step_started_at_ms,
                 ended_at_ms=step_ended_at_ms,
             )
         )
     table = Table("Run Id", "Step Id", "Latency (ms)", "Result")
     for _run in runs:
         table.add_row(
-            _run.step_id,
+            _run.id,
             _run.step_id,
             str(round(_run.execute_duration_ms, 2)),
             json.dumps(_run.execute_response.body)[0:output_length],
         )
     console.print(table)
     path = Path(output_file)
     if not path.exists():
         # do this check just in case you do not have filesystem directory write access
         path.parent.mkdir(parents=True, exist_ok=True)
-        v = TypeAdapter(list[StepRun]).dump_json(runs)
-        path.write_bytes(v)
+    v = TypeAdapter(list[StepRun]).dump_json(runs)
+    path.write_bytes(v)
 
 
 @app.command()
 def hi():
     console.print("hi")
```

### Comparing `whitecloak-0.2.1/PKG-INFO` & `whitecloak-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitecloak
-Version: 0.2.1
+Version: 0.3.1
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

