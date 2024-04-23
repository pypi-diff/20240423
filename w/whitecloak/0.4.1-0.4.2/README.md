# Comparing `tmp/whitecloak-0.4.1.tar.gz` & `tmp/whitecloak-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitecloak-0.4.1.tar", max compression
+gzip compressed data, was "whitecloak-0.4.2.tar", max compression
```

## Comparing `whitecloak-0.4.1.tar` & `whitecloak-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       16 2024-04-19 00:23:31.429374 whitecloak-0.4.1/README.md
--rw-r--r--   0        0        0      500 2024-04-22 22:08:52.188734 whitecloak-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 00:18:15.153562 whitecloak-0.4.1/whitecloak/__init__.py
--rw-r--r--   0        0        0       51 2024-04-19 00:30:27.087597 whitecloak-0.4.1/whitecloak/__main__.py
--rw-r--r--   0        0        0     5105 2024-04-22 22:08:33.256022 whitecloak-0.4.1/whitecloak/main.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 whitecloak-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-19 00:23:31.429374 whitecloak-0.4.2/README.md
+-rw-r--r--   0        0        0      500 2024-04-23 14:46:24.397777 whitecloak-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 00:18:15.153562 whitecloak-0.4.2/whitecloak/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-19 00:30:27.087597 whitecloak-0.4.2/whitecloak/__main__.py
+-rw-r--r--   0        0        0     5657 2024-04-23 14:45:37.550182 whitecloak-0.4.2/whitecloak/main.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 whitecloak-0.4.2/PKG-INFO
```

### Comparing `whitecloak-0.4.1/whitecloak/main.py` & `whitecloak-0.4.2/whitecloak/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,24 +83,35 @@
     *,
     json_file: T.Annotated[
         T.Optional[str], typer.Option(help="Path to the JSON file to run.")
     ] = None,
     json_string: T.Annotated[
         T.Optional[str], typer.Option(help="JSON string to run.")
     ] = None,
-    output_file: T.Annotated[str, typer.Option(help="Path to the output file.")],
+    output_file: T.Annotated[
+        T.Optional[str], typer.Option(help="Path to the output file.")
+    ] = None,
+    return_json: T.Annotated[
+        T.Optional[bool],
+        typer.Option(
+            help="True if stdout should only print the runs. This is headless mode."
+        ),
+    ] = None,
     output_length: T.Annotated[
         T.Optional[int],
-        typer.Option(help="Number of characters to print for the output of each step."),
+        typer.Option(
+            help="Number of characters to print for the output of each step. Ignored if --return-json is given."
+        ),
     ] = 200,
 ):
     """
     Provide either a --json_file or a --json_string to run.
     Provide an optional --output-length for the length of the output of the run to display.
     """
+    is_headless = bool(return_json)
     if not json_file and not json_string:
         err_console.print(
             "[bold red]Error:[/bold red] Please provide either [green]--json_file[/green] or [green]--json_string[/green]."
         )
         return
     if json_file and json_string:
         err_console.print(
@@ -114,16 +125,19 @@
         else:
             err_console.print(
                 f"[bold red]Error:[/bold red] No file found at {json_file}"
             )
             return
     steps_input = StepsInput.model_validate_json(json_string)
     runs: list[StepRun] = []
-    for step in track(steps_input.steps, description="Running steps..."):
-        console.log(f"running step {step.id}")
+    for step in track(
+        steps_input.steps, description="Running steps...", disable=is_headless
+    ):
+        if not is_headless:
+            console.log(f"running step {step.id}")
         step_started_at_ms = time.time() * 1_000
         plugin = steps_input.plugins[step.plugin_id]
         valid_input(schema=plugin.input_schema, input=step.input)  # TODO
         run_id = f"run_{uuid.uuid4()}"
         r = httpx.post(
             url=plugin.execute_url,
             json=step.input,
@@ -159,21 +173,26 @@
     for _run in runs:
         table.add_row(
             _run.id,
             _run.step_id,
             str(round(_run.execute_duration_ms, 2)),
             json.dumps(_run.execute_response.body)[0:output_length],
         )
-    console.print(table)
-    path = Path(output_file)
-    if not path.exists():
-        # do this check just in case you do not have filesystem directory write access
-        path.parent.mkdir(parents=True, exist_ok=True)
+    if not is_headless:
+        console.print(table)
     response = StepsResponse(version=steps_input.version, runs=runs)
-    path.write_text(response.model_dump_json())
+    response_json = response.model_dump_json()
+    if output_file is not None:
+        path = Path(output_file)
+        if not path.exists():
+            # do this check just in case you do not have filesystem directory write access
+            path.parent.mkdir(parents=True, exist_ok=True)
+        path.write_text(response_json)
+    if is_headless:
+        console.print(response_json)
 
 
 @app.command()
 def hi():
     console.print("hi")
```

### Comparing `whitecloak-0.4.1/PKG-INFO` & `whitecloak-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitecloak
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

