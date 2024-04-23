# Comparing `tmp/assetsstore-1.0.9.tar.gz` & `tmp/assetsstore-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assetsstore-1.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "assetsstore-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `assetsstore-1.0.9.tar` & `assetsstore-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       91 2024-04-10 15:51:30.190093 assetsstore-1.0.9/.flake8
--rw-r--r--   0        0        0     1776 2024-04-10 15:51:30.190093 assetsstore-1.0.9/.gitignore
--rw-r--r--   0        0        0      366 2024-04-10 15:51:30.190093 assetsstore-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2024-04-08 11:14:38.232095 assetsstore-1.0.9/LICENSE
--rw-r--r--   0        0        0     2179 2024-04-10 15:51:30.190093 assetsstore-1.0.9/README.md
--rw-r--r--   0        0        0      104 2024-04-10 15:51:30.190093 assetsstore-1.0.9/assetsstore/__init__.py
--rw-r--r--   0        0        0      296 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/__init__.py
--rw-r--r--   0        0        0     6331 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/assets.py
--rw-r--r--   0        0        0       62 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/azr/__init__.py
--rw-r--r--   0        0        0     5690 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/azr/azure_files.py
--rw-r--r--   0        0        0       62 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/local/__init__.py
--rw-r--r--   0        0        0     4241 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/local/local_files.py
--rw-r--r--   0        0        0       56 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/minio/__init__.py
--rw-r--r--   0        0        0     8983 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/minio/minio.py
--rw-r--r--   0        0        0     6234 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/minio/progress.py
--rw-r--r--   0        0        0       53 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/s3/__init__.py
--rw-r--r--   0        0        0    11381 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/s3/s3_files.py
--rw-r--r--   0        0        0       65 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/server/__init__.py
--rw-r--r--   0        0        0     7486 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/assets/server/server_files.py
--rw-r--r--   0        0        0        0 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/tests/__init__.py
--rw-r--r--   0        0        0     1744 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/tests/assets_test.py
--rw-r--r--   0        0        0        0 2024-04-08 11:14:38.232095 assetsstore-1.0.9/assetsstore/tests/fixtures/test.txt
--rw-r--r--   0        0        0       19 2024-04-08 11:14:38.232095 assetsstore-1.0.9/assetsstore/tests/fixtures/test_folder/test2.txt
--rw-r--r--   0        0        0     4085 2024-04-10 15:51:30.194093 assetsstore-1.0.9/assetsstore/tests/test_minio.py
--rw-r--r--   0        0        0      262 2024-04-08 11:14:38.232095 assetsstore-1.0.9/docker-compose.yml
--rw-r--r--   0        0        0      962 2024-04-10 15:51:30.194093 assetsstore-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 assetsstore-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-10 15:51:30.190093 assetsstore-1.1.0/.flake8
+-rw-r--r--   0        0        0     1776 2024-04-10 15:51:30.190093 assetsstore-1.1.0/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-10 15:51:30.190093 assetsstore-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2024-04-08 11:14:38.232095 assetsstore-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2179 2024-04-10 15:51:30.190093 assetsstore-1.1.0/README.md
+-rw-r--r--   0        0        0      104 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/assets/__init__.py
+-rw-r--r--   0        0        0     6667 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/assets/assets.py
+-rw-r--r--   0        0        0       62 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/azr/__init__.py
+-rw-r--r--   0        0        0     5690 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/azr/azure_files.py
+-rw-r--r--   0        0        0       62 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/local/__init__.py
+-rw-r--r--   0        0        0     4241 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/local/local_files.py
+-rw-r--r--   0        0        0       56 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/minio/__init__.py
+-rw-r--r--   0        0        0     8983 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/minio/minio.py
+-rw-r--r--   0        0        0     6234 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/minio/progress.py
+-rw-r--r--   0        0        0       53 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/s3/__init__.py
+-rw-r--r--   0        0        0    11381 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/s3/s3_files.py
+-rw-r--r--   0        0        0       65 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/server/__init__.py
+-rw-r--r--   0        0        0     7486 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/assets/server/server_files.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/tests/__init__.py
+-rw-r--r--   0        0        0     1751 2024-04-23 09:37:13.843635 assetsstore-1.1.0/assetsstore/tests/assets_test.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:14:38.232095 assetsstore-1.1.0/assetsstore/tests/fixtures/test.txt
+-rw-r--r--   0        0        0       19 2024-04-08 11:14:38.232095 assetsstore-1.1.0/assetsstore/tests/fixtures/test_folder/test2.txt
+-rw-r--r--   0        0        0     4085 2024-04-10 15:51:30.194093 assetsstore-1.1.0/assetsstore/tests/test_minio.py
+-rw-r--r--   0        0        0      262 2024-04-08 11:14:38.232095 assetsstore-1.1.0/docker-compose.yml
+-rw-r--r--   0        0        0      960 2024-04-23 09:37:13.843635 assetsstore-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 assetsstore-1.1.0/PKG-INFO
```

### Comparing `assetsstore-1.0.9/.gitignore` & `assetsstore-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/LICENSE` & `assetsstore-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/README.md` & `assetsstore-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/assetsstore/assets/assets.py` & `assetsstore-1.1.0/assetsstore/assets/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import abc
 import os
 import uuid
 import zipfile
 import logging
 import requests
 import json
