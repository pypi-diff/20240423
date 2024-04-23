# Comparing `tmp/gai-lib-0.97.tar.gz` & `tmp/gai-lib-0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gai-lib-0.97.tar", last modified: Fri Apr 19 22:08:43 2024, max compression
+gzip compressed data, was "gai-lib-0.98.tar", last modified: Mon Apr 22 11:26:09 2024, max compression
```

## Comparing `gai-lib-0.97.tar` & `gai-lib-0.98.tar`

### file list

```diff
@@ -1,52 +1,50 @@
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/
--rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.97/MANIFEST.in
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-19 22:08:43.367512 gai-lib-0.97/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-19 22:04:19.000000 gai-lib-0.97/VERSION
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/common/
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1040 2024-04-19 21:38:04.000000 gai-lib-0.97/gai/common/StatusListener.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1842 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/StatusUpdater.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/constants.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.97/gai/common/errors.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4222 2024-02-22 17:41:30.000000 gai-lib-0.97/gai/common/file_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     5369 2024-04-02 15:12:34.000000 gai-lib-0.97/gai/common/generators_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     8401 2024-04-19 21:57:05.000000 gai-lib-0.97/gai/common/http_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.97/gai/common/image_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.97/gai/common/logging.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.97/gai/common/overlap_splitter.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.97/gai/common/sound_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/utils.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/lib/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.97/gai/lib/ClientBase.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4158 2024-02-23 13:22:53.000000 gai-lib-0.97/gai/lib/GGG.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.97/gai/lib/ITTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4382 2024-04-19 21:59:14.000000 gai-lib-0.97/gai/lib/RAGClientAsync.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     7499 2024-04-19 21:19:32.000000 gai-lib-0.97/gai/lib/RAGClientSync.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.97/gai/lib/STTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.97/gai/lib/TTSClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/lib/ttt/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/AnthropicChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/ChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/OpenAIChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     7026 2024-04-16 11:50:57.000000 gai-lib-0.97/gai/lib/ttt/TTTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/tools/
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.97/gai/tools/Chunker.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.97/gai/tools/Googler.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/tools/PDFConvert.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/tools/Scraper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/tools/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3178 2024-04-19 22:01:42.000000 gai-lib-0.97/gai.yml
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai_lib.egg-info/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1016 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/SOURCES.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/dependency_links.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/entry_points.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/requires.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/top_level.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.97/requirements.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-04-19 22:08:43.367512 gai-lib-0.97/setup.cfg
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.97/setup.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.074779 gai-lib-0.98/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.98/MANIFEST.in
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-22 11:26:09.064779 gai-lib-0.98/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-22 11:26:02.000000 gai-lib-0.98/VERSION
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.054779 gai-lib-0.98/gai/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.054779 gai-lib-0.98/gai/common/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1084 2024-04-22 09:25:34.000000 gai-lib-0.98/gai/common/StatusListener.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.98/gai/common/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.98/gai/common/constants.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.98/gai/common/errors.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4222 2024-02-22 17:41:30.000000 gai-lib-0.98/gai/common/file_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     5369 2024-04-02 15:12:34.000000 gai-lib-0.98/gai/common/generators_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     8918 2024-04-22 09:37:38.000000 gai-lib-0.98/gai/common/http_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.98/gai/common/image_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.98/gai/common/logging.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.98/gai/common/overlap_splitter.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.98/gai/common/sound_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.98/gai/common/utils.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai/lib/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.98/gai/lib/ClientBase.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4144 2024-04-21 09:26:10.000000 gai-lib-0.98/gai/lib/GGG.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.98/gai/lib/ITTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     5331 2024-04-22 09:33:44.000000 gai-lib-0.98/gai/lib/RAGClientAsync.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.98/gai/lib/STTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.98/gai/lib/TTSClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai/lib/ttt/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/AnthropicChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/ChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/OpenAIChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     7026 2024-04-16 11:50:57.000000 gai-lib-0.98/gai/lib/ttt/TTTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/lib/ttt/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai/tools/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.98/gai/tools/Chunker.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.98/gai/tools/Googler.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/tools/PDFConvert.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/tools/Scraper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.98/gai/tools/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3178 2024-04-21 08:24:16.000000 gai-lib-0.98/gai.yml
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-22 11:26:09.064779 gai-lib-0.98/gai_lib.egg-info/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      963 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/entry_points.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/requires.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-22 11:26:08.000000 gai-lib-0.98/gai_lib.egg-info/top_level.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.98/requirements.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-04-22 11:26:09.074779 gai-lib-0.98/setup.cfg
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.98/setup.py
```

### Comparing `gai-lib-0.97/PKG-INFO` & `gai-lib-0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.97
+Version: 0.98
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.97/gai/common/errors.py` & `gai-lib-0.98/gai/common/errors.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/common/file_utils.py` & `gai-lib-0.98/gai/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/common/generators_utils.py` & `gai-lib-0.98/gai/common/generators_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/common/http_utils.py` & `gai-lib-0.98/gai/common/http_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import pprint
 import re
 import httpx
 import requests
 import json
 from gai.common.logging import getLogger
