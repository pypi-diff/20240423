# Comparing `tmp/pldag-0.6.8.tar.gz` & `tmp/pldag-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.6.8.tar", max compression
+gzip compressed data, was "pldag-0.6.9.tar", max compression
```

## Comparing `pldag-0.6.8.tar` & `pldag-0.6.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.8/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.6.8/README.md
--rw-r--r--   0        0        0    31135 2024-04-22 15:00:50.811385 pldag-0.6.8/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.6.8/pldag/solver/__init__.py
--rw-r--r--   0        0        0      857 2024-04-22 11:08:59.392759 pldag-0.6.8/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-22 15:00:59.575789 pldag-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.9/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.6.9/README.md
+-rw-r--r--   0        0        0    31135 2024-04-22 15:00:50.811385 pldag-0.6.9/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.6.9/pldag/solver/__init__.py
+-rw-r--r--   0        0        0      973 2024-04-22 15:04:47.780408 pldag-0.6.9/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-22 15:04:56.568103 pldag-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.6.9/PKG-INFO
```

### Comparing `pldag-0.6.8/LICENSE` & `pldag-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.6.8/README.md` & `pldag-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.6.8/pldag/__init__.py` & `pldag-0.6.9/pldag/__init__.py`

 * *Files identical despite different names*

### Comparing `pldag-0.6.8/pldag/solver/glpk_solver.py` & `pldag-0.6.9/pldag/solver/glpk_solver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import numpy as np
-import npycvx
 import functools
 
+try:
+    import npycvx
+except ImportError:
+    raise ImportError("Please install the npycvx package to use GLPK solver module.")
+
 def solve_lp(A: np.ndarray, b: np.ndarray, objectives: np.ndarray, int_vrs: set=set()):
     """
     Solve the linear programming problem:
     minimize c^T x
     subject to Ax >= b
 
     for each c in objectives.
```

### Comparing `pldag-0.6.8/PKG-INFO` & `pldag-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.6.8
+Version: 0.6.9
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

