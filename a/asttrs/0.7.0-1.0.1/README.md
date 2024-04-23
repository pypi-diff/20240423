# Comparing `tmp/asttrs-0.7.0.tar.gz` & `tmp/asttrs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asttrs-0.7.0.tar", max compression
+gzip compressed data, was "asttrs-1.0.1.tar", last modified: Tue Apr 23 16:38:07 2024, max compression
```

## Comparing `asttrs-0.7.0.tar` & `asttrs-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,30 @@
--rw-r--r--   0        0        0     1062 2021-09-26 15:04:09.993793 asttrs-0.7.0/LICENSE
--rw-r--r--   0        0        0       46 2021-09-26 16:26:26.868873 asttrs-0.7.0/README.md
--rw-r--r--   0        0        0      591 2022-08-21 10:09:29.888739 asttrs-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       28 2022-04-04 10:33:54.667640 asttrs-0.7.0/src/asttrs/__init__.py
--rw-r--r--   0        0        0     1492 2022-04-04 12:14:44.791791 asttrs-0.7.0/src/asttrs/_ast.py
--rw-r--r--   0        0        0     5335 2022-04-04 10:02:31.255617 asttrs-0.7.0/src/asttrs/_base.py
--rw-r--r--   0        0        0    53636 2022-08-21 10:07:36.318592 asttrs-0.7.0/src/asttrs/_py3_10.py
--rw-r--r--   0        0        0     8844 2022-04-04 11:49:24.014295 asttrs-0.7.0/src/asttrs/_py3_7.py
--rw-r--r--   0        0        0     9314 2022-08-21 10:06:51.421788 asttrs-0.7.0/src/asttrs/_py3_8.py
--rw-r--r--   0        0        0    41115 2022-08-21 10:05:49.788729 asttrs-0.7.0/src/asttrs/_py3_9.py
--rw-r--r--   0        0        0      857 2022-04-04 09:33:31.909519 asttrs-0.7.0/src/asttrs/utils.py
--rw-r--r--   0        0        0      785 2022-08-21 10:12:41.082104 asttrs-0.7.0/setup.py
--rw-r--r--   0        0        0      752 2022-08-21 10:12:41.082366 asttrs-0.7.0/PKG-INFO
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1062 2021-09-26 15:04:09.000000 asttrs-1.0.1/LICENSE
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-23 16:38:07.018184 asttrs-1.0.1/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2547 2023-12-23 20:09:41.000000 asttrs-1.0.1/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      546 2024-04-23 16:37:52.000000 asttrs-1.0.1/pyproject.toml
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2024-04-23 16:38:07.018184 asttrs-1.0.1/setup.cfg
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.006183 asttrs-1.0.1/src/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/src/asttrs/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       28 2022-04-04 10:33:54.000000 asttrs-1.0.1/src/asttrs/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1892 2024-04-23 16:30:14.000000 asttrs-1.0.1/src/asttrs/_ast.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5719 2023-12-31 14:22:25.000000 asttrs-1.0.1/src/asttrs/_base.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    53618 2023-12-23 17:33:56.000000 asttrs-1.0.1/src/asttrs/_py3_10.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    56914 2024-04-23 16:24:32.000000 asttrs-1.0.1/src/asttrs/_py3_11.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    60807 2023-12-23 19:24:22.000000 asttrs-1.0.1/src/asttrs/_py3_12.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-12-23 17:28:57.000000 asttrs-1.0.1/src/asttrs/_py3_7.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9314 2023-12-23 17:29:36.000000 asttrs-1.0.1/src/asttrs/_py3_8.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    41099 2023-12-23 17:30:42.000000 asttrs-1.0.1/src/asttrs/_py3_9.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      857 2023-12-27 04:28:14.000000 asttrs-1.0.1/src/asttrs/utils.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/src/asttrs.egg-info/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      512 2024-04-23 16:38:07.000000 asttrs-1.0.1/src/asttrs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        7 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/top_level.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/tests/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:53:28.000000 asttrs-1.0.1/tests/test_expr.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1266 2022-04-04 12:18:55.000000 asttrs-1.0.1/tests/test_misc.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 17:08:43.000000 asttrs-1.0.1/tests/test_operator.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:54:10.000000 asttrs-1.0.1/tests/test_stmt.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      420 2023-12-23 18:31:52.000000 asttrs-1.0.1/tests/test_utils.py
```

### Comparing `asttrs-0.7.0/LICENSE` & `asttrs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asttrs-0.7.0/src/asttrs/_ast.py` & `asttrs-1.0.1/src/asttrs/_ast.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Abstract Syntax Trees: https://docs.python.org/3/library/ast.html
 """
+
 import ast as _ast
 import sys
+import warnings
 from typing import Type
 
 from ._base import AST, immutable
 
 if (3, 7) <= sys.version_info < (3, 8):
     import asttrs._py3_7 as _asttrs
     from asttrs._py3_7 import *  # noqa
@@ -28,16 +30,33 @@
 
 elif (3, 10) <= sys.version_info < (3, 11):
     import asttrs._py3_10 as _asttrs
     from asttrs._py3_10 import *  # noqa
 
     pass
 
+elif (3, 11) <= sys.version_info < (3, 12):
+    import asttrs._py3_11 as _asttrs
+    from asttrs._py3_11 import *  # noqa
+
+    pass
+
 else:
-    raise ImportError("Support only Python 3.7 to 3.10")
+    import asttrs._py3_12 as _asttrs
+    from asttrs._py3_12 import *  # noqa
+
+    pass
+
+
+if (3, 11) <= sys.version_info:
+    warnings.warn(
+        "For Python 3.11 and later, a few ast types may not be supported, such as FunctionType, ParamSpec, TypeAlias, TypeVar, and etc.",
+        UserWarning,
+    )
+
 
 stmt = getattr(_asttrs, "stmt", AST)
 
 
 @immutable
 class Comment(stmt):
     """A Comment wrapper for convenient purpose, since there's no comment node in ast.