+import inspect
 logger = getLogger(__name__)
 
 
 def is_url(s):
     return re.match(r'^https?:\/\/.*[\r\n]*', s) is not None
 
 # Check if URL contains a file extension (e.g. .pdf, .jpg, .png, etc.)
@@ -63,62 +64,77 @@
         if 'message' in error_data:
             raise ApiException(status_code=response.status_code, code=error_code, message=error_data['message']) 
         
     raise ApiException(status_code=response.status_code, code=error_code, message=json.dumps(error_data)) 
 
 async def _handle_failed_response_async(response):
     error_code = "unknown"
-    if response.status == 401:
-        raise ApiException(status_code=401, code=error_code, message="Unauthorized")
+
+    # Check for access token
+    if hasattr(response,"status"):
+        if response.status == 401:
+            raise ApiException(status_code=401, code=error_code, message="Unauthorized")
+    elif hasattr(response,"status_code"):
+        if response.status_code == 401:
+            raise ApiException(status_code=401, code=error_code, message="Unauthorized")
 
     content_type = response.headers.get("Content-Type")
     if content_type and "application/json" in content_type:
-        error_data = await response.json()
+        if inspect.iscoroutine(response.json):
+            error_data = await response.json()
+        else:
+            error_data = response.json()
     else:
         if isinstance(response.text, str):
             error_data = response.text
         else:
             error_data = await response.text()
 
+    # Build exception
     e = Exception()
     e.response = response
-    e.status = response.status
+    if hasattr(response,"status"):
+        e.status = response.status
+    elif hasattr(response, "status_code"):
+        e.status = response.status_code
+    else:
+        e.status = "unknown_status_code"
 
     if isinstance(error_data, str):
-        raise ApiException(status_code=response.status, code=error_code, message=error_data)
+        raise ApiException(status_code=e.status, code=error_code, message=error_data)
 
     if 'detail' in error_data:
 
         if isinstance(error_data['detail'], str):
-            raise ApiException(status_code=response.status_code, code=error_code, message=error_data['detail'])
+            raise ApiException(status_code=e.status, code=error_code, message=error_data['detail'])
 
         if 'code' in error_data['detail']:
             error_code = error_data['detail']['code']
 
         if 'message' in error_data['detail'] and isinstance(error_data['detail']['message'], str):
-            raise ApiException(status_code=response.status_code, code=error_code, message=error_data['detail']['message'])
+            raise ApiException(status_code=e.status, code=error_code, message=error_data['detail']['message'])
 
     if 'code' in error_data:
         error_code = error_data['code']
         if 'message' in error_data:
-            raise ApiException(status_code=response.status_code, code=error_code, message=error_data['message'] )
+            raise ApiException(status_code=e.status, code=error_code, message=error_data['message'] )
         
-    raise ApiException(status_code=response.status_code, code=error_code, message=json.dumps(error_data) )
+    raise ApiException(status_code=e.status, code=error_code, message=json.dumps(error_data) )
 
 async def http_post_async(url, data=None, files=None):
     return await httppost_async(url, data, files)
 
 async def httppost_async(url, data=None,files=None):
     if data == None and files == None:
         raise Exception("No data or files provided")
 
     logger.debug(f"httppost:url={url}")
     logger.debug(f"httppost:data={pprint.pformat(data)}")
 
