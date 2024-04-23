# Comparing `tmp/pysource_codegen-0.5.1.tar.gz` & `tmp/pysource_codegen-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysource_codegen-0.5.1.tar", max compression
+gzip compressed data, was "pysource_codegen-0.5.2.tar", max compression
```

## Comparing `pysource_codegen-0.5.1.tar` & `pysource_codegen-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2671 2023-11-12 22:20:52.803065 pysource_codegen-0.5.1/README.md
--rw-r--r--   0        0        0     1222 2024-01-23 11:35:54.265315 pysource_codegen-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       31 2024-01-23 11:31:01.343357 pysource_codegen-0.5.1/pysource_codegen/__init__.py
--rw-r--r--   0        0        0      733 2023-09-10 14:14:12.309809 pysource_codegen-0.5.1/pysource_codegen/__main__.py
--rw-r--r--   0        0        0    52513 2024-01-23 11:35:54.269315 pysource_codegen-0.5.1/pysource_codegen/_codegen.py
--rw-r--r--   0        0        0      654 2023-10-01 08:45:04.090187 pysource_codegen-0.5.1/pysource_codegen/_limits.py
--rw-r--r--   0        0        0      349 2024-01-23 11:35:54.269315 pysource_codegen-0.5.1/pysource_codegen/_utils.py
--rw-r--r--   0        0        0        0 2023-09-10 14:14:12.309809 pysource_codegen-0.5.1/pysource_codegen/py.typed
--rw-r--r--   0        0        0    14002 2024-01-23 11:35:54.269315 pysource_codegen-0.5.1/pysource_codegen/static_type_info.py
--rw-r--r--   0        0        0      555 2023-09-10 14:14:12.309809 pysource_codegen-0.5.1/pysource_codegen/types.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 pysource_codegen-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2671 2023-11-12 22:20:52.803065 pysource_codegen-0.5.2/README.md
+-rw-r--r--   0        0        0     1222 2024-04-23 19:37:54.559043 pysource_codegen-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-23 19:37:54.547042 pysource_codegen-0.5.2/pysource_codegen/__init__.py
+-rw-r--r--   0        0        0      733 2023-09-10 14:14:12.309809 pysource_codegen-0.5.2/pysource_codegen/__main__.py
+-rw-r--r--   0        0        0    52569 2024-04-23 19:36:12.180923 pysource_codegen-0.5.2/pysource_codegen/_codegen.py
+-rw-r--r--   0        0        0      654 2023-10-01 08:45:04.090187 pysource_codegen-0.5.2/pysource_codegen/_limits.py
+-rw-r--r--   0        0        0      349 2024-01-23 11:35:54.269315 pysource_codegen-0.5.2/pysource_codegen/_utils.py
+-rw-r--r--   0        0        0        0 2023-09-10 14:14:12.309809 pysource_codegen-0.5.2/pysource_codegen/py.typed
+-rw-r--r--   0        0        0    14002 2024-01-23 11:35:54.269315 pysource_codegen-0.5.2/pysource_codegen/static_type_info.py
+-rw-r--r--   0        0        0      555 2023-09-10 14:14:12.309809 pysource_codegen-0.5.2/pysource_codegen/types.py
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 pysource_codegen-0.5.2/PKG-INFO
```

### Comparing `pysource_codegen-0.5.1/README.md` & `pysource_codegen-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pysource_codegen-0.5.1/pyproject.toml` & `pysource_codegen-0.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysource-codegen"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "pysource_codegen"}]
 
 [tool.commitizen]
 changelog_incremental = true
```

### Comparing `pysource_codegen-0.5.1/pysource_codegen/__main__.py` & `pysource_codegen-0.5.2/pysource_codegen/__main__.py`

 * *Files identical despite different names*

### Comparing `pysource_codegen-0.5.1/pysource_codegen/_codegen.py` & `pysource_codegen-0.5.2/pysource_codegen/_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1040,17 +1040,19 @@
                     fix_tree(value, parents + [(node.__class__.__name__, field)]),
                 )
             if isinstance(value, list):
                 setattr(
                     node,
                     field,
                     [
-                        fix_tree(v, parents + [(node.__class__.__name__, field)])
-                        if isinstance(v, ast.AST)
-                        else v
+                        (
+                            fix_tree(v, parents + [(node.__class__.__name__, field)])
+                            if isinstance(v, ast.AST)
+                            else v
+                        )
                         for v in value
                     ],
                 )
 
         return fix(node, parents)
 
     tree_copy = fix_tree(tree_copy, [])
@@ -1608,16 +1610,15 @@
 @dataclass
 class PartialNode:
     _node_type_name: str
     parent_ref: ParentRef | None
     _defined_attrs: dict
     _context: dict
 
-    def inside(self, spec) -> PartialNode | None:
-        ...
+    def inside(self, spec) -> PartialNode | None: ...
 
     @property
     def parent(self):
         return self.parent_ref.node
 
     def __getattr__(self, name):
         if name.startswith("ctx_"):
```

### Comparing `pysource_codegen-0.5.1/pysource_codegen/_limits.py` & `pysource_codegen-0.5.2/pysource_codegen/_limits.py`

 * *Files identical despite different names*

### Comparing `pysource_codegen-0.5.1/pysource_codegen/static_type_info.py` & `pysource_codegen-0.5.2/pysource_codegen/static_type_info.py`

 * *Files identical despite different names*

### Comparing `pysource_codegen-0.5.1/pysource_codegen/types.py` & `pysource_codegen-0.5.2/pysource_codegen/types.py`

 * *Files identical despite different names*

### Comparing `pysource_codegen-0.5.1/PKG-INFO` & `pysource_codegen-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pysource-codegen
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astunparse (>=1.6.3) ; python_version < "3.9"
 Requires-Dist: typing-extensions (>=4.7.1)
 Description-Content-Type: text/markdown
 
 [![pypi version](https://img.shields.io/pypi/v/pysource-codegen.svg)](https://pypi.org/project/pysource-codegen/)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pysource-codegen)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/pysource-codegen)
```

