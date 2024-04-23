# Comparing `tmp/ziptimezone-1.0.0.tar.gz` & `tmp/ziptimezone-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-1.0.0.tar", max compression
+gzip compressed data, was "ziptimezone-1.0.1.tar", max compression
```

## Comparing `ziptimezone-1.0.0.tar` & `ziptimezone-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.0.0/LICENSE
--rw-r--r--   0        0        0      846 2024-04-22 09:20:56.262154 ziptimezone-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1788 2024-04-21 15:19:35.140920 ziptimezone-1.0.0/README.rst
--rw-r--r--   0        0        0     1183 2024-04-21 13:54:36.748759 ziptimezone-1.0.0/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1968 2024-04-21 13:54:36.748759 ziptimezone-1.0.0/ziptimezone/batch_processor.py
--rw-r--r--   0        0        0     1801 2024-04-21 13:54:36.748759 ziptimezone-1.0.0/ziptimezone/core.py
--rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.0.0/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.0.0/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.0.0/ziptimezone/globals.py
--rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.0.0/ziptimezone/mappings.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 ziptimezone-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.0.1/LICENSE
+-rw-r--r--   0        0        0      846 2024-04-23 11:19:26.042008 ziptimezone-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1788 2024-04-21 15:19:35.140920 ziptimezone-1.0.1/README.rst
+-rw-r--r--   0        0        0     1183 2024-04-23 11:02:12.525191 ziptimezone-1.0.1/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1968 2024-04-21 13:54:36.748759 ziptimezone-1.0.1/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     1801 2024-04-21 13:54:36.748759 ziptimezone-1.0.1/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.0.1/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.0.1/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.0.1/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.0.1/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 ziptimezone-1.0.1/PKG-INFO
```

### Comparing `ziptimezone-1.0.0/pyproject.toml` & `ziptimezone-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "1.0.0"
+version = "1.0.1"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.rst"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
```

### Comparing `ziptimezone-1.0.0/README.rst` & `ziptimezone-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/ziptimezone/__init__.py` & `ziptimezone-1.0.1/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/ziptimezone/batch_processor.py` & `ziptimezone-1.0.1/ziptimezone/batch_processor.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/ziptimezone/core.py` & `ziptimezone-1.0.1/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/ziptimezone/data_manager.py` & `ziptimezone-1.0.1/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/ziptimezone/geocode.py` & `ziptimezone-1.0.1/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/ziptimezone/globals.py` & `ziptimezone-1.0.1/ziptimezone/globals.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/ziptimezone/mappings.py` & `ziptimezone-1.0.1/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.0/PKG-INFO` & `ziptimezone-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

