# Comparing `tmp/quantum_serverless-0.8.2.tar.gz` & `tmp/quantum_serverless-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.8.2.tar", last modified: Fri Jan  5 16:27:13 2024, max compression
+gzip compressed data, was "quantum_serverless-0.9.0.tar", last modified: Wed Jan 31 16:27:59 2024, max compression
```

## Comparing `quantum_serverless-0.8.2.tar` & `quantum_serverless-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.715827 quantum_serverless-0.8.2/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/quantum_serverless/visualizaiton/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/visualizaiton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/quantum_serverless/visualizaiton/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.715827 quantum_serverless-0.8.2/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-05 16:27:13.000000 quantum_serverless-0.8.2/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-01-05 16:27:13.000000 quantum_serverless-0.8.2/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 16:27:13.000000 quantum_serverless-0.8.2/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-05 16:27:13.000000 quantum_serverless-0.8.2/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-05 16:27:13.000000 quantum_serverless-0.8.2/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/core/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/core/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/core/test_program_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/tests/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:13.719827 quantum_serverless-0.8.2/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-05 16:27:07.000000 quantum_serverless-0.8.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.995234 quantum_serverless-0.9.0/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.995234 quantum_serverless-0.9.0/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.995234 quantum_serverless-0.9.0/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/quantum_serverless/visualizaiton/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/visualizaiton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/quantum_serverless/visualizaiton/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.995234 quantum_serverless-0.9.0/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-31 16:27:58.000000 quantum_serverless-0.9.0/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-01-31 16:27:58.000000 quantum_serverless-0.9.0/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:27:58.000000 quantum_serverless-0.9.0/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-31 16:27:58.000000 quantum_serverless-0.9.0/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-31 16:27:58.000000 quantum_serverless-0.9.0/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/core/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/core/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/core/test_program_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:58.999234 quantum_serverless-0.9.0/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-31 16:27:52.000000 quantum_serverless-0.9.0/tests/utils.py
```

### Comparing `quantum_serverless-0.8.2/PKG-INFO` & `quantum_serverless-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.8.2
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.8.2/README.md` & `quantum_serverless-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/__init__.py` & `quantum_serverless-0.9.0/quantum_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/__init__.py` & `quantum_serverless-0.9.0/quantum_serverless/core/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/constants.py` & `quantum_serverless-0.9.0/quantum_serverless/core/constants.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/decorators.py` & `quantum_serverless-0.9.0/quantum_serverless/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/files.py` & `quantum_serverless-0.9.0/quantum_serverless/core/files.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/job.py` & `quantum_serverless-0.9.0/quantum_serverless/core/job.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/pattern.py` & `quantum_serverless-0.9.0/quantum_serverless/core/pattern.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/provider.py` & `quantum_serverless-0.9.0/quantum_serverless/core/provider.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/core/tracing.py` & `quantum_serverless-0.9.0/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/exception.py` & `quantum_serverless-0.9.0/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/library/__init__.py` & `quantum_serverless-0.9.0/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.9.0/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.9.0/quantum_serverless/quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.9.0/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.9.0/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.9.0/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.9.0/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/utils/errors.py` & `quantum_serverless-0.9.0/quantum_serverless/utils/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/utils/json.py` & `quantum_serverless-0.9.0/quantum_serverless/utils/json.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/utils/storage.py` & `quantum_serverless-0.9.0/quantum_serverless/utils/storage.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/visualizaiton/__init__.py` & `quantum_serverless-0.9.0/quantum_serverless/visualizaiton/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless/visualizaiton/widget.py` & `quantum_serverless-0.9.0/quantum_serverless/visualizaiton/widget.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.9.0/quantum_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.8.2
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.8.2/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.9.0/quantum_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/setup.py` & `quantum_serverless-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/core/test_decorator.py` & `quantum_serverless-0.9.0/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/core/test_job.py` & `quantum_serverless-0.9.0/tests/core/test_job.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/core/test_pattern.py` & `quantum_serverless-0.9.0/tests/core/test_pattern.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/core/test_program_repository.py` & `quantum_serverless-0.9.0/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/library/test_transpiler.py` & `quantum_serverless-0.9.0/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.9.0/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/serializers/test_serializers.py` & `quantum_serverless-0.9.0/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/test_quantum_serverless.py` & `quantum_serverless-0.9.0/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.8.2/tests/utils.py` & `quantum_serverless-0.9.0/tests/utils.py`

 * *Files identical despite different names*