-    async with httpx.AsyncClient() as client:
+    async with httpx.AsyncClient(timeout=30.0) as client:
         try:
             if files:
                 if data and "stream" in data:
                     files["stream"] = (None, data["stream"])
                 response = await client.post(url, files=files)
             else:
                 if "stream" in data:
```

### Comparing `gai-lib-0.97/gai/common/image_utils.py` & `gai-lib-0.98/gai/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/common/logging.py` & `gai-lib-0.98/gai/common/logging.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/common/overlap_splitter.py` & `gai-lib-0.98/gai/common/overlap_splitter.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/common/sound_utils.py` & `gai-lib-0.98/gai/common/sound_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/common/utils.py` & `gai-lib-0.98/gai/common/utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/lib/GGG.py` & `gai-lib-0.98/gai/lib/GGG.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,14 +88,13 @@
                     {"role": "user", "content": [
                         {"type": "text", "text": text},
                         {"type": "image_url", "image_url": image_url}
                     ]}
                 ]
                 return self.client(messages=messages, **model_params)
         elif category.lower() == "index":
-            self.client = RAGClientSync(self.config_path)
-            return self.client.index_file(**model_params)
+            raise Exception("The 'index' command has deprecated in GGG. Use RAGClientAsync instead.")
         elif category.lower() == "retrieve":
             self.client = RAGClientSync(self.config_path)
             return self.client.retrieve(**model_params)
         else:
             raise Exception(f"Unknown category: {category}")
```

### Comparing `gai-lib-0.97/gai/lib/ITTClient.py` & `gai-lib-0.98/gai/lib/ITTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/lib/RAGClientAsync.py` & `gai-lib-0.98/gai/lib/RAGClientAsync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 import os
 import json
-from fastapi import WebSocketDisconnect
-from gai.common.StatusListener import StatusListener
+import uuid
 from gai.common.http_utils import http_post_async, http_get_async,http_delete_async
 from gai.common.logging import getLogger
 from gai.common.errors import ApiException
 logger = getLogger(__name__)
+logger.setLevel("DEBUG")
 from gai.lib.ClientBase import ClientBase
+import websockets
+from gai.common.StatusListener import StatusListener
 
 class RAGClientBase(ClientBase):
     
     def __init__(self,config_path=None):
         super().__init__(config_path)
         self.base_url = os.path.join(
             self.config["gai_url"], 
@@ -29,57 +31,76 @@
             return files
 
 class RAGClientAsync(RAGClientBase):
 
     def __init__(self,config_path=None):
         super().__init__(config_path)
 
-### ----------------- INDEXING ----------------- ###
+    ### ----------------- INDEXING ----------------- ###
 
     # Provides an updater to get chunk indexing status
     # NOTE: The update is only relevant if this library is used in a FastAPI application with a websocket connection
     async def index_file_async(
         self, 
         collection_name, 
         file_path, 
         title="",
         source="",
         authors="",
         publisher="",
         published_date="",
         comments="",
         keywords="", 
-        progress_updater=None):
+        ws_manager=None):
+        
         url=os.path.join(self.base_url,"index-file")
         metadata = {
             "title": title,
             "source": source,
             "authors": authors,
             "publisher": publisher,
             "published_date": published_date,
             "comments": comments,
             "keywords": keywords
         }
 
-        if progress_updater:
-            listener = StatusListener("ws://localhost:12031/ws")
-            asyncio.create_task(listener.listen(progress_updater))
+        # Send file
+        async def send():
+            try:
+                mode = 'rb'
+                with open(file_path, mode) as f:
+                    files = {
+                        "file": (os.path.basename(file_path), f, "application/pdf"),
+                        "metadata": (None, json.dumps(metadata), "application/json"),
+                        "collection_name": (None, collection_name, "text/plain")
+                    }
+                    response = await http_post_async(url=url, files=files)
+                    return response
+            except Exception as e:
+                logger.error(e)
+                raise e
+    
+        if ws_manager:
 