+from pydoc import locate
 
 logger = logging.getLogger(__name__)
 
 
 class FileAssets(metaclass=abc.ABCMeta):
     """
     The `FileAssets` class is an abstract base class that provides
     a common interface for working with different types of file assets.
     It defines abstract methods that need to be implemented by its subclasses.
     The class also provides some common functionality for working with files,
     such as uploading, downloading, and deleting files.
     """
 
+    ASSETS_MAP = {
+        "S3Files": "assetsstore.assets.s3.s3_files.S3Files",
+        "AzureFiles": "assetsstore.assets.azr.azure_files.AzureFiles",
+        "LocalFiles": "assetsstore.assets.local.local_files.LocalFiles",
+        "ServerFiles": "assetsstore.assets.server.server_files.ServerFiles",
+        "MinioFiles": "assetsstore.assets.minio.minio.MinioFiles",
+    }
+
     def __init__(self):
         """
         Initializes the `FileAssets` object and sets the
         local store path based on the LOCAL_STORE environment variable.
         This variable is important since our local store paths will act as
         a medium between the asset store and the local file system.
         """
@@ -104,28 +113,25 @@
 
     @classmethod
     def get_asset(cls):
         """
         Class method that returns an instance of the appropriate
         subclass based on the value of the ASSET_STORE environment variable.
         """
-        asset = None
         selected = os.getenv("ASSET_STORE")
-        for sub_cls in cls.__subclasses__():
-            if selected.lower() == sub_cls.__name__.lower():
-                asset = sub_cls
-        if not asset:
+        if selected is None:
+            raise Exception("Environment variable ASSET_STORE is not set.")
+        if selected not in cls.ASSETS_MAP.keys():
             raise Exception(
-                """There is no asset by name '{}' please set environment variable
-                ASSET_STORE to one of the following:
-                LocalFiles, ServerFiles, S3Files, AzureFiles, MinioFiles""".format(
-                    selected
+                """Invalid ASSET_STORE value '{}'.
+                Please set it to one of the following: {}""".format(
+                    selected, ", ".join(cls.ASSETS_MAP.keys())
                 )
             )
-        return asset()
+        return locate(cls.ASSETS_MAP[selected])()
 
     def compress(self, file: str):
         """
         Compresses a file into a ZIP archive.
         """
         with zipfile.ZipFile(
             file.replace(".csv", ".zip"), "w", zipfile.ZIP_DEFLATED
```

### Comparing `assetsstore-1.0.9/assetsstore/assets/azr/azure_files.py` & `assetsstore-1.1.0/assetsstore/assets/azr/azure_files.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/assetsstore/assets/local/local_files.py` & `assetsstore-1.1.0/assetsstore/assets/local/local_files.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/assetsstore/assets/minio/minio.py` & `assetsstore-1.1.0/assetsstore/assets/minio/minio.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/assetsstore/assets/minio/progress.py` & `assetsstore-1.1.0/assetsstore/assets/minio/progress.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/assetsstore/assets/s3/s3_files.py` & `assetsstore-1.1.0/assetsstore/assets/s3/s3_files.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/assetsstore/assets/server/server_files.py` & `assetsstore-1.1.0/assetsstore/assets/server/server_files.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/assetsstore/tests/assets_test.py` & `assetsstore-1.1.0/assetsstore/tests/assets_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 from assetsstore.assets import FileAssets
 import glob
 import os
 import logging
 
 
 class AsssetsLocalTest(TestCase):
-
     def setUp(self):
         self.maxDiff = None
         logging.basicConfig(level=logging.INFO)
 
     def test_no_asset_store_set(self):
         os.environ["ASSET_STORE"] = ""
         with self.assertRaises(Exception) as context:
             FileAssets.get_asset()
         print(context.exception)
-        self.assertTrue("There is no asset" in str(context.exception))
+        self.assertTrue("Invalid ASSET_STORE value" in str(context.exception))
 
     def test_upload_and_download_from_local(self):
         # get set store
         os.environ["ASSET_STORE"] = "LocalFiles"
 
         os.environ["ASSET_ACCESS_KEY_ID"] = ""
         os.environ["ASSET_SECRET_ACCESS_KEY"] = ""
```

### Comparing `assetsstore-1.0.9/assetsstore/tests/test_minio.py` & `assetsstore-1.1.0/assetsstore/tests/test_minio.py`

 * *Files identical despite different names*

### Comparing `assetsstore-1.0.9/PKG-INFO` & `assetsstore-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: AssetsStore
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python package for managing file upload/download via selected file system.
 Author-email: Nebojsa Mrkic <mrkic.nebojsa@gmail.com>
 Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: requests>=2.28.2
 Requires-Dist: urllib3>=2.0.0
 Requires-Dist: azure-storage-blob==2.1.0 ; extra == "azure"
 Requires-Dist: minio>=7.1.13 ; extra == "minio"
 Requires-Dist: boto3>=1.26.66 ; extra == "s3"
 Requires-Dist: paramiko>=3.2.0 ; extra == "server"
 Requires-Dist: pytest ; extra == "tests"
```

