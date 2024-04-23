# Comparing `tmp/waylay-sdk-data-2.14.0rc1.tar.gz` & `tmp/waylay-sdk-data-2.14.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-sdk-data-2.14.0rc1.tar", last modified: Tue Mar 26 16:19:48 2024, max compression
+gzip compressed data, was "waylay-sdk-data-2.14.0rc2.tar", last modified: Wed Mar 27 14:43:26 2024, max compression
```

## Comparing `waylay-sdk-data-2.14.0rc1.tar` & `waylay-sdk-data-2.14.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.087920 waylay-sdk-data-2.14.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-03-26 16:19:48.087920 waylay-sdk-data-2.14.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:19:48.087920 waylay-sdk-data-2.14.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.083920 waylay-sdk-data-2.14.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.079920 waylay-sdk-data-2.14.0rc1/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.083920 waylay-sdk-data-2.14.0rc1/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.083920 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.083920 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27790 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24532 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/messages_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    49124 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/series_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/version_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.083920 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/service/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-26 16:19:36.000000 waylay-sdk-data-2.14.0rc1/src/waylay/services/data/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:19:48.087920 waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-03-26 16:19:48.000000 waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-26 16:19:48.000000 waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:19:48.000000 waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-26 16:19:48.000000 waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-26 16:19:48.000000 waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 16:19:48.000000 waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.940952 waylay-sdk-data-2.14.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-27 14:43:26.940952 waylay-sdk-data-2.14.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 14:43:26.940952 waylay-sdk-data-2.14.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.932952 waylay-sdk-data-2.14.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.932952 waylay-sdk-data-2.14.0rc2/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.932952 waylay-sdk-data-2.14.0rc2/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.932952 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.936951 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27770 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24512 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/messages_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    49089 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/series_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.936951 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-27 14:43:21.000000 waylay-sdk-data-2.14.0rc2/src/waylay/services/data/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:43:26.936951 waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-27 14:43:26.000000 waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-27 14:43:26.000000 waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:43:26.000000 waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 14:43:26.000000 waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-27 14:43:26.000000 waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 14:43:26.000000 waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/top_level.txt
```

### Comparing `waylay-sdk-data-2.14.0rc1/LICENSE.txt` & `waylay-sdk-data-2.14.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-2.14.0rc1/PKG-INFO` & `waylay-sdk-data-2.14.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-data
-Version: 2.14.0rc1
+Version: 2.14.0rc2
 Summary: Waylay Broker
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -12,20 +12,23 @@
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Project-URL: Homepage, https://www.waylay.io/
+Project-URL: Documentation, https://docs.waylay.io/#/
+Project-URL: Repository, https://github.com/waylayio/waylay-sdk-data-py.git
 Keywords: Waylay Broker
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk~=0.0.4rc4
-Requires-Dist: waylay-sdk-data==2.14.0rc1
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-data==2.14.0rc2
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay-sdk-data-2.14.0rc1/README.md` & `waylay-sdk-data-2.14.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-2.14.0rc1/pyproject.toml` & `waylay-sdk-data-2.14.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-data"
-version = "2.14.0rc1"
+version = "2.14.0rc2"
 description = "Waylay Broker"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Broker"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk ~= 0.0.4rc4",
-    "waylay-sdk-data == 2.14.0rc1",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-data == 2.14.0rc2",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
+[project.urls]
+Homepage = "https://www.waylay.io/"
+Documentation = "https://docs.waylay.io/#/"
+Repository = "https://github.com/waylayio/waylay-sdk-data-py.git"
+
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
     "types-python-dateutil",
