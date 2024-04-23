# Comparing `tmp/atas_client-0.0.9.tar.gz` & `tmp/atas_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atas_client-0.0.9.tar", last modified: Fri Mar 29 02:04:17 2024, max compression
+gzip compressed data, was "atas_client-0.1.0.tar", last modified: Tue Apr 23 03:16:29 2024, max compression
```

## Comparing `atas_client-0.0.9.tar` & `atas_client-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-03-29 02:04:17.871779 atas_client-0.0.9/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-0.0.9/LICENSE
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-03-29 02:04:17.871482 atas_client-0.0.9/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-0.0.9/README.md
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2024-03-29 01:54:40.000000 atas_client-0.0.9/pyproject.toml
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2024-03-29 02:04:17.871823 atas_client-0.0.9/setup.cfg
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-03-29 02:04:17.868006 atas_client-0.0.9/src/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-0.0.9/src/__init__.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-03-29 02:04:17.869311 atas_client-0.0.9/src/atas_client/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     2753 2023-08-08 09:40:20.000000 atas_client-0.0.9/src/atas_client/CoreATASApi.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1353 2024-03-29 01:25:29.000000 atas_client-0.0.9/src/atas_client/HttpUtil.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-0.0.9/src/atas_client/__init__.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1158 2023-10-17 09:40:06.000000 atas_client-0.0.9/src/atas_client/atas_client.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-03-29 02:04:17.871158 atas_client-0.0.9/src/atas_client.egg-info/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-03-29 02:04:17.000000 atas_client-0.0.9/src/atas_client.egg-info/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2024-03-29 02:04:17.000000 atas_client-0.0.9/src/atas_client.egg-info/SOURCES.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2024-03-29 02:04:17.000000 atas_client-0.0.9/src/atas_client.egg-info/dependency_links.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2024-03-29 02:04:17.000000 atas_client-0.0.9/src/atas_client.egg-info/top_level.txt
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:16:29.548601 atas_client-0.1.0/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-0.1.0/LICENSE
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-04-23 03:16:29.548305 atas_client-0.1.0/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-0.1.0/README.md
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2024-04-23 03:13:17.000000 atas_client-0.1.0/pyproject.toml
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2024-04-23 03:16:29.548642 atas_client-0.1.0/setup.cfg
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:16:29.544401 atas_client-0.1.0/src/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-0.1.0/src/__init__.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:16:29.545948 atas_client-0.1.0/src/atas_client/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     2821 2024-04-23 03:14:26.000000 atas_client-0.1.0/src/atas_client/CoreATASApi.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1353 2024-03-29 01:25:29.000000 atas_client-0.1.0/src/atas_client/HttpUtil.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-0.1.0/src/atas_client/__init__.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1158 2023-10-17 09:40:06.000000 atas_client-0.1.0/src/atas_client/atas_client.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2024-04-23 03:16:29.547946 atas_client-0.1.0/src/atas_client.egg-info/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2024-04-23 03:16:29.000000 atas_client-0.1.0/src/atas_client.egg-info/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2024-04-23 03:16:29.000000 atas_client-0.1.0/src/atas_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2024-04-23 03:16:29.000000 atas_client-0.1.0/src/atas_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2024-04-23 03:16:29.000000 atas_client-0.1.0/src/atas_client.egg-info/top_level.txt
```

### Comparing `atas_client-0.0.9/LICENSE` & `atas_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.9/PKG-INFO` & `atas_client-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas_client
-Version: 0.0.9
+Version: 0.1.0
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `atas_client-0.0.9/pyproject.toml` & `atas_client-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atas_client"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="tao.ding", email="tao.ding@rakuten.com" },
 ]
 description = "ATAS Automation API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `atas_client-0.0.9/src/atas_client/CoreATASApi.py` & `atas_client-0.1.0/src/atas_client/CoreATASApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from .HttpUtil import HttpUtil
 
 
 class CoreATASApi:
 
     @staticmethod
-    def init_result(uri, token, launch, executor):
+    def init_result(uri, token, launch, executor, job_execution_id):
         headers = "{\"Content-Type\": \"application/json;charset=UTF-8\",\"auth-key\": \"" + token + "\"}"
         url = uri + "/automation/launch/init"
-        body = "{\"launchName\":\"" + launch + "\", \"executor\": \"" + executor + "\"}"
+        body = "{\"launchName\":\"" + launch + "\", \"executor\": \"" + executor + "\", \"jobExecutionId\": \"" + job_execution_id + "\"}"
         method = "post"
         try:
             res = HttpUtil.http_request(url, method, None, None, json.loads(body), headers=eval(headers))
         except Exception:
             raise
         execution_id = json.loads(res)['data']['executionId']
         return execution_id
```

### Comparing `atas_client-0.0.9/src/atas_client/HttpUtil.py` & `atas_client-0.1.0/src/atas_client/HttpUtil.py`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.9/src/atas_client/atas_client.py` & `atas_client-0.1.0/src/atas_client/atas_client.py`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.9/src/atas_client.egg-info/PKG-INFO` & `atas_client-0.1.0/src/atas_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas_client
-Version: 0.0.9
+Version: 0.1.0
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

