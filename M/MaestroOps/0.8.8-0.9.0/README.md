# Comparing `tmp/MaestroOps-0.8.8.tar.gz` & `tmp/maestroops-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MaestroOps-0.8.8.tar", last modified: Mon Jan 13 22:28:35 2020, max compression
+gzip compressed data, was "maestroops-0.9.0.tar", last modified: Tue Apr 23 19:15:35 2024, max compression
```

## Comparing `MaestroOps-0.8.8.tar` & `maestroops-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        0 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/
-drwxr-xr-x   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        0 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/MaestroOps.egg-info/
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      270 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/MaestroOps.egg-info/PKG-INFO
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      640 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/MaestroOps.egg-info/SOURCES.txt
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        1 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/MaestroOps.egg-info/dependency_links.txt
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)       16 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/MaestroOps.egg-info/requires.txt
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        8 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/MaestroOps.egg-info/top_level.txt
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      270 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/PKG-INFO
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      115 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/README.md
-drwxr-xr-x   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        0 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/maestro/
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)       46 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/__init__.py
-drwxr-xr-x   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        0 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/maestro/aws/
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)       84 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/aws/__init__.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)    30006 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/aws/cf_stack.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)    20046 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/aws/dynamodb.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)     9237 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/aws/parameter_store.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)    11716 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/aws/r53.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)    12289 2020-01-08 17:55:30.000000 MaestroOps-0.8.8/maestro/aws/s3.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)    10701 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/aws/ssm_documents.py
-drwxr-xr-x   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        0 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/maestro/core/
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)       39 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/core/__init__.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)     1487 2020-01-08 17:55:30.000000 MaestroOps-0.8.8/maestro/core/execute.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)     2554 2020-01-08 17:55:30.000000 MaestroOps-0.8.8/maestro/core/ioc.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)     4583 2020-01-13 22:24:41.000000 MaestroOps-0.8.8/maestro/core/module.py
-drwxr-xr-x   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        0 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/maestro/jenkins/
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)       19 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/jenkins/__init__.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)     6683 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/jenkins/jobs.py
-drwxr-xr-x   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)        0 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/maestro/tools/
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)       37 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/tools/__init__.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      481 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/tools/file.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      742 2020-01-06 21:56:43.000000 MaestroOps-0.8.8/maestro/tools/os_tools.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)     3425 2020-01-08 17:55:30.000000 MaestroOps-0.8.8/maestro/tools/path.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      423 2020-01-08 17:55:30.000000 MaestroOps-0.8.8/maestro/tools/string.py
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)       38 2020-01-13 22:28:35.000000 MaestroOps-0.8.8/setup.cfg
--rw-r--r--   0 wjia     (787203365) SIGNIANTOTT\Domain Users (1513040830)      423 2020-01-13 22:27:42.000000 MaestroOps-0.8.8/setup.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.844902 maestroops-0.9.0/
+-rw-r--r--   0 mperttula   (502) staff       (20)     1081 2024-02-27 16:30:05.000000 maestroops-0.9.0/LICENSE
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.842962 maestroops-0.9.0/MaestroOps.egg-info/
+-rw-r--r--   0 mperttula   (502) staff       (20)      285 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      648 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/SOURCES.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/dependency_links.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       17 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/requires.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        8 2024-04-23 19:15:35.000000 maestroops-0.9.0/MaestroOps.egg-info/top_level.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)      285 2024-04-23 19:15:35.843952 maestroops-0.9.0/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      115 2024-02-27 16:30:05.000000 maestroops-0.9.0/README.md
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.671670 maestroops-0.9.0/maestro/
+-rw-r--r--   0 mperttula   (502) staff       (20)       46 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/__init__.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.743088 maestroops-0.9.0/maestro/aws/
+-rw-r--r--   0 mperttula   (502) staff       (20)       84 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    30006 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/cf_stack.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    20046 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/dynamodb.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     9237 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/parameter_store.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    11716 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/r53.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    13344 2024-04-23 19:13:16.000000 maestroops-0.9.0/maestro/aws/s3.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    10701 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/aws/ssm_documents.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.785483 maestroops-0.9.0/maestro/core/
+-rw-r--r--   0 mperttula   (502) staff       (20)       39 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/core/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1487 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/core/execute.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     2554 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/core/ioc.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     4583 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/core/module.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.799343 maestroops-0.9.0/maestro/jenkins/
+-rw-r--r--   0 mperttula   (502) staff       (20)       19 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/jenkins/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     6683 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/jenkins/jobs.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-04-23 19:15:35.841928 maestroops-0.9.0/maestro/tools/
+-rw-r--r--   0 mperttula   (502) staff       (20)       37 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/tools/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1713 2024-04-23 19:13:16.000000 maestroops-0.9.0/maestro/tools/file.py
+-rw-r--r--   0 mperttula   (502) staff       (20)      742 2024-02-27 16:30:05.000000 maestroops-0.9.0/maestro/tools/os_tools.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     3425 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/tools/path.py
+-rw-r--r--   0 mperttula   (502) staff       (20)      423 2024-02-27 16:30:09.000000 maestroops-0.9.0/maestro/tools/string.py
+-rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-04-23 19:15:35.845073 maestroops-0.9.0/setup.cfg
+-rw-r--r--   0 mperttula   (502) staff       (20)      424 2024-04-23 19:13:16.000000 maestroops-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MaestroOps-0.8.8/MaestroOps.egg-info/SOURCES.txt` & `maestroops-0.9.0/MaestroOps.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 MaestroOps.egg-info/PKG-INFO
 MaestroOps.egg-info/SOURCES.txt
 MaestroOps.egg-info/dependency_links.txt
 MaestroOps.egg-info/requires.txt
 MaestroOps.egg-info/top_level.txt
