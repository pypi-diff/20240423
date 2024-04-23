# Comparing `tmp/finalsa-common-lambdas-0.1.0.tar.gz` & `tmp/finalsa_common_lambdas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-common-lambdas-0.1.0.tar", last modified: Sat Mar 30 07:15:38 2024, max compression
+gzip compressed data, was "finalsa_common_lambdas-0.1.1.tar", last modified: Tue Apr 23 04:02:42 2024, max compression
```

## Comparing `finalsa-common-lambdas-0.1.0.tar` & `finalsa_common_lambdas-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.644793 finalsa-common-lambdas-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-30 07:15:38.644793 finalsa-common-lambdas-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.636793 finalsa-common-lambdas-0.1.0/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.636793 finalsa-common-lambdas-0.1.0/finalsa/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.640793 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.640793 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/app/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/app/App.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/app/AppEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.640793 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/http/
--rw-r--r--   0 runner    (1001) docker     (127)    10968 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/http/HttpHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/http/HttpHeaders.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.640793 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/sqs/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/sqs/SqsEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/sqs/SqsHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/sqs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.644793 finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-30 07:15:38.000000 finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-30 07:15:38.000000 finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 07:15:38.000000 finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-30 07:15:38.000000 finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-30 07:15:38.000000 finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 07:15:38.000000 finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-30 07:15:38.644793 finalsa-common-lambdas-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:15:38.644793 finalsa-common-lambdas-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/tests/test_http_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-03-30 07:15:32.000000 finalsa-common-lambdas-0.1.0/tests/test_sqs_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.501569 finalsa_common_lambdas-0.1.1/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.501569 finalsa_common_lambdas-0.1.1/finalsa/common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/App.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/AppEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHeaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.505569 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:02:42.000000 finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:02:42.509569 finalsa_common_lambdas-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_http_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-23 04:02:33.000000 finalsa_common_lambdas-0.1.1/tests/test_sqs_service.py
```

### Comparing `finalsa-common-lambdas-0.1.0/LICENSE.md` & `finalsa_common_lambdas-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/PKG-INFO` & `finalsa_common_lambdas-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-common-lambdas
-Version: 0.1.0
+Version: 0.1.1
 Summary: An utils package for using finalsa common lambas.
 Home-page: https://github.com/finalsa/finalsa-common-lambda
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
```

### Comparing `finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/app/App.py` & `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/App.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/app/AppEntry.py` & `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/app/AppEntry.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/http/HttpHandler.py` & `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,18 @@
     @staticmethod
     def parse_body(headers: Dict, body: str) -> Any:
         content_type = headers.get("Content-Type", "")
         if "application/json" in content_type:
             return loads(body)
         if 'text/plain' in content_type:
             return body
-        return body
+        try:
+            return loads(body)
+        except:
+            return body
 
     @staticmethod
     def parse_response(response: Tuple[str, int], default_headers: Dict = {}) -> Tuple[str, int]:
         headers = {}
         body = response[0]
         if isinstance(body, str):
             body = body
```

### Comparing `finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/http/HttpHeaders.py` & `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/http/HttpHeaders.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/sqs/SqsEvent.py` & `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsEvent.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/finalsa/common/lambdas/sqs/SqsHandler.py` & `finalsa_common_lambdas-0.1.1/finalsa/common/lambdas/sqs/SqsHandler.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/PKG-INFO` & `finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-common-lambdas
-Version: 0.1.0
+Version: 0.1.1
 Summary: An utils package for using finalsa common lambas.
 Home-page: https://github.com/finalsa/finalsa-common-lambda
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
```

### Comparing `finalsa-common-lambdas-0.1.0/finalsa_common_lambdas.egg-info/SOURCES.txt` & `finalsa_common_lambdas-0.1.1/finalsa_common_lambdas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/setup.py` & `finalsa_common_lambdas-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/tests/test_app.py` & `finalsa_common_lambdas-0.1.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/tests/test_http_service.py` & `finalsa_common_lambdas-0.1.1/tests/test_http_service.py`

 * *Files identical despite different names*

### Comparing `finalsa-common-lambdas-0.1.0/tests/test_sqs_service.py` & `finalsa_common_lambdas-0.1.1/tests/test_sqs_service.py`

 * *Files identical despite different names*

