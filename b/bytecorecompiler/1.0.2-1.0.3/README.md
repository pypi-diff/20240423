# Comparing `tmp/bytecorecompiler-1.0.2.tar.gz` & `tmp/bytecorecompiler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecorecompiler-1.0.2.tar", last modified: Mon Apr 22 14:58:48 2024, max compression
+gzip compressed data, was "bytecorecompiler-1.0.3.tar", last modified: Tue Apr 23 21:48:28 2024, max compression
```

## Comparing `bytecorecompiler-1.0.2.tar` & `bytecorecompiler-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-22 14:58:48.829845 bytecorecompiler-1.0.2/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1074 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5070 2024-04-22 14:58:48.829845 bytecorecompiler-1.0.2/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4332 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/README.md
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      925 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/pyproject.toml
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-22 14:58:48.829845 bytecorecompiler-1.0.2/setup.cfg
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-22 14:58:48.825845 bytecorecompiler-1.0.2/src/
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-22 14:58:48.825845 bytecorecompiler-1.0.2/src/bytecorecompiler/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1120 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/compiler.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      124 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/exception.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2995 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/lexical_analysis.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      701 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/parser.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/py.typed
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2897 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/semantic_analysis.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1169 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/syntax.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4692 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/syntax_analysis.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3913 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/src/bytecorecompiler/syntax_tree.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-22 14:58:48.829845 bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5070 2024-04-22 14:58:48.000000 bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      788 2024-04-22 14:58:48.000000 bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-22 14:58:48.000000 bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       16 2024-04-22 14:58:48.000000 bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       17 2024-04-22 14:58:48.000000 bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/top_level.txt
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-22 14:58:48.829845 bytecorecompiler-1.0.2/tests/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6183 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/tests/test_compiler.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1802 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/tests/test_examples.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3011 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/tests/test_lexical_analysis.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1553 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/tests/test_parser.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3765 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/tests/test_semantic_analysis.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7437 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/tests/test_syntax_analysis.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1611 2024-04-22 14:57:11.000000 bytecorecompiler-1.0.2/tests/test_syntax_tree.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:48:28.229433 bytecorecompiler-1.0.3/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1074 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5070 2024-04-23 21:48:28.229433 bytecorecompiler-1.0.3/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4332 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/README.md
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      925 2024-04-23 21:43:57.000000 bytecorecompiler-1.0.3/pyproject.toml
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-23 21:48:28.229433 bytecorecompiler-1.0.3/setup.cfg
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:48:28.225433 bytecorecompiler-1.0.3/src/
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:48:28.225433 bytecorecompiler-1.0.3/src/bytecorecompiler/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1120 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/compiler.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      124 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/exception.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2995 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/lexical_analysis.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      701 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/parser.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/py.typed
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2897 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/semantic_analysis.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1169 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/syntax.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4692 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/syntax_analysis.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3913 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/src/bytecorecompiler/syntax_tree.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:48:28.229433 bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5070 2024-04-23 21:48:28.000000 bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      788 2024-04-23 21:48:28.000000 bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-23 21:48:28.000000 bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       16 2024-04-23 21:48:28.000000 bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       17 2024-04-23 21:48:28.000000 bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:48:28.229433 bytecorecompiler-1.0.3/tests/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6183 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/tests/test_compiler.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1802 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/tests/test_examples.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3011 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/tests/test_lexical_analysis.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1553 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/tests/test_parser.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3765 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/tests/test_semantic_analysis.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7437 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/tests/test_syntax_analysis.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1611 2024-04-23 21:42:24.000000 bytecorecompiler-1.0.3/tests/test_syntax_tree.py
```

### Comparing `bytecorecompiler-1.0.2/LICENSE` & `bytecorecompiler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/PKG-INFO` & `bytecorecompiler-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bytecorecompiler
-Version: 1.0.2
+Version: 1.0.3
 Summary: A compiler that transforms ByteCore assembly code into executable memory bytes, seamlessly bridging the gap between high-level assembly instructions and the ByteCore Emulator's low-level functionality.
 Author-email: Joakim Winum Lien <joakim@winum.xyz>
 Project-URL: Homepage, https://github.com/joakimwinum/bytecorecompiler
 Project-URL: Bug Tracker, https://github.com/joakimwinum/bytecorecompiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: bytecore==1.1.0