```

### Comparing `MaestroOps-0.8.8/maestro/aws/cf_stack.py` & `maestroops-0.9.0/maestro/aws/cf_stack.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/aws/dynamodb.py` & `maestroops-0.9.0/maestro/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/aws/parameter_store.py` & `maestroops-0.9.0/maestro/aws/parameter_store.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/aws/r53.py` & `maestroops-0.9.0/maestro/aws/r53.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/aws/s3.py` & `maestroops-0.9.0/maestro/aws/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 import botocore
 from botocore.handlers import disable_signing
 from botocore import UNSIGNED
 from botocore.client import Config
 from ..core import module
 
 
-def find_files(bucket, prefix, case_sensitive=True, connection=None, anonymous=True):
+def find_files(bucket, prefix, case_sensitive=True, connection=None, anonymous=True, sha256=False):
     """
     find_files will connect and return files found in bucket with prefix, all other keys are ignored.
 
     Optional: case_sensitive, connection
 
     Returns a boto3 objectCollection containing matching files, or an empty collection. Will not return any non-file keys.
     Will raise a DownloadError with an appropriate error message when unable to return a collection.
     """
-
     s3client = None
     if connection is None:
         try:
             connection = get_s3_connection(anonymous=False)
             s3client = boto3.client('s3')
         except Exception:
             connection = get_s3_connection(anonymous=True)
@@ -47,21 +46,36 @@
     files = list()
 
     # Look for matching files if case insensitive mode
     if not case_sensitive:
         # Iterate over objects, and append only ones that match lower case and don't end with '/'
         for obj in remote_bucket.objects.all():
             if obj.key.lower().startswith(prefix.lower()) and not obj.key.endswith("/"):
