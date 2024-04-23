# Comparing `tmp/vadi-0.0.2.tar.gz` & `tmp/vadi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vadi-0.0.2.tar", max compression
+gzip compressed data, was "vadi-0.0.3.tar", max compression
```

## Comparing `vadi-0.0.2.tar` & `vadi-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2024-04-07 18:58:17.517436 vadi-0.0.2/LICENSE
--rw-r--r--   0        0        0     2776 2024-04-23 09:41:26.986913 vadi-0.0.2/README.md
--rw-r--r--   0        0        0     2006 2024-04-23 09:49:44.283587 vadi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 18:58:47.327273 vadi-0.0.2/src/utils/__init__.py
--rw-r--r--   0        0        0      430 2024-04-22 15:10:35.660108 vadi-0.0.2/src/utils/console.py
--rw-r--r--   0        0        0      188 2024-04-08 16:57:12.949917 vadi-0.0.2/src/utils/constants.py
--rw-r--r--   0        0        0      239 2024-04-22 15:13:33.966777 vadi-0.0.2/src/utils/helpers.py
--rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.2/src/utils/py.typed
--rw-r--r--   0        0        0        0 2024-04-07 18:58:17.517436 vadi-0.0.2/src/vadi/__init__.py
--rw-r--r--   0        0        0     3789 2024-04-22 15:12:06.623443 vadi-0.0.2/src/vadi/interpreter.py
--rw-r--r--   0        0        0     2066 2024-04-22 15:12:06.623443 vadi-0.0.2/src/vadi/lexer.py
--rw-r--r--   0        0        0      454 2024-04-22 15:12:06.623443 vadi-0.0.2/src/vadi/memory.py
--rw-r--r--   0        0        0     2997 2024-04-22 15:12:06.623443 vadi-0.0.2/src/vadi/parser.py
--rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.2/src/vadi/py.typed
--rw-r--r--   0        0        0     1054 2024-04-22 15:10:35.660108 vadi-0.0.2/src/vadi/repl.py
--rw-r--r--   0        0        0      747 2024-04-08 03:01:51.703473 vadi-0.0.2/src/vadi/tokens.py
--rw-r--r--   0        0        0      484 2024-04-22 15:13:33.966777 vadi-0.0.2/src/vadi/typedef.py
--rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 vadi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-07 18:58:17.517436 vadi-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2826 2024-04-23 09:51:12.136922 vadi-0.0.3/README.md
+-rw-r--r--   0        0        0     2006 2024-04-23 09:51:55.780256 vadi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 18:58:47.327273 vadi-0.0.3/src/utils/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-22 15:10:35.660108 vadi-0.0.3/src/utils/console.py
+-rw-r--r--   0        0        0      188 2024-04-08 16:57:12.949917 vadi-0.0.3/src/utils/constants.py
+-rw-r--r--   0        0        0      239 2024-04-22 15:13:33.966777 vadi-0.0.3/src/utils/helpers.py
+-rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.3/src/utils/py.typed
+-rw-r--r--   0        0        0        0 2024-04-07 18:58:17.517436 vadi-0.0.3/src/vadi/__init__.py
+-rw-r--r--   0        0        0     3789 2024-04-22 15:12:06.623443 vadi-0.0.3/src/vadi/interpreter.py
+-rw-r--r--   0        0        0     2066 2024-04-22 15:12:06.623443 vadi-0.0.3/src/vadi/lexer.py
+-rw-r--r--   0        0        0      454 2024-04-22 15:12:06.623443 vadi-0.0.3/src/vadi/memory.py
+-rw-r--r--   0        0        0     2997 2024-04-22 15:12:06.623443 vadi-0.0.3/src/vadi/parser.py
+-rw-r--r--   0        0        0       57 2024-04-07 19:51:41.123190 vadi-0.0.3/src/vadi/py.typed
+-rw-r--r--   0        0        0     1054 2024-04-22 15:10:35.660108 vadi-0.0.3/src/vadi/repl.py
+-rw-r--r--   0        0        0      747 2024-04-08 03:01:51.703473 vadi-0.0.3/src/vadi/tokens.py
+-rw-r--r--   0        0        0      484 2024-04-22 15:13:33.966777 vadi-0.0.3/src/vadi/typedef.py
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 vadi-0.0.3/PKG-INFO
```

### Comparing `vadi-0.0.2/LICENSE` & `vadi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vadi-0.0.2/README.md` & `vadi-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Banner](./assets/banner.png)
+![Banner](https://raw.githubusercontent.com/Vyogami/Vadi/main/assets/banner.png)
 
 ---
 
 Vadi is a simple, interpreted and dynamically-typed programming language. It comes with its own tool called a REPL, which lets you try out code quickly.
 
 The interpreter which is the part of Vadi that runs your code, uses a technique named "Recursive Descent Parsing." This technique helps the interpreter understand your high-level code by creating a data-structure called a `parse tree`. Then, the interpreter uses this parse tree to figure out what your code is asking it to do.You can check out the Vadi's [Syntax Grammar](#grammar) in BNF for more information.
```

### Comparing `vadi-0.0.2/pyproject.toml` & `vadi-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vadi"
-version = "0.0.2"
+version = "0.0.3"
 description = "REPL of a simple, interpreted and statically-typed programming language."
 authors = ["Shivam Shandilya <fvyogami@gmail.com>"]
 repository = "https://github.com/vyogami/Vadi"
 documentation = "https://github.com/vyogami/Vadi/blob/main/CONTRIBUTING.md"
 readme = "README.md"
 packages = [
   { include = "vadi", from = "src" },
```

### Comparing `vadi-0.0.2/src/vadi/interpreter.py` & `vadi-0.0.3/src/vadi/interpreter.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.2/src/vadi/lexer.py` & `vadi-0.0.3/src/vadi/lexer.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.2/src/vadi/parser.py` & `vadi-0.0.3/src/vadi/parser.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.2/src/vadi/repl.py` & `vadi-0.0.3/src/vadi/repl.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.2/src/vadi/tokens.py` & `vadi-0.0.3/src/vadi/tokens.py`

 * *Files identical despite different names*

### Comparing `vadi-0.0.2/PKG-INFO` & `vadi-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vadi
-Version: 0.0.2
+Version: 0.0.3
 Summary: REPL of a simple, interpreted and statically-typed programming language.
 Home-page: https://github.com/vyogami/Vadi
 Author: Shivam Shandilya
 Author-email: fvyogami@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Project-URL: Documentation, https://github.com/vyogami/Vadi/blob/main/CONTRIBUTING.md
 Project-URL: Repository, https://github.com/vyogami/Vadi
 Description-Content-Type: text/markdown
 
-![Banner](./assets/banner.png)
+![Banner](https://raw.githubusercontent.com/Vyogami/Vadi/main/assets/banner.png)
 
 ---
 
 Vadi is a simple, interpreted and dynamically-typed programming language. It comes with its own tool called a REPL, which lets you try out code quickly.
 
 The interpreter which is the part of Vadi that runs your code, uses a technique named "Recursive Descent Parsing." This technique helps the interpreter understand your high-level code by creating a data-structure called a `parse tree`. Then, the interpreter uses this parse tree to figure out what your code is asking it to do.You can check out the Vadi's [Syntax Grammar](#grammar) in BNF for more information.
```