```

### Comparing `asttrs-0.7.0/src/asttrs/_base.py` & `asttrs-1.0.1/src/asttrs/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any
 from typing import Dict as DICT
 from typing import List as LIST
 from typing import Optional
 from typing import Tuple as TUPLE
 from typing import Type, Union
 
-import astor
+import ast_decompiler
 import attr
 import cattr
 
 immutable = attr.s(auto_attribs=True, slots=True, frozen=True, kw_only=True)
 
 
 @immutable
@@ -89,20 +89,32 @@
 
                 kwargs.update({name: value})
 
         return ast_type(**kwargs)
 
     @classmethod
     def from_source(cls, source: str) -> "AST":
+        from ast import Module
 
-        return cls.from_ast(_ast.parse(source))
+        mod = _ast.parse(source)
 
-    def to_source(self) -> str:
+        if cls.__name__ == Module.__name__:
+            return cls.from_ast(mod)
+        
+        assert len(mod.body) == 1
+
+        mod = mod.body[0]
 
-        return astor.to_source(self.to_ast())
+        if cls.__name__ == mod.__class__.__name__:
+            return cls.from_ast(mod)
+        
+        raise TypeError(f"Type dismatch -> got: {mod.__class__.__name__}, expected: {cls.__name__}")
+
+    def to_source(self) -> str:
+        return ast_decompiler.decompile(self.to_ast())
 
     def show(self) -> None:
         print(self.to_source().strip())
 
     @classmethod
     def from_file(cls, filepath: str) -> "AST":
```

### Comparing `asttrs-0.7.0/src/asttrs/_py3_10.py` & `asttrs-1.0.1/src/asttrs/_py3_10.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,27 +274,27 @@
     ...             target=Attribute(
     ...                 value=Name(id='a', ctx=Load()),
     ...                 attr='b',
     ...                 ctx=Store()),
     ...             annotation=Name(id='int', ctx=Load()),
     ...             simple=0)],
     ...     type_ignores=[]).show()
-    a.b: int
+    (a.b): int
 
     >>> Module(
     ...     body=[
     ...         AnnAssign(
     ...             target=Subscript(
     ...                 value=Name(id='a', ctx=Load()),
     ...                 slice=Constant(value=1),
     ...                 ctx=Store()),
     ...             annotation=Name(id='int', ctx=Load()),
     ...             simple=0)],
     ...     type_ignores=[]).show()
-    a[1]: int
+    (a[1]): int
     """
 
     target: "expr"
     annotation: "expr"
     value: "expr" = None
     simple: "int"
 
@@ -718,15 +718,15 @@
 
     >>> Expression(
     ...     body=BoolOp(
     ...         op=Or(),
     ...         values=[
     ...             Name(id='x', ctx=Load()),
     ...             Name(id='y', ctx=Load())])).show()
-    (x or y)
+    x or y
     """
 
     op: "boolop"
     values: LIST["expr"] = attr.ib(factory=list)
 
 
 @immutable
@@ -759,15 +759,15 @@
     Examples:
 
     >>> Expression(
     ...     body=BinOp(
     ...         left=Name(id='x', ctx=Load()),
     ...         op=Add(),
     ...         right=Name(id='y', ctx=Load()))).show()
-    (x + y)
+    x + y
     """
 
     left: "expr"
     op: "operator"
     right: "expr"
 
 
@@ -779,15 +779,15 @@
 
     Examples:
 
     >>> Expression(
     ...     body=UnaryOp(
     ...         op=Not(),
     ...         operand=Name(id='x', ctx=Load()))).show()
-    (not x)
+    not x
     """
 
     op: "unaryop"
     operand: "expr"
 
 
 @immutable
