# Comparing `tmp/valor_client-0.22.1.tar.gz` & `tmp/valor_client-0.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.22.1.tar", last modified: Mon Apr 22 16:27:28 2024, max compression
+gzip compressed data, was "valor_client-0.22.2.tar", last modified: Tue Apr 23 16:16:39 2024, max compression
```

## Comparing `valor_client-0.22.1.tar` & `valor_client-0.22.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.333879 valor_client-0.22.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 16:27:24.000000 valor_client-0.22.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-22 16:27:28.333879 valor_client-0.22.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 16:27:24.000000 valor_client-0.22.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:27:28.333879 valor_client-0.22.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-22 16:27:24.000000 valor_client-0.22.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.325878 valor_client-0.22.1/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.325878 valor_client-0.22.1/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.325878 valor_client-0.22.1/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.325878 valor_client-0.22.1/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.325878 valor_client-0.22.1/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.329878 valor_client-0.22.1/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-22 16:27:24.000000 valor_client-0.22.1/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.329878 valor_client-0.22.1/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53627 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.329878 valor_client-0.22.1/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.329878 valor_client-0.22.1/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-22 16:27:24.000000 valor_client-0.22.1/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:27:28.333879 valor_client-0.22.1/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-22 16:27:28.000000 valor_client-0.22.1/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-22 16:27:28.000000 valor_client-0.22.1/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:27:28.000000 valor_client-0.22.1/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 16:27:28.000000 valor_client-0.22.1/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 16:27:28.000000 valor_client-0.22.1/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.314195 valor_client-0.22.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 16:16:34.000000 valor_client-0.22.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 16:16:39.310195 valor_client-0.22.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 16:16:34.000000 valor_client-0.22.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:16:39.314195 valor_client-0.22.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 16:16:34.000000 valor_client-0.22.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.306195 valor_client-0.22.2/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-23 16:16:34.000000 valor_client-0.22.2/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29256 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54413 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-23 16:16:34.000000 valor_client-0.22.2/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:39.310195 valor_client-0.22.2/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 16:16:39.000000 valor_client-0.22.2/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.22.1/LICENSE` & `valor_client-0.22.2/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/PKG-INFO` & `valor_client-0.22.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.22.1
+Version: 0.22.2
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.22.1/pyproject.toml` & `valor_client-0.22.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/conftest.py` & `valor_client-0.22.2/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/coretypes/test_core.py` & `valor_client-0.22.2/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.22.2/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/coretypes/test_filtering.py` & `valor_client-0.22.2/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/schemas/test_filters.py` & `valor_client-0.22.2/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/schemas/test_geojson.py` & `valor_client-0.22.2/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/schemas/test_label.py` & `valor_client-0.22.2/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.22.2/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.22.2/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.22.2/unit-tests/symbolic/collections/test_structures.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/symbolic/test_operators.py` & `valor_client-0.22.2/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.22.2/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.22.2/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/test_client.py` & `valor_client-0.22.2/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/unit-tests/test_viz.py` & `valor_client-0.22.2/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/__init__.py` & `valor_client-0.22.2/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/client.py` & `valor_client-0.22.2/valor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -794,32 +794,38 @@
         Parameters
         ----------
         name : str
             The name of the model to be deleted.
         """
         self._requests_delete_rel_host(f"models/{name}")
 
-    def evaluate(self, request: EvaluationRequest) -> List[dict]:
+    def evaluate(
+        self, request: EvaluationRequest, allow_retries: bool = False
+    ) -> List[dict]:
         """
         Creates as many evaluations as necessary to fulfill the request.
 
         `CREATE` endpoint.
 
         Parameters
         ----------
         request : schemas.EvaluationRequest
             The requested evaluation parameters.
+        allow_retries : bool, default = False
+            Option to retry previously failed evaluations.
 
         Returns
         -------
         List[dict]
             A list of evaluations that meet the parameters.
         """
+        query_str = urlencode({"allow_retries": allow_retries})
+        endpoint = f"evaluations?{query_str}"
         return self._requests_post_rel_host(
-            "evaluations", json=asdict(request)
+            endpoint, json=asdict(request)
         ).json()
 
     def get_evaluations(
         self,
         *,
         evaluation_ids: Optional[List[int]] = None,
         models: Optional[List[str]] = None,
```

### Comparing `valor_client-0.22.1/valor/coretypes.py` & `valor_client-0.22.2/valor/coretypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -896,28 +896,31 @@
 
     def evaluate_classification(
         self,
         datasets: Optional[Union[Dataset, List[Dataset]]] = None,
         filter_by: Optional[FilterType] = None,
         label_map: Optional[Dict[Label, Label]] = None,
         compute_pr_curves: bool = False,
+        allow_retries: bool = False,
     ) -> Evaluation:
         """
         Start a classification evaluation job.
 
         Parameters
         ----------
         datasets : Union[Dataset, List[Dataset]], optional
             The dataset or list of datasets to evaluate against.
         filter_by : FilterType, optional
             Optional set of constraints to filter evaluation by.
         label_map : Dict[Label, Label], optional
             Optional mapping of individual labels to a grouper label. Useful when you need to evaluate performance using labels that differ across datasets and models.
         compute_pr_curves: bool
             A boolean which determines whether we calculate precision-recall curves or not.
