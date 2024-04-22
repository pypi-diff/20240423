# Comparing `tmp/baserun-0.9.8b2.tar.gz` & `tmp/baserun-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-0.9.8b2.tar", last modified: Wed Jan 17 19:20:07 2024, max compression
+gzip compressed data, was "baserun-0.9.9.tar", last modified: Mon Jan 29 17:36:21 2024, max compression
```

## Comparing `baserun-0.9.8b2.tar` & `baserun-0.9.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-17 19:20:07.128632 baserun-0.9.8b2/
--rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-0.9.8b2/LICENSE
--rw-r--r--   0 epeterson   (501) staff       (20)     6553 2024-01-17 19:20:07.128481 baserun-0.9.8b2/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     4582 2023-12-01 13:51:58.000000 baserun-0.9.8b2/README.md
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-17 19:20:07.117122 baserun-0.9.8b2/baserun/
--rw-r--r--   0 epeterson   (501) staff       (20)     1386 2024-01-17 18:48:39.000000 baserun-0.9.8b2/baserun/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     5793 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/annotation.py
--rw-r--r--   0 epeterson   (501) staff       (20)      393 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/api_key.py
--rw-r--r--   0 epeterson   (501) staff       (20)    14980 2024-01-17 18:48:39.000000 baserun-0.9.8b2/baserun/baserun.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1469 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/checks.py
--rw-r--r--   0 epeterson   (501) staff       (20)      162 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/constants.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-17 19:20:07.120711 baserun-0.9.8b2/baserun/evals/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:37.000000 baserun-0.9.8b2/baserun/evals/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    13545 2024-01-10 22:46:42.000000 baserun-0.9.8b2/baserun/evals/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)      154 2023-12-01 13:51:37.000000 baserun-0.9.8b2/baserun/evals/json.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1162 2024-01-16 22:00:28.000000 baserun-0.9.8b2/baserun/exporter.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1375 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/grpc.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1122 2024-01-16 22:00:28.000000 baserun-0.9.8b2/baserun/helpers.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-17 19:20:07.124434 baserun-0.9.8b2/baserun/instrumentation/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/instrumentation/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1771 2024-01-16 22:00:28.000000 baserun-0.9.8b2/baserun/instrumentation/anthropic.py
--rw-r--r--   0 epeterson   (501) staff       (20)    13427 2024-01-17 18:48:43.000000 baserun-0.9.8b2/baserun/instrumentation/base_instrumentor.py
--rw-r--r--   0 epeterson   (501) staff       (20)      557 2024-01-16 22:00:28.000000 baserun-0.9.8b2/baserun/instrumentation/instrumented_wrapper.py
--rw-r--r--   0 epeterson   (501) staff       (20)     4465 2023-12-06 13:41:54.000000 baserun-0.9.8b2/baserun/instrumentation/langchain.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2964 2024-01-16 22:00:28.000000 baserun-0.9.8b2/baserun/instrumentation/openai.py
--rw-r--r--   0 epeterson   (501) staff       (20)      278 2024-01-16 22:00:28.000000 baserun-0.9.8b2/baserun/instrumentation/span_attributes.py
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/model_configs.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2116 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/pytest_plugin.py
--rw-r--r--   0 epeterson   (501) staff       (20)     5347 2024-01-16 22:00:28.000000 baserun-0.9.8b2/baserun/sessions.py
--rw-r--r--   0 epeterson   (501) staff       (20)     8565 2024-01-17 18:48:39.000000 baserun-0.9.8b2/baserun/templates.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1130 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/thread_wrapper.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1105 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/users.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-17 19:20:07.126448 baserun-0.9.8b2/baserun/v1/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.8b2/baserun/v1/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    19701 2024-01-17 18:48:39.000000 baserun-0.9.8b2/baserun/v1/baserun_pb2.py
--rw-r--r--   0 epeterson   (501) staff       (20)    30165 2024-01-17 18:48:39.000000 baserun-0.9.8b2/baserun/v1/baserun_pb2.pyi
--rw-r--r--   0 epeterson   (501) staff       (20)    24083 2024-01-16 22:41:50.000000 baserun-0.9.8b2/baserun/v1/baserun_pb2_grpc.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-17 19:20:07.128040 baserun-0.9.8b2/baserun.egg-info/
--rw-r--r--   0 epeterson   (501) staff       (20)     6553 2024-01-17 19:20:07.000000 baserun-0.9.8b2/baserun.egg-info/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     1023 2024-01-17 19:20:07.000000 baserun-0.9.8b2/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-01-17 19:20:07.000000 baserun-0.9.8b2/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-01-17 19:20:07.000000 baserun-0.9.8b2/baserun.egg-info/entry_points.txt
--rw-r--r--   0 epeterson   (501) staff       (20)      189 2024-01-17 19:20:07.000000 baserun-0.9.8b2/baserun.egg-info/requires.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-01-17 19:20:07.000000 baserun-0.9.8b2/baserun.egg-info/top_level.txt
--rw-r--r--   0 epeterson   (501) staff       (20)      865 2024-01-17 18:48:39.000000 baserun-0.9.8b2/pyproject.toml
--rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-01-17 19:20:07.129166 baserun-0.9.8b2/setup.cfg
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-17 19:20:07.127498 baserun-0.9.8b2/tests/
--rw-r--r--   0 epeterson   (501) staff       (20)    22353 2024-01-17 19:01:27.000000 baserun-0.9.8b2/tests/testing_functions.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.513314 baserun-0.9.9/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-0.9.9/LICENSE
+-rw-r--r--   0 epeterson   (501) staff       (20)     6425 2024-01-29 17:36:21.513164 baserun-0.9.9/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     4582 2023-12-01 13:51:58.000000 baserun-0.9.9/README.md
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.494687 baserun-0.9.9/baserun/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1386 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     5793 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/annotation.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      393 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/api_key.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    15124 2024-01-22 23:33:49.000000 baserun-0.9.9/baserun/baserun.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1469 2024-01-23 19:41:18.000000 baserun-0.9.9/baserun/checks.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      162 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/constants.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.500156 baserun-0.9.9/baserun/evals/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:37.000000 baserun-0.9.9/baserun/evals/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    13545 2024-01-25 20:00:32.000000 baserun-0.9.9/baserun/evals/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      154 2023-12-01 13:51:37.000000 baserun-0.9.9/baserun/evals/json.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1162 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/exporter.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1375 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/grpc.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1122 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/helpers.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.506096 baserun-0.9.9/baserun/instrumentation/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/instrumentation/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1771 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/anthropic.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    13427 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/instrumentation/base_instrumentor.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      557 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/instrumented_wrapper.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     4465 2023-12-06 13:41:54.000000 baserun-0.9.9/baserun/instrumentation/langchain.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2964 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/openai.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      278 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/span_attributes.py
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/model_configs.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2116 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/pytest_plugin.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     5347 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/sessions.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     8565 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/templates.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1130 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/thread_wrapper.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1105 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/users.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.509911 baserun-0.9.9/baserun/v1/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/v1/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    19701 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/v1/baserun_pb2.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    30165 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/v1/baserun_pb2.pyi
+-rw-r--r--   0 epeterson   (501) staff       (20)    24083 2024-01-16 22:41:50.000000 baserun-0.9.9/baserun/v1/baserun_pb2_grpc.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.512184 baserun-0.9.9/baserun.egg-info/
+-rw-r--r--   0 epeterson   (501) staff       (20)     6425 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     1023 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)      108 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/requires.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/top_level.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)      762 2024-01-29 17:34:28.000000 baserun-0.9.9/pyproject.toml
+-rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-01-29 17:36:21.513986 baserun-0.9.9/setup.cfg
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.510982 baserun-0.9.9/tests/
+-rw-r--r--   0 epeterson   (501) staff       (20)    21901 2024-01-22 22:57:10.000000 baserun-0.9.9/tests/testing_functions.py
```

### Comparing `baserun-0.9.8b2/LICENSE` & `baserun-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/PKG-INFO` & `baserun-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 0.9.8b2
+Version: 0.9.9
 Summary: Tools for testing, debugging, and evaluating LLM features.
 Author-email: Adam Ginzberg <adam@baserun.ai>, Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,22 +27,19 @@
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
-Requires-Dist: openai>=1.1.1
-Requires-Dist: wrapt~=1.15.0
-Requires-Dist: opentelemetry-instrumentation>=0.43b0
-Requires-Dist: opentelemetry-sdk>=1.20.0
+Requires-Dist: openai>=1.7.2
+Requires-Dist: opentelemetry-sdk>=1.21
 Requires-Dist: grpcio~=1.58.0
 Requires-Dist: protobuf~=4.24.3
 Requires-Dist: grpcio-tools~=1.58.0
