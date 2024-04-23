# Comparing `tmp/squiral-0.4.3.tar.gz` & `tmp/squiral-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squiral-0.4.3.tar", max compression
+gzip compressed data, was "squiral-0.4.4.tar", max compression
```

## Comparing `squiral-0.4.3.tar` & `squiral-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-09-21 22:59:15.384263 squiral-0.4.3/LICENSE
--rw-r--r--   0        0        0     3182 2023-09-21 22:59:15.384263 squiral-0.4.3/README.md
--rw-r--r--   0        0        0      531 2023-09-21 22:59:15.388264 squiral-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      184 2023-09-21 22:59:15.388264 squiral-0.4.3/squiral/__init__.py
--rw-r--r--   0        0        0      151 2023-09-21 22:59:15.388264 squiral-0.4.3/squiral/__main__.py
--rw-r--r--   0        0        0      744 2023-09-21 22:59:15.388264 squiral-0.4.3/squiral/main.py
--rw-r--r--   0        0        0     2464 2023-09-21 22:59:15.388264 squiral-0.4.3/squiral/squiral.py
--rw-r--r--   0        0        0     3803 1970-01-01 00:00:00.000000 squiral-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-23 20:01:47.169035 squiral-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3182 2024-04-23 20:01:47.173035 squiral-0.4.4/README.md
+-rw-r--r--   0        0        0      531 2024-04-23 20:01:47.173035 squiral-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/__main__.py
+-rw-r--r--   0        0        0      744 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/main.py
+-rw-r--r--   0        0        0     2464 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/squiral.py
+-rw-r--r--   0        0        0     3854 1970-01-01 00:00:00.000000 squiral-0.4.4/PKG-INFO
```

### Comparing `squiral-0.4.3/LICENSE` & `squiral-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `squiral-0.4.3/README.md` & `squiral-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `squiral-0.4.3/pyproject.toml` & `squiral-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squiral"
-version = "0.4.3"
+version = "0.4.4"
 description = "squiral - square spiral"
 authors = ["SADIK KUZU <sadikkuzu@hotmail.com>"]
 homepage = "https://github.com/sadikkuzu/squiral"
 readme = "README.md"
 license = "MIT"
 packages = [{include = "squiral"}]
```

### Comparing `squiral-0.4.3/squiral/main.py` & `squiral-0.4.4/squiral/main.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.3/squiral/squiral.py` & `squiral-0.4.4/squiral/squiral.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.3/PKG-INFO` & `squiral-0.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: squiral
-Version: 0.4.3
+Version: 0.4.4
 Summary: squiral - square spiral
 Home-page: https://github.com/sadikkuzu/squiral
 License: MIT
 Author: SADIK KUZU
 Author-email: sadikkuzu@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # squiral
 [![](https://img.shields.io/pypi/v/squiral)](https://pypi.org/project/squiral/)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![](https://img.shields.io/pypi/pyversions/squiral.svg)](https://pypi.org/project/squiral/)
 [![Downloads](https://pepy.tech/badge/squiral)](https://pepy.tech/project/squiral)
```