+        allow_retries : bool, default = False
+            Option to retry previously failed evaluations.
 
         Returns
         -------
         Evaluation
             A job object that can be used to track the status of the job and get the metrics of it upon completion.
         """
         if not datasets and not filter_by:
@@ -935,15 +938,17 @@
                 label_map=self._create_label_map(label_map=label_map),
                 compute_pr_curves=compute_pr_curves,
             ),
             meta={},
         )
 
         # create evaluation
-        evaluation = Client(self.conn).evaluate(request)
+        evaluation = Client(self.conn).evaluate(
+            request, allow_retries=allow_retries
+        )
         if len(evaluation) != 1:
             raise RuntimeError
         return evaluation[0]
 
     def evaluate_detection(
         self,
         datasets: Optional[Union[Dataset, List[Dataset]]] = None,
@@ -951,14 +956,15 @@
         convert_annotations_to_type: Optional[AnnotationType] = None,
         iou_thresholds_to_compute: Optional[List[float]] = None,
         iou_thresholds_to_return: Optional[List[float]] = None,
         label_map: Optional[Dict[Label, Label]] = None,
         recall_score_threshold: float = 0,
         compute_pr_curves: bool = False,
         pr_curve_iou_threshold: float = 0.5,
+        allow_retries: bool = False,
     ) -> Evaluation:
         """
         Start an object-detection evaluation job.
 
         Parameters
         ----------
         datasets : Union[Dataset, List[Dataset]], optional
@@ -975,14 +981,16 @@
             Optional mapping of individual labels to a grouper label. Useful when you need to evaluate performance using labels that differ across datasets and models.
         recall_score_threshold: float, default=0
             The confidence score threshold for use when determining whether to count a prediction as a true positive or not while calculating Average Recall.
         compute_pr_curves: bool, optional
             A boolean which determines whether we calculate precision-recall curves or not.
         pr_curve_iou_threshold: float, optional
             The IOU threshold to use when calculating precision-recall curves. Defaults to 0.5. Does nothing when compute_pr_curves is set to False or None.
+        allow_retries : bool, default = False
+            Option to retry previously failed evaluations.
 
 
         Returns
         -------
         Evaluation
             A job object that can be used to track the status of the job and get the metrics of it upon completion.
         """
@@ -1009,36 +1017,41 @@
             model_names=[self.get_name()],
             datum_filter=datum_filter,
             parameters=parameters,
             meta={},
         )
 
         # create evaluation
-        evaluation = Client(self.conn).evaluate(request)
+        evaluation = Client(self.conn).evaluate(
+            request, allow_retries=allow_retries
+        )
         if len(evaluation) != 1:
             raise RuntimeError
         return evaluation[0]
 
     def evaluate_segmentation(
         self,
         datasets: Optional[Union[Dataset, List[Dataset]]] = None,
         filter_by: Optional[FilterType] = None,
         label_map: Optional[Dict[Label, Label]] = None,
+        allow_retries: bool = False,
     ) -> Evaluation:
         """
         Start a semantic-segmentation evaluation job.
 
         Parameters
         ----------
         datasets : Union[Dataset, List[Dataset]], optional
             The dataset or list of datasets to evaluate against.
         filter_by : FilterType, optional
             Optional set of constraints to filter evaluation by.
         label_map : Dict[Label, Label], optional
             Optional mapping of individual labels to a grouper label. Useful when you need to evaluate performance using labels that differ across datasets and models.
+        allow_retries : bool, default = False
+            Option to retry previously failed evaluations.
 
         Returns
         -------
         Evaluation
             A job object that can be used to track the status of the job and get the metrics of it upon completion
         """
         # format request
@@ -1050,15 +1063,17 @@
                 task_type=TaskType.SEMANTIC_SEGMENTATION,
                 label_map=self._create_label_map(label_map=label_map),
             ),
             meta={},
         )
 
         # create evaluation
-        evaluation = Client(self.conn).evaluate(request)
+        evaluation = Client(self.conn).evaluate(
+            request, allow_retries=allow_retries
+        )
         if len(evaluation) != 1:
             raise RuntimeError
         return evaluation[0]
 
     def delete(self, timeout: int = 0):
         """
         Delete the `Model` object from the back end.
@@ -1740,25 +1755,31 @@
             for evaluation in self.conn.get_evaluations(
                 evaluation_ids=evaluation_ids,
                 models=models,
                 datasets=datasets,
             )
         ]
 
-    def evaluate(self, request: EvaluationRequest) -> List[Evaluation]:
+    def evaluate(
+        self, request: EvaluationRequest, allow_retries: bool = False
+    ) -> List[Evaluation]:
         """
         Creates as many evaluations as necessary to fulfill the request.
 
         Parameters
         ----------
         request : schemas.EvaluationRequest
             The requested evaluation parameters.
+        allow_retries : bool, default = False
+            Option to retry previously failed evaluations.
 
         Returns
         -------
         List[Evaluation]
             A list of evaluations that meet the parameters.
         """
         return [
             Evaluation(**evaluation)
-            for evaluation in self.conn.evaluate(request)
+            for evaluation in self.conn.evaluate(
+                request, allow_retries=allow_retries
+            )
         ]
```

### Comparing `valor_client-0.22.1/valor/enums.py` & `valor_client-0.22.2/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/exceptions.py` & `valor_client-0.22.2/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/metatypes.py` & `valor_client-0.22.2/valor/metatypes.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/schemas/__init__.py` & `valor_client-0.22.2/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/schemas/evaluation.py` & `valor_client-0.22.2/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/schemas/filters.py` & `valor_client-0.22.2/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/schemas/symbolic/collections.py` & `valor_client-0.22.2/valor/schemas/symbolic/collections.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/schemas/symbolic/operators.py` & `valor_client-0.22.2/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/schemas/symbolic/types.py` & `valor_client-0.22.2/valor/schemas/symbolic/types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/type_checks.py` & `valor_client-0.22.2/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor/viz.py` & `valor_client-0.22.2/valor/viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.22.1/valor_client.egg-info/PKG-INFO` & `valor_client-0.22.2/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.22.1
+Version: 0.22.2
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.22.1/valor_client.egg-info/SOURCES.txt` & `valor_client-0.22.2/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

