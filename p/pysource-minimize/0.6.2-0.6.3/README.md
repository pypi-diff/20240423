# Comparing `tmp/pysource_minimize-0.6.2.tar.gz` & `tmp/pysource_minimize-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysource_minimize-0.6.2.tar", max compression
+gzip compressed data, was "pysource_minimize-0.6.3.tar", max compression
```

## Comparing `pysource_minimize-0.6.2.tar` & `pysource_minimize-0.6.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1465 2023-10-22 07:19:25.553357 pysource_minimize-0.6.2/README.md
--rw-r--r--   0        0        0     1315 2024-03-25 07:48:22.415688 pysource_minimize-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      142 2024-03-25 07:48:22.395687 pysource_minimize-0.6.2/pysource_minimize/__init__.py
--rw-r--r--   0        0        0     2015 2023-11-03 18:43:29.034047 pysource_minimize-0.6.2/pysource_minimize/__main__.py
--rw-r--r--   0        0        0     2631 2023-11-24 08:17:10.585299 pysource_minimize-0.6.2/pysource_minimize/_minimize.py
--rw-r--r--   0        0        0    10401 2024-02-22 14:34:56.930071 pysource_minimize-0.6.2/pysource_minimize/_minimize_base.py
--rw-r--r--   0        0        0    24292 2024-03-25 07:20:24.032324 pysource_minimize-0.6.2/pysource_minimize/_minimize_structure.py
--rw-r--r--   0        0        0     2442 2023-11-12 19:51:19.746756 pysource_minimize-0.6.2/pysource_minimize/_minimize_value.py
--rw-r--r--   0        0        0      337 2023-11-23 18:46:43.452140 pysource_minimize-0.6.2/pysource_minimize/_utils.py
--rw-r--r--   0        0        0        0 2023-11-12 19:51:19.746756 pysource_minimize-0.6.2/pysource_minimize/py.typed
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 pysource_minimize-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1465 2023-10-22 07:19:25.553357 pysource_minimize-0.6.3/README.md
+-rw-r--r--   0        0        0     1315 2024-04-23 19:15:07.386627 pysource_minimize-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-23 19:15:07.374626 pysource_minimize-0.6.3/pysource_minimize/__init__.py
+-rw-r--r--   0        0        0     2015 2023-11-03 18:43:29.034047 pysource_minimize-0.6.3/pysource_minimize/__main__.py
+-rw-r--r--   0        0        0     3015 2024-04-23 19:13:52.233048 pysource_minimize-0.6.3/pysource_minimize/_minimize.py
+-rw-r--r--   0        0        0    10401 2024-04-23 19:09:08.811056 pysource_minimize-0.6.3/pysource_minimize/_minimize_base.py
+-rw-r--r--   0        0        0    24292 2024-04-23 19:09:08.823056 pysource_minimize-0.6.3/pysource_minimize/_minimize_structure.py
+-rw-r--r--   0        0        0     2442 2023-11-12 19:51:19.746756 pysource_minimize-0.6.3/pysource_minimize/_minimize_value.py
+-rw-r--r--   0        0        0      337 2024-04-23 19:09:08.851057 pysource_minimize-0.6.3/pysource_minimize/_utils.py
+-rw-r--r--   0        0        0        0 2023-11-12 19:51:19.746756 pysource_minimize-0.6.3/pysource_minimize/py.typed
+-rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 pysource_minimize-0.6.3/PKG-INFO
```

### Comparing `pysource_minimize-0.6.2/README.md` & `pysource_minimize-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pysource_minimize-0.6.2/pyproject.toml` & `pysource_minimize-0.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysource-minimize"
-version = "0.6.2"
+version = "0.6.3"
 description = "minimize python source code"
 authors = ["Frank Hoffmann"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pysource_minimize"}]
 
 [tool.commitizen]
```

### Comparing `pysource_minimize-0.6.2/pysource_minimize/__main__.py` & `pysource_minimize-0.6.3/pysource_minimize/__main__.py`

 * *Files identical despite different names*

### Comparing `pysource_minimize-0.6.2/pysource_minimize/_minimize.py` & `pysource_minimize-0.6.3/pysource_minimize/_minimize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
+
 import ast
 import warnings
+from collections.abc import Callable
 
 from ._minimize_base import equal_ast
 from ._minimize_structure import MinimizeStructure
 from ._minimize_value import MinimizeValue
 from ._utils import parse
 from ._utils import unparse
 
@@ -47,16 +50,24 @@
             last_success = 0
         else:
             last_success += 1
 
     return current_ast
 
 
+class CouldNotMinimize(ValueError):
+    """Raised to indicate that the source code could not be minimized."""
+
+
 def minimize(
-    source: str, checker, *, progress_callback=lambda current, total: None, retries=1
+    source: str,
+    checker: Callable[[str], bool],
+    *,
+    progress_callback: Callable[[int, int], object] = lambda current, total: None,
+    retries: int = 1,
 ) -> str:
     """
     minimzes the source code
 
     Args:
         source: the source code to minimize
         checker: a function which gets the source and returns `True` when the criteria is fullfilled.
@@ -76,15 +87,18 @@
                 compile(source, "<string>", "exec")
         except:
             return False
 
         return checker(source)
 
     if not source_checker(original_ast):
-        raise ValueError("ast.unparse removes the error minimize can not help here")
+        raise CouldNotMinimize(
+            "Source code cannot be minimized: the error failed to reproduce "
+            "after roundtripping the source using `ast.parse()` and `ast.unparse()`"
+        )
 
     minimized_ast = minimize_ast(
         original_ast,
         source_checker,
         progress_callback=progress_callback,
         retries=retries,
     )
```

### Comparing `pysource_minimize-0.6.2/pysource_minimize/_minimize_base.py` & `pysource_minimize-0.6.3/pysource_minimize/_minimize_base.py`

 * *Files identical despite different names*

### Comparing `pysource_minimize-0.6.2/pysource_minimize/_minimize_structure.py` & `pysource_minimize-0.6.3/pysource_minimize/_minimize_structure.py`

 * *Files identical despite different names*

### Comparing `pysource_minimize-0.6.2/pysource_minimize/_minimize_value.py` & `pysource_minimize-0.6.3/pysource_minimize/_minimize_value.py`

 * *Files identical despite different names*

### Comparing `pysource_minimize-0.6.2/PKG-INFO` & `pysource_minimize-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysource-minimize
-Version: 0.6.2
+Version: 0.6.3
 Summary: minimize python source code
 License: MIT
 Author: Frank Hoffmann
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

