# Comparing `tmp/sprocketship-0.6.0.tar.gz` & `tmp/sprocketship-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.6.0.tar", last modified: Tue Apr  9 13:38:42 2024, max compression
+gzip compressed data, was "sprocketship-1.0.0.tar", last modified: Tue Apr 23 03:20:35 2024, max compression
```

## Comparing `sprocketship-0.6.0.tar` & `sprocketship-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:38:42.095734 sprocketship-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 13:38:37.000000 sprocketship-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 13:38:37.000000 sprocketship-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-09 13:38:42.091734 sprocketship-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-09 13:38:37.000000 sprocketship-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 13:38:37.000000 sprocketship-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:38:42.095734 sprocketship-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:38:42.091734 sprocketship-0.6.0/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-09 13:38:37.000000 sprocketship-0.6.0/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:38:42.091734 sprocketship-0.6.0/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 13:38:37.000000 sprocketship-0.6.0/sprocketship/templates/javascript.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 13:38:37.000000 sprocketship-0.6.0/sprocketship/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:38:42.091734 sprocketship-0.6.0/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-09 13:38:42.000000 sprocketship-0.6.0/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-09 13:38:42.000000 sprocketship-0.6.0/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:38:42.000000 sprocketship-0.6.0/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 13:38:42.000000 sprocketship-0.6.0/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 13:38:42.000000 sprocketship-0.6.0/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:38:42.000000 sprocketship-0.6.0/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.280539 sprocketship-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 03:20:31.000000 sprocketship-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 03:20:31.000000 sprocketship-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-23 03:20:35.280539 sprocketship-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-23 03:20:31.000000 sprocketship-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-23 03:20:31.000000 sprocketship-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:20:35.280539 sprocketship-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.276539 sprocketship-1.0.0/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-23 03:20:31.000000 sprocketship-1.0.0/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.280539 sprocketship-1.0.0/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 03:20:31.000000 sprocketship-1.0.0/sprocketship/templates/javascript.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-23 03:20:31.000000 sprocketship-1.0.0/sprocketship/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.280539 sprocketship-1.0.0/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.6.0/LICENSE` & `sprocketship-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.6.0/PKG-INFO` & `sprocketship-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.6.0
+Version: 1.0.0
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.6.0 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.0 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
```

### Comparing `sprocketship-0.6.0/README.md` & `sprocketship-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.6.0/pyproject.toml` & `sprocketship-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.6.0"
+version = "1.0.0"
 authors = [
   { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-0.6.0/sprocketship/utils.py` & `sprocketship-1.0.0/sprocketship/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,34 +12,58 @@
             for item in value:
                 item["path"] = new_path
         elif isinstance(value, dict):
             configs.update(extract_configs(value, new_path))
     return configs
 
 
+def get_file_config(path: Path, config: dict, dir: str):
+    filename = path.stem
+    keys = str(path.relative_to(dir)).split("/")[:-1] + [filename]
+
+    file_config = {"path": str(path), "name": filename}
+    curr_config = config
+    for key in keys:
+        file_config.update(
+            {k[1:]: v for k, v in curr_config.items() if k.startswith("+")}
+        )
+        if key in curr_config:
+            curr_config = curr_config[key]
+        else:
+            return file_config
+    file_config.update(curr_config)
+    return file_config
+
+
 def get_full_file_path(proc_config):
     extension_map = {"javascript": ".js", "python": ".py"}
     file_name = proc_config["name"] + extension_map[proc_config["language"]]
     return os.path.join("procedures", proc_config["path"], file_name)
 
 
-def get_file_contents(fpath):
-    with open(fpath, "r") as file:
-        return file.read()
+def get_file_contents(fpath, extra_context):
+    return render_file(fpath, return_dict=True, extra_context=extra_context)
 
 
 def create_javascript_stored_procedure(**kwargs):
-    path = os.path.join(kwargs["project_dir"], get_full_file_path(kwargs))
-    procedure_def_dict = {"procedure_definition": get_file_contents(path)}
-    return render_file(
-        os.path.join(Path(__file__).parent, "templates/javascript.sql"),
-        **kwargs,
-        **procedure_def_dict,
+    # Render the javascript file
+    file_contents = render_file(kwargs["path"], return_dict=True)
+    procedure_def_dict = {"procedure_definition": file_contents["absql_body"]}
+
+    context = kwargs
+    context.update(file_contents)
+    context.update(procedure_def_dict)
+
+    # Render the stored procedure template with the procedure definition
+    rendered_file = render_file(
+        os.path.join(Path(__file__).parent, "templates/javascript.sql"), **context
     )
+    return {**kwargs, "rendered_file": rendered_file}
+
 
 def grant_usage(proc, con):
-    types = [arg['type'] for arg in proc['args']]
+    types = [arg["type"] for arg in proc["args"]]
     types_str = f"({','.join(types)})"
-    for grantee_type in proc['grant_usage']:
-        for grantee in proc['grant_usage'][grantee_type]:
+    for grantee_type in proc["grant_usage"]:
+        for grantee in proc["grant_usage"][grantee_type]:
             query = f"GRANT USAGE ON PROCEDURE {proc['database']}.{proc['schema']}.{proc['name']}{types_str} TO {grantee_type} {grantee}"
             con.cursor().execute(query)
```

### Comparing `sprocketship-0.6.0/sprocketship.egg-info/PKG-INFO` & `sprocketship-1.0.0/sprocketship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.6.0
+Version: 1.0.0
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.6.0 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.0 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
```