-Requires-Dist: python-Levenshtein~=0.23.0
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
```

### Comparing `baserun-0.9.8b2/README.md` & `baserun-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/__init__.py` & `baserun-0.9.9/baserun/__init__.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/annotation.py` & `baserun-0.9.9/baserun/annotation.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/baserun.py` & `baserun-0.9.9/baserun/baserun.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,26 +156,31 @@
             run.completion_timestamp.FromDatetime(datetime.utcnow())
             Baserun.set_context(set_value(BASERUN_RUN, run, Baserun.get_context()))
             get_or_create_submission_service().EndRun.future(EndRunRequest(run=run))
         except Exception as e:
             logger.warning(f"Failed to submit run end to Baserun: {e}")
 
     @staticmethod
+    def create_run(*args, **kwargs):
+        return Baserun.get_or_create_current_run(*args, **kwargs, force_new=True)
+
+    @staticmethod
     def get_or_create_current_run(
         name: str = None,
         suite_id: str = None,
         start_timestamp: datetime = None,
         completion_timestamp: datetime = None,
         trace_type: Run.RunType = None,
         metadata: dict[str, Any] = None,
         session_id: str = None,
+        force_new: bool = False,
     ) -> Run:
         """Gets the current run or creates one"""
         existing_run = Baserun.current_run()