@@ -828,15 +828,15 @@
     Examples:
 
     >>> Expression(
     ...     body=IfExp(
     ...         test=Name(id='b', ctx=Load()),
     ...         body=Name(id='a', ctx=Load()),
     ...         orelse=Name(id='c', ctx=Load()))).show()
-    (a if b else c)
+    a if b else c
     """
 
     test: "expr"
     body: "expr"
     orelse: "expr"
 
 
@@ -942,15 +942,15 @@
     ...             right=Constant(value=2)),
     ...         generators=[
     ...             comprehension(
     ...                 target=Name(id='x', ctx=Store()),
     ...                 iter=Name(id='numbers', ctx=Load()),
     ...                 ifs=[],
     ...                 is_async=0)])).show()
-    {x: (x ** 2) for x in numbers}
+    {x: x ** 2 for x in numbers}
 
     >>> Expression(
     ...     body=SetComp(
     ...         elt=Name(id='x', ctx=Load()),
     ...         generators=[
     ...             comprehension(
     ...                 target=Name(id='x', ctx=Store()),
@@ -1064,15 +1064,15 @@
     ...         left=Constant(value=1),
     ...         ops=[
     ...             LtE(),
     ...             Lt()],
     ...         comparators=[
     ...             Name(id='a', ctx=Load()),
     ...             Constant(value=10)])).show()
-    (1 <= a < 10)
+    1 <= a < 10
     """
 
     left: "expr"
     ops: LIST["cmpop"] = attr.ib(factory=list)
     comparators: LIST["expr"] = attr.ib(factory=list)
 
 
@@ -1156,15 +1156,15 @@
     ...                     args=[
     ...                         Name(id='a', ctx=Load())],
     ...                     keywords=[]),
     ...                 conversion=-1,
     ...                 format_spec=JoinedStr(
     ...                     values=[
     ...                         Constant(value='.3')]))])).show()
-    f""\"sin({a}) is {sin(a):.3}""\"
+    f'sin({a}) is {sin(a):.3}'
     """
 
     values: LIST["expr"] = attr.ib(factory=list)
 
 
 @immutable
 class Constant(expr):
@@ -1174,15 +1174,15 @@
     such as a number, string or ``None``, but also immutable container types
     (tuples and frozensets) if all of their elements are constant.
 
     Examples:
 
     >>> Expression(
     ...     body=Constant(value=123)).show()
-    (123)
+    123
     """
 
     value: "constant"
     kind: "string" = None
 
 
 @immutable
@@ -1654,15 +1654,15 @@
     ...                     pattern=MatchValue(
     ...                         value=Constant(value='Relevant')),
     ...                     body=[
     ...                         Expr(
     ...                             value=Constant(value=Ellipsis))])])],
     ...     type_ignores=[]).show()
     match x:
-        case "Relevant":
+        case 'Relevant':
             ...
     """
 
     value: "expr"
 
 
 @immutable
@@ -1956,15 +1956,15 @@
     ...                                     MatchAs(name='x')]),
     ...                             MatchAs(name='y')]),
     ...                     body=[
     ...                         Expr(
     ...                             value=Constant(value=Ellipsis))])])],
     ...     type_ignores=[]).show()
     match x:
-        case [x] | (y):
+        case [x] | y:
             ...
     """
 
     patterns: LIST["pattern"] = attr.ib(factory=list)
 
 
 class type_ignore(AST):
```

### Comparing `asttrs-0.7.0/src/asttrs/_py3_7.py` & `asttrs-1.0.1/src/asttrs/_py3_7.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     names: LIST["alias"] = attr.ib(factory=list)
 
 
 @immutable
 class ImportFrom(stmt):
     module: "identifier" = None
     names: LIST["alias"] = attr.ib(factory=list)
-    level: "int" = None
+    level: "int" = 0
 
 
 @immutable
 class Global(stmt):
     names: LIST["identifier"] = attr.ib(factory=list)
 
 
@@ -311,15 +311,15 @@
 class Str(expr):
     s: "string"
 
 
 @immutable
 class FormattedValue(expr):
     value: "expr"
-    conversion: "int" = None
+    conversion: "int" = 0
     format_spec: "expr" = None
 
 
 @immutable
 class JoinedStr(expr):
     values: LIST["expr"] = attr.ib(factory=list)