-       # We will assume file ending with *.pdf to be PDF but this check should be done before the call.
-        mode = 'rb'
-        with open(file_path, mode) as f:
-            files = {
-                "file": (os.path.basename(file_path), f, "application/pdf"),
-                "metadata": (None, json.dumps(metadata), "application/json"),
-                "collection_name": (None, collection_name, "text/plain")
-            }
-            response = await http_post_async(url=url, files=files)
+            # Create listener
+            ws_url=os.path.join(self.base_url,f"index-file/ws").replace("http","ws")
+            listener = StatusListener(ws_url, collection_name)
+
+            # Start both tasks and return when first task completes then cancel the other
+            send_task=asyncio.create_task(send())
+            listen_task=asyncio.create_task(listener.listen(ws_manager))
+            pending, done = await asyncio.wait([send_task, listen_task], return_when=asyncio.FIRST_COMPLETED)
+            for task in pending:
+                task.cancel()
+        else:
+            await send()
 
-        return json.loads(response.text)
+        logger.info("Indexing complete.")
 
+    ### ----------------- RETRIEVAL ----------------- ###
 
     async def retrieve_async(self, collection_name, query_texts, n_results=None):
         url = os.path.join(self.base_url,"retrieve")
         data = {
             "collection_name": collection_name,
             "query_texts": query_texts
         }
@@ -110,8 +131,13 @@
 
 #Documents-------------------------------------------------------------------------------------------------------------------------------------------
 
     async def list_documents_async(self):
         url = os.path.join(self.base_url,"documents")
         response = await http_get_async(url)
         return json.loads(response.text)
+
+    async def delete_document_async(self,collection_name,document_id):
+        url = os.path.join(self.base_url,f"document/{collection_name}/{document_id}")
+        response = await http_delete_async(url)
+        return json.loads(response.text)
```

### Comparing `gai-lib-0.97/gai/lib/STTClient.py` & `gai-lib-0.98/gai/lib/STTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/lib/TTSClient.py` & `gai-lib-0.98/gai/lib/TTSClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/lib/ttt/ChunkWrapper.py` & `gai-lib-0.98/gai/lib/ttt/ChunkWrapper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/lib/ttt/TTTClient.py` & `gai-lib-0.98/gai/lib/ttt/TTTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/tools/Chunker.py` & `gai-lib-0.98/gai/tools/Chunker.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/tools/Googler.py` & `gai-lib-0.98/gai/tools/Googler.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai/tools/Scraper.py` & `gai-lib-0.98/gai/tools/Scraper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.97/gai.yml` & `gai-lib-0.98/gai.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 default_generator: mistral7b-exllama
-#gai_url: "http://localhost:12031"
-gai_url: "https://gaiaio.ai/api/gen"
+gai_url: "http://localhost:12031"
+#gai_url: "https://gaiaio.ai/api/gen"
 generators:
     mistral7b-exllama:
         type: ttt
-        #url: "/gen/v1/chat/completions"
-        url: "/v1/chat/completions"
+        url: "/gen/v1/chat/completions"
+        #url: "/v1/chat/completions"
         whitelist:
             - temperature
             - top_p
             - min_p
             - top_k
             - max_new_tokens
             - typical
```

### Comparing `gai-lib-0.97/gai_lib.egg-info/PKG-INFO` & `gai-lib-0.98/gai_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.97
+Version: 0.98
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.97/gai_lib.egg-info/SOURCES.txt` & `gai-lib-0.98/gai_lib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 MANIFEST.in
 VERSION
 gai.yml
 requirements.txt
 setup.py
 gai/__init__.py
 gai/common/StatusListener.py
-gai/common/StatusUpdater.py
 gai/common/__init__.py
 gai/common/constants.py
 gai/common/errors.py
 gai/common/file_utils.py
 gai/common/generators_utils.py
 gai/common/http_utils.py
 gai/common/image_utils.py
@@ -17,15 +16,14 @@
 gai/common/overlap_splitter.py
 gai/common/sound_utils.py
 gai/common/utils.py
 gai/lib/ClientBase.py
 gai/lib/GGG.py
 gai/lib/ITTClient.py
 gai/lib/RAGClientAsync.py
-gai/lib/RAGClientSync.py
 gai/lib/STTClient.py
 gai/lib/TTSClient.py
 gai/lib/__init__.py
 gai/lib/ttt/AnthropicChunkWrapper.py
 gai/lib/ttt/ChunkWrapper.py
 gai/lib/ttt/OpenAIChunkWrapper.py
 gai/lib/ttt/TTTClient.py
```

### Comparing `gai-lib-0.97/setup.py` & `gai-lib-0.98/setup.py`

 * *Files identical despite different names*

