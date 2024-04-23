# Comparing `tmp/large-image-source-multi-1.28.2.dev4.tar.gz` & `tmp/large-image-source-multi-1.28.2.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-multi-1.28.2.dev4.tar", last modified: Mon Apr 15 12:55:05 2024, max compression
+gzip compressed data, was "large-image-source-multi-1.28.2.dev6.tar", last modified: Tue Apr 23 16:00:20 2024, max compression
```

## Comparing `large-image-source-multi-1.28.2.dev4.tar` & `large-image-source-multi-1.28.2.dev6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:55:05.866132 large-image-source-multi-1.28.2.dev4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-04-15 12:55:05.866132 large-image-source-multi-1.28.2.dev4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:55:05.862132 large-image-source-multi-1.28.2.dev4/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2024-04-15 12:52:04.000000 large-image-source-multi-1.28.2.dev4/docs/specification.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:55:05.862132 large-image-source-multi-1.28.2.dev4/large_image_source_multi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54069 2024-04-15 12:52:04.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-04-15 12:52:04.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-15 12:55:05.866132 large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-15 12:55:05.000000 large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-15 12:52:04.000000 large-image-source-multi-1.28.2.dev4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-15 12:55:05.866132 large-image-source-multi-1.28.2.dev4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2569 2024-04-15 12:52:04.000000 large-image-source-multi-1.28.2.dev4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-23 16:00:20.818238 large-image-source-multi-1.28.2.dev6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-04-23 16:00:20.818238 large-image-source-multi-1.28.2.dev6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-23 16:00:20.814238 large-image-source-multi-1.28.2.dev6/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2024-04-23 15:56:50.000000 large-image-source-multi-1.28.2.dev6/docs/specification.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-23 16:00:20.814238 large-image-source-multi-1.28.2.dev6/large_image_source_multi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54069 2024-04-23 15:56:50.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-04-23 15:56:50.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-23 16:00:20.814238 large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-23 16:00:20.000000 large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-23 15:56:50.000000 large-image-source-multi-1.28.2.dev6/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-23 16:00:20.818238 large-image-source-multi-1.28.2.dev6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2569 2024-04-23 15:56:50.000000 large-image-source-multi-1.28.2.dev6/setup.py
```

### Comparing `large-image-source-multi-1.28.2.dev4/LICENSE` & `large-image-source-multi-1.28.2.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev4/PKG-INFO` & `large-image-source-multi-1.28.2.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.28.2.dev4
+Version: 1.28.2.dev6
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: jsonschema
-Requires-Dist: large-image>=1.28.2.dev4
+Requires-Dist: large-image>=1.28.2.dev6
 Requires-Dist: pyyaml
 Provides-Extra: all
 Requires-Dist: scikit-image; extra == "all"
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev4; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.2.dev6; extra == "girder"
 
 A tilesource for large_image to composite other tile sources
 
 See the large-image package for more details.
```

### Comparing `large-image-source-multi-1.28.2.dev4/README.rst` & `large-image-source-multi-1.28.2.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev4/docs/specification.rst` & `large-image-source-multi-1.28.2.dev6/docs/specification.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev4/large_image_source_multi/__init__.py` & `large-image-source-multi-1.28.2.dev6/large_image_source_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev4/large_image_source_multi/girder_source.py` & `large-image-source-multi-1.28.2.dev6/large_image_source_multi/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev4/large_image_source_multi.egg-info/PKG-INFO` & `large-image-source-multi-1.28.2.dev6/large_image_source_multi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.28.2.dev4
+Version: 1.28.2.dev6
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: jsonschema
-Requires-Dist: large-image>=1.28.2.dev4
+Requires-Dist: large-image>=1.28.2.dev6
 Requires-Dist: pyyaml
 Provides-Extra: all
 Requires-Dist: scikit-image; extra == "all"
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev4; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.2.dev6; extra == "girder"
 
 A tilesource for large_image to composite other tile sources
 
 See the large-image package for more details.
```

### Comparing `large-image-source-multi-1.28.2.dev4/setup.py` & `large-image-source-multi-1.28.2.dev6/setup.py`

 * *Files identical despite different names*

