# Comparing `tmp/pushable-0.1.6.tar.gz` & `tmp/pushable-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushable-0.1.6.tar", max compression
+gzip compressed data, was "pushable-0.1.7.tar", max compression
```

## Comparing `pushable-0.1.6.tar` & `pushable-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-01-21 16:52:10.856183 pushable-0.1.6/LICENSE
--rw-r--r--   0        0        0     3379 2023-01-25 00:02:56.178128 pushable-0.1.6/README.md
--rw-r--r--   0        0        0     1009 2023-08-19 10:22:31.456169 pushable-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       38 2023-01-22 13:21:18.390008 pushable-0.1.6/src/pushable/__init__.py
--rw-r--r--   0        0        0     8196 2023-02-13 08:27:57.610305 pushable-0.1.6/src/pushable/pushable.py
--rw-r--r--   0        0        0        0 2023-02-13 08:17:35.291343 pushable-0.1.6/src/pushable/py.typed
--rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 pushable-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-21 16:52:10.856183 pushable-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3379 2023-01-25 00:02:56.178128 pushable-0.1.7/README.md
+-rw-r--r--   0        0        0     1027 2024-04-23 19:04:29.843584 pushable-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-01-22 13:21:18.390008 pushable-0.1.7/src/pushable/__init__.py
+-rw-r--r--   0        0        0     8196 2023-02-13 08:27:57.610305 pushable-0.1.7/src/pushable/pushable.py
+-rw-r--r--   0        0        0        0 2023-02-13 08:17:35.291343 pushable-0.1.7/src/pushable/py.typed
+-rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 pushable-0.1.7/PKG-INFO
```

### Comparing `pushable-0.1.6/LICENSE` & `pushable-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pushable-0.1.6/README.md` & `pushable-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pushable-0.1.6/pyproject.toml` & `pushable-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pushable"
-version = "0.1.6"
+version = "0.1.7"
 description = "Convert iterators into peekable, pushable iterators"
 authors = ["Stephen Leach <sfkleach@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme="README.md"
 homepage="https://pushable.readthedocs.io/en/latest/"
 documentation="https://pushable.readthedocs.io/en/latest/"
 repository = "https://github.com/sfkleach/pushable"
@@ -22,11 +22,12 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 mypy = "^1.0.0"
+Sphinx = "^7.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pushable-0.1.6/src/pushable/pushable.py` & `pushable-0.1.7/src/pushable/pushable.py`

 * *Files identical despite different names*

### Comparing `pushable-0.1.6/PKG-INFO` & `pushable-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushable
-Version: 0.1.6
+Version: 0.1.7
 Summary: Convert iterators into peekable, pushable iterators
 Home-page: https://pushable.readthedocs.io/en/latest/
 License: GPL-3.0-or-later
 Keywords: iterators,pushable,peekable
 Author: Stephen Leach
 Author-email: sfkleach@gmail.com
 Requires-Python: >=3.10,<4.0
```

