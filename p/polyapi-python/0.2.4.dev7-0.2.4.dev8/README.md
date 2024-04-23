# Comparing `tmp/polyapi_python-0.2.4.dev7.tar.gz` & `tmp/polyapi_python-0.2.4.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.4.dev7.tar", last modified: Mon Apr 22 19:33:55 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.4.dev8.tar", last modified: Tue Apr 23 16:41:14 2024, max compression
```

## Comparing `polyapi_python-0.2.4.dev7.tar` & `polyapi_python-0.2.4.dev8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:33:55.943737 polyapi_python-0.2.4.dev7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-22 19:33:55.943737 polyapi_python-0.2.4.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:33:55.939737 polyapi_python-0.2.4.dev7/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/poly_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:33:55.943737 polyapi_python-0.2.4.dev7/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-22 19:33:55.000000 polyapi_python-0.2.4.dev7/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-22 19:33:55.000000 polyapi_python-0.2.4.dev7/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:33:55.000000 polyapi_python-0.2.4.dev7/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-22 19:33:55.000000 polyapi_python-0.2.4.dev7/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 19:33:55.000000 polyapi_python-0.2.4.dev7/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:33:55.943737 polyapi_python-0.2.4.dev7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:33:55.943737 polyapi_python-0.2.4.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-22 19:33:52.000000 polyapi_python-0.2.4.dev7/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/poly_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.4.dev7/LICENSE` & `polyapi_python-0.2.4.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/PKG-INFO` & `polyapi_python-0.2.4.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev7
+Version: 0.2.4.dev8
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.4.dev7/README.md` & `polyapi_python-0.2.4.dev8/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/api.py` & `polyapi_python-0.2.4.dev8/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/auth.py` & `polyapi_python-0.2.4.dev8/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/cli.py` & `polyapi_python-0.2.4.dev8/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/client.py` & `polyapi_python-0.2.4.dev8/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/config.py` & `polyapi_python-0.2.4.dev8/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/error_handler.py` & `polyapi_python-0.2.4.dev8/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/execute.py` & `polyapi_python-0.2.4.dev8/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/function_cli.py` & `polyapi_python-0.2.4.dev8/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/generate.py` & `polyapi_python-0.2.4.dev8/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/schema.py` & `polyapi_python-0.2.4.dev8/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/server.py` & `polyapi_python-0.2.4.dev8/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/typedefs.py` & `polyapi_python-0.2.4.dev8/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/utils.py` & `polyapi_python-0.2.4.dev8/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/variables.py` & `polyapi_python-0.2.4.dev8/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/polyapi/webhook.py` & `polyapi_python-0.2.4.dev8/polyapi/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     _, base_url = get_api_key_and_url()
     global client
     client = socketio.AsyncClient()
     await client.connect(base_url, transports=["websocket"], namespaces=["/events"])
 
 
 async def unregister(data: Dict[str, Any]):
-    print(f"stopping error handler for '{data['webhookHandleID']}'...")
+    print(f"stopping webhook handler for '{data['webhookHandleID']}'...")
     assert client
     await client.emit(
         "unregisterWebhookEventHandler",
         {
             "clientID": data["clientID"],
             "webhookHandleID": data["webhookHandleID"],
             "apiKey": data["apiKey"],
```

### Comparing `polyapi_python-0.2.4.dev7/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.4.dev8/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev7
+Version: 0.2.4.dev8
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.4.dev7/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.4.dev8/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/pyproject.toml` & `polyapi_python-0.2.4.dev8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.4.dev7"
+version = "0.2.4.dev8"
 description = "The Python Client for PolyAPI, the IPaaS by Developers for Developers"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.4.dev7/tests/test_api.py` & `polyapi_python-0.2.4.dev8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/tests/test_auth.py` & `polyapi_python-0.2.4.dev8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/tests/test_function_cli.py` & `polyapi_python-0.2.4.dev8/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/tests/test_server.py` & `polyapi_python-0.2.4.dev8/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/tests/test_utils.py` & `polyapi_python-0.2.4.dev8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev7/tests/test_variables.py` & `polyapi_python-0.2.4.dev8/tests/test_variables.py`

 * *Files identical despite different names*

