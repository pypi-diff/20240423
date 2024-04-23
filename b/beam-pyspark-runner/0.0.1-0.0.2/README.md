# Comparing `tmp/beam_pyspark_runner-0.0.1.tar.gz` & `tmp/beam_pyspark_runner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_pyspark_runner-0.0.1.tar", last modified: Mon Apr 15 21:44:21 2024, max compression
+gzip compressed data, was "beam_pyspark_runner-0.0.2.tar", last modified: Tue Apr 23 15:32:27 2024, max compression
```

## Comparing `beam_pyspark_runner-0.0.1.tar` & `beam_pyspark_runner-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:44:21.738937 beam_pyspark_runner-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-15 21:44:21.738937 beam_pyspark_runner-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:44:21.734937 beam_pyspark_runner-0.0.1/beam_pyspark_runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/eval_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/pyspark_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/pyspark_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/transform_evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:44:21.734937 beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-15 21:44:21.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-15 21:44:21.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:44:21.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 21:44:21.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 21:44:21.000000 beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-15 21:44:14.000000 beam_pyspark_runner-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:44:21.738937 beam_pyspark_runner-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:32:27.919907 beam_pyspark_runner-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-23 15:32:27.919907 beam_pyspark_runner-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:32:27.915907 beam_pyspark_runner-0.0.2/beam_pyspark_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/eval_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/pyspark_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/pyspark_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/transform_evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:32:27.919907 beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-23 15:32:27.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 15:32:27.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:32:27.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-23 15:32:27.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 15:32:27.000000 beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-23 15:32:20.000000 beam_pyspark_runner-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:32:27.919907 beam_pyspark_runner-0.0.2/setup.cfg
```

### Comparing `beam_pyspark_runner-0.0.1/PKG-INFO` & `beam_pyspark_runner-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beam-pyspark-runner
-Version: 0.0.1
+Version: 0.0.2
 Summary: An Apache Beam pipeline Runner built on Apache Spark's python API
 Author-email: Nathan Zimmerman <npzimmerman@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/moradology/beam-pyspark-runner
 Project-URL: repository, https://github.com/moradology/beam-pyspark-runner.git
 Keywords: virtualenv,dependencies
 Classifier: Intended Audience :: Developers
@@ -12,16 +12,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: apache-beam==2.53.0
 Requires-Dist: pyspark==3.5.1
 Requires-Dist: psutil==5.9.8
 Provides-Extra: dev
 Requires-Dist: pytest>=8.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Provides-Extra: lint
```

### Comparing `beam_pyspark_runner-0.0.1/README.md` & `beam_pyspark_runner-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner/eval_context.py` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner/eval_context.py`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner/evaluator.py` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner/evaluator.py`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner/execution_plan.py` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner/execution_plan.py`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner/overrides.py` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner/overrides.py`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner/pyspark_runner.py` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner/pyspark_runner.py`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner/pyspark_visitors.py` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner/pyspark_visitors.py`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner/transform_evaluators.py` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner/transform_evaluators.py`

 * *Files identical despite different names*

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/PKG-INFO` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beam-pyspark-runner
-Version: 0.0.1
+Version: 0.0.2
 Summary: An Apache Beam pipeline Runner built on Apache Spark's python API
 Author-email: Nathan Zimmerman <npzimmerman@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/moradology/beam-pyspark-runner
 Project-URL: repository, https://github.com/moradology/beam-pyspark-runner.git
 Keywords: virtualenv,dependencies
 Classifier: Intended Audience :: Developers
@@ -12,16 +12,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: apache-beam==2.53.0
 Requires-Dist: pyspark==3.5.1
 Requires-Dist: psutil==5.9.8
 Provides-Extra: dev
 Requires-Dist: pytest>=8.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Provides-Extra: lint
```

### Comparing `beam_pyspark_runner-0.0.1/beam_pyspark_runner.egg-info/SOURCES.txt` & `beam_pyspark_runner-0.0.2/beam_pyspark_runner.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 beam_pyspark_runner/__init__.py
 beam_pyspark_runner/eval_context.py
 beam_pyspark_runner/evaluator.py
 beam_pyspark_runner/execution_plan.py
 beam_pyspark_runner/overrides.py
```

### Comparing `beam_pyspark_runner-0.0.1/pyproject.toml` & `beam_pyspark_runner-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ]
 keywords=["virtualenv", "dependencies"]
 authors=[{ name = "Nathan Zimmerman", email = "npzimmerman@gmail.com"}]
 license= { text = "MIT" }
-requires-python=">=3.8"
+requires-python=">=3.7"
 dependencies = ["apache-beam==2.53.0", "pyspark==3.5.1", "psutil==5.9.8"]
 dynamic = ["version", "readme"]
 
 [project.urls]
 homepage = "https://github.com/moradology/beam-pyspark-runner"
 repository = "https://github.com/moradology/beam-pyspark-runner.git"
```

