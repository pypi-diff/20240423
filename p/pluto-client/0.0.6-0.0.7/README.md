# Comparing `tmp/pluto_client-0.0.6.tar.gz` & `tmp/pluto_client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluto_client-0.0.6.tar", max compression
+gzip compressed data, was "pluto_client-0.0.7.tar", max compression
```

## Comparing `pluto_client-0.0.6.tar` & `pluto_client-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0    10139 2024-04-12 09:11:51.818491 pluto_client-0.0.6/LICENSE
--rw-r--r--   0        0        0      241 2024-04-12 09:11:51.818491 pluto_client-0.0.6/README.md
--rw-r--r--   0        0        0      213 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/__init__.py
--rw-r--r--   0        0        0      153 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/__init__.py
--rw-r--r--   0        0        0     2788 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/function_lambda.py
--rw-r--r--   0        0        0     1018 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/kvstore_dynamodb.py
--rw-r--r--   0        0        0     1198 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/queue_sns.py
--rw-r--r--   0        0        0     1058 2024-04-22 07:59:31.588729 pluto_client-0.0.6/pluto_client/clients/aws/sagemaker.py
--rw-r--r--   0        0        0      566 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/utils.py
--rw-r--r--   0        0        0      187 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/errors.py
--rw-r--r--   0        0        0       33 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/shared/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/shared/router.py
--rw-r--r--   0        0        0     1811 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/function.py
--rw-r--r--   0        0        0     1703 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/kvstore.py
--rw-r--r--   0        0        0     1889 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/queue.py
--rw-r--r--   0        0        0     2059 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/router.py
--rw-r--r--   0        0        0     3610 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/sagemaker.py
--rw-r--r--   0        0        0      796 2024-04-22 08:01:10.773787 pluto_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    10139 2024-04-12 09:11:51.818491 pluto_client-0.0.7/LICENSE
+-rw-r--r--   0        0        0      241 2024-04-12 09:11:51.818491 pluto_client-0.0.7/README.md
+-rw-r--r--   0        0        0      593 2024-04-23 09:34:27.660381 pluto_client-0.0.7/pluto_client/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-23 09:17:42.415282 pluto_client-0.0.7/pluto_client/bucket.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-23 09:09:43.024707 pluto_client-0.0.7/pluto_client/clients/aws/__init__.py
+-rw-r--r--   0        0        0     1139 2024-04-23 13:39:35.016299 pluto_client-0.0.7/pluto_client/clients/aws/bucket_s3.py
+-rw-r--r--   0        0        0     2788 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/aws/function_lambda.py
+-rw-r--r--   0        0        0     1018 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/aws/kvstore_dynamodb.py
+-rw-r--r--   0        0        0     1198 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/aws/queue_sns.py
+-rw-r--r--   0        0        0     1058 2024-04-22 13:09:52.133703 pluto_client-0.0.7/pluto_client/clients/aws/sagemaker.py
+-rw-r--r--   0        0        0      376 2024-04-23 13:16:59.263894 pluto_client-0.0.7/pluto_client/clients/aws/test.py
+-rw-r--r--   0        0        0      575 2024-04-23 09:49:31.514283 pluto_client-0.0.7/pluto_client/clients/aws/utils.py
+-rw-r--r--   0        0        0      187 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/errors.py
+-rw-r--r--   0        0        0       33 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/shared/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/shared/router.py
+-rw-r--r--   0        0        0     1882 2024-04-23 08:14:10.375522 pluto_client-0.0.7/pluto_client/function.py
+-rw-r--r--   0        0        0     1703 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/kvstore.py
+-rw-r--r--   0        0        0     1889 2024-04-23 09:23:49.411273 pluto_client-0.0.7/pluto_client/queue.py
+-rw-r--r--   0        0        0     2059 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/router.py
+-rw-r--r--   0        0        0     3610 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/sagemaker.py
+-rw-r--r--   0        0        0     1276 2024-04-23 09:38:53.027207 pluto_client-0.0.7/pluto_client/schedule.py
+-rw-r--r--   0        0        0      796 2024-04-23 13:53:53.724431 pluto_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.7/PKG-INFO
```

### Comparing `pluto_client-0.0.6/LICENSE` & `pluto_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/clients/aws/function_lambda.py` & `pluto_client-0.0.7/pluto_client/clients/aws/function_lambda.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/clients/aws/kvstore_dynamodb.py` & `pluto_client-0.0.7/pluto_client/clients/aws/kvstore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/clients/aws/queue_sns.py` & `pluto_client-0.0.7/pluto_client/clients/aws/queue_sns.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/clients/aws/sagemaker.py` & `pluto_client-0.0.7/pluto_client/clients/aws/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/clients/aws/utils.py` & `pluto_client-0.0.7/pluto_client/clients/aws/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import hashlib
 import json
 
 RESOURCE_NAME_MAX_LENGTH = 50
 
 
 def gen_aws_resource_name(*parts: str) -> str:
-    resource_full_id = re.sub(r"[^-0-9a-zA-Z]+", "-", "_".join(parts))
+    resource_full_id = re.sub(r"[^-0-9a-zA-Z]+", "-", "_".join(parts)).lower()
+
     if len(resource_full_id) <= RESOURCE_NAME_MAX_LENGTH:
         return resource_full_id.strip("-")
     else:
         hash = hashlib.md5(json.dumps(resource_full_id).encode("utf-8")).hexdigest()[:8]
         start = len(resource_full_id) - (RESOURCE_NAME_MAX_LENGTH - len(hash))
         end = len(resource_full_id)
         return (resource_full_id[start:end] + hash).strip("-")
```

### Comparing `pluto_client-0.0.6/pluto_client/function.py` & `pluto_client-0.0.7/pluto_client/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     code: int
     body: Any
 
 
 @dataclass
 class FunctionOptions:
     name: str | None = None
+    memory: int | None = 128  # The memory size in MB, default is 128.
     envs: Dict[str, Any] | None = None
 
 
 class IFunctionClientApi(Generic[FnHandler], IResourceClientApi):
     def invoke(self, *args, **kwargs) -> Any:
         raise NotImplementedError
```

### Comparing `pluto_client-0.0.6/pluto_client/kvstore.py` & `pluto_client-0.0.7/pluto_client/kvstore.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/queue.py` & `pluto_client-0.0.7/pluto_client/queue.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/router.py` & `pluto_client-0.0.7/pluto_client/router.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pluto_client/sagemaker.py` & `pluto_client-0.0.7/pluto_client/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.6/pyproject.toml` & `pluto_client-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pluto-client"
-version = "0.0.6"
+version = "0.0.7"
 description = "The Client Library for Pluto Programming Language."
 authors = ["Jade Zheng <zheng.shoujian@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
     'Development Status :: 1 - Planning',
     'Environment :: Console',
```

### Comparing `pluto_client-0.0.6/PKG-INFO` & `pluto_client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluto-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Client Library for Pluto Programming Language.
 License: Apache-2.0
 Author: Jade Zheng
 Author-email: zheng.shoujian@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

