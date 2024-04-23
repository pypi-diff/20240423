# Comparing `tmp/maphash-0.1.1.tar.gz` & `tmp/maphash-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maphash-0.1.1.tar", max compression
+gzip compressed data, was "maphash-0.1.2.tar", max compression
```

## Comparing `maphash-0.1.1.tar` & `maphash-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-03-15 21:12:41.031841 maphash-0.1.1/LICENSE
--rw-r--r--   0        0        0      665 2024-03-15 21:12:41.031993 maphash-0.1.1/Readme.rst
--rw-r--r--   0        0        0      680 2024-03-15 21:12:41.032196 maphash-0.1.1/maphash/__init__.py
--rw-r--r--   0        0        0      330 2024-03-15 21:23:44.922944 maphash-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 maphash-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-15 21:12:41.031841 maphash-0.1.2/LICENSE
+-rw-r--r--   0        0        0      665 2024-03-15 21:12:41.031993 maphash-0.1.2/Readme.rst
+-rw-r--r--   0        0        0      680 2024-03-15 21:12:41.032196 maphash-0.1.2/maphash/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:15:47.221157 maphash-0.1.2/maphash/py.typed
+-rw-r--r--   0        0        0      327 2024-04-23 13:16:12.392332 maphash-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 maphash-0.1.2/PKG-INFO
```

### Comparing `maphash-0.1.1/LICENSE` & `maphash-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maphash-0.1.1/Readme.rst` & `maphash-0.1.2/Readme.rst`

 * *Files identical despite different names*

### Comparing `maphash-0.1.1/maphash/__init__.py` & `maphash-0.1.2/maphash/__init__.py`

 * *Files identical despite different names*

### Comparing `maphash-0.1.1/PKG-INFO` & `maphash-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maphash
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Jakob Klepp
 Author-email: jakob.klepp@moonvision.io
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

