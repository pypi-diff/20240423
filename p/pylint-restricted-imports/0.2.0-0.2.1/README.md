# Comparing `tmp/pylint_restricted_imports-0.2.0.tar.gz` & `tmp/pylint_restricted_imports-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_restricted_imports-0.2.0.tar", max compression
+gzip compressed data, was "pylint_restricted_imports-0.2.1.tar", max compression
```

## Comparing `pylint_restricted_imports-0.2.0.tar` & `pylint_restricted_imports-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1052 2021-07-08 11:19:36.000000 pylint_restricted_imports-0.2.0/LICENSE
--rw-r--r--   0        0        0     1950 2021-07-09 13:59:48.000000 pylint_restricted_imports-0.2.0/README.rst
--rw-r--r--   0        0        0     7320 2024-01-10 15:13:47.660419 pylint_restricted_imports-0.2.0/pylint_restricted_imports/__init__.py
--rw-r--r--   0        0        0     1210 2024-01-10 15:17:53.496232 pylint_restricted_imports-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 pylint_restricted_imports-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2021-07-08 11:19:36.000000 pylint_restricted_imports-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1950 2021-07-09 13:59:48.000000 pylint_restricted_imports-0.2.1/README.rst
+-rw-r--r--   0        0        0     7421 2024-04-23 09:50:30.037148 pylint_restricted_imports-0.2.1/pylint_restricted_imports/__init__.py
+-rw-r--r--   0        0        0     1209 2024-04-23 09:56:42.429859 pylint_restricted_imports-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 pylint_restricted_imports-0.2.1/PKG-INFO
```

### Comparing `pylint_restricted_imports-0.2.0/LICENSE` & `pylint_restricted_imports-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_restricted_imports-0.2.0/README.rst` & `pylint_restricted_imports-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pylint_restricted_imports-0.2.0/pylint_restricted_imports/__init__.py` & `pylint_restricted_imports-0.2.1/pylint_restricted_imports/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from collections import defaultdict
 from typing import Optional, List, Union, Set, Dict
 
-from astroid import Import, Module, ImportFrom, AstroidBuildingException
+from astroid import Import, Module, ImportFrom
+
+try:
+    from astroid.exceptions import AstroidBuildingError
+except ImportError:
+    from astroid import AstroidBuildingError
 
 try:
     from astroid.nodes.node_classes import NodeNG
 except ImportError:
     from astroid.node_classes import NodeNG
 from pylint.checkers import BaseChecker
```

### Comparing `pylint_restricted_imports-0.2.0/pyproject.toml` & `pylint_restricted_imports-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-restricted-imports"
-version = "0.2.0"
+version = "0.2.1"
 license = "MIT"
 description = "pylint-restricted-imports is a Pylint plugin to restrict what imports are allowed in different modules"
 authors = [
     "Pexip AS <packaging@pexip.com>",
     "Huw Jones <huw@pexip.com>",
 ]
 repository = "https://github.com/pexip/pylint-restricted-imports"
@@ -36,8 +36,8 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 astroid = ">=1.0"
 pylint = ">=2.16"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=1.0"
-black = "^23.12.1"
+black = "^24.3.0"
```

### Comparing `pylint_restricted_imports-0.2.0/PKG-INFO` & `pylint_restricted_imports-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-restricted-imports
-Version: 0.2.0
+Version: 0.2.1
 Summary: pylint-restricted-imports is a Pylint plugin to restrict what imports are allowed in different modules
 Home-page: https://github.com/pexip/pylint-restricted-imports
 License: MIT
 Keywords: pylint,plugin,imports
 Author: Pexip AS
 Author-email: packaging@pexip.com
 Requires-Python: >=3.8,<4.0
```