@@ -53,17 +58,18 @@
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
 # allow duplicate imports
 ignore=["F811"]
 # https://docs.astral.sh/ruff/rules
 select= [
-    "UP007", "FA102", "I001",  # convert Union to | (pep-604)
-    "F401", "E303",  # remove unused imports
+    "UP007", "FA102",  # convert Union to | (pep-604)
+    "I001", "F401",  # sort and remove unused imports
     "PIE790",  # remove unnecessary pass statements
+    "E303",  # too many blank lines
 ]
 
 [tool.ruff.lint.per-file-ignores]
 # do not touch imports here
 "__init__.py" = ["F401"]
 "conftest.py" = ["F401"]
```

### Comparing `waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/events_api.py` & `waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/events_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             method="POST",
             resource_path="/data/v1/events",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def post_series_for_resource(
         self,
@@ -437,15 +437,15 @@
             method="POST",
             resource_path="/data/v1/events/{resourceId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def remove(
         self,
@@ -602,15 +602,15 @@
             method="DELETE",
             resource_path="/data/v1/{resourceId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def stream_events(
         self,
@@ -761,11 +761,11 @@
             method="GET",
             resource_path="/data/v1/events/{resourceId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
```

### Comparing `waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/messages_api.py` & `waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/messages_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             method="DELETE",
             resource_path="/data/v1/messages/{resourceId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get_latest_document(
         self,
@@ -412,15 +412,15 @@
             method="GET",
             resource_path="/data/v1/messages/{resourceId}/current",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get_latest_messages(
         self,
@@ -569,15 +569,15 @@
             method="GET",
             resource_path="/data/v1/messages/{resourceId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def query_messages(
         self,
@@ -718,11 +718,11 @@
             method="POST",
             resource_path="/data/v1/messages/query",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
```

### Comparing `waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/series_api.py` & `waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/series_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
             method="DELETE",
             resource_path="/data/v1/series/{resourceId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get_datapoints_for_metric_raw(
         self,
@@ -473,15 +473,15 @@
             method="GET",
             resource_path="/data/v1/series/{resourceId}/{metric}/raw",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get_last_datapoints_for_metric(
         self,
@@ -657,15 +657,15 @@
             method="GET",
             resource_path="/data/v1/series/{resourceId}/{metric}/last",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get_last_metric(
         self,
@@ -837,15 +837,15 @@
             method="GET",
             resource_path="/data/v1/series/{resourceId}/{metric}/latest",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get_metric_series(
         self,
@@ -1029,15 +1029,15 @@
             method="GET",
             resource_path="/data/v1/series/{resourceId}/{metric}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get_series(
         self,
@@ -1186,15 +1186,15 @@
             method="GET",
             resource_path="/data/v1/series/{resourceId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def query_time_series(
         self,
@@ -1335,11 +1335,11 @@
             method="POST",
             resource_path="/data/v1/series/query",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
```

### Comparing `waylay-sdk-data-2.14.0rc1/src/waylay/services/data/api/version_api.py` & `waylay-sdk-data-2.14.0rc2/src/waylay/services/data/api/version_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,11 +187,11 @@
             method="GET",
             resource_path="/data/v1/",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
-            response_types_map=response_types_map,
+            response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
```

### Comparing `waylay-sdk-data-2.14.0rc1/src/waylay/services/data/service/service.py` & `waylay-sdk-data-2.14.0rc2/src/waylay/services/data/service/service.py`

 * *Files identical despite different names*

### Comparing `waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/PKG-INFO` & `waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-data
-Version: 2.14.0rc1
+Version: 2.14.0rc2
 Summary: Waylay Broker
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -12,20 +12,23 @@
         
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Project-URL: Homepage, https://www.waylay.io/
+Project-URL: Documentation, https://docs.waylay.io/#/
+Project-URL: Repository, https://github.com/waylayio/waylay-sdk-data-py.git
 Keywords: Waylay Broker
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk~=0.0.4rc4
-Requires-Dist: waylay-sdk-data==2.14.0rc1
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-data==2.14.0rc2
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay-sdk-data-2.14.0rc1/src/waylay_sdk_data.egg-info/SOURCES.txt` & `waylay-sdk-data-2.14.0rc2/src/waylay_sdk_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

