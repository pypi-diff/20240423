# Comparing `tmp/literalai-0.0.506.tar.gz` & `tmp/literalai-0.0.507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.506.tar", last modified: Thu Apr 18 13:49:20 2024, max compression
+gzip compressed data, was "literalai-0.0.507.tar", last modified: Tue Apr 23 12:04:29 2024, max compression
```

## Comparing `literalai-0.0.506.tar` & `literalai-0.0.507.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.447400 literalai-0.0.506/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 13:49:11.000000 literalai-0.0.506/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 13:49:20.447400 literalai-0.0.506/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 13:49:11.000000 literalai-0.0.506/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.435400 literalai-0.0.506/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.443400 literalai-0.0.506/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    40395 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.443400 literalai-0.0.506/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.447400 literalai-0.0.506/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.439400 literalai-0.0.506/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:49:20.447400 literalai-0.0.506/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 13:49:11.000000 literalai-0.0.506/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.447400 literalai-0.0.506/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.755336 literalai-0.0.507/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 12:04:23.000000 literalai-0.0.507/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 12:04:29.755336 literalai-0.0.507/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-23 12:04:23.000000 literalai-0.0.507/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    81103 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20172 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.755336 literalai-0.0.507/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:04:29.755336 literalai-0.0.507/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 12:04:23.000000 literalai-0.0.507/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.755336 literalai-0.0.507/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/tests/__init__.py
```

### Comparing `literalai-0.0.506/LICENSE` & `literalai-0.0.507/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/README.md` & `literalai-0.0.507/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/api/attachment_helpers.py` & `literalai-0.0.507/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/api/dataset_helpers.py` & `literalai-0.0.507/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/api/generation_helpers.py` & `literalai-0.0.507/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/api/gql.py` & `literalai-0.0.507/literalai/api/gql.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,24 +179,26 @@
     $before: ID,
     $cursorAnchor: DateTime,
     $filters: [ThreadsInputType!],
     $orderBy: ThreadsOrderByInput,
     $first: Int,
     $last: Int,
     $projectId: String,
+    $stepTypesToKeep: [StepType!],
     ) {
     threads(
         after: $after,
         before: $before,
         cursorAnchor: $cursorAnchor,
         filters: $filters,
         orderBy: $orderBy,
         first: $first,
         last: $last,
         projectId: $projectId,
+        stepTypesToKeep: $stepTypesToKeep,
         ) {
         pageInfo {
             startCursor
             endCursor
             hasNextPage
             hasPreviousPage
         }
```

### Comparing `literalai-0.0.506/literalai/api/prompt_helpers.py` & `literalai-0.0.507/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/api/score_helpers.py` & `literalai-0.0.507/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/api/step_helpers.py` & `literalai-0.0.507/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/api/thread_helpers.py` & `literalai-0.0.507/literalai/api/thread_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from typing import Any, Dict, List, Optional
 
 from literalai.filter import threads_filters, threads_order_by
 from literalai.my_types import PaginatedResponse
+from literalai.step import StepType
 from literalai.thread import Thread
 
 from . import gql
 
 
 def get_threads_helper(
     first: Optional[int] = None,
     after: Optional[str] = None,
     before: Optional[str] = None,
     filters: Optional[threads_filters] = None,
     order_by: Optional[threads_order_by] = None,
+    step_types_to_keep: Optional[List[StepType]] = None,
 ):
     variables: Dict[str, Any] = {}
 
     if first:
         variables["first"] = first
     if after:
         variables["after"] = after
     if before:
         variables["before"] = before
     if filters:
         variables["filters"] = filters
     if order_by:
         variables["orderBy"] = order_by
+    if step_types_to_keep:
+        variables["stepTypesToKeep"] = step_types_to_keep
 
     def process_response(response):
         processed_response = response["data"]["threads"]
         processed_response["data"] = [
             edge["node"] for edge in processed_response["edges"]
         ]
         del processed_response["edges"]
```

### Comparing `literalai-0.0.506/literalai/api/user_helpers.py` & `literalai-0.0.507/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/callback/langchain_callback.py` & `literalai-0.0.507/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/callback/llama_index_callback.py` & `literalai-0.0.507/literalai/callback/llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/client.py` & `literalai-0.0.507/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/dataset.py` & `literalai-0.0.507/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/dataset_experiment.py` & `literalai-0.0.507/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/dataset_item.py` & `literalai-0.0.507/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/event_processor.py` & `literalai-0.0.507/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/filter.py` & `literalai-0.0.507/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/helper.py` & `literalai-0.0.507/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/instrumentation/openai.py` & `literalai-0.0.507/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/message.py` & `literalai-0.0.507/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/my_types.py` & `literalai-0.0.507/literalai/my_types.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/prompt.py` & `literalai-0.0.507/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/requirements.py` & `literalai-0.0.507/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/step.py` & `literalai-0.0.507/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai/thread.py` & `literalai-0.0.507/literalai/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class Thread:
     id: str
     name: Optional[str]
     metadata: Optional[Dict]
     tags: Optional[List[str]]
     steps: Optional[List[Step]]
     participant_id: Optional[str]
-    participant_identifier: Optional[str]
+    participant_identifier: Optional[str] = None
     created_at: Optional[str]  # read-only, set by server
     needs_upsert: Optional[bool]
 
     def __init__(
         self,
         id: str,
         steps: Optional[List[Step]] = [],
@@ -60,15 +60,15 @@
             "tags": self.tags,
             "name": self.name,
             "steps": [step.to_dict() for step in self.steps] if self.steps else [],
             "participant": UserDict(
                 id=self.participant_id, identifier=self.participant_identifier
             )
             if self.participant_id
-            else None,
+            else UserDict(),
             "createdAt": getattr(self, "created_at", None),
         }
 
     @classmethod
     def from_dict(cls, thread_dict: ThreadDict) -> "Thread":
         step_dict_list = thread_dict.get("steps", None) or []
         id = thread_dict.get("id", None) or ""
@@ -121,15 +121,15 @@
             "id": thread_data["id"],
             "name": thread_data["name"],
         }
         if metadata := thread_data.get("metadata"):
             thread_data_to_upsert["metadata"] = metadata
         if tags := thread_data.get("tags"):
             thread_data_to_upsert["tags"] = tags
-        if participant_id := thread_data.get("participant_id"):
+        if participant_id := thread_data.get("participant", {}).get("id"):
             thread_data_to_upsert["participant_id"] = participant_id
 
         try:
             self.client.to_sync().api.upsert_thread(**thread_data_to_upsert)
         except Exception:
             logger.error(f"Failed to upsert thread: {traceback.format_exc()}")
```

### Comparing `literalai-0.0.506/literalai/wrappers.py` & `literalai-0.0.507/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.506/literalai.egg-info/SOURCES.txt` & `literalai-0.0.507/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

