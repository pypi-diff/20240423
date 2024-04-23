# Comparing `tmp/types-s2clientprotocol-5.0.0.20240302.tar.gz` & `tmp/types-s2clientprotocol-5.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-s2clientprotocol-5.0.0.20240302.tar", last modified: Sat Mar  2 02:11:05 2024, max compression
+gzip compressed data, was "types-s2clientprotocol-5.0.0.3.tar", last modified: Sun Oct 29 02:16:45 2023, max compression
```

## Comparing `types-s2clientprotocol-5.0.0.20240302.tar` & `types-s2clientprotocol-5.0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 02:11:05.088095 types-s2clientprotocol-5.0.0.20240302/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-02 02:11:04.000000 types-s2clientprotocol-5.0.0.20240302/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-02 02:11:04.000000 types-s2clientprotocol-5.0.0.20240302/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-02 02:11:05.088095 types-s2clientprotocol-5.0.0.20240302/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 02:11:05.084095 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-02 02:11:04.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18925 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/data_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18382 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24185 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/error_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    31823 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/raw_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    96075 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/sc2api_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/score_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23418 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/spatial_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-03-02 02:10:35.000000 types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/ui_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 02:11:05.088095 types-s2clientprotocol-5.0.0.20240302/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-02 02:11:04.000000 types-s2clientprotocol-5.0.0.20240302/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 02:11:05.088095 types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-02 02:11:05.000000 types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-02 02:11:05.000000 types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 02:11:05.000000 types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-02 02:11:05.000000 types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-02 02:11:05.000000 types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:45.611756 types-s2clientprotocol-5.0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-29 02:16:44.000000 types-s2clientprotocol-5.0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-29 02:16:44.000000 types-s2clientprotocol-5.0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-10-29 02:16:45.611756 types-s2clientprotocol-5.0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:45.611756 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-29 02:16:44.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18925 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18382 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24185 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/error_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    31823 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/raw_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    96075 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/sc2api_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/score_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23418 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/spatial_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2023-10-29 02:16:08.000000 types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/ui_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 02:16:45.611756 types-s2clientprotocol-5.0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-10-29 02:16:44.000000 types-s2clientprotocol-5.0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:45.611756 types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-10-29 02:16:45.000000 types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-10-29 02:16:45.000000 types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 02:16:45.000000 types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-29 02:16:45.000000 types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-29 02:16:45.000000 types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/top_level.txt
```

### Comparing `types-s2clientprotocol-5.0.0.20240302/PKG-INFO` & `types-s2clientprotocol-5.0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: types-s2clientprotocol
-Version: 5.0.0.20240302
+Version: 5.0.0.3
 Summary: Typing stubs for s2clientprotocol
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/s2clientprotocol.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for s2clientprotocol
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`s2clientprotocol`](https://github.com/Blizzard/s2client-proto) package.
 It can be used by type-checking tools like
@@ -28,10 +28,10 @@
 This version of `types-s2clientprotocol` aims to provide accurate annotations
 for `s2clientprotocol==5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/s2clientprotocol. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5e4483618a02b4bf182940e3b89e8178855e6f32` and was tested
-with mypy 1.8.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
+with mypy 1.6.1, pyright 1.1.332, and
+pytype 2023.10.17.
```

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/common_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/data_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/debug_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/error_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/query_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/query_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
-import typing as typing_extensions
+import sys
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import s2clientprotocol.common_pb2
 import s2clientprotocol.error_pb2
 
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
+
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
 class RequestQuery(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PATHING_FIELD_NUMBER: builtins.int
```

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/raw_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/raw_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/sc2api_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/sc2api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/score_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/spatial_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/spatial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/s2clientprotocol-stubs/ui_pb2.pyi` & `types-s2clientprotocol-5.0.0.3/s2clientprotocol-stubs/ui_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.20240302/setup.py` & `types-s2clientprotocol-5.0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,35 +17,35 @@
 This version of `types-s2clientprotocol` aims to provide accurate annotations
 for `s2clientprotocol==5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/s2clientprotocol. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5e4483618a02b4bf182940e3b89e8178855e6f32` and was tested
-with mypy 1.8.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
+with mypy 1.6.1, pyright 1.1.332, and
+pytype 2023.10.17.
 '''.lstrip()
 
 setup(name=name,
-      version="5.0.0.20240302",
+      version="5.0.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/s2clientprotocol.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-protobuf'],
       packages=['s2clientprotocol-stubs'],
       package_data={'s2clientprotocol-stubs': ['build.pyi', 'common_pb2.pyi', 'data_pb2.pyi', 'debug_pb2.pyi', 'error_pb2.pyi', 'query_pb2.pyi', 'raw_pb2.pyi', 'sc2api_pb2.pyi', 'score_pb2.pyi', 'spatial_pb2.pyi', 'ui_pb2.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
-      python_requires=">=3.8",
+      python_requires=">=3.7",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/PKG-INFO` & `types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: types-s2clientprotocol
-Version: 5.0.0.20240302
+Version: 5.0.0.3
 Summary: Typing stubs for s2clientprotocol
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/s2clientprotocol.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for s2clientprotocol
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`s2clientprotocol`](https://github.com/Blizzard/s2client-proto) package.
 It can be used by type-checking tools like
@@ -28,10 +28,10 @@
 This version of `types-s2clientprotocol` aims to provide accurate annotations
 for `s2clientprotocol==5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/s2clientprotocol. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5e4483618a02b4bf182940e3b89e8178855e6f32` and was tested
-with mypy 1.8.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
+with mypy 1.6.1, pyright 1.1.332, and
+pytype 2023.10.17.
```

### Comparing `types-s2clientprotocol-5.0.0.20240302/types_s2clientprotocol.egg-info/SOURCES.txt` & `types-s2clientprotocol-5.0.0.3/types_s2clientprotocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