+Requires-Dist: bytecore==1.1.1
 
 # ByteCoreCompiler
 
 The ByteCoreCompiler transforms ByteCore assembly code into a 64KB memory byte array, compatible with the [ByteCore Emulator](https://github.com/joakimwinum/bytecore). It includes features to identify syntax errors and guide developers through debugging their code.
 
 ## Overview
```

### Comparing `bytecorecompiler-1.0.2/README.md` & `bytecorecompiler-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/pyproject.toml` & `bytecorecompiler-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bytecorecompiler"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Joakim Winum Lien", email="joakim@winum.xyz" },
 ]
 description = "A compiler that transforms ByteCore assembly code into executable memory bytes, seamlessly bridging the gap between high-level assembly instructions and the ByteCore Emulator's low-level functionality."
 dependencies = [
-  "bytecore==1.1.0"
+  "bytecore==1.1.1"
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler/compiler.py` & `bytecorecompiler-1.0.3/src/bytecorecompiler/compiler.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler/lexical_analysis.py` & `bytecorecompiler-1.0.3/src/bytecorecompiler/lexical_analysis.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler/parser.py` & `bytecorecompiler-1.0.3/src/bytecorecompiler/parser.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler/semantic_analysis.py` & `bytecorecompiler-1.0.3/src/bytecorecompiler/semantic_analysis.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler/syntax.py` & `bytecorecompiler-1.0.3/src/bytecorecompiler/syntax.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler/syntax_analysis.py` & `bytecorecompiler-1.0.3/src/bytecorecompiler/syntax_analysis.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler/syntax_tree.py` & `bytecorecompiler-1.0.3/src/bytecorecompiler/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/PKG-INFO` & `bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bytecorecompiler
-Version: 1.0.2
+Version: 1.0.3
 Summary: A compiler that transforms ByteCore assembly code into executable memory bytes, seamlessly bridging the gap between high-level assembly instructions and the ByteCore Emulator's low-level functionality.
 Author-email: Joakim Winum Lien <joakim@winum.xyz>
 Project-URL: Homepage, https://github.com/joakimwinum/bytecorecompiler
 Project-URL: Bug Tracker, https://github.com/joakimwinum/bytecorecompiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: bytecore==1.1.0
+Requires-Dist: bytecore==1.1.1
 
 # ByteCoreCompiler
 
 The ByteCoreCompiler transforms ByteCore assembly code into a 64KB memory byte array, compatible with the [ByteCore Emulator](https://github.com/joakimwinum/bytecore). It includes features to identify syntax errors and guide developers through debugging their code.
 
 ## Overview
```

### Comparing `bytecorecompiler-1.0.2/src/bytecorecompiler.egg-info/SOURCES.txt` & `bytecorecompiler-1.0.3/src/bytecorecompiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/tests/test_compiler.py` & `bytecorecompiler-1.0.3/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/tests/test_examples.py` & `bytecorecompiler-1.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/tests/test_lexical_analysis.py` & `bytecorecompiler-1.0.3/tests/test_lexical_analysis.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/tests/test_parser.py` & `bytecorecompiler-1.0.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/tests/test_semantic_analysis.py` & `bytecorecompiler-1.0.3/tests/test_semantic_analysis.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/tests/test_syntax_analysis.py` & `bytecorecompiler-1.0.3/tests/test_syntax_analysis.py`

 * *Files identical despite different names*

### Comparing `bytecorecompiler-1.0.2/tests/test_syntax_tree.py` & `bytecorecompiler-1.0.3/tests/test_syntax_tree.py`

 * *Files identical despite different names*