-                objsum = s3client.get_object(Bucket=bucket, Key=obj.key)["ETag"][1:-1]
+                if sha256:
+                    try:
+                        objsum = s3client.head_object(Bucket=bucket, Key=obj.key, ChecksumMode='ENABLED')['ResponseMetadata']['HTTPHeaders']["x-amz-checksum-sha256"]
+                    except Exception:
+                        raise ChecksumFailure(f"Unable head object for checksum. Please verify sha256 exists on object {bucket}/{obj.key}")
+                        objsum = "unknown"
+                else:
+                    objsum = s3client.get_object(Bucket=bucket, Key=obj.key)["ETag"][1:-1]
                 files.append((obj, objsum))
     else:  # If we're case sensitive, just use the filter
         files = remote_bucket.objects.filter(Prefix=prefix)
         sum_files = list()
         for f in files:
-            objsum = s3client.get_object(Bucket=bucket, Key=f.key)["ETag"][1:-1]
+            if sha256:
+                try:
+                    objsum = s3client.head_object(Bucket=bucket, Key=f.key, ChecksumMode='ENABLED')['ResponseMetadata']['HTTPHeaders']["x-amz-checksum-sha256"]
+                except Exception:
+                    raise ChecksumFailure(
+                        f"Unable head object for checksum. Please verify sha256 exists on object {bucket}/{obj.key}")
+                    objsum = "unknown"
+            else:
+                objsum = s3client.get_object_attributes(Bucket=bucket, Key=f.key, ObjectAttributes=['ETag'])[1:-1]
             sum_files.append((f, objsum))
         files = sum_files
 
     return files
 
 
 def get_s3_connection(anonymous=True):
@@ -140,14 +154,17 @@
         else:
             raise e
 
 
 class DownloadError(Exception):
     pass
 
+class ChecksumFailure(Exception):
+    pass
+
 
 # MODULES #
 
 BUCKET_KEYS = ["b", "bucket"]
 CASE_INSENSITIVE_KEYS = ["i", "case-insensitive"]
 DESTINATION_KEYS = ["d", "destination"]
 PATH_KEYS = ["p", "prefix"]
@@ -186,14 +203,15 @@
         bucket_name = None
         case_insensitive = False
         destination_path = None
         prefix = None
         region = None
         source_url = None
         anonymous = None
+        sha256 = False
 
         def run(self, kwargs):
             if kwargs is not None and len(kwargs) > 0:
                 if not self.__parse_kwargs__(kwargs):
                     return
             self.__verify_arguments__()
             return self.download()
@@ -252,15 +270,15 @@
                 verify_bucket(self.bucket_name, s3)
 
             # Stupid s3 can't provide a length to their collections...
             count = 0
             # Return value
             destination_files = list()
             # Loop through found files
-            for obj, checksum in find_files(self.bucket_name, self.prefix, case_sensitive=not self.case_insensitive, connection=s3, anonymous=self.anonymous):
+            for obj, checksum in find_files(self.bucket_name, self.prefix, case_sensitive=not self.case_insensitive, connection=s3, anonymous=self.anonymous, sha256=self.sha256):
                 if obj.key.endswith("/"):
                     continue
                 destination = self.destination_path
                 # Case: Provided path exists
                 if os.path.exists(destination):
                     # Case Provided path is a directory
                     if os.path.isdir(destination):
```

### Comparing `MaestroOps-0.8.8/maestro/aws/ssm_documents.py` & `maestroops-0.9.0/maestro/aws/ssm_documents.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/core/execute.py` & `maestroops-0.9.0/maestro/core/execute.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/core/ioc.py` & `maestroops-0.9.0/maestro/core/ioc.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/core/module.py` & `maestroops-0.9.0/maestro/core/module.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/jenkins/jobs.py` & `maestroops-0.9.0/maestro/jenkins/jobs.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/tools/os_tools.py` & `maestroops-0.9.0/maestro/tools/os_tools.py`

 * *Files identical despite different names*

### Comparing `MaestroOps-0.8.8/maestro/tools/path.py` & `maestroops-0.9.0/maestro/tools/path.py`

 * *Files identical despite different names*

