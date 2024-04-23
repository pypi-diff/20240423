# Comparing `tmp/whitecloak-0.3.1.tar.gz` & `tmp/whitecloak-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitecloak-0.3.1.tar", max compression
+gzip compressed data, was "whitecloak-0.4.1.tar", max compression
```

## Comparing `whitecloak-0.3.1.tar` & `whitecloak-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       16 2024-04-19 00:23:31.429374 whitecloak-0.3.1/README.md
--rw-r--r--   0        0        0      500 2024-04-22 21:55:17.523153 whitecloak-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 00:18:15.153562 whitecloak-0.3.1/whitecloak/__init__.py
--rw-r--r--   0        0        0       51 2024-04-19 00:30:27.087597 whitecloak-0.3.1/whitecloak/__main__.py
--rw-r--r--   0        0        0     4971 2024-04-22 21:54:10.191344 whitecloak-0.3.1/whitecloak/main.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 whitecloak-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-19 00:23:31.429374 whitecloak-0.4.1/README.md
+-rw-r--r--   0        0        0      500 2024-04-22 22:08:52.188734 whitecloak-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 00:18:15.153562 whitecloak-0.4.1/whitecloak/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-19 00:30:27.087597 whitecloak-0.4.1/whitecloak/__main__.py
+-rw-r--r--   0        0        0     5105 2024-04-22 22:08:33.256022 whitecloak-0.4.1/whitecloak/main.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 whitecloak-0.4.1/PKG-INFO
```

### Comparing `whitecloak-0.3.1/whitecloak/main.py` & `whitecloak-0.4.1/whitecloak/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,18 +64,24 @@
 
 class Plugin(BaseModel):
     input_schema: dict[str, T.Any]
     execute_url: str
 
 
 class StepsInput(BaseModel):
+    version: str
     steps: list[Step]
     plugins: dict[str, Plugin]
 
 
+class StepsResponse(BaseModel):
+    version: str
+    runs: list[StepRun]
+
+
 @app.command()
 def run(
     *,
     json_file: T.Annotated[
         T.Optional[str], typer.Option(help="Path to the JSON file to run.")
     ] = None,
     json_string: T.Annotated[
@@ -158,16 +164,16 @@
             json.dumps(_run.execute_response.body)[0:output_length],
         )
     console.print(table)
     path = Path(output_file)
     if not path.exists():
         # do this check just in case you do not have filesystem directory write access
         path.parent.mkdir(parents=True, exist_ok=True)
-    v = TypeAdapter(list[StepRun]).dump_json(runs)
-    path.write_bytes(v)
+    response = StepsResponse(version=steps_input.version, runs=runs)
+    path.write_text(response.model_dump_json())
 
 
 @app.command()
 def hi():
     console.print("hi")
```

### Comparing `whitecloak-0.3.1/PKG-INFO` & `whitecloak-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitecloak
-Version: 0.3.1
+Version: 0.4.1
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