```

### Comparing `asttrs-0.7.0/src/asttrs/_py3_8.py` & `asttrs-1.0.1/src/asttrs/_py3_8.py`

 * *Files identical despite different names*

### Comparing `asttrs-0.7.0/src/asttrs/_py3_9.py` & `asttrs-1.0.1/src/asttrs/_py3_9.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,27 +274,27 @@
     ...             target=Attribute(
     ...                 value=Name(id='a', ctx=Load()),
     ...                 attr='b',
     ...                 ctx=Store()),
     ...             annotation=Name(id='int', ctx=Load()),
     ...             simple=0)],
     ...     type_ignores=[]).show()
-    a.b: int
+    (a.b): int
 
     >>> Module(
     ...     body=[
     ...         AnnAssign(
     ...             target=Subscript(
     ...                 value=Name(id='a', ctx=Load()),
     ...                 slice=Constant(value=1),
     ...                 ctx=Store()),
     ...             annotation=Name(id='int', ctx=Load()),
     ...             simple=0)],
     ...     type_ignores=[]).show()
-    a[1]: int
+    (a[1]): int
     """
 
     target: "expr"
     annotation: "expr"
     value: "expr" = None
     simple: "int"
 
@@ -706,15 +706,15 @@
 
     >>> Expression(
     ...     body=BoolOp(
     ...         op=Or(),
     ...         values=[
     ...             Name(id='x', ctx=Load()),
     ...             Name(id='y', ctx=Load())])).show()
-    (x or y)
+    x or y
     """
 
     op: "boolop"
     values: LIST["expr"] = attr.ib(factory=list)
 
 
 @immutable
@@ -747,15 +747,15 @@
     Examples:
 
     >>> Expression(
     ...     body=BinOp(
     ...         left=Name(id='x', ctx=Load()),
     ...         op=Add(),
     ...         right=Name(id='y', ctx=Load()))).show()
-    (x + y)
+    x + y
     """
 
     left: "expr"
     op: "operator"
     right: "expr"
 
 
@@ -767,15 +767,15 @@
 
     Examples:
 
     >>> Expression(
     ...     body=UnaryOp(
     ...         op=Not(),
     ...         operand=Name(id='x', ctx=Load()))).show()
-    (not x)
+    not x
     """
 
     op: "unaryop"
     operand: "expr"
 
 
 @immutable
@@ -816,15 +816,15 @@
     Examples:
 
     >>> Expression(
     ...     body=IfExp(
     ...         test=Name(id='b', ctx=Load()),
     ...         body=Name(id='a', ctx=Load()),
     ...         orelse=Name(id='c', ctx=Load()))).show()
-    (a if b else c)
+    a if b else c
     """
 
     test: "expr"
     body: "expr"
     orelse: "expr"
 
 
@@ -930,15 +930,15 @@
     ...             right=Constant(value=2)),
     ...         generators=[
     ...             comprehension(
     ...                 target=Name(id='x', ctx=Store()),
     ...                 iter=Name(id='numbers', ctx=Load()),
     ...                 ifs=[],
     ...                 is_async=0)])).show()
-    {x: (x ** 2) for x in numbers}
+    {x: x ** 2 for x in numbers}
 
     >>> Expression(
     ...     body=SetComp(
     ...         elt=Name(id='x', ctx=Load()),
     ...         generators=[
     ...             comprehension(
     ...                 target=Name(id='x', ctx=Store()),
@@ -1052,15 +1052,15 @@
     ...         left=Constant(value=1),
     ...         ops=[
     ...             LtE(),
     ...             Lt()],
     ...         comparators=[
     ...             Name(id='a', ctx=Load()),
     ...             Constant(value=10)])).show()
-    (1 <= a < 10)
+    1 <= a < 10
     """
 
     left: "expr"
     ops: LIST["cmpop"] = attr.ib(factory=list)
     comparators: LIST["expr"] = attr.ib(factory=list)
 
 
@@ -1144,15 +1144,15 @@
     ...                     args=[
     ...                         Name(id='a', ctx=Load())],
     ...                     keywords=[]),
     ...                 conversion=-1,
     ...                 format_spec=JoinedStr(
     ...                     values=[
     ...                         Constant(value='.3')]))])).show()
-    f""\"sin({a}) is {sin(a):.3}""\"
+    f'sin({a}) is {sin(a):.3}'
     """
 
     values: LIST["expr"] = attr.ib(factory=list)
 
 
 @immutable
 class Constant(expr):
@@ -1162,15 +1162,15 @@
     such as a number, string or ``None``, but also immutable container types
     (tuples and frozensets) if all of their elements are constant.
 
     Examples:
 
     >>> Expression(
     ...     body=Constant(value=123)).show()
-    (123)
+    123
     """
 
     value: "constant"
     kind: "string" = None
 
 
 @immutable
```

### Comparing `asttrs-0.7.0/src/asttrs/utils.py` & `asttrs-1.0.1/src/asttrs/utils.py`

 * *Files identical despite different names*