-        if existing_run:
+        if existing_run and not force_new:
             return existing_run
 
         run_id = str(uuid.uuid4())
         if not trace_type:
             trace_type = Run.RunType.RUN_TYPE_TEST if Baserun.current_test_suite else Run.RunType.RUN_TYPE_PRODUCTION
 
         if not name:
@@ -240,15 +245,15 @@
         if inspect.iscoroutinefunction(func):
 
             async def wrapper(*args, **kwargs):
                 if not Baserun._initialized:
                     return await func(*args, **kwargs)
 
                 session_id = get_session_id()
-                run = Baserun.get_or_create_current_run(
+                run = Baserun.create_run(
                     name=run_name,
                     trace_type=run_type,
                     metadata=metadata,
                     suite_id=suite_id,
                     session_id=session_id,
                 )
                 old_context = Baserun.get_context()
@@ -271,15 +276,15 @@
 
             async def wrapper(*args, **kwargs):
                 if not Baserun._initialized:
                     async for item in func(*args, **kwargs):
                         yield item
 
                 session_id = get_session_id()
-                run = Baserun.get_or_create_current_run(
+                run = Baserun.create_run(
                     name=run_name,
                     trace_type=run_type,
                     metadata=metadata,
                     suite_id=suite_id,
                     session_id=session_id,
                 )
 
@@ -306,15 +311,15 @@
         else:
 
             def wrapper(*args, **kwargs):
                 if not Baserun._initialized:
                     return func(*args, **kwargs)
 
                 session_id = get_session_id()
-                run = Baserun.get_or_create_current_run(
+                run = Baserun.create_run(
                     name=run_name,
                     trace_type=run_type,
                     metadata=metadata,
                     suite_id=suite_id,
                     session_id=session_id,
                 )
```

### Comparing `baserun-0.9.8b2/baserun/checks.py` & `baserun-0.9.9/baserun/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 def check_includes(
     name: str,
     actual: str,
     expected: Union[str, list[str]],
     metadata: dict[str, Any] = None,
 ):
     expected_list = [expected] if isinstance(expected, str) else expected
-    result = any(actual in item for item in expected_list)
+    result = any(item in actual for item in expected_list)
 
     return check(
         name=name,
         eval_type="match",
         metadata=metadata,
         actual=actual,
         expected=expected,
```

### Comparing `baserun-0.9.8b2/baserun/evals/evals.py` & `baserun-0.9.9/baserun/evals/evals.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/exporter.py` & `baserun-0.9.9/baserun/exporter.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/grpc.py` & `baserun-0.9.9/baserun/grpc.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/helpers.py` & `baserun-0.9.9/baserun/helpers.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/instrumentation/anthropic.py` & `baserun-0.9.9/baserun/instrumentation/anthropic.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/instrumentation/base_instrumentor.py` & `baserun-0.9.9/baserun/instrumentation/base_instrumentor.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/instrumentation/instrumented_wrapper.py` & `baserun-0.9.9/baserun/instrumentation/instrumented_wrapper.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/instrumentation/langchain.py` & `baserun-0.9.9/baserun/instrumentation/langchain.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/instrumentation/openai.py` & `baserun-0.9.9/baserun/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/pytest_plugin.py` & `baserun-0.9.9/baserun/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/sessions.py` & `baserun-0.9.9/baserun/sessions.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/templates.py` & `baserun-0.9.9/baserun/templates.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/thread_wrapper.py` & `baserun-0.9.9/baserun/thread_wrapper.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/users.py` & `baserun-0.9.9/baserun/users.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/v1/baserun_pb2.py` & `baserun-0.9.9/baserun/v1/baserun_pb2.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/v1/baserun_pb2.pyi` & `baserun-0.9.9/baserun/v1/baserun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun/v1/baserun_pb2_grpc.py` & `baserun-0.9.9/baserun/v1/baserun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/baserun.egg-info/PKG-INFO` & `baserun-0.9.9/baserun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 0.9.8b2
+Version: 0.9.9
 Summary: Tools for testing, debugging, and evaluating LLM features.
 Author-email: Adam Ginzberg <adam@baserun.ai>, Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,22 +27,19 @@
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
-Requires-Dist: openai>=1.1.1
-Requires-Dist: wrapt~=1.15.0
-Requires-Dist: opentelemetry-instrumentation>=0.43b0
-Requires-Dist: opentelemetry-sdk>=1.20.0
+Requires-Dist: openai>=1.7.2
+Requires-Dist: opentelemetry-sdk>=1.21
 Requires-Dist: grpcio~=1.58.0
 Requires-Dist: protobuf~=4.24.3
 Requires-Dist: grpcio-tools~=1.58.0
-Requires-Dist: python-Levenshtein~=0.23.0
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
```

### Comparing `baserun-0.9.8b2/baserun.egg-info/SOURCES.txt` & `baserun-0.9.9/baserun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baserun-0.9.8b2/pyproject.toml` & `baserun-0.9.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baserun"
-version = "0.9.8b2"
+version = "0.9.9"
 description = "Tools for testing, debugging, and evaluating LLM features."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Adam Ginzberg", email = "adam@baserun.ai" },
     { name = "Erik Peterson", email = "erik@baserun.ai" }
 ]
 requires-python = ">=3.7.1"
 dependencies = [
     "requests>=2.31.0",
-    "openai>=1.1.1",
-    "wrapt~=1.15.0",
-    "opentelemetry-instrumentation>=0.43b0",
-    "opentelemetry-sdk>=1.20.0",
+    "openai>=1.7.2",
+    "opentelemetry-sdk>=1.21",
     "grpcio~=1.58.0",
     "protobuf~=4.24.3",
     "grpcio-tools~=1.58.0",
-    "python-Levenshtein~=0.23.0"
 ]
 
 [project.urls]
 Homepage = "https://baserun.ai"
 Repository = "https://github.com/baserun-ai/baserun-py"
 
 [project.entry-points.pytest11]
```

### Comparing `baserun-0.9.8b2/tests/testing_functions.py` & `baserun-0.9.9/tests/testing_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -585,28 +585,14 @@
         messages=[{"role": "user", "content": prompt}],
     )
     content = completion.choices[0].message.content
     baserun.check_includes("openai_chat.content", content, "Washington")
     return content
 
 
-@baserun.trace
-def litellm_chat(prompt="What is the capital of the US?") -> str:
-    # Must `pip install litellm` (it's not a project dependency)
-    from litellm import completion
-
-    completion = completion(
-        model="command-nightly",
-        messages=[{"role": "user", "content": prompt}],
-    )
-    content = completion.choices[0].message.content
-    baserun.check_includes("openai_chat.content", content, "Washington")
-    return content
-
-
 def call_function(functions, function_name: str, parsed_args: argparse.Namespace):
     function_to_call = functions.get(function_name)
     if function_to_call is None:
         function_to_call = {f: globals().get(f) for f in globals()}.get(function_name)
 
     if inspect.iscoroutinefunction(function_to_call):
         if parsed_args.prompt:
```

