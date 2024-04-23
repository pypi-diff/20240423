# Comparing `tmp/alibabacloud_fc20230330_py2-4.0.0.tar.gz` & `tmp/alibabacloud_fc20230330_py2-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_fc20230330_py2-4.0.0.tar", last modified: Mon Apr 15 08:39:51 2024, max compression
+gzip compressed data, was "dist/alibabacloud_fc20230330_py2-4.1.0.tar", last modified: Tue Apr 23 06:21:25 2024, max compression
```

## Comparing `alibabacloud_fc20230330_py2-4.0.0.tar` & `alibabacloud_fc20230330_py2-4.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/
--rw-r--r--   0 root         (0) root         (0)     4427 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2480 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62079 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330/client.py
--rw-r--r--   0 root         (0) root         (0)   279059 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2480 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2912 2024-04-15 08:39:51.000000 alibabacloud_fc20230330_py2-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)     4632 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66736 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330/client.py
+-rw-r--r--   0 root         (0) root         (0)   287454 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 06:21:25.000000 alibabacloud_fc20230330_py2-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-23 06:21:24.000000 alibabacloud_fc20230330_py2-4.1.0/setup.py
```

### Comparing `alibabacloud_fc20230330_py2-4.0.0/ChangeLog.md` & `alibabacloud_fc20230330_py2-4.1.0/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2024-04-15 Version: 4.0.0
+- Delete API GetResourceTags.
+- Delete API ListTaggedResources.
+- Delete API TagResource.
+- Delete API UntagResource.
+- Update API InvokeFunction: add param x-fc-async-task-id.
+
+
 2024-03-22 Version: 3.1.0
 - Support API ListTagResources.
 - Support API TagResources.
 - Support API UntagResources.
 - Update API CreateAlias: update response param.
 - Update API CreateCustomDomain: update response param.
 - Update API CreateFunction: update response param.
```

### Comparing `alibabacloud_fc20230330_py2-4.0.0/LICENSE` & `alibabacloud_fc20230330_py2-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330_py2-4.0.0/PKG-INFO` & `alibabacloud_fc20230330_py2-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_fc20230330_py2
-Version: 4.0.0
+Version: 4.1.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330_py2-4.0.0/README-CN.md` & `alibabacloud_fc20230330_py2-4.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330_py2-4.0.0/README.md` & `alibabacloud_fc20230330_py2-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330/client.py` & `alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,14 +504,44 @@
         )
 
     def get_async_invoke_config(self, function_name, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_async_invoke_config_with_options(function_name, request, headers, runtime)
 
+    def get_async_task_with_options(self, function_name, task_id, request, headers, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.qualifier):
+            query['qualifier'] = request.qualifier
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAsyncTask',
+            version='2023-03-30',
+            protocol='HTTPS',
+            pathname='/2023-03-30/functions/%s/async-tasks/%s' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(task_id))),
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            fc20230330_models.GetAsyncTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_async_task(self, function_name, task_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_async_task_with_options(function_name, task_id, request, headers, runtime)
+
     def get_concurrency_config_with_options(self, function_name, headers, runtime):
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetConcurrencyConfig',
             version='2023-03-30',
@@ -836,14 +866,60 @@
         )
 
     def list_async_invoke_configs(self, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_async_invoke_configs_with_options(request, headers, runtime)
 
+    def list_async_tasks_with_options(self, function_name, request, headers, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.include_payload):
+            query['includePayload'] = request.include_payload
+        if not UtilClient.is_unset(request.limit):
+            query['limit'] = request.limit
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.prefix):
+            query['prefix'] = request.prefix
+        if not UtilClient.is_unset(request.qualifier):
+            query['qualifier'] = request.qualifier
+        if not UtilClient.is_unset(request.sort_order_by_time):
+            query['sortOrderByTime'] = request.sort_order_by_time
+        if not UtilClient.is_unset(request.started_time_begin):
+            query['startedTimeBegin'] = request.started_time_begin
+        if not UtilClient.is_unset(request.started_time_end):
+            query['startedTimeEnd'] = request.started_time_end
+        if not UtilClient.is_unset(request.status):
+            query['status'] = request.status
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListAsyncTasks',
+            version='2023-03-30',
+            protocol='HTTPS',
+            pathname='/2023-03-30/functions/%s/async-tasks' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)),
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            fc20230330_models.ListAsyncTasksResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_async_tasks(self, function_name, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_async_tasks_with_options(function_name, request, headers, runtime)
+
     def list_concurrency_configs_with_options(self, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.function_name):
             query['functionName'] = request.function_name
         if not UtilClient.is_unset(request.limit):
             query['limit'] = request.limit
@@ -1357,14 +1433,44 @@
         )
 
     def put_provision_config(self, function_name, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.put_provision_config_with_options(function_name, request, headers, runtime)
 
+    def stop_async_task_with_options(self, function_name, task_id, request, headers, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.qualifier):
+            query['qualifier'] = request.qualifier
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='StopAsyncTask',
+            version='2023-03-30',
+            protocol='HTTPS',
+            pathname='/2023-03-30/functions/%s/async-tasks/%s/stop' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(function_name)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(task_id))),
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            fc20230330_models.StopAsyncTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def stop_async_task(self, function_name, task_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.stop_async_task_with_options(function_name, task_id, request, headers, runtime)
+
     def tag_resources_with_options(self, request, headers, runtime):
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
```

### Comparing `alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330/models.py` & `alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12964,4479 +12964,5003 @@
 00032a30: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
 00032a40: 656c 203d 2041 7379 6e63 436f 6e66 6967  el = AsyncConfig
 00032a50: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
 00032a60: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
 00032a70: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
 00032a80: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
 00032a90: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00032aa0: 636c 6173 7320 4765 7443 6f6e 6375 7272  class GetConcurr
-00032ab0: 656e 6379 436f 6e66 6967 5265 7370 6f6e  encyConfigRespon
-00032ac0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-00032ad0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00032ae0: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
-00032af0: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
-00032b00: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
-00032b10: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-00032b20: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
-00032b30: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
-00032b40: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
-00032b50: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00032b60: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
-00032b70: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
-00032b80: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00032b90: 626f 6479 2020 2320 7479 7065 3a20 436f  body  # type: Co
-00032ba0: 6e63 7572 7265 6e63 7943 6f6e 6669 670a  ncurrencyConfig.
-00032bb0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00032bc0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00032bd0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00032be0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00032bf0: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-00032c00: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00032c10: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00032c20: 6d61 7020 3d20 7375 7065 7228 4765 7443  map = super(GetC
-00032c30: 6f6e 6375 7272 656e 6379 436f 6e66 6967  oncurrencyConfig
-00032c40: 5265 7370 6f6e 7365 2c20 7365 6c66 292e  Response, self).
-00032c50: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00032c60: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00032c70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00032c80: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00032c90: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00032ca0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00032cb0: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-00032cc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00032cd0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00032ce0: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-00032cf0: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-00032d00: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-00032d10: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-00032d20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00032d30: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-00032d40: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-00032d50: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-00032d60: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-00032d70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00032d80: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-00032d90: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-00032da0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00032db0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00032dc0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00032dd0: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-00032de0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00032df0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00032e00: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-00032e10: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00032e20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00032e30: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-00032e40: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-00032e50: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-00032e60: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-00032e70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00032e80: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-00032e90: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-00032ea0: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-00032eb0: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
-00032ec0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-00032ed0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00032ee0: 705f 6d6f 6465 6c20 3d20 436f 6e63 7572  p_model = Concur
-00032ef0: 7265 6e63 7943 6f6e 6669 6728 290a 2020  rencyConfig().  
-00032f00: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00032f10: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-00032f20: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-00032f30: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-00032f40: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00032f50: 2047 6574 4375 7374 6f6d 446f 6d61 696e   GetCustomDomain
-00032f60: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00032f70: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00032f80: 6974 5f5f 2873 656c 662c 2068 6561 6465  it__(self, heade
-00032f90: 7273 3d4e 6f6e 652c 2073 7461 7475 735f  rs=None, status_
-00032fa0: 636f 6465 3d4e 6f6e 652c 2062 6f64 793d  code=None, body=
-00032fb0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-00032fc0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-00032fd0: 6164 6572 7320 2023 2074 7970 653a 2064  aders  # type: d
-00032fe0: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
-00032ff0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00033000: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-00033010: 636f 6465 2020 2320 7479 7065 3a20 696e  code  # type: in
-00033020: 740a 2020 2020 2020 2020 7365 6c66 2e62  t.        self.b
-00033030: 6f64 7920 3d20 626f 6479 2020 2320 7479  ody = body  # ty
-00033040: 7065 3a20 4375 7374 6f6d 446f 6d61 696e  pe: CustomDomain
-00033050: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00033060: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00033070: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-00033080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00033090: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-000330a0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000330b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000330c0: 5f6d 6170 203d 2073 7570 6572 2847 6574  _map = super(Get
-000330d0: 4375 7374 6f6d 446f 6d61 696e 5265 7370  CustomDomainResp
-000330e0: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
-000330f0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00033100: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00033110: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00033120: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00033130: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00033140: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00033150: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-00033160: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00033170: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-00033180: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-00033190: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-000331a0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000331b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000331c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000331d0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-000331e0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000331f0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00033200: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-00033210: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00033220: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-00033230: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-00033240: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-00033250: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00033260: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00033270: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-00033280: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00033290: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000332a0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-000332b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000332c0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000332d0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-000332e0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-000332f0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00033300: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00033310: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00033320: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00033330: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-00033340: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-00033350: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-00033360: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00033370: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-00033380: 6465 6c20 3d20 4375 7374 6f6d 446f 6d61  del = CustomDoma
-00033390: 696e 2829 0a20 2020 2020 2020 2020 2020  in().           
-000333a0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-000333b0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-000333c0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-000333d0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-000333e0: 0a0a 636c 6173 7320 4765 7446 756e 6374  ..class GetFunct
-000333f0: 696f 6e52 6571 7565 7374 2854 6561 4d6f  ionRequest(TeaMo
-00033400: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00033410: 696e 6974 5f5f 2873 656c 662c 2071 7561  init__(self, qua
-00033420: 6c69 6669 6572 3d4e 6f6e 6529 3a0a 2020  lifier=None):.  
-00033430: 2020 2020 2020 2320 5468 6520 7665 7273        # The vers
-00033440: 696f 6e20 6f72 2061 6c69 6173 206f 6620  ion or alias of 
-00033450: 7468 6520 6675 6e63 7469 6f6e 2e0a 2020  the function..  
-00033460: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
-00033470: 6669 6572 203d 2071 7561 6c69 6669 6572  fier = qualifier
-00033480: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
-00033490: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-000334a0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-000334b0: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-000334c0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-000334d0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-000334e0: 4765 7446 756e 6374 696f 6e52 6571 7565  GetFunctionReque
-000334f0: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
-00033500: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00033510: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00033520: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00033530: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00033540: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00033550: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00033560: 2e71 7561 6c69 6669 6572 2069 7320 6e6f  .qualifier is no
-00033570: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00033580: 2020 2020 7265 7375 6c74 5b27 7175 616c      result['qual
-00033590: 6966 6965 7227 5d20 3d20 7365 6c66 2e71  ifier'] = self.q
-000335a0: 7561 6c69 6669 6572 0a20 2020 2020 2020  ualifier.       
-000335b0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000335c0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000335d0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-000335e0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000335f0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00033600: 6966 206d 2e67 6574 2827 7175 616c 6966  if m.get('qualif
-00033610: 6965 7227 2920 6973 206e 6f74 204e 6f6e  ier') is not Non
-00033620: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00033630: 656c 662e 7175 616c 6966 6965 7220 3d20  elf.qualifier = 
-00033640: 6d2e 6765 7428 2771 7561 6c69 6669 6572  m.get('qualifier
-00033650: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00033660: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2047  n self...class G
-00033670: 6574 4675 6e63 7469 6f6e 5265 7370 6f6e  etFunctionRespon
-00033680: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-00033690: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-000336a0: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
-000336b0: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
-000336c0: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
-000336d0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-000336e0: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
-000336f0: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
-00033700: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
-00033710: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00033720: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
-00033730: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
-00033740: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00033750: 626f 6479 2020 2320 7479 7065 3a20 4675  body  # type: Fu
-00033760: 6e63 7469 6f6e 0a0a 2020 2020 6465 6620  nction..    def 
-00033770: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00033780: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00033790: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-000337a0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-000337b0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-000337c0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-000337d0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000337e0: 6572 2847 6574 4675 6e63 7469 6f6e 5265  er(GetFunctionRe
-000337f0: 7370 6f6e 7365 2c20 7365 6c66 292e 746f  sponse, self).to
-00033800: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00033810: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00033820: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00033830: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00033840: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00033850: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00033860: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-00033870: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00033880: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-00033890: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-000338a0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-000338b0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-000338c0: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-000338d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000338e0: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-000338f0: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-00033900: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-00033910: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-00033920: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00033930: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-00033940: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-00033950: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-00033960: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00033970: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00033980: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
-00033990: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-000339a0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000339b0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000339c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000339d0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-000339e0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-000339f0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-00033a00: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-00033a10: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-00033a20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00033a30: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00033a40: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-00033a50: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-00033a60: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-00033a70: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00033a80: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00033a90: 6d6f 6465 6c20 3d20 4675 6e63 7469 6f6e  model = Function
-00033aa0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00033ab0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00033ac0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00033ad0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00033ae0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00033af0: 636c 6173 7320 4765 7446 756e 6374 696f  class GetFunctio
-00033b00: 6e43 6f64 6552 6571 7565 7374 2854 6561  nCodeRequest(Tea
-00033b10: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00033b20: 5f5f 696e 6974 5f5f 2873 656c 662c 2071  __init__(self, q
-00033b30: 7561 6c69 6669 6572 3d4e 6f6e 6529 3a0a  ualifier=None):.
-00033b40: 2020 2020 2020 2020 2320 5468 6520 7665          # The ve
-00033b50: 7273 696f 6e20 6f72 2061 6c69 6173 206f  rsion or alias o
-00033b60: 6620 7468 6520 6675 6e63 7469 6f6e 2e0a  f the function..
-00033b70: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
-00033b80: 6c69 6669 6572 203d 2071 7561 6c69 6669  lifier = qualifi
-00033b90: 6572 2020 2320 7479 7065 3a20 7374 720a  er  # type: str.
-00033ba0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00033bb0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00033bc0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00033bd0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00033be0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00033bf0: 7228 4765 7446 756e 6374 696f 6e43 6f64  r(GetFunctionCod
-00033c00: 6552 6571 7565 7374 2c20 7365 6c66 292e  eRequest, self).
-00033c10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00033c20: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00033c30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00033c40: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00033c50: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00033c60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00033c70: 6620 7365 6c66 2e71 7561 6c69 6669 6572  f self.qualifier
-00033c80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00033c90: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00033ca0: 5b27 7175 616c 6966 6965 7227 5d20 3d20  ['qualifier'] = 
-00033cb0: 7365 6c66 2e71 7561 6c69 6669 6572 0a20  self.qualifier. 
-00033cc0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00033cd0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00033ce0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-00033cf0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00033d00: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00033d10: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00033d20: 7175 616c 6966 6965 7227 2920 6973 206e  qualifier') is n
-00033d30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00033d40: 2020 2020 2073 656c 662e 7175 616c 6966       self.qualif
-00033d50: 6965 7220 3d20 6d2e 6765 7428 2771 7561  ier = m.get('qua
-00033d60: 6c69 6669 6572 2729 0a20 2020 2020 2020  lifier').       
-00033d70: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00033d80: 6c61 7373 2047 6574 4675 6e63 7469 6f6e  lass GetFunction
-00033d90: 436f 6465 5265 7370 6f6e 7365 2854 6561  CodeResponse(Tea
-00033da0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00033db0: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
-00033dc0: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
-00033dd0: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
-00033de0: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
-00033df0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00033e00: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
-00033e10: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
-00033e20: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
-00033e30: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-00033e40: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
-00033e50: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
-00033e60: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
-00033e70: 2320 7479 7065 3a20 4f75 7470 7574 4675  # type: OutputFu
-00033e80: 6e63 436f 6465 0a0a 2020 2020 6465 6620  ncCode..    def 
-00033e90: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00033ea0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00033eb0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-00033ec0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-00033ed0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-00033ee0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00033ef0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00033f00: 6572 2847 6574 4675 6e63 7469 6f6e 436f  er(GetFunctionCo
-00033f10: 6465 5265 7370 6f6e 7365 2c20 7365 6c66  deResponse, self
-00033f20: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00033f30: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00033f40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00033f50: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00033f60: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00033f70: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00033f80: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00033f90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00033fa0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00033fb0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00033fc0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-00033fd0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00033fe0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00033ff0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00034000: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00034010: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00034020: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00034030: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00034040: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00034050: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00034060: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00034070: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00034080: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00034090: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-000340a0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-000340b0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000340c0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000340d0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-000340e0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-000340f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00034100: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-00034110: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-00034120: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00034130: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00034140: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00034150: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00034160: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00034170: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00034180: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00034190: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-000341a0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-000341b0: 656d 705f 6d6f 6465 6c20 3d20 4f75 7470  emp_model = Outp
-000341c0: 7574 4675 6e63 436f 6465 2829 0a20 2020  utFuncCode().   
-000341d0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-000341e0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-000341f0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-00034200: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-00034210: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00034220: 4765 744c 6179 6572 5665 7273 696f 6e52  GetLayerVersionR
-00034230: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00034240: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00034250: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
-00034260: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
-00034270: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
-00034280: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00034290: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-000342a0: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
-000342b0: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
-000342c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000342d0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-000342e0: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
-000342f0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-00034300: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
-00034310: 653a 204c 6179 6572 0a0a 2020 2020 6465  e: Layer..    de
-00034320: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00034330: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00034340: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00034350: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00034360: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00034370: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00034380: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00034390: 7570 6572 2847 6574 4c61 7965 7256 6572  uper(GetLayerVer
-000343a0: 7369 6f6e 5265 7370 6f6e 7365 2c20 7365  sionResponse, se
-000343b0: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-000343c0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000343d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000343e0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000343f0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00034400: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00034410: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-00034420: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-00034430: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00034440: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-00034450: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-00034460: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00034470: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-00034480: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00034490: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-000344a0: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-000344b0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-000344c0: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-000344d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000344e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000344f0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-00034500: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-00034510: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00034520: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00034530: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-00034540: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00034550: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00034560: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-00034570: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-00034580: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00034590: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-000345a0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-000345b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000345c0: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-000345d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000345e0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-000345f0: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-00034600: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-00034610: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00034620: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-00034630: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00034640: 2074 656d 705f 6d6f 6465 6c20 3d20 4c61   temp_model = La
-00034650: 7965 7228 290a 2020 2020 2020 2020 2020  yer().          
-00034660: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-00034670: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-00034680: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-00034690: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000346a0: 0a0a 0a63 6c61 7373 2047 6574 4c61 7965  ...class GetLaye
-000346b0: 7256 6572 7369 6f6e 4279 4172 6e52 6573  rVersionByArnRes
-000346c0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-000346d0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000346e0: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
-000346f0: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
-00034700: 653d 4e6f 6e65 2c20 626f 6479 3d4e 6f6e  e=None, body=Non
-00034710: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00034720: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-00034730: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
-00034740: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
-00034750: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00034760: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-00034770: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
-00034780: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00034790: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
-000347a0: 204c 6179 6572 0a0a 2020 2020 6465 6620   Layer..    def 
-000347b0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000347c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000347d0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-000347e0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-000347f0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-00034800: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00034810: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00034820: 6572 2847 6574 4c61 7965 7256 6572 7369  er(GetLayerVersi
-00034830: 6f6e 4279 4172 6e52 6573 706f 6e73 652c  onByArnResponse,
-00034840: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-00034850: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00034860: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00034870: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00034880: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00034890: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-000348a0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-000348b0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-000348c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000348d0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-000348e0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-000348f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00034900: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-00034910: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00034920: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-00034930: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-00034940: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-00034950: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00034960: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00034970: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00034980: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-00034990: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-000349a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000349b0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000349c0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-000349d0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000349e0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000349f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00034a00: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-00034a10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00034a20: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00034a30: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-00034a40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00034a50: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-00034a60: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00034a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00034a80: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-00034a90: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-00034aa0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00034ab0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-00034ac0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00034ad0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-00034ae0: 204c 6179 6572 2829 0a20 2020 2020 2020   Layer().       
-00034af0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00034b00: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-00034b10: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-00034b20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00034b30: 656c 660a 0a0a 636c 6173 7320 4765 7450  elf...class GetP
-00034b40: 726f 7669 7369 6f6e 436f 6e66 6967 5265  rovisionConfigRe
-00034b50: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-00034b60: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00034b70: 5f28 7365 6c66 2c20 7175 616c 6966 6965  _(self, qualifie
-00034b80: 723d 4e6f 6e65 293a 0a20 2020 2020 2020  r=None):.       
-00034b90: 2023 2054 6865 2066 756e 6374 696f 6e20   # The function 
-00034ba0: 616c 6961 7320 6f72 204c 4154 4553 542e  alias or LATEST.
-00034bb0: 0a20 2020 2020 2020 2073 656c 662e 7175  .        self.qu
-00034bc0: 616c 6966 6965 7220 3d20 7175 616c 6966  alifier = qualif
-00034bd0: 6965 7220 2023 2074 7970 653a 2073 7472  ier  # type: str
-00034be0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00034bf0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00034c00: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00034c10: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00034c20: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00034c30: 6572 2847 6574 5072 6f76 6973 696f 6e43  er(GetProvisionC
-00034c40: 6f6e 6669 6752 6571 7565 7374 2c20 7365  onfigRequest, se
-00034c50: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-00034c60: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00034c70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00034c80: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00034c90: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00034ca0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00034cb0: 2020 2069 6620 7365 6c66 2e71 7561 6c69     if self.quali
-00034cc0: 6669 6572 2069 7320 6e6f 7420 4e6f 6e65  fier is not None
-00034cd0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00034ce0: 7375 6c74 5b27 7175 616c 6966 6965 7227  sult['qualifier'
-00034cf0: 5d20 3d20 7365 6c66 2e71 7561 6c69 6669  ] = self.qualifi
-00034d00: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
-00034d10: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00034d20: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00034d30: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-00034d40: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00034d50: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00034d60: 6574 2827 7175 616c 6966 6965 7227 2920  et('qualifier') 
-00034d70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00034d80: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
-00034d90: 616c 6966 6965 7220 3d20 6d2e 6765 7428  alifier = m.get(
-00034da0: 2771 7561 6c69 6669 6572 2729 0a20 2020  'qualifier').   
-00034db0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00034dc0: 0a0a 0a63 6c61 7373 2047 6574 5072 6f76  ...class GetProv
-00034dd0: 6973 696f 6e43 6f6e 6669 6752 6573 706f  isionConfigRespo
-00034de0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-00034df0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00034e00: 7365 6c66 2c20 6865 6164 6572 733d 4e6f  self, headers=No
-00034e10: 6e65 2c20 7374 6174 7573 5f63 6f64 653d  ne, status_code=
-00034e20: 4e6f 6e65 2c20 626f 6479 3d4e 6f6e 6529  None, body=None)
-00034e30: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-00034e40: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-00034e50: 2020 2320 7479 7065 3a20 6469 6374 5b73    # type: dict[s
-00034e60: 7472 2c20 7374 725d 0a20 2020 2020 2020  tr, str].       
-00034e70: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00034e80: 6520 3d20 7374 6174 7573 5f63 6f64 6520  e = status_code 
-00034e90: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
-00034ea0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00034eb0: 2062 6f64 7920 2023 2074 7970 653a 2050   body  # type: P
-00034ec0: 726f 7669 7369 6f6e 436f 6e66 6967 0a0a  rovisionConfig..
-00034ed0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00034ee0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00034ef0: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-00034f00: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00034f10: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-00034f20: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00034f30: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00034f40: 6170 203d 2073 7570 6572 2847 6574 5072  ap = super(GetPr
-00034f50: 6f76 6973 696f 6e43 6f6e 6669 6752 6573  ovisionConfigRes
-00034f60: 706f 6e73 652c 2073 656c 6629 2e74 6f5f  ponse, self).to_
-00034f70: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00034f80: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00034f90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00034fa0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00034fb0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00034fc0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00034fd0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-00034fe0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00034ff0: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-00035000: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-00035010: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-00035020: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00035030: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00035040: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00035050: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-00035060: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-00035070: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-00035080: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-00035090: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000350a0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-000350b0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-000350c0: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-000350d0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000350e0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000350f0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-00035100: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00035110: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00035120: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-00035130: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00035140: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-00035150: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-00035160: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-00035170: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-00035180: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-00035190: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000351a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000351b0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-000351c0: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-000351d0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-000351e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000351f0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-00035200: 6f64 656c 203d 2050 726f 7669 7369 6f6e  odel = Provision
-00035210: 436f 6e66 6967 2829 0a20 2020 2020 2020  Config().       
-00035220: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00035230: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-00035240: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-00035250: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00035260: 656c 660a 0a0a 636c 6173 7320 4765 7454  elf...class GetT
-00035270: 7269 6767 6572 5265 7370 6f6e 7365 2854  riggerResponse(T
-00035280: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00035290: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-000352a0: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
-000352b0: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
-000352c0: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
-000352d0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-000352e0: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
-000352f0: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
-00035300: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
-00035310: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-00035320: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
-00035330: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-00035340: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-00035350: 2020 2320 7479 7065 3a20 5472 6967 6765    # type: Trigge
-00035360: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-00035370: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00035380: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-00035390: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000353a0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-000353b0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000353c0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000353d0: 205f 6d61 7020 3d20 7375 7065 7228 4765   _map = super(Ge
-000353e0: 7454 7269 6767 6572 5265 7370 6f6e 7365  tTriggerResponse
-000353f0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-00035400: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00035410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00035420: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00035430: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00035440: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00035450: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00035460: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-00035470: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00035480: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-00035490: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-000354a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000354b0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-000354c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000354d0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-000354e0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-000354f0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-00035500: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00035510: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-00035520: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00035530: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-00035540: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-00035550: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00035560: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00035570: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
-00035580: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00035590: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000355a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000355b0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-000355c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000355d0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-000355e0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-000355f0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-00035600: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00035610: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00035620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035630: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-00035640: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00035650: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00035660: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-00035670: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00035680: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-00035690: 3d20 5472 6967 6765 7228 290a 2020 2020  = Trigger().    
-000356a0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-000356b0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-000356c0: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-000356d0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-000356e0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2049  n self...class I
-000356f0: 6e76 6f6b 6546 756e 6374 696f 6e48 6561  nvokeFunctionHea
-00035700: 6465 7273 2854 6561 4d6f 6465 6c29 3a0a  ders(TeaModel):.
-00035710: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00035720: 2873 656c 662c 2063 6f6d 6d6f 6e5f 6865  (self, common_he
-00035730: 6164 6572 733d 4e6f 6e65 2c20 785f 6663  aders=None, x_fc
-00035740: 5f61 7379 6e63 5f74 6173 6b5f 6964 3d4e  _async_task_id=N
-00035750: 6f6e 652c 2078 5f66 635f 696e 766f 6361  one, x_fc_invoca
-00035760: 7469 6f6e 5f74 7970 653d 4e6f 6e65 2c20  tion_type=None, 
-00035770: 785f 6663 5f6c 6f67 5f74 7970 653d 4e6f  x_fc_log_type=No
-00035780: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
-00035790: 662e 636f 6d6d 6f6e 5f68 6561 6465 7273  f.common_headers
-000357a0: 203d 2063 6f6d 6d6f 6e5f 6865 6164 6572   = common_header
-000357b0: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
-000357c0: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
-000357d0: 2020 7365 6c66 2e78 5f66 635f 6173 796e    self.x_fc_asyn
-000357e0: 635f 7461 736b 5f69 6420 3d20 785f 6663  c_task_id = x_fc
-000357f0: 5f61 7379 6e63 5f74 6173 6b5f 6964 2020  _async_task_id  
-00035800: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00035810: 2020 2020 2320 5468 6520 7479 7065 206f      # The type o
-00035820: 6620 6675 6e63 7469 6f6e 2069 6e76 6f63  f function invoc
-00035830: 6174 696f 6e2e 2056 616c 6964 2076 616c  ation. Valid val
-00035840: 7565 733a 2053 796e 6320 616e 6420 4173  ues: Sync and As
-00035850: 796e 632e 0a20 2020 2020 2020 2073 656c  ync..        sel
-00035860: 662e 785f 6663 5f69 6e76 6f63 6174 696f  f.x_fc_invocatio
-00035870: 6e5f 7479 7065 203d 2078 5f66 635f 696e  n_type = x_fc_in
-00035880: 766f 6361 7469 6f6e 5f74 7970 6520 2023  vocation_type  #
-00035890: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-000358a0: 2020 2023 2054 6865 206c 6f67 2074 7970     # The log typ
-000358b0: 6520 6f66 2066 756e 6374 696f 6e20 696e  e of function in
-000358c0: 766f 6361 7469 6f6e 2e20 5661 6c69 6420  vocation. Valid 
-000358d0: 7661 6c75 6573 3a20 4e6f 6e65 2061 6e64  values: None and
-000358e0: 2054 6169 6c2e 0a20 2020 2020 2020 2073   Tail..        s
-000358f0: 656c 662e 785f 6663 5f6c 6f67 5f74 7970  elf.x_fc_log_typ
-00035900: 6520 3d20 785f 6663 5f6c 6f67 5f74 7970  e = x_fc_log_typ
-00035910: 6520 2023 2074 7970 653a 2073 7472 0a0a  e  # type: str..
-00035920: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00035930: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00035940: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-00035950: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00035960: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00035970: 2849 6e76 6f6b 6546 756e 6374 696f 6e48  (InvokeFunctionH
-00035980: 6561 6465 7273 2c20 7365 6c66 292e 746f  eaders, self).to
-00035990: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000359a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000359b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000359c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000359d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000359e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000359f0: 7365 6c66 2e63 6f6d 6d6f 6e5f 6865 6164  self.common_head
-00035a00: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-00035a10: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00035a20: 756c 745b 2763 6f6d 6d6f 6e48 6561 6465  ult['commonHeade
-00035a30: 7273 275d 203d 2073 656c 662e 636f 6d6d  rs'] = self.comm
-00035a40: 6f6e 5f68 6561 6465 7273 0a20 2020 2020  on_headers.     
-00035a50: 2020 2069 6620 7365 6c66 2e78 5f66 635f     if self.x_fc_
-00035a60: 6173 796e 635f 7461 736b 5f69 6420 6973  async_task_id is
-00035a70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00035a80: 2020 2020 2020 2072 6573 756c 745b 2778         result['x
-00035a90: 2d66 632d 6173 796e 632d 7461 736b 2d69  -fc-async-task-i
-00035aa0: 6427 5d20 3d20 7365 6c66 2e78 5f66 635f  d'] = self.x_fc_
-00035ab0: 6173 796e 635f 7461 736b 5f69 640a 2020  async_task_id.  
-00035ac0: 2020 2020 2020 6966 2073 656c 662e 785f        if self.x_
-00035ad0: 6663 5f69 6e76 6f63 6174 696f 6e5f 7479  fc_invocation_ty
-00035ae0: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-00035af0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00035b00: 6c74 5b27 782d 6663 2d69 6e76 6f63 6174  lt['x-fc-invocat
-00035b10: 696f 6e2d 7479 7065 275d 203d 2073 656c  ion-type'] = sel
-00035b20: 662e 785f 6663 5f69 6e76 6f63 6174 696f  f.x_fc_invocatio
-00035b30: 6e5f 7479 7065 0a20 2020 2020 2020 2069  n_type.        i
-00035b40: 6620 7365 6c66 2e78 5f66 635f 6c6f 675f  f self.x_fc_log_
-00035b50: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-00035b60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00035b70: 7375 6c74 5b27 782d 6663 2d6c 6f67 2d74  sult['x-fc-log-t
-00035b80: 7970 6527 5d20 3d20 7365 6c66 2e78 5f66  ype'] = self.x_f
-00035b90: 635f 6c6f 675f 7479 7065 0a20 2020 2020  c_log_type.     
-00035ba0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00035bb0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00035bc0: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
-00035bd0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00035be0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00035bf0: 2020 6966 206d 2e67 6574 2827 636f 6d6d    if m.get('comm
-00035c00: 6f6e 4865 6164 6572 7327 2920 6973 206e  onHeaders') is n
-00035c10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00035c20: 2020 2020 2073 656c 662e 636f 6d6d 6f6e       self.common
-00035c30: 5f68 6561 6465 7273 203d 206d 2e67 6574  _headers = m.get
-00035c40: 2827 636f 6d6d 6f6e 4865 6164 6572 7327  ('commonHeaders'
-00035c50: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00035c60: 6574 2827 782d 6663 2d61 7379 6e63 2d74  et('x-fc-async-t
-00035c70: 6173 6b2d 6964 2729 2069 7320 6e6f 7420  ask-id') is not 
-00035c80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00035c90: 2020 7365 6c66 2e78 5f66 635f 6173 796e    self.x_fc_asyn
-00035ca0: 635f 7461 736b 5f69 6420 3d20 6d2e 6765  c_task_id = m.ge
-00035cb0: 7428 2778 2d66 632d 6173 796e 632d 7461  t('x-fc-async-ta
-00035cc0: 736b 2d69 6427 290a 2020 2020 2020 2020  sk-id').        
-00035cd0: 6966 206d 2e67 6574 2827 782d 6663 2d69  if m.get('x-fc-i
-00035ce0: 6e76 6f63 6174 696f 6e2d 7479 7065 2729  nvocation-type')
-00035cf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00035d00: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
-00035d10: 5f66 635f 696e 766f 6361 7469 6f6e 5f74  _fc_invocation_t
-00035d20: 7970 6520 3d20 6d2e 6765 7428 2778 2d66  ype = m.get('x-f
-00035d30: 632d 696e 766f 6361 7469 6f6e 2d74 7970  c-invocation-typ
-00035d40: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00035d50: 2e67 6574 2827 782d 6663 2d6c 6f67 2d74  .get('x-fc-log-t
-00035d60: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
-00035d70: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00035d80: 656c 662e 785f 6663 5f6c 6f67 5f74 7970  elf.x_fc_log_typ
-00035d90: 6520 3d20 6d2e 6765 7428 2778 2d66 632d  e = m.get('x-fc-
-00035da0: 6c6f 672d 7479 7065 2729 0a20 2020 2020  log-type').     
-00035db0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00035dc0: 0a63 6c61 7373 2049 6e76 6f6b 6546 756e  .class InvokeFun
-00035dd0: 6374 696f 6e52 6571 7565 7374 2854 6561  ctionRequest(Tea
-00035de0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00035df0: 5f5f 696e 6974 5f5f 2873 656c 662c 2062  __init__(self, b
-00035e00: 6f64 793d 4e6f 6e65 2c20 7175 616c 6966  ody=None, qualif
-00035e10: 6965 723d 4e6f 6e65 293a 0a20 2020 2020  ier=None):.     
-00035e20: 2020 2023 2054 6865 2072 6571 7565 7374     # The request
-00035e30: 2070 6172 616d 6574 6572 7320 6f66 2066   parameters of f
-00035e40: 756e 6374 696f 6e20 696e 766f 6361 7469  unction invocati
-00035e50: 6f6e 2e0a 2020 2020 2020 2020 7365 6c66  on..        self
-00035e60: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
-00035e70: 7479 7065 3a20 5245 4144 4142 4c45 0a20  type: READABLE. 
-00035e80: 2020 2020 2020 2023 2054 6865 2076 6572         # The ver
-00035e90: 7369 6f6e 206f 7220 616c 6961 7320 6f66  sion or alias of
-00035ea0: 2074 6865 2066 756e 6374 696f 6e2e 0a20   the function.. 
-00035eb0: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
-00035ec0: 6966 6965 7220 3d20 7175 616c 6966 6965  ifier = qualifie
-00035ed0: 7220 2023 2074 7970 653a 2073 7472 0a0a  r  # type: str..
-00035ee0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00035ef0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00035f00: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-00035f10: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00035f20: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00035f30: 2849 6e76 6f6b 6546 756e 6374 696f 6e52  (InvokeFunctionR
-00035f40: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
-00035f50: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00035f60: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00035f70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00035f80: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00035f90: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00035fa0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00035fb0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-00035fc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00035fd0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-00035fe0: 5d20 3d20 7365 6c66 2e62 6f64 790a 2020  ] = self.body.  
-00035ff0: 2020 2020 2020 6966 2073 656c 662e 7175        if self.qu
-00036000: 616c 6966 6965 7220 6973 206e 6f74 204e  alifier is not N
-00036010: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00036020: 2072 6573 756c 745b 2771 7561 6c69 6669   result['qualifi
-00036030: 6572 275d 203d 2073 656c 662e 7175 616c  er'] = self.qual
-00036040: 6966 6965 720a 2020 2020 2020 2020 7265  ifier.        re
-00036050: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00036060: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00036070: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
-00036080: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-00036090: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000360a0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-000360b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000360c0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-000360d0: 203d 206d 2e67 6574 2827 626f 6479 2729   = m.get('body')
-000360e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000360f0: 7428 2771 7561 6c69 6669 6572 2729 2069  t('qualifier') i
-00036100: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00036110: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
-00036120: 6c69 6669 6572 203d 206d 2e67 6574 2827  lifier = m.get('
-00036130: 7175 616c 6966 6965 7227 290a 2020 2020  qualifier').    
-00036140: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00036150: 0a0a 636c 6173 7320 496e 766f 6b65 4675  ..class InvokeFu
-00036160: 6e63 7469 6f6e 5265 7370 6f6e 7365 2854  nctionResponse(T
-00036170: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00036180: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00036190: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
-000361a0: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
-000361b0: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
-000361c0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-000361d0: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
-000361e0: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
-000361f0: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
-00036200: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-00036210: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
-00036220: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-00036230: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-00036240: 2020 2320 7479 7065 3a20 5245 4144 4142    # type: READAB
-00036250: 4c45 0a0a 2020 2020 6465 6620 7661 6c69  LE..    def vali
-00036260: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00036270: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00036280: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00036290: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-000362a0: 7570 6572 2849 6e76 6f6b 6546 756e 6374  uper(InvokeFunct
-000362b0: 696f 6e52 6573 706f 6e73 652c 2073 656c  ionResponse, sel
-000362c0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-000362d0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-000362e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000362f0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00036300: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00036310: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00036320: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-00036330: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00036340: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00036350: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-00036360: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-00036370: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00036380: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-00036390: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000363a0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-000363b0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-000363c0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-000363d0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-000363e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000363f0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00036400: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00036410: 790a 2020 2020 2020 2020 7265 7475 726e  y.        return
-00036420: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00036430: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00036440: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-00036450: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00036460: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00036470: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
-00036480: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00036490: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-000364a0: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
-000364b0: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
-000364c0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-000364d0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
-000364e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000364f0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-00036500: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-00036510: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
-00036520: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-00036530: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00036540: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00036550: 203d 206d 2e67 6574 2827 626f 6479 2729   = m.get('body')
-00036560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00036570: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-00036580: 7441 6c69 6173 6573 5265 7175 6573 7428  tAliasesRequest(
-00036590: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-000365a0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000365b0: 2c20 6c69 6d69 743d 4e6f 6e65 2c20 6e65  , limit=None, ne
-000365c0: 7874 5f74 6f6b 656e 3d4e 6f6e 652c 2070  xt_token=None, p
-000365d0: 7265 6669 783d 4e6f 6e65 293a 0a20 2020  refix=None):.   
-000365e0: 2020 2020 2023 2054 6865 206e 756d 6265       # The numbe
-000365f0: 7220 6f66 2061 6c69 6173 6573 2072 6574  r of aliases ret
-00036600: 7572 6e65 642e 0a20 2020 2020 2020 2073  urned..        s
-00036610: 656c 662e 6c69 6d69 7420 3d20 6c69 6d69  elf.limit = limi
-00036620: 7420 2023 2074 7970 653a 2069 6e74 0a20  t  # type: int. 
-00036630: 2020 2020 2020 2023 2054 6865 2070 6167         # The pag
-00036640: 696e 6174 696f 6e20 746f 6b65 6e20 7468  ination token th
-00036650: 6174 2069 7320 7573 6564 2069 6e20 7468  at is used in th
-00036660: 6520 6e65 7874 2072 6571 7565 7374 2074  e next request t
-00036670: 6f20 7265 7472 6965 7665 2061 206e 6577  o retrieve a new
-00036680: 2070 6167 6520 6f66 2072 6573 756c 7473   page of results
-00036690: 2e0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-000366a0: 6578 745f 746f 6b65 6e20 3d20 6e65 7874  ext_token = next
-000366b0: 5f74 6f6b 656e 2020 2320 7479 7065 3a20  _token  # type: 
-000366c0: 7374 720a 2020 2020 2020 2020 2320 5468  str.        # Th
-000366d0: 6520 616c 6961 7320 7072 6566 6978 2e0a  e alias prefix..
-000366e0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-000366f0: 6669 7820 3d20 7072 6566 6978 2020 2320  fix = prefix  # 
-00036700: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-00036710: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00036720: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00036730: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00036740: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00036750: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
-00036760: 416c 6961 7365 7352 6571 7565 7374 2c20  AliasesRequest, 
-00036770: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-00036780: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00036790: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000367a0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000367b0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-000367c0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-000367d0: 2020 2020 2069 6620 7365 6c66 2e6c 696d       if self.lim
-000367e0: 6974 2069 7320 6e6f 7420 4e6f 6e65 3a0a  it is not None:.
-000367f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00036800: 6c74 5b27 6c69 6d69 7427 5d20 3d20 7365  lt['limit'] = se
-00036810: 6c66 2e6c 696d 6974 0a20 2020 2020 2020  lf.limit.       
-00036820: 2069 6620 7365 6c66 2e6e 6578 745f 746f   if self.next_to
-00036830: 6b65 6e20 6973 206e 6f74 204e 6f6e 653a  ken is not None:
-00036840: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00036850: 756c 745b 276e 6578 7454 6f6b 656e 275d  ult['nextToken']
-00036860: 203d 2073 656c 662e 6e65 7874 5f74 6f6b   = self.next_tok
-00036870: 656e 0a20 2020 2020 2020 2069 6620 7365  en.        if se
-00036880: 6c66 2e70 7265 6669 7820 6973 206e 6f74  lf.prefix is not
-00036890: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000368a0: 2020 2072 6573 756c 745b 2770 7265 6669     result['prefi
-000368b0: 7827 5d20 3d20 7365 6c66 2e70 7265 6669  x'] = self.prefi
-000368c0: 780a 2020 2020 2020 2020 7265 7475 726e  x.        return
-000368d0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-000368e0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-000368f0: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-00036900: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00036910: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00036920: 7428 276c 696d 6974 2729 2069 7320 6e6f  t('limit') is no
-00036930: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036940: 2020 2020 7365 6c66 2e6c 696d 6974 203d      self.limit =
-00036950: 206d 2e67 6574 2827 6c69 6d69 7427 290a   m.get('limit').
-00036960: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00036970: 2827 6e65 7874 546f 6b65 6e27 2920 6973  ('nextToken') is
-00036980: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00036990: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
-000369a0: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
-000369b0: 6e65 7874 546f 6b65 6e27 290a 2020 2020  nextToken').    
-000369c0: 2020 2020 6966 206d 2e67 6574 2827 7072      if m.get('pr
-000369d0: 6566 6978 2729 2069 7320 6e6f 7420 4e6f  efix') is not No
-000369e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000369f0: 7365 6c66 2e70 7265 6669 7820 3d20 6d2e  self.prefix = m.
-00036a00: 6765 7428 2770 7265 6669 7827 290a 2020  get('prefix').  
-00036a10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00036a20: 660a 0a0a 636c 6173 7320 4c69 7374 416c  f...class ListAl
-00036a30: 6961 7365 7352 6573 706f 6e73 6528 5465  iasesResponse(Te
-00036a40: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00036a50: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00036a60: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
-00036a70: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
-00036a80: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
-00036a90: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00036aa0: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
-00036ab0: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
-00036ac0: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
-00036ad0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-00036ae0: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
-00036af0: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-00036b00: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
-00036b10: 2023 2074 7970 653a 204c 6973 7441 6c69   # type: ListAli
-00036b20: 6173 6573 4f75 7470 7574 0a0a 2020 2020  asesOutput..    
-00036b30: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00036b40: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00036b50: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
-00036b60: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
-00036b70: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
-00036b80: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-00036b90: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-00036ba0: 2073 7570 6572 284c 6973 7441 6c69 6173   super(ListAlias
-00036bb0: 6573 5265 7370 6f6e 7365 2c20 7365 6c66  esResponse, self
-00036bc0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00036bd0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00036be0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036bf0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00036c00: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00036c10: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00036c20: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00036c30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00036c40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00036c50: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00036c60: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-00036c70: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00036c80: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00036c90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00036ca0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00036cb0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00036cc0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00036cd0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00036ce0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00036cf0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00036d00: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00036d10: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00036d20: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00036d30: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00036d40: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00036d50: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00036d60: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00036d70: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-00036d80: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-00036d90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00036da0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-00036db0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-00036dc0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00036dd0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00036de0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00036df0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00036e00: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00036e10: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00036e20: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00036e30: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-00036e40: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00036e50: 656d 705f 6d6f 6465 6c20 3d20 4c69 7374  emp_model = List
-00036e60: 416c 6961 7365 734f 7574 7075 7428 290a  AliasesOutput().
-00036e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00036e80: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-00036e90: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-00036ea0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-00036eb0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00036ec0: 7373 204c 6973 7441 7379 6e63 496e 766f  ss ListAsyncInvo
-00036ed0: 6b65 436f 6e66 6967 7352 6571 7565 7374  keConfigsRequest
-00036ee0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00036ef0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00036f00: 662c 2066 756e 6374 696f 6e5f 6e61 6d65  f, function_name
-00036f10: 3d4e 6f6e 652c 206c 696d 6974 3d4e 6f6e  =None, limit=Non
-00036f20: 652c 206e 6578 745f 746f 6b65 6e3d 4e6f  e, next_token=No
-00036f30: 6e65 293a 0a20 2020 2020 2020 2023 2054  ne):.        # T
-00036f40: 6865 2066 756e 6374 696f 6e20 6e61 6d65  he function name
-00036f50: 2e20 4966 2079 6f75 2064 6f20 6e6f 7420  . If you do not 
-00036f60: 636f 6e66 6967 7572 6520 7468 6973 2070  configure this p
-00036f70: 6172 616d 6574 6572 2c20 7468 6520 6173  arameter, the as
-00036f80: 796e 6368 726f 6e6f 7573 2069 6e76 6f63  ynchronous invoc
-00036f90: 6174 696f 6e20 636f 6e66 6967 7572 6174  ation configurat
-00036fa0: 696f 6e73 206f 6620 616c 6c20 6675 6e63  ions of all func
-00036fb0: 7469 6f6e 7320 6172 6520 6469 7370 6c61  tions are displa
-00036fc0: 7965 642e 0a20 2020 2020 2020 2073 656c  yed..        sel
-00036fd0: 662e 6675 6e63 7469 6f6e 5f6e 616d 6520  f.function_name 
-00036fe0: 3d20 6675 6e63 7469 6f6e 5f6e 616d 6520  = function_name 
-00036ff0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-00037000: 2020 2020 2023 2054 6865 206d 6178 696d       # The maxim
-00037010: 756d 206e 756d 6265 7220 6f66 2065 6e74  um number of ent
-00037020: 7269 6573 2074 6f20 6265 2072 6574 7572  ries to be retur
-00037030: 6e65 642e 0a20 2020 2020 2020 2073 656c  ned..        sel
-00037040: 662e 6c69 6d69 7420 3d20 6c69 6d69 7420  f.limit = limit 
-00037050: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
-00037060: 2020 2020 2023 2054 6865 2070 6167 696e       # The pagin
-00037070: 6720 696e 666f 726d 6174 696f 6e2e 2054  g information. T
-00037080: 6869 7320 7061 7261 6d65 7465 7220 7370  his parameter sp
-00037090: 6563 6966 6965 7320 7468 6520 7374 6172  ecifies the star
-000370a0: 7420 706f 696e 7420 6f66 2074 6865 2071  t point of the q
-000370b0: 7565 7279 2e0a 2020 2020 2020 2020 7365  uery..        se
-000370c0: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
-000370d0: 6e65 7874 5f74 6f6b 656e 2020 2320 7479  next_token  # ty
-000370e0: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-000370f0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-00037100: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00037110: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00037120: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00037130: 7020 3d20 7375 7065 7228 4c69 7374 4173  p = super(ListAs
-00037140: 796e 6349 6e76 6f6b 6543 6f6e 6669 6773  yncInvokeConfigs
-00037150: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
-00037160: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00037170: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00037180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00037190: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000371a0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000371b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000371c0: 2073 656c 662e 6675 6e63 7469 6f6e 5f6e   self.function_n
-000371d0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-000371e0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000371f0: 756c 745b 2766 756e 6374 696f 6e4e 616d  ult['functionNam
-00037200: 6527 5d20 3d20 7365 6c66 2e66 756e 6374  e'] = self.funct
-00037210: 696f 6e5f 6e61 6d65 0a20 2020 2020 2020  ion_name.       
-00037220: 2069 6620 7365 6c66 2e6c 696d 6974 2069   if self.limit i
-00037230: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00037240: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00037250: 6c69 6d69 7427 5d20 3d20 7365 6c66 2e6c  limit'] = self.l
-00037260: 696d 6974 0a20 2020 2020 2020 2069 6620  imit.        if 
-00037270: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
-00037280: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00037290: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000372a0: 276e 6578 7454 6f6b 656e 275d 203d 2073  'nextToken'] = s
-000372b0: 656c 662e 6e65 7874 5f74 6f6b 656e 0a20  elf.next_token. 
-000372c0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000372d0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000372e0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-000372f0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00037300: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00037310: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00037320: 6675 6e63 7469 6f6e 4e61 6d65 2729 2069  functionName') i
-00037330: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00037340: 2020 2020 2020 2020 7365 6c66 2e66 756e          self.fun
-00037350: 6374 696f 6e5f 6e61 6d65 203d 206d 2e67  ction_name = m.g
-00037360: 6574 2827 6675 6e63 7469 6f6e 4e61 6d65  et('functionName
-00037370: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00037380: 6765 7428 276c 696d 6974 2729 2069 7320  get('limit') is 
-00037390: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000373a0: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
-000373b0: 203d 206d 2e67 6574 2827 6c69 6d69 7427   = m.get('limit'
-000373c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000373d0: 6574 2827 6e65 7874 546f 6b65 6e27 2920  et('nextToken') 
-000373e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000373f0: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-00037400: 7874 5f74 6f6b 656e 203d 206d 2e67 6574  xt_token = m.get
-00037410: 2827 6e65 7874 546f 6b65 6e27 290a 2020  ('nextToken').  
-00037420: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00037430: 660a 0a0a 636c 6173 7320 4c69 7374 4173  f...class ListAs
-00037440: 796e 6349 6e76 6f6b 6543 6f6e 6669 6773  yncInvokeConfigs
-00037450: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00037460: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00037470: 6974 5f5f 2873 656c 662c 2068 6561 6465  it__(self, heade
-00037480: 7273 3d4e 6f6e 652c 2073 7461 7475 735f  rs=None, status_
-00037490: 636f 6465 3d4e 6f6e 652c 2062 6f64 793d  code=None, body=
-000374a0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-000374b0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-000374c0: 6164 6572 7320 2023 2074 7970 653a 2064  aders  # type: d
-000374d0: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
-000374e0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-000374f0: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-00037500: 636f 6465 2020 2320 7479 7065 3a20 696e  code  # type: in
-00037510: 740a 2020 2020 2020 2020 7365 6c66 2e62  t.        self.b
-00037520: 6f64 7920 3d20 626f 6479 2020 2320 7479  ody = body  # ty
-00037530: 7065 3a20 4c69 7374 4173 796e 6349 6e76  pe: ListAsyncInv
-00037540: 6f6b 6543 6f6e 6669 674f 7574 7075 740a  okeConfigOutput.
-00037550: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00037560: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00037570: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00037580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00037590: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-000375a0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000375b0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000375c0: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
-000375d0: 4173 796e 6349 6e76 6f6b 6543 6f6e 6669  AsyncInvokeConfi
-000375e0: 6773 5265 7370 6f6e 7365 2c20 7365 6c66  gsResponse, self
-000375f0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00037600: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00037610: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00037620: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00037630: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00037640: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00037650: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00037660: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00037670: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00037680: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00037690: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-000376a0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-000376b0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-000376c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000376d0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-000376e0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-000376f0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00037700: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00037710: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00037720: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00037730: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00037740: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00037750: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00037760: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00037770: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00037780: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00037790: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000377a0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-000377b0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-000377c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000377d0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-000377e0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-000377f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00037800: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00037810: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00037820: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00037830: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00037840: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00037850: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00037860: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-00037870: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00037880: 656d 705f 6d6f 6465 6c20 3d20 4c69 7374  emp_model = List
-00037890: 4173 796e 6349 6e76 6f6b 6543 6f6e 6669  AsyncInvokeConfi
-000378a0: 674f 7574 7075 7428 290a 2020 2020 2020  gOutput().      
-000378b0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-000378c0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
-000378d0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
-000378e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000378f0: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-00037900: 7443 6f6e 6375 7272 656e 6379 436f 6e66  tConcurrencyConf
-00037910: 6967 7352 6571 7565 7374 2854 6561 4d6f  igsRequest(TeaMo
-00037920: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00037930: 696e 6974 5f5f 2873 656c 662c 2066 756e  init__(self, fun
-00037940: 6374 696f 6e5f 6e61 6d65 3d4e 6f6e 652c  ction_name=None,
-00037950: 206c 696d 6974 3d4e 6f6e 652c 206e 6578   limit=None, nex
-00037960: 745f 746f 6b65 6e3d 4e6f 6e65 293a 0a20  t_token=None):. 
-00037970: 2020 2020 2020 2023 2054 6865 2066 756e         # The fun
-00037980: 6374 696f 6e20 6e61 6d65 2e20 4966 2079  ction name. If y
-00037990: 6f75 206c 6561 7665 2074 6869 7320 7061  ou leave this pa
-000379a0: 7261 6d65 7465 7220 656d 7074 792c 2074  rameter empty, t
-000379b0: 6865 2063 6f6e 6375 7272 656e 6379 2063  he concurrency c
-000379c0: 6f6e 6669 6775 7261 7469 6f6e 7320 6f66  onfigurations of
-000379d0: 2061 6c6c 2066 756e 6374 696f 6e73 2061   all functions a
-000379e0: 7265 2072 6574 7572 6e65 642e 0a20 2020  re returned..   
-000379f0: 2020 2020 2073 656c 662e 6675 6e63 7469       self.functi
-00037a00: 6f6e 5f6e 616d 6520 3d20 6675 6e63 7469  on_name = functi
-00037a10: 6f6e 5f6e 616d 6520 2023 2074 7970 653a  on_name  # type:
-00037a20: 2073 7472 0a20 2020 2020 2020 2023 2054   str.        # T
-00037a30: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-00037a40: 7220 6f66 2065 6e74 7269 6573 2072 6574  r of entries ret
-00037a50: 7572 6e65 642e 0a20 2020 2020 2020 2073  urned..        s
-00037a60: 656c 662e 6c69 6d69 7420 3d20 6c69 6d69  elf.limit = limi
-00037a70: 7420 2023 2074 7970 653a 2069 6e74 0a20  t  # type: int. 
-00037a80: 2020 2020 2020 2023 2054 6865 2070 6167         # The pag
-00037a90: 696e 6174 696f 6e20 746f 6b65 6e20 7468  ination token th
-00037aa0: 6174 2069 7320 7573 6564 2069 6e20 7468  at is used in th
-00037ab0: 6520 6e65 7874 2072 6571 7565 7374 2074  e next request t
-00037ac0: 6f20 7265 7472 6965 7665 2061 206e 6577  o retrieve a new
-00037ad0: 2070 6167 6520 6f66 2072 6573 756c 7473   page of results
-00037ae0: 2e0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-00037af0: 6578 745f 746f 6b65 6e20 3d20 6e65 7874  ext_token = next
-00037b00: 5f74 6f6b 656e 2020 2320 7479 7065 3a20  _token  # type: 
-00037b10: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
-00037b20: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00037b30: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00037b40: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00037b50: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00037b60: 7375 7065 7228 4c69 7374 436f 6e63 7572  super(ListConcur
-00037b70: 7265 6e63 7943 6f6e 6669 6773 5265 7175  rencyConfigsRequ
-00037b80: 6573 742c 2073 656c 6629 2e74 6f5f 6d61  est, self).to_ma
-00037b90: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00037ba0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00037bb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00037bc0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00037bd0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00037be0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00037bf0: 662e 6675 6e63 7469 6f6e 5f6e 616d 6520  f.function_name 
-00037c00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00037c10: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00037c20: 2766 756e 6374 696f 6e4e 616d 6527 5d20  'functionName'] 
-00037c30: 3d20 7365 6c66 2e66 756e 6374 696f 6e5f  = self.function_
-00037c40: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
-00037c50: 7365 6c66 2e6c 696d 6974 2069 7320 6e6f  self.limit is no
-00037c60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00037c70: 2020 2020 7265 7375 6c74 5b27 6c69 6d69      result['limi
-00037c80: 7427 5d20 3d20 7365 6c66 2e6c 696d 6974  t'] = self.limit
-00037c90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00037ca0: 2e6e 6578 745f 746f 6b65 6e20 6973 206e  .next_token is n
-00037cb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00037cc0: 2020 2020 2072 6573 756c 745b 276e 6578       result['nex
-00037cd0: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
-00037ce0: 6e65 7874 5f74 6f6b 656e 0a20 2020 2020  next_token.     
-00037cf0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00037d00: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00037d10: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
-00037d20: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00037d30: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00037d40: 2020 6966 206d 2e67 6574 2827 6675 6e63    if m.get('func
-00037d50: 7469 6f6e 4e61 6d65 2729 2069 7320 6e6f  tionName') is no
-00037d60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00037d70: 2020 2020 7365 6c66 2e66 756e 6374 696f      self.functio
-00037d80: 6e5f 6e61 6d65 203d 206d 2e67 6574 2827  n_name = m.get('
-00037d90: 6675 6e63 7469 6f6e 4e61 6d65 2729 0a20  functionName'). 
-00037da0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00037db0: 276c 696d 6974 2729 2069 7320 6e6f 7420  'limit') is not 
-00037dc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00037dd0: 2020 7365 6c66 2e6c 696d 6974 203d 206d    self.limit = m
-00037de0: 2e67 6574 2827 6c69 6d69 7427 290a 2020  .get('limit').  
-00037df0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00037e00: 6e65 7874 546f 6b65 6e27 2920 6973 206e  nextToken') is n
-00037e10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00037e20: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
-00037e30: 6f6b 656e 203d 206d 2e67 6574 2827 6e65  oken = m.get('ne
-00037e40: 7874 546f 6b65 6e27 290a 2020 2020 2020  xtToken').      
-00037e50: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00037e60: 636c 6173 7320 4c69 7374 436f 6e63 7572  class ListConcur
-00037e70: 7265 6e63 7943 6f6e 6669 6773 5265 7370  rencyConfigsResp
-00037e80: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-00037e90: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00037ea0: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
-00037eb0: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
-00037ec0: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
-00037ed0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00037ee0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-00037ef0: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
-00037f00: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
-00037f10: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00037f20: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-00037f30: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
-00037f40: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-00037f50: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
-00037f60: 4c69 7374 436f 6e63 7572 7265 6e63 7943  ListConcurrencyC
-00037f70: 6f6e 6669 6773 4f75 7470 7574 0a0a 2020  onfigsOutput..  
-00037f80: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00037f90: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00037fa0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-00037fb0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00037fc0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-00037fd0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00037fe0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00037ff0: 203d 2073 7570 6572 284c 6973 7443 6f6e   = super(ListCon
-00038000: 6375 7272 656e 6379 436f 6e66 6967 7352  currencyConfigsR
-00038010: 6573 706f 6e73 652c 2073 656c 6629 2e74  esponse, self).t
-00038020: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00038030: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00038040: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00038050: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00038060: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00038070: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00038080: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-00038090: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000380a0: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-000380b0: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-000380c0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-000380d0: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-000380e0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-000380f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00038100: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-00038110: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-00038120: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-00038130: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-00038140: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00038150: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-00038160: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-00038170: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-00038180: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00038190: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000381a0: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
-000381b0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000381c0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000381d0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-000381e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000381f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00038200: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00038210: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00038220: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00038230: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00038240: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00038250: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00038260: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-00038270: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-00038280: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-00038290: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000382a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000382b0: 5f6d 6f64 656c 203d 204c 6973 7443 6f6e  _model = ListCon
-000382c0: 6375 7272 656e 6379 436f 6e66 6967 734f  currencyConfigsO
-000382d0: 7574 7075 7428 290a 2020 2020 2020 2020  utput().        
-000382e0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-000382f0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00038300: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-00038310: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00038320: 6c66 0a0a 0a63 6c61 7373 204c 6973 7443  lf...class ListC
-00038330: 7573 746f 6d44 6f6d 6169 6e73 5265 7175  ustomDomainsRequ
-00038340: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-00038350: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00038360: 7365 6c66 2c20 6c69 6d69 743d 4e6f 6e65  self, limit=None
-00038370: 2c20 6e65 7874 5f74 6f6b 656e 3d4e 6f6e  , next_token=Non
-00038380: 652c 2070 7265 6669 783d 4e6f 6e65 293a  e, prefix=None):
-00038390: 0a20 2020 2020 2020 2023 2054 6865 206e  .        # The n
-000383a0: 756d 6265 7220 6f66 2063 7573 746f 6d20  umber of custom 
-000383b0: 646f 6d61 696e 206e 616d 6573 2072 6574  domain names ret
-000383c0: 7572 6e65 642e 0a20 2020 2020 2020 2073  urned..        s
-000383d0: 656c 662e 6c69 6d69 7420 3d20 6c69 6d69  elf.limit = limi
-000383e0: 7420 2023 2074 7970 653a 2069 6e74 0a20  t  # type: int. 
-000383f0: 2020 2020 2020 2023 2054 6865 2070 6167         # The pag
-00038400: 696e 6174 696f 6e20 746f 6b65 6e20 7468  ination token th
-00038410: 6174 2069 7320 7573 6564 2069 6e20 7468  at is used in th
-00038420: 6520 6e65 7874 2072 6571 7565 7374 2074  e next request t
-00038430: 6f20 7265 7472 6965 7665 2061 206e 6577  o retrieve a new
-00038440: 2070 6167 6520 6f66 2072 6573 756c 7473   page of results
-00038450: 2e0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-00038460: 6578 745f 746f 6b65 6e20 3d20 6e65 7874  ext_token = next
-00038470: 5f74 6f6b 656e 2020 2320 7479 7065 3a20  _token  # type: 
-00038480: 7374 720a 2020 2020 2020 2020 2320 5468  str.        # Th
-00038490: 6520 646f 6d61 696e 206e 616d 6520 7072  e domain name pr
-000384a0: 6566 6978 2e0a 2020 2020 2020 2020 7365  efix..        se
-000384b0: 6c66 2e70 7265 6669 7820 3d20 7072 6566  lf.prefix = pref
-000384c0: 6978 2020 2320 7479 7065 3a20 7374 720a  ix  # type: str.
-000384d0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-000384e0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000384f0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00038500: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00038510: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00038520: 7228 4c69 7374 4375 7374 6f6d 446f 6d61  r(ListCustomDoma
-00038530: 696e 7352 6571 7565 7374 2c20 7365 6c66  insRequest, self
-00038540: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00038550: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00038560: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00038570: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00038580: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00038590: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000385a0: 2069 6620 7365 6c66 2e6c 696d 6974 2069   if self.limit i
-000385b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000385c0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000385d0: 6c69 6d69 7427 5d20 3d20 7365 6c66 2e6c  limit'] = self.l
-000385e0: 696d 6974 0a20 2020 2020 2020 2069 6620  imit.        if 
-000385f0: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
-00038600: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00038610: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00038620: 276e 6578 7454 6f6b 656e 275d 203d 2073  'nextToken'] = s
-00038630: 656c 662e 6e65 7874 5f74 6f6b 656e 0a20  elf.next_token. 
-00038640: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00038650: 7265 6669 7820 6973 206e 6f74 204e 6f6e  refix is not Non
-00038660: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00038670: 6573 756c 745b 2770 7265 6669 7827 5d20  esult['prefix'] 
-00038680: 3d20 7365 6c66 2e70 7265 6669 780a 2020  = self.prefix.  
-00038690: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000386a0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-000386b0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-000386c0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-000386d0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-000386e0: 2020 2020 2069 6620 6d2e 6765 7428 276c       if m.get('l
-000386f0: 696d 6974 2729 2069 7320 6e6f 7420 4e6f  imit') is not No
-00038700: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00038710: 7365 6c66 2e6c 696d 6974 203d 206d 2e67  self.limit = m.g
-00038720: 6574 2827 6c69 6d69 7427 290a 2020 2020  et('limit').    
-00038730: 2020 2020 6966 206d 2e67 6574 2827 6e65      if m.get('ne
-00038740: 7874 546f 6b65 6e27 2920 6973 206e 6f74  xtToken') is not
-00038750: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00038760: 2020 2073 656c 662e 6e65 7874 5f74 6f6b     self.next_tok
-00038770: 656e 203d 206d 2e67 6574 2827 6e65 7874  en = m.get('next
-00038780: 546f 6b65 6e27 290a 2020 2020 2020 2020  Token').        
-00038790: 6966 206d 2e67 6574 2827 7072 6566 6978  if m.get('prefix
-000387a0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000387b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000387c0: 2e70 7265 6669 7820 3d20 6d2e 6765 7428  .prefix = m.get(
-000387d0: 2770 7265 6669 7827 290a 2020 2020 2020  'prefix').      
-000387e0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000387f0: 636c 6173 7320 4c69 7374 4375 7374 6f6d  class ListCustom
-00038800: 446f 6d61 696e 7352 6573 706f 6e73 6528  DomainsResponse(
-00038810: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00038820: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00038830: 2c20 6865 6164 6572 733d 4e6f 6e65 2c20  , headers=None, 
-00038840: 7374 6174 7573 5f63 6f64 653d 4e6f 6e65  status_code=None
-00038850: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
-00038860: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00038870: 7273 203d 2068 6561 6465 7273 2020 2320  rs = headers  # 
-00038880: 7479 7065 3a20 6469 6374 5b73 7472 2c20  type: dict[str, 
-00038890: 7374 725d 0a20 2020 2020 2020 2073 656c  str].        sel
-000388a0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-000388b0: 7374 6174 7573 5f63 6f64 6520 2023 2074  status_code  # t
-000388c0: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
-000388d0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-000388e0: 7920 2023 2074 7970 653a 204c 6973 7443  y  # type: ListC
-000388f0: 7573 746f 6d44 6f6d 6169 6e4f 7574 7075  ustomDomainOutpu
-00038900: 740a 0a20 2020 2064 6566 2076 616c 6964  t..    def valid
-00038910: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00038920: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-00038930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00038940: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-00038950: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-00038960: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00038970: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
-00038980: 7374 4375 7374 6f6d 446f 6d61 696e 7352  stCustomDomainsR
-00038990: 6573 706f 6e73 652c 2073 656c 6629 2e74  esponse, self).t
-000389a0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000389b0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000389c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000389d0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000389e0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000389f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00038a00: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-00038a10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00038a20: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-00038a30: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-00038a40: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-00038a50: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-00038a60: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-00038a70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00038a80: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-00038a90: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-00038aa0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-00038ab0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-00038ac0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00038ad0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-00038ae0: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-00038af0: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-00038b00: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00038b10: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00038b20: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
-00038b30: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00038b40: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00038b50: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00038b60: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00038b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00038b80: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00038b90: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00038ba0: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00038bb0: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00038bc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00038bd0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00038be0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-00038bf0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-00038c00: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-00038c10: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00038c20: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00038c30: 5f6d 6f64 656c 203d 204c 6973 7443 7573  _model = ListCus
-00038c40: 746f 6d44 6f6d 6169 6e4f 7574 7075 7428  tomDomainOutput(
-00038c50: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00038c60: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-00038c70: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-00038c80: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-00038c90: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00038ca0: 6c61 7373 204c 6973 7446 756e 6374 696f  lass ListFunctio
-00038cb0: 6e56 6572 7369 6f6e 7352 6571 7565 7374  nVersionsRequest
-00038cc0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00038cd0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00038ce0: 662c 2064 6972 6563 7469 6f6e 3d4e 6f6e  f, direction=Non
-00038cf0: 652c 206c 696d 6974 3d4e 6f6e 652c 206e  e, limit=None, n
-00038d00: 6578 745f 746f 6b65 6e3d 4e6f 6e65 293a  ext_token=None):
-00038d10: 0a20 2020 2020 2020 2023 2054 6865 2073  .        # The s
-00038d20: 6f72 7469 6e67 206d 6f64 6520 6f66 2066  orting mode of f
-00038d30: 756e 6374 696f 6e20 7665 7273 696f 6e73  unction versions
-00038d40: 2e20 5661 6c69 6420 7661 6c75 6573 3a20  . Valid values: 
-00038d50: 4241 434b 5741 5244 2061 6e64 2046 4f52  BACKWARD and FOR
-00038d60: 5741 5244 2e0a 2020 2020 2020 2020 7365  WARD..        se
-00038d70: 6c66 2e64 6972 6563 7469 6f6e 203d 2064  lf.direction = d
-00038d80: 6972 6563 7469 6f6e 2020 2320 7479 7065  irection  # type
-00038d90: 3a20 7374 720a 2020 2020 2020 2020 2320  : str.        # 
-00038da0: 5468 6520 6e75 6d62 6572 206f 6620 6675  The number of fu
-00038db0: 6e63 7469 6f6e 2076 6572 7369 6f6e 7320  nction versions 
-00038dc0: 7468 6174 2061 7265 2072 6574 7572 6e65  that are returne
-00038dd0: 642e 0a20 2020 2020 2020 2073 656c 662e  d..        self.
-00038de0: 6c69 6d69 7420 3d20 6c69 6d69 7420 2023  limit = limit  #
-00038df0: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
-00038e00: 2020 2023 2054 6865 2070 6167 696e 6174     # The paginat
-00038e10: 696f 6e20 746f 6b65 6e20 7468 6174 2069  ion token that i
-00038e20: 7320 7573 6564 2069 6e20 7468 6520 6e65  s used in the ne
-00038e30: 7874 2072 6571 7565 7374 2074 6f20 7265  xt request to re
-00038e40: 7472 6965 7665 2061 206e 6577 2070 6167  trieve a new pag
-00038e50: 6520 6f66 2072 6573 756c 7473 2e0a 2020  e of results..  
-00038e60: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
-00038e70: 746f 6b65 6e20 3d20 6e65 7874 5f74 6f6b  token = next_tok
-00038e80: 656e 2020 2320 7479 7065 3a20 7374 720a  en  # type: str.
-00038e90: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00038ea0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00038eb0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00038ec0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00038ed0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00038ee0: 7228 4c69 7374 4675 6e63 7469 6f6e 5665  r(ListFunctionVe
-00038ef0: 7273 696f 6e73 5265 7175 6573 742c 2073  rsionsRequest, s
-00038f00: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-00038f10: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00038f20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00038f30: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00038f40: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00038f50: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00038f60: 2020 2020 6966 2073 656c 662e 6469 7265      if self.dire
-00038f70: 6374 696f 6e20 6973 206e 6f74 204e 6f6e  ction is not Non
-00038f80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00038f90: 6573 756c 745b 2764 6972 6563 7469 6f6e  esult['direction
-00038fa0: 275d 203d 2073 656c 662e 6469 7265 6374  '] = self.direct
-00038fb0: 696f 6e0a 2020 2020 2020 2020 6966 2073  ion.        if s
-00038fc0: 656c 662e 6c69 6d69 7420 6973 206e 6f74  elf.limit is not
-00038fd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00038fe0: 2020 2072 6573 756c 745b 276c 696d 6974     result['limit
-00038ff0: 275d 203d 2073 656c 662e 6c69 6d69 740a  '] = self.limit.
-00039000: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00039010: 6e65 7874 5f74 6f6b 656e 2069 7320 6e6f  next_token is no
-00039020: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00039030: 2020 2020 7265 7375 6c74 5b27 6e65 7874      result['next
-00039040: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e6e  Token'] = self.n
-00039050: 6578 745f 746f 6b65 6e0a 2020 2020 2020  ext_token.      
-00039060: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00039070: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00039080: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00039090: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000390a0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000390b0: 2069 6620 6d2e 6765 7428 2764 6972 6563   if m.get('direc
-000390c0: 7469 6f6e 2729 2069 7320 6e6f 7420 4e6f  tion') is not No
-000390d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000390e0: 7365 6c66 2e64 6972 6563 7469 6f6e 203d  self.direction =
-000390f0: 206d 2e67 6574 2827 6469 7265 6374 696f   m.get('directio
-00039100: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
-00039110: 2e67 6574 2827 6c69 6d69 7427 2920 6973  .get('limit') is
-00039120: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00039130: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
-00039140: 7420 3d20 6d2e 6765 7428 276c 696d 6974  t = m.get('limit
-00039150: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00039160: 6765 7428 276e 6578 7454 6f6b 656e 2729  get('nextToken')
-00039170: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00039180: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00039190: 6578 745f 746f 6b65 6e20 3d20 6d2e 6765  ext_token = m.ge
-000391a0: 7428 276e 6578 7454 6f6b 656e 2729 0a20  t('nextToken'). 
-000391b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000391c0: 6c66 0a0a 0a63 6c61 7373 204c 6973 7446  lf...class ListF
-000391d0: 756e 6374 696f 6e56 6572 7369 6f6e 7352  unctionVersionsR
-000391e0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-000391f0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00039200: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
-00039210: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
-00039220: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
-00039230: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00039240: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-00039250: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
-00039260: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
-00039270: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00039280: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-00039290: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
-000392a0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-000392b0: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
-000392c0: 653a 204c 6973 7456 6572 7369 6f6e 734f  e: ListVersionsO
-000392d0: 7574 7075 740a 0a20 2020 2064 6566 2076  utput..    def v
-000392e0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000392f0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00039300: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-00039310: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-00039320: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00039330: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00039340: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00039350: 7228 4c69 7374 4675 6e63 7469 6f6e 5665  r(ListFunctionVe
-00039360: 7273 696f 6e73 5265 7370 6f6e 7365 2c20  rsionsResponse, 
-00039370: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-00039380: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00039390: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000393a0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000393b0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-000393c0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-000393d0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-000393e0: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-000393f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00039400: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-00039410: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-00039420: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00039430: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-00039440: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00039450: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-00039460: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-00039470: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-00039480: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-00039490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000394a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000394b0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-000394c0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-000394d0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000394e0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-000394f0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-00039500: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00039510: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00039520: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-00039530: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-00039540: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00039550: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00039560: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00039570: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00039580: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-00039590: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000395a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000395b0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
-000395c0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-000395d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000395e0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-000395f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00039600: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-00039610: 4c69 7374 5665 7273 696f 6e73 4f75 7470  ListVersionsOutp
-00039620: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-00039630: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-00039640: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-00039650: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-00039660: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00039670: 0a0a 636c 6173 7320 4c69 7374 4675 6e63  ..class ListFunc
-00039680: 7469 6f6e 7352 6571 7565 7374 2854 6561  tionsRequest(Tea
-00039690: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-000396a0: 5f5f 696e 6974 5f5f 2873 656c 662c 206c  __init__(self, l
-000396b0: 696d 6974 3d4e 6f6e 652c 206e 6578 745f  imit=None, next_
-000396c0: 746f 6b65 6e3d 4e6f 6e65 2c20 7072 6566  token=None, pref
-000396d0: 6978 3d4e 6f6e 6529 3a0a 2020 2020 2020  ix=None):.      
-000396e0: 2020 2320 5468 6520 6e75 6d62 6572 206f    # The number o
-000396f0: 6620 6675 6e63 7469 6f6e 7320 746f 2072  f functions to r
-00039700: 6574 7572 6e2e 2054 6865 206d 696e 696d  eturn. The minim
-00039710: 756d 2076 616c 7565 2069 7320 3120 616e  um value is 1 an
-00039720: 6420 7468 6520 6d61 7869 6d75 6d20 7661  d the maximum va
-00039730: 6c75 6520 6973 2031 3030 2e0a 2020 2020  lue is 100..    
-00039740: 2020 2020 7365 6c66 2e6c 696d 6974 203d      self.limit =
-00039750: 206c 696d 6974 2020 2320 7479 7065 3a20   limit  # type: 
-00039760: 696e 740a 2020 2020 2020 2020 2320 5468  int.        # Th
-00039770: 6520 7061 6769 6e61 7469 6f6e 2074 6f6b  e pagination tok
-00039780: 656e 2e0a 2020 2020 2020 2020 7365 6c66  en..        self
-00039790: 2e6e 6578 745f 746f 6b65 6e20 3d20 6e65  .next_token = ne
-000397a0: 7874 5f74 6f6b 656e 2020 2320 7479 7065  xt_token  # type
-000397b0: 3a20 7374 720a 2020 2020 2020 2020 2320  : str.        # 
-000397c0: 5468 6520 7072 6566 6978 206f 6620 7468  The prefix of th
-000397d0: 6520 6675 6e63 7469 6f6e 206e 616d 652e  e function name.
-000397e0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-000397f0: 6566 6978 203d 2070 7265 6669 7820 2023  efix = prefix  #
-00039800: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
-00039810: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00039820: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00039830: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00039840: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00039850: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
-00039860: 7446 756e 6374 696f 6e73 5265 7175 6573  tFunctionsReques
-00039870: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
-00039880: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-00039890: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000398a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000398b0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-000398c0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000398d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000398e0: 6c69 6d69 7420 6973 206e 6f74 204e 6f6e  limit is not Non
-000398f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00039900: 6573 756c 745b 276c 696d 6974 275d 203d  esult['limit'] =
-00039910: 2073 656c 662e 6c69 6d69 740a 2020 2020   self.limit.    
-00039920: 2020 2020 6966 2073 656c 662e 6e65 7874      if self.next
-00039930: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
-00039940: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00039950: 7265 7375 6c74 5b27 6e65 7874 546f 6b65  result['nextToke
-00039960: 6e27 5d20 3d20 7365 6c66 2e6e 6578 745f  n'] = self.next_
-00039970: 746f 6b65 6e0a 2020 2020 2020 2020 6966  token.        if
-00039980: 2073 656c 662e 7072 6566 6978 2069 7320   self.prefix is 
-00039990: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000399a0: 2020 2020 2020 7265 7375 6c74 5b27 7072        result['pr
-000399b0: 6566 6978 275d 203d 2073 656c 662e 7072  efix'] = self.pr
-000399c0: 6566 6978 0a20 2020 2020 2020 2072 6574  efix.        ret
-000399d0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000399e0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000399f0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-00039a00: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00039a10: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00039a20: 2e67 6574 2827 6c69 6d69 7427 2920 6973  .get('limit') is
-00039a30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00039a40: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
-00039a50: 7420 3d20 6d2e 6765 7428 276c 696d 6974  t = m.get('limit
-00039a60: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00039a70: 6765 7428 276e 6578 7454 6f6b 656e 2729  get('nextToken')
-00039a80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00039a90: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00039aa0: 6578 745f 746f 6b65 6e20 3d20 6d2e 6765  ext_token = m.ge
-00039ab0: 7428 276e 6578 7454 6f6b 656e 2729 0a20  t('nextToken'). 
-00039ac0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00039ad0: 2770 7265 6669 7827 2920 6973 206e 6f74  'prefix') is not
-00039ae0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00039af0: 2020 2073 656c 662e 7072 6566 6978 203d     self.prefix =
-00039b00: 206d 2e67 6574 2827 7072 6566 6978 2729   m.get('prefix')
-00039b10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00039b20: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-00039b30: 7446 756e 6374 696f 6e73 5265 7370 6f6e  tFunctionsRespon
-00039b40: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-00039b50: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00039b60: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
-00039b70: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
-00039b80: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
-00039b90: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-00039ba0: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
-00039bb0: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
-00039bc0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
-00039bd0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00039be0: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
-00039bf0: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
-00039c00: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00039c10: 626f 6479 2020 2320 7479 7065 3a20 4c69  body  # type: Li
-00039c20: 7374 4675 6e63 7469 6f6e 734f 7574 7075  stFunctionsOutpu
-00039c30: 740a 0a20 2020 2064 6566 2076 616c 6964  t..    def valid
-00039c40: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00039c50: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-00039c60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00039c70: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-00039c80: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-00039c90: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00039ca0: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
-00039cb0: 7374 4675 6e63 7469 6f6e 7352 6573 706f  stFunctionsRespo
-00039cc0: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
-00039cd0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00039ce0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00039cf0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00039d00: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00039d10: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00039d20: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00039d30: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00039d40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00039d50: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00039d60: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00039d70: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00039d80: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00039d90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00039da0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00039db0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-00039dc0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00039dd0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00039de0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00039df0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00039e00: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00039e10: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00039e20: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00039e30: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00039e40: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00039e50: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-00039e60: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00039e70: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00039e80: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-00039e90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00039ea0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00039eb0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00039ec0: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00039ed0: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00039ee0: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00039ef0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00039f00: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00039f10: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-00039f20: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-00039f30: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-00039f40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00039f50: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-00039f60: 656c 203d 204c 6973 7446 756e 6374 696f  el = ListFunctio
-00039f70: 6e73 4f75 7470 7574 2829 0a20 2020 2020  nsOutput().     
-00039f80: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00039f90: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-00039fa0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-00039fb0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00039fc0: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
-00039fd0: 7374 496e 7374 616e 6365 7352 6571 7565  stInstancesReque
-00039fe0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-00039ff0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0003a000: 656c 662c 2071 7561 6c69 6669 6572 3d4e  elf, qualifier=N
-0003a010: 6f6e 652c 2077 6974 685f 616c 6c5f 6163  one, with_all_ac
-0003a020: 7469 7665 3d4e 6f6e 6529 3a0a 2020 2020  tive=None):.    
-0003a030: 2020 2020 2320 5468 6520 6675 6e63 7469      # The functi
-0003a040: 6f6e 2076 6572 7369 6f6e 206f 7220 616c  on version or al
-0003a050: 6961 732e 0a20 2020 2020 2020 2073 656c  ias..        sel
-0003a060: 662e 7175 616c 6966 6965 7220 3d20 7175  f.qualifier = qu
-0003a070: 616c 6966 6965 7220 2023 2074 7970 653a  alifier  # type:
-0003a080: 2073 7472 0a20 2020 2020 2020 2023 2053   str.        # S
-0003a090: 7065 6369 6669 6573 2077 6865 7468 6572  pecifies whether
-0003a0a0: 2074 6f20 6c69 7374 2061 6c6c 2069 6e73   to list all ins
-0003a0b0: 7461 6e63 6573 2e20 5661 6c69 6420 7661  tances. Valid va
-0003a0c0: 6c75 6573 3a20 7472 7565 2061 6e64 2066  lues: true and f
-0003a0d0: 616c 7365 2e0a 2020 2020 2020 2020 7365  alse..        se
-0003a0e0: 6c66 2e77 6974 685f 616c 6c5f 6163 7469  lf.with_all_acti
-0003a0f0: 7665 203d 2077 6974 685f 616c 6c5f 6163  ve = with_all_ac
-0003a100: 7469 7665 2020 2320 7479 7065 3a20 626f  tive  # type: bo
-0003a110: 6f6c 0a0a 2020 2020 6465 6620 7661 6c69  ol..    def vali
-0003a120: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0003a130: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-0003a140: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0003a150: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0003a160: 7570 6572 284c 6973 7449 6e73 7461 6e63  uper(ListInstanc
-0003a170: 6573 5265 7175 6573 742c 2073 656c 6629  esRequest, self)
-0003a180: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0003a190: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0003a1a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003a1b0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0003a1c0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0003a1d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0003a1e0: 6966 2073 656c 662e 7175 616c 6966 6965  if self.qualifie
-0003a1f0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-0003a200: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003a210: 745b 2771 7561 6c69 6669 6572 275d 203d  t['qualifier'] =
-0003a220: 2073 656c 662e 7175 616c 6966 6965 720a   self.qualifier.
-0003a230: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003a240: 7769 7468 5f61 6c6c 5f61 6374 6976 6520  with_all_active 
-0003a250: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003a260: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003a270: 2777 6974 6841 6c6c 4163 7469 7665 275d  'withAllActive']
-0003a280: 203d 2073 656c 662e 7769 7468 5f61 6c6c   = self.with_all
-0003a290: 5f61 6374 6976 650a 2020 2020 2020 2020  _active.        
-0003a2a0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0003a2b0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0003a2c0: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-0003a2d0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-0003a2e0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0003a2f0: 6620 6d2e 6765 7428 2771 7561 6c69 6669  f m.get('qualifi
-0003a300: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
-0003a310: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0003a320: 6c66 2e71 7561 6c69 6669 6572 203d 206d  lf.qualifier = m
-0003a330: 2e67 6574 2827 7175 616c 6966 6965 7227  .get('qualifier'
-0003a340: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003a350: 6574 2827 7769 7468 416c 6c41 6374 6976  et('withAllActiv
-0003a360: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0003a370: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003a380: 662e 7769 7468 5f61 6c6c 5f61 6374 6976  f.with_all_activ
-0003a390: 6520 3d20 6d2e 6765 7428 2777 6974 6841  e = m.get('withA
-0003a3a0: 6c6c 4163 7469 7665 2729 0a20 2020 2020  llActive').     
-0003a3b0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0003a3c0: 0a63 6c61 7373 204c 6973 7449 6e73 7461  .class ListInsta
-0003a3d0: 6e63 6573 5265 7370 6f6e 7365 2854 6561  ncesResponse(Tea
-0003a3e0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0003a3f0: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
-0003a400: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
-0003a410: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
-0003a420: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
-0003a430: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0003a440: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
-0003a450: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
-0003a460: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
-0003a470: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-0003a480: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
-0003a490: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
-0003a4a0: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
-0003a4b0: 2320 7479 7065 3a20 4c69 7374 496e 7374  # type: ListInst
-0003a4c0: 616e 6365 734f 7574 7075 740a 0a20 2020  ancesOutput..   
-0003a4d0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0003a4e0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-0003a4f0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-0003a500: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0003a510: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-0003a520: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-0003a530: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-0003a540: 3d20 7375 7065 7228 4c69 7374 496e 7374  = super(ListInst
-0003a550: 616e 6365 7352 6573 706f 6e73 652c 2073  ancesResponse, s
-0003a560: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-0003a570: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003a580: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003a590: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003a5a0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003a5b0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003a5c0: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-0003a5d0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-0003a5e0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003a5f0: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-0003a600: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-0003a610: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0003a620: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-0003a630: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003a640: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-0003a650: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-0003a660: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0003a670: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0003a680: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003a690: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003a6a0: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0003a6b0: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0003a6c0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0003a6d0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0003a6e0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-0003a6f0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0003a700: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0003a710: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-0003a720: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-0003a730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003a740: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0003a750: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0003a760: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003a770: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-0003a780: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003a790: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-0003a7a0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-0003a7b0: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-0003a7c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003a7d0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-0003a7e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003a7f0: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
-0003a800: 6973 7449 6e73 7461 6e63 6573 4f75 7470  istInstancesOutp
-0003a810: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-0003a820: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-0003a830: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-0003a840: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-0003a850: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0003a860: 0a0a 636c 6173 7320 4c69 7374 4c61 7965  ..class ListLaye
-0003a870: 7256 6572 7369 6f6e 7352 6571 7565 7374  rVersionsRequest
-0003a880: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0003a890: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0003a8a0: 662c 206c 696d 6974 3d4e 6f6e 652c 2073  f, limit=None, s
-0003a8b0: 7461 7274 5f76 6572 7369 6f6e 3d4e 6f6e  tart_version=Non
-0003a8c0: 6529 3a0a 2020 2020 2020 2020 2320 5468  e):.        # Th
-0003a8d0: 6520 6e75 6d62 6572 206f 6620 7665 7273  e number of vers
-0003a8e0: 696f 6e73 2074 6f20 6265 2072 6574 7572  ions to be retur
-0003a8f0: 6e65 642e 0a20 2020 2020 2020 2073 656c  ned..        sel
-0003a900: 662e 6c69 6d69 7420 3d20 6c69 6d69 7420  f.limit = limit 
-0003a910: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
-0003a920: 2020 2020 2023 2054 6865 2069 6e69 7469       # The initi
-0003a930: 616c 2076 6572 7369 6f6e 206f 6620 7468  al version of th
-0003a940: 6520 6c61 7965 722e 0a20 2020 2020 2020  e layer..       
-0003a950: 2073 656c 662e 7374 6172 745f 7665 7273   self.start_vers
-0003a960: 696f 6e20 3d20 7374 6172 745f 7665 7273  ion = start_vers
-0003a970: 696f 6e20 2023 2074 7970 653a 2073 7472  ion  # type: str
-0003a980: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0003a990: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0003a9a0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0003a9b0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0003a9c0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0003a9d0: 6572 284c 6973 744c 6179 6572 5665 7273  er(ListLayerVers
-0003a9e0: 696f 6e73 5265 7175 6573 742c 2073 656c  ionsRequest, sel
-0003a9f0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-0003aa00: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0003aa10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003aa20: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0003aa30: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0003aa40: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0003aa50: 2020 6966 2073 656c 662e 6c69 6d69 7420    if self.limit 
-0003aa60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003aa70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003aa80: 276c 696d 6974 275d 203d 2073 656c 662e  'limit'] = self.
-0003aa90: 6c69 6d69 740a 2020 2020 2020 2020 6966  limit.        if
-0003aaa0: 2073 656c 662e 7374 6172 745f 7665 7273   self.start_vers
-0003aab0: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-0003aac0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003aad0: 756c 745b 2773 7461 7274 5665 7273 696f  ult['startVersio
-0003aae0: 6e27 5d20 3d20 7365 6c66 2e73 7461 7274  n'] = self.start
-0003aaf0: 5f76 6572 7369 6f6e 0a20 2020 2020 2020  _version.       
-0003ab00: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0003ab10: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0003ab20: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0003ab30: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0003ab40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0003ab50: 6966 206d 2e67 6574 2827 6c69 6d69 7427  if m.get('limit'
-0003ab60: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003ab70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003ab80: 6c69 6d69 7420 3d20 6d2e 6765 7428 276c  limit = m.get('l
-0003ab90: 696d 6974 2729 0a20 2020 2020 2020 2069  imit').        i
-0003aba0: 6620 6d2e 6765 7428 2773 7461 7274 5665  f m.get('startVe
-0003abb0: 7273 696f 6e27 2920 6973 206e 6f74 204e  rsion') is not N
-0003abc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003abd0: 2073 656c 662e 7374 6172 745f 7665 7273   self.start_vers
-0003abe0: 696f 6e20 3d20 6d2e 6765 7428 2773 7461  ion = m.get('sta
-0003abf0: 7274 5665 7273 696f 6e27 290a 2020 2020  rtVersion').    
-0003ac00: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0003ac10: 0a0a 636c 6173 7320 4c69 7374 4c61 7965  ..class ListLaye
-0003ac20: 7256 6572 7369 6f6e 7352 6573 706f 6e73  rVersionsRespons
-0003ac30: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-0003ac40: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0003ac50: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
-0003ac60: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
-0003ac70: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
-0003ac80: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0003ac90: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
-0003aca0: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
-0003acb0: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
-0003acc0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0003acd0: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
-0003ace0: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
-0003acf0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-0003ad00: 6f64 7920 2023 2074 7970 653a 204c 6973  ody  # type: Lis
-0003ad10: 744c 6179 6572 5665 7273 696f 6e4f 7574  tLayerVersionOut
-0003ad20: 7075 740a 0a20 2020 2064 6566 2076 616c  put..    def val
-0003ad30: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0003ad40: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0003ad50: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0003ad60: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-0003ad70: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0003ad80: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0003ad90: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0003ada0: 4c69 7374 4c61 7965 7256 6572 7369 6f6e  ListLayerVersion
-0003adb0: 7352 6573 706f 6e73 652c 2073 656c 6629  sResponse, self)
-0003adc0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0003add0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0003ade0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003adf0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0003ae00: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0003ae10: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0003ae20: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0003ae30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003ae40: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003ae50: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0003ae60: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0003ae70: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0003ae80: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0003ae90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003aea0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0003aeb0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0003aec0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0003aed0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0003aee0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003aef0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0003af00: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0003af10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0003af20: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0003af30: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0003af40: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0003af50: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0003af60: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0003af70: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-0003af80: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-0003af90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003afa0: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-0003afb0: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-0003afc0: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-0003afd0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-0003afe0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003aff0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0003b000: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-0003b010: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-0003b020: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-0003b030: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-0003b040: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-0003b050: 6d70 5f6d 6f64 656c 203d 204c 6973 744c  mp_model = ListL
-0003b060: 6179 6572 5665 7273 696f 6e4f 7574 7075  ayerVersionOutpu
-0003b070: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0003b080: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-0003b090: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-0003b0a0: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-0003b0b0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0003b0c0: 0a63 6c61 7373 204c 6973 744c 6179 6572  .class ListLayer
-0003b0d0: 7352 6571 7565 7374 2854 6561 4d6f 6465  sRequest(TeaMode
-0003b0e0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0003b0f0: 6974 5f5f 2873 656c 662c 206c 696d 6974  it__(self, limit
-0003b100: 3d4e 6f6e 652c 206e 6578 745f 746f 6b65  =None, next_toke
-0003b110: 6e3d 4e6f 6e65 2c20 6f66 6669 6369 616c  n=None, official
-0003b120: 3d4e 6f6e 652c 2070 7265 6669 783d 4e6f  =None, prefix=No
-0003b130: 6e65 2c20 7075 626c 6963 3d4e 6f6e 6529  ne, public=None)
-0003b140: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
-0003b150: 6e75 6d62 6572 206f 6620 6c61 7965 7273  number of layers
-0003b160: 2074 6861 7420 6172 6520 7265 7475 726e   that are return
-0003b170: 6564 0a20 2020 2020 2020 2073 656c 662e  ed.        self.
-0003b180: 6c69 6d69 7420 3d20 6c69 6d69 7420 2023  limit = limit  #
-0003b190: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
-0003b1a0: 2020 2023 2054 6865 2070 6167 696e 6174     # The paginat
-0003b1b0: 696f 6e20 746f 6b65 6e20 7468 6174 2069  ion token that i
-0003b1c0: 7320 7573 6564 2069 6e20 7468 6520 6e65  s used in the ne
-0003b1d0: 7874 2072 6571 7565 7374 2074 6f20 7265  xt request to re
-0003b1e0: 7472 6965 7665 2061 206e 6577 2070 6167  trieve a new pag
-0003b1f0: 6520 6f66 2072 6573 756c 7473 2e0a 2020  e of results..  
-0003b200: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
-0003b210: 746f 6b65 6e20 3d20 6e65 7874 5f74 6f6b  token = next_tok
-0003b220: 656e 2020 2320 7479 7065 3a20 7374 720a  en  # type: str.
-0003b230: 2020 2020 2020 2020 2320 5370 6563 6966          # Specif
-0003b240: 6965 7320 7768 6574 6865 7220 7468 6520  ies whether the 
-0003b250: 6c61 7965 7220 6973 206f 6666 6963 6961  layer is officia
-0003b260: 6c2e 2056 616c 6964 2076 616c 7565 733a  l. Valid values:
-0003b270: 2074 7275 6520 616e 6420 6661 6c73 652e   true and false.
-0003b280: 0a20 2020 2020 2020 2073 656c 662e 6f66  .        self.of
-0003b290: 6669 6369 616c 203d 206f 6666 6963 6961  ficial = officia
-0003b2a0: 6c20 2023 2074 7970 653a 2073 7472 0a20  l  # type: str. 
-0003b2b0: 2020 2020 2020 2023 2054 6865 206e 616d         # The nam
-0003b2c0: 6520 7072 6566 6978 206f 6620 7468 6520  e prefix of the 
-0003b2d0: 6c61 7965 722e 0a20 2020 2020 2020 2073  layer..        s
-0003b2e0: 656c 662e 7072 6566 6978 203d 2070 7265  elf.prefix = pre
-0003b2f0: 6669 7820 2023 2074 7970 653a 2073 7472  fix  # type: str
-0003b300: 0a20 2020 2020 2020 2023 2053 7065 6369  .        # Speci
-0003b310: 6669 6573 2077 6865 7468 6572 2074 6865  fies whether the
-0003b320: 206c 6179 6572 2069 7320 7075 626c 6963   layer is public
-0003b330: 2e20 5661 6c69 6420 7661 6c75 6573 3a20  . Valid values: 
-0003b340: 7472 7565 2061 6e64 2066 616c 7365 2e0a  true and false..
-0003b350: 2020 2020 2020 2020 7365 6c66 2e70 7562          self.pub
-0003b360: 6c69 6320 3d20 7075 626c 6963 2020 2320  lic = public  # 
-0003b370: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-0003b380: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0003b390: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0003b3a0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0003b3b0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0003b3c0: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
-0003b3d0: 4c61 7965 7273 5265 7175 6573 742c 2073  LayersRequest, s
-0003b3e0: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-0003b3f0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003b400: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003b410: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003b420: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003b430: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003b440: 2020 2020 6966 2073 656c 662e 6c69 6d69      if self.limi
-0003b450: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-0003b460: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003b470: 745b 276c 696d 6974 275d 203d 2073 656c  t['limit'] = sel
-0003b480: 662e 6c69 6d69 740a 2020 2020 2020 2020  f.limit.        
-0003b490: 6966 2073 656c 662e 6e65 7874 5f74 6f6b  if self.next_tok
-0003b4a0: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
-0003b4b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0003b4c0: 6c74 5b27 6e65 7874 546f 6b65 6e27 5d20  lt['nextToken'] 
-0003b4d0: 3d20 7365 6c66 2e6e 6578 745f 746f 6b65  = self.next_toke
-0003b4e0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0003b4f0: 662e 6f66 6669 6369 616c 2069 7320 6e6f  f.official is no
-0003b500: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003b510: 2020 2020 7265 7375 6c74 5b27 6f66 6669      result['offi
-0003b520: 6369 616c 275d 203d 2073 656c 662e 6f66  cial'] = self.of
-0003b530: 6669 6369 616c 0a20 2020 2020 2020 2069  ficial.        i
-0003b540: 6620 7365 6c66 2e70 7265 6669 7820 6973  f self.prefix is
-0003b550: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003b560: 2020 2020 2020 2072 6573 756c 745b 2770         result['p
-0003b570: 7265 6669 7827 5d20 3d20 7365 6c66 2e70  refix'] = self.p
-0003b580: 7265 6669 780a 2020 2020 2020 2020 6966  refix.        if
-0003b590: 2073 656c 662e 7075 626c 6963 2069 7320   self.public is 
-0003b5a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003b5b0: 2020 2020 2020 7265 7375 6c74 5b27 7075        result['pu
-0003b5c0: 626c 6963 275d 203d 2073 656c 662e 7075  blic'] = self.pu
-0003b5d0: 626c 6963 0a20 2020 2020 2020 2072 6574  blic.        ret
-0003b5e0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0003b5f0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0003b600: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0003b610: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0003b620: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0003b630: 2e67 6574 2827 6c69 6d69 7427 2920 6973  .get('limit') is
-0003b640: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003b650: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
-0003b660: 7420 3d20 6d2e 6765 7428 276c 696d 6974  t = m.get('limit
-0003b670: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0003b680: 6765 7428 276e 6578 7454 6f6b 656e 2729  get('nextToken')
-0003b690: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003b6a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0003b6b0: 6578 745f 746f 6b65 6e20 3d20 6d2e 6765  ext_token = m.ge
-0003b6c0: 7428 276e 6578 7454 6f6b 656e 2729 0a20  t('nextToken'). 
-0003b6d0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003b6e0: 276f 6666 6963 6961 6c27 2920 6973 206e  'official') is n
-0003b6f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003b700: 2020 2020 2073 656c 662e 6f66 6669 6369       self.offici
-0003b710: 616c 203d 206d 2e67 6574 2827 6f66 6669  al = m.get('offi
-0003b720: 6369 616c 2729 0a20 2020 2020 2020 2069  cial').        i
-0003b730: 6620 6d2e 6765 7428 2770 7265 6669 7827  f m.get('prefix'
-0003b740: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003b750: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003b760: 7072 6566 6978 203d 206d 2e67 6574 2827  prefix = m.get('
-0003b770: 7072 6566 6978 2729 0a20 2020 2020 2020  prefix').       
-0003b780: 2069 6620 6d2e 6765 7428 2770 7562 6c69   if m.get('publi
-0003b790: 6327 2920 6973 206e 6f74 204e 6f6e 653a  c') is not None:
-0003b7a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003b7b0: 662e 7075 626c 6963 203d 206d 2e67 6574  f.public = m.get
-0003b7c0: 2827 7075 626c 6963 2729 0a20 2020 2020  ('public').     
-0003b7d0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0003b7e0: 0a63 6c61 7373 204c 6973 744c 6179 6572  .class ListLayer
-0003b7f0: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
-0003b800: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0003b810: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
-0003b820: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
-0003b830: 5f63 6f64 653d 4e6f 6e65 2c20 626f 6479  _code=None, body
-0003b840: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0003b850: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
-0003b860: 6561 6465 7273 2020 2320 7479 7065 3a20  eaders  # type: 
-0003b870: 6469 6374 5b73 7472 2c20 7374 725d 0a20  dict[str, str]. 
-0003b880: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0003b890: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-0003b8a0: 5f63 6f64 6520 2023 2074 7970 653a 2069  _code  # type: i
-0003b8b0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
-0003b8c0: 626f 6479 203d 2062 6f64 7920 2023 2074  body = body  # t
-0003b8d0: 7970 653a 204c 6973 744c 6179 6572 734f  ype: ListLayersO
-0003b8e0: 7574 7075 740a 0a20 2020 2064 6566 2076  utput..    def v
-0003b8f0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0003b900: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0003b910: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-0003b920: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-0003b930: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-0003b940: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0003b950: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0003b960: 7228 4c69 7374 4c61 7965 7273 5265 7370  r(ListLayersResp
-0003b970: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
-0003b980: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0003b990: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0003b9a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003b9b0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0003b9c0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0003b9d0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0003b9e0: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-0003b9f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003ba00: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-0003ba10: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-0003ba20: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-0003ba30: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003ba40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003ba50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003ba60: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-0003ba70: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003ba80: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0003ba90: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-0003baa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003bab0: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-0003bac0: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-0003bad0: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0003bae0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0003baf0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0003bb00: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-0003bb10: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0003bb20: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0003bb30: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-0003bb40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003bb50: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0003bb60: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-0003bb70: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-0003bb80: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-0003bb90: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-0003bba0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003bbb0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003bbc0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-0003bbd0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-0003bbe0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-0003bbf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003bc00: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-0003bc10: 6465 6c20 3d20 4c69 7374 4c61 7965 7273  del = ListLayers
-0003bc20: 4f75 7470 7574 2829 0a20 2020 2020 2020  Output().       
-0003bc30: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0003bc40: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-0003bc50: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-0003bc60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0003bc70: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
-0003bc80: 5072 6f76 6973 696f 6e43 6f6e 6669 6773  ProvisionConfigs
-0003bc90: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-0003bca0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0003bcb0: 745f 5f28 7365 6c66 2c20 6675 6e63 7469  t__(self, functi
-0003bcc0: 6f6e 5f6e 616d 653d 4e6f 6e65 2c20 6c69  on_name=None, li
-0003bcd0: 6d69 743d 4e6f 6e65 2c20 6e65 7874 5f74  mit=None, next_t
-0003bce0: 6f6b 656e 3d4e 6f6e 6529 3a0a 2020 2020  oken=None):.    
-0003bcf0: 2020 2020 2320 5468 6520 6e61 6d65 206f      # The name o
-0003bd00: 6620 7468 6520 6675 6e63 7469 6f6e 2e20  f the function. 
-0003bd10: 4966 2074 6869 7320 7061 7261 6d65 7465  If this paramete
-0003bd20: 7220 6973 206e 6f74 2073 7065 6369 6669  r is not specifi
-0003bd30: 6564 2c20 7468 6520 7072 6f76 6973 696f  ed, the provisio
-0003bd40: 6e65 6420 636f 6e66 6967 7572 6174 696f  ned configuratio
-0003bd50: 6e73 206f 6620 616c 6c20 6675 6e63 7469  ns of all functi
-0003bd60: 6f6e 7320 6172 6520 6c69 7374 6564 2e0a  ons are listed..
-0003bd70: 2020 2020 2020 2020 7365 6c66 2e66 756e          self.fun
-0003bd80: 6374 696f 6e5f 6e61 6d65 203d 2066 756e  ction_name = fun
-0003bd90: 6374 696f 6e5f 6e61 6d65 2020 2320 7479  ction_name  # ty
-0003bda0: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-0003bdb0: 2320 4e75 6d62 6572 206f 6620 7072 6f76  # Number of prov
-0003bdc0: 6973 696f 6e65 6420 636f 6e66 6967 7572  isioned configur
-0003bdd0: 6174 696f 6e73 2074 6f20 7265 7475 726e  ations to return
-0003bde0: 2e0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-0003bdf0: 696d 6974 203d 206c 696d 6974 2020 2320  imit = limit  # 
-0003be00: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
-0003be10: 2020 2320 4120 7061 6769 6e61 7469 6f6e    # A pagination
-0003be20: 2074 6f6b 656e 2e0a 2020 2020 2020 2020   token..        
-0003be30: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
-0003be40: 3d20 6e65 7874 5f74 6f6b 656e 2020 2320  = next_token  # 
-0003be50: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-0003be60: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0003be70: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0003be80: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0003be90: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0003bea0: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
-0003beb0: 5072 6f76 6973 696f 6e43 6f6e 6669 6773  ProvisionConfigs
-0003bec0: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
-0003bed0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0003bee0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0003bef0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003bf00: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0003bf10: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0003bf20: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0003bf30: 2073 656c 662e 6675 6e63 7469 6f6e 5f6e   self.function_n
-0003bf40: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-0003bf50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003bf60: 756c 745b 2766 756e 6374 696f 6e4e 616d  ult['functionNam
-0003bf70: 6527 5d20 3d20 7365 6c66 2e66 756e 6374  e'] = self.funct
-0003bf80: 696f 6e5f 6e61 6d65 0a20 2020 2020 2020  ion_name.       
-0003bf90: 2069 6620 7365 6c66 2e6c 696d 6974 2069   if self.limit i
-0003bfa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003bfb0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003bfc0: 6c69 6d69 7427 5d20 3d20 7365 6c66 2e6c  limit'] = self.l
-0003bfd0: 696d 6974 0a20 2020 2020 2020 2069 6620  imit.        if 
-0003bfe0: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
-0003bff0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003c000: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003c010: 276e 6578 7454 6f6b 656e 275d 203d 2073  'nextToken'] = s
-0003c020: 656c 662e 6e65 7874 5f74 6f6b 656e 0a20  elf.next_token. 
-0003c030: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0003c040: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0003c050: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-0003c060: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0003c070: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0003c080: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0003c090: 6675 6e63 7469 6f6e 4e61 6d65 2729 2069  functionName') i
-0003c0a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003c0b0: 2020 2020 2020 2020 7365 6c66 2e66 756e          self.fun
-0003c0c0: 6374 696f 6e5f 6e61 6d65 203d 206d 2e67  ction_name = m.g
-0003c0d0: 6574 2827 6675 6e63 7469 6f6e 4e61 6d65  et('functionName
-0003c0e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0003c0f0: 6765 7428 276c 696d 6974 2729 2069 7320  get('limit') is 
-0003c100: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003c110: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
-0003c120: 203d 206d 2e67 6574 2827 6c69 6d69 7427   = m.get('limit'
-0003c130: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003c140: 6574 2827 6e65 7874 546f 6b65 6e27 2920  et('nextToken') 
-0003c150: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003c160: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-0003c170: 7874 5f74 6f6b 656e 203d 206d 2e67 6574  xt_token = m.get
-0003c180: 2827 6e65 7874 546f 6b65 6e27 290a 2020  ('nextToken').  
-0003c190: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0003c1a0: 660a 0a0a 636c 6173 7320 4c69 7374 5072  f...class ListPr
-0003c1b0: 6f76 6973 696f 6e43 6f6e 6669 6773 5265  ovisionConfigsRe
-0003c1c0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-0003c1d0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003c1e0: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
-0003c1f0: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
-0003c200: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
-0003c210: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
-0003c220: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-0003c230: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
-0003c240: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
-0003c250: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-0003c260: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-0003c270: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
-0003c280: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0003c290: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
-0003c2a0: 3a20 4c69 7374 5072 6f76 6973 696f 6e43  : ListProvisionC
-0003c2b0: 6f6e 6669 6773 4f75 7470 7574 0a0a 2020  onfigsOutput..  
-0003c2c0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0003c2d0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-0003c2e0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-0003c2f0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0003c300: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-0003c310: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0003c320: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0003c330: 203d 2073 7570 6572 284c 6973 7450 726f   = super(ListPro
-0003c340: 7669 7369 6f6e 436f 6e66 6967 7352 6573  visionConfigsRes
-0003c350: 706f 6e73 652c 2073 656c 6629 2e74 6f5f  ponse, self).to_
-0003c360: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-0003c370: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-0003c380: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003c390: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-0003c3a0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-0003c3b0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-0003c3c0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-0003c3d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003c3e0: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-0003c3f0: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-0003c400: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-0003c410: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003c420: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0003c430: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003c440: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-0003c450: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-0003c460: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-0003c470: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-0003c480: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003c490: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-0003c4a0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-0003c4b0: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-0003c4c0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0003c4d0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0003c4e0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0003c4f0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0003c500: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0003c510: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-0003c520: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003c530: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-0003c540: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-0003c550: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-0003c560: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-0003c570: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-0003c580: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003c590: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003c5a0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-0003c5b0: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-0003c5c0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-0003c5d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003c5e0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-0003c5f0: 6f64 656c 203d 204c 6973 7450 726f 7669  odel = ListProvi
-0003c600: 7369 6f6e 436f 6e66 6967 734f 7574 7075  sionConfigsOutpu
-0003c610: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0003c620: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-0003c630: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-0003c640: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-0003c650: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0003c660: 0a63 6c61 7373 204c 6973 7454 6167 5265  .class ListTagRe
-0003c670: 736f 7572 6365 7352 6571 7565 7374 5461  sourcesRequestTa
-0003c680: 6728 5465 614d 6f64 656c 293a 0a20 2020  g(TeaModel):.   
-0003c690: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0003c6a0: 6c66 2c20 6b65 793d 4e6f 6e65 2c20 7661  lf, key=None, va
-0003c6b0: 6c75 653d 4e6f 6e65 293a 0a20 2020 2020  lue=None):.     
-0003c6c0: 2020 2023 20e6 a087 e7ad bee5 908d 0a20     # .......... 
-0003c6d0: 2020 2020 2020 2073 656c 662e 6b65 7920         self.key 
-0003c6e0: 3d20 6b65 7920 2023 2074 7970 653a 2073  = key  # type: s
-0003c6f0: 7472 0a20 2020 2020 2020 2023 20e6 a087  tr.        # ...
-0003c700: e7ad bee5 80bc 0a20 2020 2020 2020 2073  .......        s
-0003c710: 656c 662e 7661 6c75 6520 3d20 7661 6c75  elf.value = valu
-0003c720: 6520 2023 2074 7970 653a 2073 7472 0a0a  e  # type: str..
-0003c730: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0003c740: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0003c750: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-0003c760: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0003c770: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0003c780: 284c 6973 7454 6167 5265 736f 7572 6365  (ListTagResource
-0003c790: 7352 6571 7565 7374 5461 672c 2073 656c  sRequestTag, sel
-0003c7a0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-0003c7b0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0003c7c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003c7d0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0003c7e0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0003c7f0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0003c800: 2020 6966 2073 656c 662e 6b65 7920 6973    if self.key is
-0003c810: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003c820: 2020 2020 2020 2072 6573 756c 745b 274b         result['K
-0003c830: 6579 275d 203d 2073 656c 662e 6b65 790a  ey'] = self.key.
-0003c840: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003c850: 7661 6c75 6520 6973 206e 6f74 204e 6f6e  value is not Non
-0003c860: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003c870: 6573 756c 745b 2756 616c 7565 275d 203d  esult['Value'] =
-0003c880: 2073 656c 662e 7661 6c75 650a 2020 2020   self.value.    
-0003c890: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0003c8a0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0003c8b0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-0003c8c0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0003c8d0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0003c8e0: 2020 2069 6620 6d2e 6765 7428 274b 6579     if m.get('Key
-0003c8f0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0003c900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003c910: 2e6b 6579 203d 206d 2e67 6574 2827 4b65  .key = m.get('Ke
-0003c920: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
-0003c930: 2e67 6574 2827 5661 6c75 6527 2920 6973  .get('Value') is
-0003c940: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003c950: 2020 2020 2020 2073 656c 662e 7661 6c75         self.valu
-0003c960: 6520 3d20 6d2e 6765 7428 2756 616c 7565  e = m.get('Value
-0003c970: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0003c980: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
-0003c990: 6973 7454 6167 5265 736f 7572 6365 7352  istTagResourcesR
-0003c9a0: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-0003c9b0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003c9c0: 5f5f 2873 656c 662c 206c 696d 6974 3d4e  __(self, limit=N
-0003c9d0: 6f6e 652c 206e 6578 745f 746f 6b65 6e3d  one, next_token=
-0003c9e0: 4e6f 6e65 2c20 7265 736f 7572 6365 5f69  None, resource_i
-0003c9f0: 643d 4e6f 6e65 2c20 7265 736f 7572 6365  d=None, resource
-0003ca00: 5f74 7970 653d 4e6f 6e65 2c20 7461 673d  _type=None, tag=
-0003ca10: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0003ca20: 656c 662e 6c69 6d69 7420 3d20 6c69 6d69  elf.limit = limi
-0003ca30: 7420 2023 2074 7970 653a 2069 6e74 0a20  t  # type: int. 
-0003ca40: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
-0003ca50: 5f74 6f6b 656e 203d 206e 6578 745f 746f  _token = next_to
-0003ca60: 6b65 6e20 2023 2074 7970 653a 2073 7472  ken  # type: str
-0003ca70: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0003ca80: 736f 7572 6365 5f69 6420 3d20 7265 736f  source_id = reso
-0003ca90: 7572 6365 5f69 6420 2023 2074 7970 653a  urce_id  # type:
-0003caa0: 206c 6973 745b 7374 725d 0a20 2020 2020   list[str].     
-0003cab0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
-0003cac0: 5f74 7970 6520 3d20 7265 736f 7572 6365  _type = resource
-0003cad0: 5f74 7970 6520 2023 2074 7970 653a 2073  _type  # type: s
-0003cae0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-0003caf0: 7461 6720 3d20 7461 6720 2023 2074 7970  tag = tag  # typ
-0003cb00: 653a 206c 6973 745b 4c69 7374 5461 6752  e: list[ListTagR
-0003cb10: 6573 6f75 7263 6573 5265 7175 6573 7454  esourcesRequestT
-0003cb20: 6167 5d0a 0a20 2020 2064 6566 2076 616c  ag]..    def val
-0003cb30: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0003cb40: 2020 2020 2069 6620 7365 6c66 2e74 6167       if self.tag
-0003cb50: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0003cb60: 7220 6b20 696e 2073 656c 662e 7461 673a  r k in self.tag:
-0003cb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003cb80: 2069 6620 6b3a 0a20 2020 2020 2020 2020   if k:.         
-0003cb90: 2020 2020 2020 2020 2020 206b 2e76 616c             k.val
-0003cba0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-0003cbb0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0003cbc0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0003cbd0: 7065 7228 4c69 7374 5461 6752 6573 6f75  per(ListTagResou
-0003cbe0: 7263 6573 5265 7175 6573 742c 2073 656c  rcesRequest, sel
-0003cbf0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-0003cc00: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0003cc10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003cc20: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0003cc30: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0003cc40: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0003cc50: 2020 6966 2073 656c 662e 6c69 6d69 7420    if self.limit 
-0003cc60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003cc70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003cc80: 274c 696d 6974 275d 203d 2073 656c 662e  'Limit'] = self.
-0003cc90: 6c69 6d69 740a 2020 2020 2020 2020 6966  limit.        if
-0003cca0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
-0003ccb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003ccc0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003ccd0: 5b27 4e65 7874 546f 6b65 6e27 5d20 3d20  ['NextToken'] = 
-0003cce0: 7365 6c66 2e6e 6578 745f 746f 6b65 6e0a  self.next_token.
-0003ccf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003cd00: 7265 736f 7572 6365 5f69 6420 6973 206e  resource_id is n
-0003cd10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003cd20: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
-0003cd30: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
-0003cd40: 2e72 6573 6f75 7263 655f 6964 0a20 2020  .resource_id.   
-0003cd50: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
-0003cd60: 6f75 7263 655f 7479 7065 2069 7320 6e6f  ource_type is no
-0003cd70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003cd80: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
-0003cd90: 7572 6365 5479 7065 275d 203d 2073 656c  urceType'] = sel
-0003cda0: 662e 7265 736f 7572 6365 5f74 7970 650a  f.resource_type.
-0003cdb0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003cdc0: 5461 6727 5d20 3d20 5b5d 0a20 2020 2020  Tag'] = [].     
-0003cdd0: 2020 2069 6620 7365 6c66 2e74 6167 2069     if self.tag i
-0003cde0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003cdf0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-0003ce00: 2073 656c 662e 7461 673a 0a20 2020 2020   self.tag:.     
-0003ce10: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003ce20: 745b 2754 6167 275d 2e61 7070 656e 6428  t['Tag'].append(
-0003ce30: 6b2e 746f 5f6d 6170 2829 2069 6620 6b20  k.to_map() if k 
-0003ce40: 656c 7365 204e 6f6e 6529 0a20 2020 2020  else None).     
-0003ce50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0003ce60: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-0003ce70: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
-0003ce80: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0003ce90: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0003cea0: 2020 6966 206d 2e67 6574 2827 4c69 6d69    if m.get('Limi
-0003ceb0: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
-0003cec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003ced0: 662e 6c69 6d69 7420 3d20 6d2e 6765 7428  f.limit = m.get(
-0003cee0: 274c 696d 6974 2729 0a20 2020 2020 2020  'Limit').       
-0003cef0: 2069 6620 6d2e 6765 7428 274e 6578 7454   if m.get('NextT
-0003cf00: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
-0003cf10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003cf20: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
-0003cf30: 3d20 6d2e 6765 7428 274e 6578 7454 6f6b  = m.get('NextTok
-0003cf40: 656e 2729 0a20 2020 2020 2020 2069 6620  en').        if 
-0003cf50: 6d2e 6765 7428 2752 6573 6f75 7263 6549  m.get('ResourceI
-0003cf60: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0003cf70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003cf80: 662e 7265 736f 7572 6365 5f69 6420 3d20  f.resource_id = 
-0003cf90: 6d2e 6765 7428 2752 6573 6f75 7263 6549  m.get('ResourceI
-0003cfa0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-0003cfb0: 2e67 6574 2827 5265 736f 7572 6365 5479  .get('ResourceTy
-0003cfc0: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
-0003cfd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0003cfe0: 6c66 2e72 6573 6f75 7263 655f 7479 7065  lf.resource_type
-0003cff0: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
-0003d000: 6365 5479 7065 2729 0a20 2020 2020 2020  ceType').       
-0003d010: 2073 656c 662e 7461 6720 3d20 5b5d 0a20   self.tag = []. 
-0003d020: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003d030: 2754 6167 2729 2069 7320 6e6f 7420 4e6f  'Tag') is not No
-0003d040: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003d050: 666f 7220 6b20 696e 206d 2e67 6574 2827  for k in m.get('
-0003d060: 5461 6727 293a 0a20 2020 2020 2020 2020  Tag'):.         
-0003d070: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-0003d080: 6c20 3d20 4c69 7374 5461 6752 6573 6f75  l = ListTagResou
-0003d090: 7263 6573 5265 7175 6573 7454 6167 2829  rcesRequestTag()
-0003d0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003d0b0: 2073 656c 662e 7461 672e 6170 7065 6e64   self.tag.append
-0003d0c0: 2874 656d 705f 6d6f 6465 6c2e 6672 6f6d  (temp_model.from
-0003d0d0: 5f6d 6170 286b 2929 0a20 2020 2020 2020  _map(k)).       
-0003d0e0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0003d0f0: 6c61 7373 204c 6973 7454 6167 5265 736f  lass ListTagReso
-0003d100: 7572 6365 7353 6872 696e 6b52 6571 7565  urcesShrinkReque
-0003d110: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-0003d120: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0003d130: 656c 662c 206c 696d 6974 3d4e 6f6e 652c  elf, limit=None,
-0003d140: 206e 6578 745f 746f 6b65 6e3d 4e6f 6e65   next_token=None
-0003d150: 2c20 7265 736f 7572 6365 5f69 645f 7368  , resource_id_sh
-0003d160: 7269 6e6b 3d4e 6f6e 652c 2072 6573 6f75  rink=None, resou
-0003d170: 7263 655f 7479 7065 3d4e 6f6e 652c 2074  rce_type=None, t
-0003d180: 6167 5f73 6872 696e 6b3d 4e6f 6e65 293a  ag_shrink=None):
-0003d190: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-0003d1a0: 6d69 7420 3d20 6c69 6d69 7420 2023 2074  mit = limit  # t
-0003d1b0: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
-0003d1c0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
-0003d1d0: 203d 206e 6578 745f 746f 6b65 6e20 2023   = next_token  #
-0003d1e0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0003d1f0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
-0003d200: 5f69 645f 7368 7269 6e6b 203d 2072 6573  _id_shrink = res
-0003d210: 6f75 7263 655f 6964 5f73 6872 696e 6b20  ource_id_shrink 
-0003d220: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-0003d230: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
-0003d240: 6365 5f74 7970 6520 3d20 7265 736f 7572  ce_type = resour
-0003d250: 6365 5f74 7970 6520 2023 2074 7970 653a  ce_type  # type:
-0003d260: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-0003d270: 662e 7461 675f 7368 7269 6e6b 203d 2074  f.tag_shrink = t
-0003d280: 6167 5f73 6872 696e 6b20 2023 2074 7970  ag_shrink  # typ
-0003d290: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
-0003d2a0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0003d2b0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0003d2c0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0003d2d0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0003d2e0: 203d 2073 7570 6572 284c 6973 7454 6167   = super(ListTag
-0003d2f0: 5265 736f 7572 6365 7353 6872 696e 6b52  ResourcesShrinkR
-0003d300: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
-0003d310: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0003d320: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0003d330: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003d340: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0003d350: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0003d360: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0003d370: 7365 6c66 2e6c 696d 6974 2069 7320 6e6f  self.limit is no
-0003d380: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003d390: 2020 2020 7265 7375 6c74 5b27 4c69 6d69      result['Limi
-0003d3a0: 7427 5d20 3d20 7365 6c66 2e6c 696d 6974  t'] = self.limit
-0003d3b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0003d3c0: 2e6e 6578 745f 746f 6b65 6e20 6973 206e  .next_token is n
-0003d3d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003d3e0: 2020 2020 2072 6573 756c 745b 274e 6578       result['Nex
-0003d3f0: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
-0003d400: 6e65 7874 5f74 6f6b 656e 0a20 2020 2020  next_token.     
-0003d410: 2020 2069 6620 7365 6c66 2e72 6573 6f75     if self.resou
-0003d420: 7263 655f 6964 5f73 6872 696e 6b20 6973  rce_id_shrink is
-0003d430: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003d440: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0003d450: 6573 6f75 7263 6549 6427 5d20 3d20 7365  esourceId'] = se
-0003d460: 6c66 2e72 6573 6f75 7263 655f 6964 5f73  lf.resource_id_s
-0003d470: 6872 696e 6b0a 2020 2020 2020 2020 6966  hrink.        if
-0003d480: 2073 656c 662e 7265 736f 7572 6365 5f74   self.resource_t
-0003d490: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
-0003d4a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003d4b0: 756c 745b 2752 6573 6f75 7263 6554 7970  ult['ResourceTyp
-0003d4c0: 6527 5d20 3d20 7365 6c66 2e72 6573 6f75  e'] = self.resou
-0003d4d0: 7263 655f 7479 7065 0a20 2020 2020 2020  rce_type.       
-0003d4e0: 2069 6620 7365 6c66 2e74 6167 5f73 6872   if self.tag_shr
-0003d4f0: 696e 6b20 6973 206e 6f74 204e 6f6e 653a  ink is not None:
-0003d500: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003d510: 756c 745b 2754 6167 275d 203d 2073 656c  ult['Tag'] = sel
-0003d520: 662e 7461 675f 7368 7269 6e6b 0a20 2020  f.tag_shrink.   
-0003d530: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0003d540: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0003d550: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-0003d560: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0003d570: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0003d580: 2020 2020 6966 206d 2e67 6574 2827 4c69      if m.get('Li
-0003d590: 6d69 7427 2920 6973 206e 6f74 204e 6f6e  mit') is not Non
-0003d5a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0003d5b0: 656c 662e 6c69 6d69 7420 3d20 6d2e 6765  elf.limit = m.ge
-0003d5c0: 7428 274c 696d 6974 2729 0a20 2020 2020  t('Limit').     
-0003d5d0: 2020 2069 6620 6d2e 6765 7428 274e 6578     if m.get('Nex
-0003d5e0: 7454 6f6b 656e 2729 2069 7320 6e6f 7420  tToken') is not 
-0003d5f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003d600: 2020 7365 6c66 2e6e 6578 745f 746f 6b65    self.next_toke
-0003d610: 6e20 3d20 6d2e 6765 7428 274e 6578 7454  n = m.get('NextT
-0003d620: 6f6b 656e 2729 0a20 2020 2020 2020 2069  oken').        i
-0003d630: 6620 6d2e 6765 7428 2752 6573 6f75 7263  f m.get('Resourc
-0003d640: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-0003d650: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0003d660: 656c 662e 7265 736f 7572 6365 5f69 645f  elf.resource_id_
-0003d670: 7368 7269 6e6b 203d 206d 2e67 6574 2827  shrink = m.get('
-0003d680: 5265 736f 7572 6365 4964 2729 0a20 2020  ResourceId').   
-0003d690: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-0003d6a0: 6573 6f75 7263 6554 7970 6527 2920 6973  esourceType') is
-0003d6b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003d6c0: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-0003d6d0: 7572 6365 5f74 7970 6520 3d20 6d2e 6765  urce_type = m.ge
-0003d6e0: 7428 2752 6573 6f75 7263 6554 7970 6527  t('ResourceType'
-0003d6f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003d700: 6574 2827 5461 6727 2920 6973 206e 6f74  et('Tag') is not
-0003d710: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003d720: 2020 2073 656c 662e 7461 675f 7368 7269     self.tag_shri
-0003d730: 6e6b 203d 206d 2e67 6574 2827 5461 6727  nk = m.get('Tag'
-0003d740: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0003d750: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
-0003d760: 7374 5461 6752 6573 6f75 7263 6573 5265  stTagResourcesRe
-0003d770: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-0003d780: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003d790: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
-0003d7a0: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
-0003d7b0: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
-0003d7c0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
-0003d7d0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-0003d7e0: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
-0003d7f0: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
-0003d800: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-0003d810: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-0003d820: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
-0003d830: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0003d840: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
-0003d850: 3a20 4c69 7374 5461 6752 6573 6f75 7263  : ListTagResourc
-0003d860: 6573 4f75 7470 7574 0a0a 2020 2020 6465  esOutput..    de
-0003d870: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0003d880: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-0003d890: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-0003d8a0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-0003d8b0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-0003d8c0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0003d8d0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0003d8e0: 7570 6572 284c 6973 7454 6167 5265 736f  uper(ListTagReso
-0003d8f0: 7572 6365 7352 6573 706f 6e73 652c 2073  urcesResponse, s
-0003d900: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-0003d910: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003d920: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003d930: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003d940: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003d950: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003d960: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-0003d970: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-0003d980: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003d990: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-0003d9a0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-0003d9b0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0003d9c0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-0003d9d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003d9e0: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-0003d9f0: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-0003da00: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0003da10: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0003da20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003da30: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003da40: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0003da50: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0003da60: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0003da70: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0003da80: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-0003da90: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0003daa0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0003dab0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-0003dac0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-0003dad0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003dae0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0003daf0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0003db00: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003db10: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-0003db20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003db30: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-0003db40: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-0003db50: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-0003db60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003db70: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-0003db80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003db90: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
-0003dba0: 6973 7454 6167 5265 736f 7572 6365 734f  istTagResourcesO
-0003dbb0: 7574 7075 7428 290a 2020 2020 2020 2020  utput().        
-0003dbc0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0003dbd0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-0003dbe0: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-0003dbf0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0003dc00: 6c66 0a0a 0a63 6c61 7373 204c 6973 7454  lf...class ListT
-0003dc10: 7269 6767 6572 7352 6571 7565 7374 2854  riggersRequest(T
-0003dc20: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0003dc30: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0003dc40: 206c 696d 6974 3d4e 6f6e 652c 206e 6578   limit=None, nex
-0003dc50: 745f 746f 6b65 6e3d 4e6f 6e65 2c20 7072  t_token=None, pr
-0003dc60: 6566 6978 3d4e 6f6e 6529 3a0a 2020 2020  efix=None):.    
-0003dc70: 2020 2020 2320 5468 6520 6e75 6d62 6572      # The number
-0003dc80: 206f 6620 7472 6967 6765 7273 2072 6574   of triggers ret
-0003dc90: 7572 6e65 642e 0a20 2020 2020 2020 2073  urned..        s
-0003dca0: 656c 662e 6c69 6d69 7420 3d20 6c69 6d69  elf.limit = limi
-0003dcb0: 7420 2023 2074 7970 653a 2069 6e74 0a20  t  # type: int. 
-0003dcc0: 2020 2020 2020 2023 2054 6865 2074 6f6b         # The tok
-0003dcd0: 656e 2066 6f72 2074 6865 206e 6578 7420  en for the next 
-0003dce0: 7061 6765 2e0a 2020 2020 2020 2020 7365  page..        se
-0003dcf0: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
-0003dd00: 6e65 7874 5f74 6f6b 656e 2020 2320 7479  next_token  # ty
-0003dd10: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-0003dd20: 2320 5468 6520 7472 6967 6765 7220 6e61  # The trigger na
-0003dd30: 6d65 2070 7265 6669 782e 0a20 2020 2020  me prefix..     
-0003dd40: 2020 2073 656c 662e 7072 6566 6978 203d     self.prefix =
-0003dd50: 2070 7265 6669 7820 2023 2074 7970 653a   prefix  # type:
-0003dd60: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
-0003dd70: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-0003dd80: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0003dd90: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-0003dda0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-0003ddb0: 2073 7570 6572 284c 6973 7454 7269 6767   super(ListTrigg
-0003ddc0: 6572 7352 6571 7565 7374 2c20 7365 6c66  ersRequest, self
-0003ddd0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0003dde0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0003ddf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003de00: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0003de10: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0003de20: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0003de30: 2069 6620 7365 6c66 2e6c 696d 6974 2069   if self.limit i
-0003de40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003de50: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003de60: 6c69 6d69 7427 5d20 3d20 7365 6c66 2e6c  limit'] = self.l
-0003de70: 696d 6974 0a20 2020 2020 2020 2069 6620  imit.        if 
-0003de80: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
-0003de90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003dea0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003deb0: 276e 6578 7454 6f6b 656e 275d 203d 2073  'nextToken'] = s
-0003dec0: 656c 662e 6e65 7874 5f74 6f6b 656e 0a20  elf.next_token. 
-0003ded0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0003dee0: 7265 6669 7820 6973 206e 6f74 204e 6f6e  refix is not Non
-0003def0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003df00: 6573 756c 745b 2770 7265 6669 7827 5d20  esult['prefix'] 
-0003df10: 3d20 7365 6c66 2e70 7265 6669 780a 2020  = self.prefix.  
-0003df20: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0003df30: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0003df40: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-0003df50: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0003df60: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0003df70: 2020 2020 2069 6620 6d2e 6765 7428 276c       if m.get('l
-0003df80: 696d 6974 2729 2069 7320 6e6f 7420 4e6f  imit') is not No
-0003df90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003dfa0: 7365 6c66 2e6c 696d 6974 203d 206d 2e67  self.limit = m.g
-0003dfb0: 6574 2827 6c69 6d69 7427 290a 2020 2020  et('limit').    
-0003dfc0: 2020 2020 6966 206d 2e67 6574 2827 6e65      if m.get('ne
-0003dfd0: 7874 546f 6b65 6e27 2920 6973 206e 6f74  xtToken') is not
-0003dfe0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003dff0: 2020 2073 656c 662e 6e65 7874 5f74 6f6b     self.next_tok
-0003e000: 656e 203d 206d 2e67 6574 2827 6e65 7874  en = m.get('next
-0003e010: 546f 6b65 6e27 290a 2020 2020 2020 2020  Token').        
-0003e020: 6966 206d 2e67 6574 2827 7072 6566 6978  if m.get('prefix
-0003e030: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0003e040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003e050: 2e70 7265 6669 7820 3d20 6d2e 6765 7428  .prefix = m.get(
-0003e060: 2770 7265 6669 7827 290a 2020 2020 2020  'prefix').      
-0003e070: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0003e080: 636c 6173 7320 4c69 7374 5472 6967 6765  class ListTrigge
-0003e090: 7273 5265 7370 6f6e 7365 2854 6561 4d6f  rsResponse(TeaMo
-0003e0a0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0003e0b0: 696e 6974 5f5f 2873 656c 662c 2068 6561  init__(self, hea
-0003e0c0: 6465 7273 3d4e 6f6e 652c 2073 7461 7475  ders=None, statu
-0003e0d0: 735f 636f 6465 3d4e 6f6e 652c 2062 6f64  s_code=None, bod
-0003e0e0: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-0003e0f0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0003e100: 6865 6164 6572 7320 2023 2074 7970 653a  headers  # type:
-0003e110: 2064 6963 745b 7374 722c 2073 7472 5d0a   dict[str, str].
-0003e120: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0003e130: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
-0003e140: 735f 636f 6465 2020 2320 7479 7065 3a20  s_code  # type: 
-0003e150: 696e 740a 2020 2020 2020 2020 7365 6c66  int.        self
-0003e160: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
-0003e170: 7479 7065 3a20 4c69 7374 5472 6967 6765  type: ListTrigge
-0003e180: 7273 4f75 7470 7574 0a0a 2020 2020 6465  rsOutput..    de
-0003e190: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0003e1a0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-0003e1b0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-0003e1c0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-0003e1d0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-0003e1e0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0003e1f0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0003e200: 7570 6572 284c 6973 7454 7269 6767 6572  uper(ListTrigger
-0003e210: 7352 6573 706f 6e73 652c 2073 656c 6629  sResponse, self)
-0003e220: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0003e230: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0003e240: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003e250: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0003e260: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0003e270: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0003e280: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0003e290: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003e2a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003e2b0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0003e2c0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0003e2d0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0003e2e0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0003e2f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003e300: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0003e310: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0003e320: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0003e330: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0003e340: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003e350: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0003e360: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0003e370: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0003e380: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0003e390: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0003e3a0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0003e3b0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0003e3c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0003e3d0: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-0003e3e0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-0003e3f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003e400: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-0003e410: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-0003e420: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-0003e430: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-0003e440: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003e450: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0003e460: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-0003e470: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-0003e480: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-0003e490: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-0003e4a0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-0003e4b0: 6d70 5f6d 6f64 656c 203d 204c 6973 7454  mp_model = ListT
-0003e4c0: 7269 6767 6572 734f 7574 7075 7428 290a  riggersOutput().
-0003e4d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003e4e0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-0003e4f0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-0003e500: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-0003e510: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0003e520: 7373 204c 6973 7456 7063 4269 6e64 696e  ss ListVpcBindin
-0003e530: 6773 5265 7370 6f6e 7365 2854 6561 4d6f  gsResponse(TeaMo
-0003e540: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0003e550: 696e 6974 5f5f 2873 656c 662c 2068 6561  init__(self, hea
-0003e560: 6465 7273 3d4e 6f6e 652c 2073 7461 7475  ders=None, statu
-0003e570: 735f 636f 6465 3d4e 6f6e 652c 2062 6f64  s_code=None, bod
-0003e580: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-0003e590: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0003e5a0: 6865 6164 6572 7320 2023 2074 7970 653a  headers  # type:
-0003e5b0: 2064 6963 745b 7374 722c 2073 7472 5d0a   dict[str, str].
-0003e5c0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0003e5d0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
-0003e5e0: 735f 636f 6465 2020 2320 7479 7065 3a20  s_code  # type: 
-0003e5f0: 696e 740a 2020 2020 2020 2020 7365 6c66  int.        self
-0003e600: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
-0003e610: 7479 7065 3a20 4c69 7374 5670 6342 696e  type: ListVpcBin
-0003e620: 6469 6e67 734f 7574 7075 740a 0a20 2020  dingsOutput..   
-0003e630: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0003e640: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-0003e650: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-0003e660: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0003e670: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-0003e680: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-0003e690: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-0003e6a0: 3d20 7375 7065 7228 4c69 7374 5670 6342  = super(ListVpcB
-0003e6b0: 696e 6469 6e67 7352 6573 706f 6e73 652c  indingsResponse,
-0003e6c0: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-0003e6d0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0003e6e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003e6f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0003e700: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0003e710: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0003e720: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-0003e730: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-0003e740: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003e750: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-0003e760: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-0003e770: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003e780: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-0003e790: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003e7a0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-0003e7b0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-0003e7c0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-0003e7d0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0003e7e0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-0003e7f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003e800: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-0003e810: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-0003e820: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0003e830: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0003e840: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-0003e850: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0003e860: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0003e870: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0003e880: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-0003e890: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003e8a0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0003e8b0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-0003e8c0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0003e8d0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0003e8e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003e8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003e900: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-0003e910: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0003e920: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003e930: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-0003e940: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003e950: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-0003e960: 204c 6973 7456 7063 4269 6e64 696e 6773   ListVpcBindings
-0003e970: 4f75 7470 7574 2829 0a20 2020 2020 2020  Output().       
-0003e980: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0003e990: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-0003e9a0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-0003e9b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0003e9c0: 656c 660a 0a0a 636c 6173 7320 5075 626c  elf...class Publ
-0003e9d0: 6973 6846 756e 6374 696f 6e56 6572 7369  ishFunctionVersi
-0003e9e0: 6f6e 5265 7175 6573 7428 5465 614d 6f64  onRequest(TeaMod
-0003e9f0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0003ea00: 6e69 745f 5f28 7365 6c66 2c20 626f 6479  nit__(self, body
-0003ea10: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0003ea20: 2320 5468 6520 696e 666f 726d 6174 696f  # The informatio
-0003ea30: 6e20 6162 6f75 7420 7468 6520 6675 6e63  n about the func
-0003ea40: 7469 6f6e 2076 6572 7369 6f6e 2e0a 2020  tion version..  
-0003ea50: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0003ea60: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
-0003ea70: 5075 626c 6973 6856 6572 7369 6f6e 496e  PublishVersionIn
-0003ea80: 7075 740a 0a20 2020 2064 6566 2076 616c  put..    def val
-0003ea90: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0003eaa0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0003eab0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0003eac0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-0003ead0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0003eae0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0003eaf0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0003eb00: 5075 626c 6973 6846 756e 6374 696f 6e56  PublishFunctionV
-0003eb10: 6572 7369 6f6e 5265 7175 6573 742c 2073  ersionRequest, s
-0003eb20: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-0003eb30: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003eb40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003eb50: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003eb60: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003eb70: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003eb80: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0003eb90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003eba0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003ebb0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-0003ebc0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-0003ebd0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0003ebe0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0003ebf0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-0003ec00: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0003ec10: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0003ec20: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-0003ec30: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-0003ec40: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0003ec50: 656d 705f 6d6f 6465 6c20 3d20 5075 626c  emp_model = Publ
-0003ec60: 6973 6856 6572 7369 6f6e 496e 7075 7428  ishVersionInput(
-0003ec70: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0003ec80: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0003ec90: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0003eca0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0003ecb0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0003ecc0: 6c61 7373 2050 7562 6c69 7368 4675 6e63  lass PublishFunc
-0003ecd0: 7469 6f6e 5665 7273 696f 6e52 6573 706f  tionVersionRespo
-0003ece0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-0003ecf0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0003ed00: 7365 6c66 2c20 6865 6164 6572 733d 4e6f  self, headers=No
-0003ed10: 6e65 2c20 7374 6174 7573 5f63 6f64 653d  ne, status_code=
-0003ed20: 4e6f 6e65 2c20 626f 6479 3d4e 6f6e 6529  None, body=None)
-0003ed30: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-0003ed40: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-0003ed50: 2020 2320 7479 7065 3a20 6469 6374 5b73    # type: dict[s
-0003ed60: 7472 2c20 7374 725d 0a20 2020 2020 2020  tr, str].       
-0003ed70: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003ed80: 6520 3d20 7374 6174 7573 5f63 6f64 6520  e = status_code 
-0003ed90: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
-0003eda0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0003edb0: 2062 6f64 7920 2023 2074 7970 653a 2056   body  # type: V
-0003edc0: 6572 7369 6f6e 0a0a 2020 2020 6465 6620  ersion..    def 
-0003edd0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0003ede0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003edf0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-0003ee00: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-0003ee10: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-0003ee20: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0003ee30: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0003ee40: 6572 2850 7562 6c69 7368 4675 6e63 7469  er(PublishFuncti
-0003ee50: 6f6e 5665 7273 696f 6e52 6573 706f 6e73  onVersionRespons
-0003ee60: 652c 2073 656c 6629 2e74 6f5f 6d61 7028  e, self).to_map(
-0003ee70: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-0003ee80: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-0003ee90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0003eea0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-0003eeb0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-0003eec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003eed0: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
-0003eee0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003eef0: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
-0003ef00: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
-0003ef10: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-0003ef20: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
-0003ef30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003ef40: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
-0003ef50: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
-0003ef60: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
-0003ef70: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0003ef80: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
-0003ef90: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003efa0: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
-0003efb0: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
-0003efc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0003efd0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-0003efe0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-0003eff0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0003f000: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-0003f010: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003f020: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-0003f030: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003f040: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-0003f050: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-0003f060: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-0003f070: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0003f080: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0003f090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003f0a0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-0003f0b0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0003f0c0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0003f0d0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-0003f0e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003f0f0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-0003f100: 203d 2056 6572 7369 6f6e 2829 0a20 2020   = Version().   
-0003f110: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003f120: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-0003f130: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-0003f140: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-0003f150: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0003f160: 5075 7441 7379 6e63 496e 766f 6b65 436f  PutAsyncInvokeCo
-0003f170: 6e66 6967 5265 7175 6573 7428 5465 614d  nfigRequest(TeaM
-0003f180: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0003f190: 5f69 6e69 745f 5f28 7365 6c66 2c20 626f  _init__(self, bo
-0003f1a0: 6479 3d4e 6f6e 652c 2071 7561 6c69 6669  dy=None, qualifi
-0003f1b0: 6572 3d4e 6f6e 6529 3a0a 2020 2020 2020  er=None):.      
-0003f1c0: 2020 2320 5468 6520 636f 6e66 6967 7572    # The configur
-0003f1d0: 6174 696f 6e73 206f 6620 6173 796e 6368  ations of asynch
-0003f1e0: 726f 6e6f 7573 2066 756e 6374 696f 6e20  ronous function 
-0003f1f0: 696e 766f 6361 7469 6f6e 2e0a 2020 2020  invocation..    
-0003f200: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0003f210: 626f 6479 2020 2320 7479 7065 3a20 5075  body  # type: Pu
-0003f220: 7441 7379 6e63 496e 766f 6b65 436f 6e66  tAsyncInvokeConf
-0003f230: 6967 496e 7075 740a 2020 2020 2020 2020  igInput.        
-0003f240: 2320 5468 6520 7665 7273 696f 6e20 6f72  # The version or
-0003f250: 2061 6c69 6173 206f 6620 7468 6520 6675   alias of the fu
-0003f260: 6e63 7469 6f6e 2e0a 2020 2020 2020 2020  nction..        
-0003f270: 7365 6c66 2e71 7561 6c69 6669 6572 203d  self.qualifier =
-0003f280: 2071 7561 6c69 6669 6572 2020 2320 7479   qualifier  # ty
-0003f290: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-0003f2a0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0003f2b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0003f2c0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-0003f2d0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-0003f2e0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-0003f2f0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0003f300: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0003f310: 7065 7228 5075 7441 7379 6e63 496e 766f  per(PutAsyncInvo
-0003f320: 6b65 436f 6e66 6967 5265 7175 6573 742c  keConfigRequest,
-0003f330: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-0003f340: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0003f350: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003f360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0003f370: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0003f380: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0003f390: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-0003f3a0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-0003f3b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0003f3c0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-0003f3d0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-0003f3e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003f3f0: 7175 616c 6966 6965 7220 6973 206e 6f74  qualifier is not
-0003f400: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003f410: 2020 2072 6573 756c 745b 2771 7561 6c69     result['quali
-0003f420: 6669 6572 275d 203d 2073 656c 662e 7175  fier'] = self.qu
-0003f430: 616c 6966 6965 720a 2020 2020 2020 2020  alifier.        
-0003f440: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0003f450: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0003f460: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-0003f470: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-0003f480: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0003f490: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-0003f4a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003f4b0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-0003f4c0: 6465 6c20 3d20 5075 7441 7379 6e63 496e  del = PutAsyncIn
-0003f4d0: 766f 6b65 436f 6e66 6967 496e 7075 7428  vokeConfigInput(
-0003f4e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0003f4f0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0003f500: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0003f510: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0003f520: 2069 6620 6d2e 6765 7428 2771 7561 6c69   if m.get('quali
-0003f530: 6669 6572 2729 2069 7320 6e6f 7420 4e6f  fier') is not No
-0003f540: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003f550: 7365 6c66 2e71 7561 6c69 6669 6572 203d  self.qualifier =
-0003f560: 206d 2e67 6574 2827 7175 616c 6966 6965   m.get('qualifie
-0003f570: 7227 290a 2020 2020 2020 2020 7265 7475  r').        retu
-0003f580: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0003f590: 5075 7441 7379 6e63 496e 766f 6b65 436f  PutAsyncInvokeCo
-0003f5a0: 6e66 6967 5265 7370 6f6e 7365 2854 6561  nfigResponse(Tea
-0003f5b0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0003f5c0: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
-0003f5d0: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
-0003f5e0: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
-0003f5f0: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
-0003f600: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0003f610: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
-0003f620: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
-0003f630: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
-0003f640: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-0003f650: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
-0003f660: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
-0003f670: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
-0003f680: 2320 7479 7065 3a20 4173 796e 6343 6f6e  # type: AsyncCon
-0003f690: 6669 670a 0a20 2020 2064 6566 2076 616c  fig..    def val
-0003f6a0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0003f6b0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0003f6c0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0003f6d0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-0003f6e0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0003f6f0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0003f700: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0003f710: 5075 7441 7379 6e63 496e 766f 6b65 436f  PutAsyncInvokeCo
-0003f720: 6e66 6967 5265 7370 6f6e 7365 2c20 7365  nfigResponse, se
-0003f730: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-0003f740: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0003f750: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003f760: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0003f770: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0003f780: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0003f790: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-0003f7a0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-0003f7b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0003f7c0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-0003f7d0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-0003f7e0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-0003f7f0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-0003f800: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003f810: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-0003f820: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-0003f830: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-0003f840: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-0003f850: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003f860: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003f870: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-0003f880: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-0003f890: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0003f8a0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0003f8b0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-0003f8c0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0003f8d0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0003f8e0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-0003f8f0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-0003f900: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003f910: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-0003f920: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-0003f930: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003f940: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-0003f950: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003f960: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0003f970: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-0003f980: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-0003f990: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003f9a0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-0003f9b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003f9c0: 2074 656d 705f 6d6f 6465 6c20 3d20 4173   temp_model = As
-0003f9d0: 796e 6343 6f6e 6669 6728 290a 2020 2020  yncConfig().    
-0003f9e0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0003f9f0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-0003fa00: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-0003fa10: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-0003fa20: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2050  n self...class P
-0003fa30: 7574 436f 6e63 7572 7265 6e63 7943 6f6e  utConcurrencyCon
-0003fa40: 6669 6752 6571 7565 7374 2854 6561 4d6f  figRequest(TeaMo
-0003fa50: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0003fa60: 696e 6974 5f5f 2873 656c 662c 2062 6f64  init__(self, bod
-0003fa70: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-0003fa80: 2023 2054 6865 2063 6f6e 6375 7272 656e   # The concurren
-0003fa90: 6379 2063 6f6e 6669 6775 7261 7469 6f6e  cy configuration
-0003faa0: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-0003fab0: 626f 6479 203d 2062 6f64 7920 2023 2074  body = body  # t
-0003fac0: 7970 653a 2050 7574 436f 6e63 7572 7265  ype: PutConcurre
-0003fad0: 6e63 7949 6e70 7574 0a0a 2020 2020 6465  ncyInput..    de
-0003fae0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0003faf0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-0003fb00: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-0003fb10: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-0003fb20: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-0003fb30: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0003fb40: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0003fb50: 7570 6572 2850 7574 436f 6e63 7572 7265  uper(PutConcurre
-0003fb60: 6e63 7943 6f6e 6669 6752 6571 7565 7374  ncyConfigRequest
-0003fb70: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-0003fb80: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0003fb90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003fba0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0003fbb0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0003fbc0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0003fbd0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0003fbe0: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
-0003fbf0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003fc00: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
-0003fc10: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
-0003fc20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0003fc30: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-0003fc40: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-0003fc50: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0003fc60: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-0003fc70: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003fc80: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-0003fc90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003fca0: 2020 7465 6d70 5f6d 6f64 656c 203d 2050    temp_model = P
-0003fcb0: 7574 436f 6e63 7572 7265 6e63 7949 6e70  utConcurrencyInp
-0003fcc0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-0003fcd0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-0003fce0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-0003fcf0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-0003fd00: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0003fd10: 0a0a 636c 6173 7320 5075 7443 6f6e 6375  ..class PutConcu
-0003fd20: 7272 656e 6379 436f 6e66 6967 5265 7370  rrencyConfigResp
-0003fd30: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-0003fd40: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0003fd50: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
-0003fd60: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
-0003fd70: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
-0003fd80: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0003fd90: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-0003fda0: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
-0003fdb0: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
-0003fdc0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0003fdd0: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-0003fde0: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
-0003fdf0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0003fe00: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
-0003fe10: 436f 6e63 7572 7265 6e63 7943 6f6e 6669  ConcurrencyConfi
-0003fe20: 670a 0a20 2020 2064 6566 2076 616c 6964  g..    def valid
-0003fe30: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-0003fe40: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-0003fe50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003fe60: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-0003fe70: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-0003fe80: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0003fe90: 205f 6d61 7020 3d20 7375 7065 7228 5075   _map = super(Pu
-0003fea0: 7443 6f6e 6375 7272 656e 6379 436f 6e66  tConcurrencyConf
-0003feb0: 6967 5265 7370 6f6e 7365 2c20 7365 6c66  igResponse, self
-0003fec0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0003fed0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0003fee0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003fef0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0003ff00: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0003ff10: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0003ff20: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-0003ff30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003ff40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003ff50: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-0003ff60: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-0003ff70: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-0003ff80: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-0003ff90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003ffa0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-0003ffb0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-0003ffc0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-0003ffd0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-0003ffe0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003fff0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00040000: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00040010: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00040020: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00040030: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00040040: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00040050: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00040060: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00040070: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-00040080: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-00040090: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000400a0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-000400b0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-000400c0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000400d0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-000400e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000400f0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00040100: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00040110: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00040120: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00040130: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-00040140: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00040150: 656d 705f 6d6f 6465 6c20 3d20 436f 6e63  emp_model = Conc
-00040160: 7572 7265 6e63 7943 6f6e 6669 6728 290a  urrencyConfig().
-00040170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00040180: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-00040190: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-000401a0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-000401b0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-000401c0: 7373 2050 7574 4c61 7965 7241 434c 5265  ss PutLayerACLRe
-000401d0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-000401e0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000401f0: 5f28 7365 6c66 2c20 7075 626c 6963 3d4e  _(self, public=N
-00040200: 6f6e 6529 3a0a 2020 2020 2020 2020 2320  one):.        # 
-00040210: 5370 6563 6966 6965 7320 7768 6574 6865  Specifies whethe
-00040220: 7220 7468 6520 6c61 7965 7220 6973 2061  r the layer is a
-00040230: 2070 7562 6c69 6320 6c61 7965 722e 2056   public layer. V
-00040240: 616c 6964 2076 616c 7565 733a 2074 7275  alid values: tru
-00040250: 6520 616e 6420 6661 6c73 652e 0a20 2020  e and false..   
-00040260: 2020 2020 2073 656c 662e 7075 626c 6963       self.public
-00040270: 203d 2070 7562 6c69 6320 2023 2074 7970   = public  # typ
-00040280: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
-00040290: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000402a0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000402b0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000402c0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-000402d0: 203d 2073 7570 6572 2850 7574 4c61 7965   = super(PutLaye
-000402e0: 7241 434c 5265 7175 6573 742c 2073 656c  rACLRequest, sel
-000402f0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-00040300: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00040310: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00040320: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00040330: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00040340: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00040350: 2020 6966 2073 656c 662e 7075 626c 6963    if self.public
-00040360: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00040370: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00040380: 5b27 7075 626c 6963 275d 203d 2073 656c  ['public'] = sel
-00040390: 662e 7075 626c 6963 0a20 2020 2020 2020  f.public.       
-000403a0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000403b0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000403c0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-000403d0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000403e0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000403f0: 6966 206d 2e67 6574 2827 7075 626c 6963  if m.get('public
-00040400: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00040410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00040420: 2e70 7562 6c69 6320 3d20 6d2e 6765 7428  .public = m.get(
-00040430: 2770 7562 6c69 6327 290a 2020 2020 2020  'public').      
-00040440: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00040450: 636c 6173 7320 5075 744c 6179 6572 4143  class PutLayerAC
-00040460: 4c52 6573 706f 6e73 6528 5465 614d 6f64  LResponse(TeaMod
-00040470: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00040480: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
-00040490: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
-000404a0: 5f63 6f64 653d 4e6f 6e65 293a 0a20 2020  _code=None):.   
-000404b0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-000404c0: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
-000404d0: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
-000404e0: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
-000404f0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-00040500: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
-00040510: 7065 3a20 696e 740a 0a20 2020 2064 6566  pe: int..    def
-00040520: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-00040530: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00040540: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00040550: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00040560: 7020 3d20 7375 7065 7228 5075 744c 6179  p = super(PutLay
-00040570: 6572 4143 4c52 6573 706f 6e73 652c 2073  erACLResponse, s
-00040580: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-00040590: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-000405a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000405b0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000405c0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000405d0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000405e0: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-000405f0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-00040600: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00040610: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-00040620: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-00040630: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00040640: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-00040650: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00040660: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-00040670: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-00040680: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-00040690: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000406a0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000406b0: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
-000406c0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000406d0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000406e0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-000406f0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-00040700: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00040710: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-00040720: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-00040730: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00040740: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-00040750: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00040760: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00040770: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-00040780: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-00040790: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000407a0: 660a 0a0a 636c 6173 7320 5075 7450 726f  f...class PutPro
-000407b0: 7669 7369 6f6e 436f 6e66 6967 5265 7175  visionConfigRequ
-000407c0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-000407d0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000407e0: 7365 6c66 2c20 626f 6479 3d4e 6f6e 652c  self, body=None,
-000407f0: 2071 7561 6c69 6669 6572 3d4e 6f6e 6529   qualifier=None)
-00040800: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
-00040810: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
-00040820: 7420 7468 6520 7072 6f76 6973 696f 6e65  t the provisione
-00040830: 6420 636f 6e66 6967 7572 6174 696f 6e2e  d configuration.
-00040840: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-00040850: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
-00040860: 653a 2050 7574 5072 6f76 6973 696f 6e43  e: PutProvisionC
-00040870: 6f6e 6669 6749 6e70 7574 0a20 2020 2020  onfigInput.     
-00040880: 2020 2023 2054 6865 2066 756e 6374 696f     # The functio
-00040890: 6e20 616c 6961 7320 6f72 204c 4154 4553  n alias or LATES
-000408a0: 542e 0a20 2020 2020 2020 2073 656c 662e  T..        self.
-000408b0: 7175 616c 6966 6965 7220 3d20 7175 616c  qualifier = qual
-000408c0: 6966 6965 7220 2023 2074 7970 653a 2073  ifier  # type: s
-000408d0: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
-000408e0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-000408f0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-00040900: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00040910: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-00040920: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-00040930: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00040940: 2020 5f6d 6170 203d 2073 7570 6572 2850    _map = super(P
-00040950: 7574 5072 6f76 6973 696f 6e43 6f6e 6669  utProvisionConfi
-00040960: 6752 6571 7565 7374 2c20 7365 6c66 292e  gRequest, self).
-00040970: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00040980: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00040990: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000409a0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000409b0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000409c0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000409d0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-000409e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000409f0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-00040a00: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-00040a10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00040a20: 2069 6620 7365 6c66 2e71 7561 6c69 6669   if self.qualifi
-00040a30: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00040a40: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00040a50: 6c74 5b27 7175 616c 6966 6965 7227 5d20  lt['qualifier'] 
-00040a60: 3d20 7365 6c66 2e71 7561 6c69 6669 6572  = self.qualifier
-00040a70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00040a80: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00040a90: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00040aa0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00040ab0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00040ac0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00040ad0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-00040ae0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00040af0: 2020 7465 6d70 5f6d 6f64 656c 203d 2050    temp_model = P
-00040b00: 7574 5072 6f76 6973 696f 6e43 6f6e 6669  utProvisionConfi
-00040b10: 6749 6e70 7574 2829 0a20 2020 2020 2020  gInput().       
-00040b20: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00040b30: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-00040b40: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-00040b50: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00040b60: 2827 7175 616c 6966 6965 7227 2920 6973  ('qualifier') is
-00040b70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00040b80: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
-00040b90: 6966 6965 7220 3d20 6d2e 6765 7428 2771  ifier = m.get('q
-00040ba0: 7561 6c69 6669 6572 2729 0a20 2020 2020  ualifier').     
-00040bb0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00040bc0: 0a63 6c61 7373 2050 7574 5072 6f76 6973  .class PutProvis
-00040bd0: 696f 6e43 6f6e 6669 6752 6573 706f 6e73  ionConfigRespons
-00040be0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-00040bf0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00040c00: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
-00040c10: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
-00040c20: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
-00040c30: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00040c40: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
-00040c50: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
-00040c60: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
-00040c70: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00040c80: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
-00040c90: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
-00040ca0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-00040cb0: 6f64 7920 2023 2074 7970 653a 2050 726f  ody  # type: Pro
-00040cc0: 7669 7369 6f6e 436f 6e66 6967 0a0a 2020  visionConfig..  
-00040cd0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00040ce0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00040cf0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-00040d00: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00040d10: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-00040d20: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00040d30: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00040d40: 203d 2073 7570 6572 2850 7574 5072 6f76   = super(PutProv
-00040d50: 6973 696f 6e43 6f6e 6669 6752 6573 706f  isionConfigRespo
-00040d60: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
-00040d70: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00040d80: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00040d90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00040da0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00040db0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00040dc0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00040dd0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00040de0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00040df0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00040e00: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00040e10: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00040e20: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00040e30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00040e40: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00040e50: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-00040e60: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00040e70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00040e80: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00040e90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00040ea0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00040eb0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00040ec0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00040ed0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00040ee0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00040ef0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-00040f00: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00040f10: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00040f20: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-00040f30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00040f40: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00040f50: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00040f60: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00040f70: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00040f80: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00040f90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00040fa0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00040fb0: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-00040fc0: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-00040fd0: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-00040fe0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00040ff0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-00041000: 656c 203d 2050 726f 7669 7369 6f6e 436f  el = ProvisionCo
-00041010: 6e66 6967 2829 0a20 2020 2020 2020 2020  nfig().         
-00041020: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-00041030: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-00041040: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-00041050: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00041060: 660a 0a0a 636c 6173 7320 5461 6752 6573  f...class TagRes
-00041070: 6f75 7263 6573 5265 7175 6573 7428 5465  ourcesRequest(Te
-00041080: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00041090: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-000410a0: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
-000410b0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-000410c0: 626f 6479 2020 2320 7479 7065 3a20 5461  body  # type: Ta
-000410d0: 6752 6573 6f75 7263 6573 496e 7075 740a  gResourcesInput.
-000410e0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-000410f0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00041100: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00041110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00041120: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-00041130: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00041140: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00041150: 6d61 7020 3d20 7375 7065 7228 5461 6752  map = super(TagR
-00041160: 6573 6f75 7263 6573 5265 7175 6573 742c  esourcesRequest,
-00041170: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-00041180: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00041190: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000411a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000411b0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-000411c0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-000411d0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-000411e0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-000411f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00041200: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-00041210: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-00041220: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00041230: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00041240: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
-00041250: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00041260: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00041270: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00041280: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-00041290: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000412a0: 2074 656d 705f 6d6f 6465 6c20 3d20 5461   temp_model = Ta
-000412b0: 6752 6573 6f75 7263 6573 496e 7075 7428  gResourcesInput(
-000412c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000412d0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-000412e0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-000412f0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-00041300: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00041310: 6c61 7373 2054 6167 5265 736f 7572 6365  lass TagResource
-00041320: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
-00041330: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00041340: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
-00041350: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
-00041360: 5f63 6f64 653d 4e6f 6e65 293a 0a20 2020  _code=None):.   
-00041370: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00041380: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
-00041390: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
-000413a0: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
-000413b0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-000413c0: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
-000413d0: 7065 3a20 696e 740a 0a20 2020 2064 6566  pe: int..    def
-000413e0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000413f0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00041400: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00041410: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00041420: 7020 3d20 7375 7065 7228 5461 6752 6573  p = super(TagRes
-00041430: 6f75 7263 6573 5265 7370 6f6e 7365 2c20  ourcesResponse, 
-00041440: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-00041450: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00041460: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041470: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00041480: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00041490: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-000414a0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-000414b0: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-000414c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000414d0: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-000414e0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-000414f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00041500: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-00041510: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00041520: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-00041530: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-00041540: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-00041550: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00041560: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00041570: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-00041580: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00041590: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-000415a0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-000415b0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-000415c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000415d0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-000415e0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-000415f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00041600: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-00041610: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041620: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00041630: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-00041640: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-00041650: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00041660: 6c66 0a0a 0a63 6c61 7373 2055 6e74 6167  lf...class Untag
-00041670: 5265 736f 7572 6365 7352 6571 7565 7374  ResourcesRequest
-00041680: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00041690: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000416a0: 662c 2061 6c6c 3d4e 6f6e 652c 2072 6573  f, all=None, res
-000416b0: 6f75 7263 655f 6964 3d4e 6f6e 652c 2072  ource_id=None, r
-000416c0: 6573 6f75 7263 655f 7479 7065 3d4e 6f6e  esource_type=Non
-000416d0: 652c 2074 6167 5f6b 6579 3d4e 6f6e 6529  e, tag_key=None)
-000416e0: 3a0a 2020 2020 2020 2020 7365 6c66 2e61  :.        self.a
-000416f0: 6c6c 203d 2061 6c6c 2020 2320 7479 7065  ll = all  # type
-00041700: 3a20 626f 6f6c 0a20 2020 2020 2020 2073  : bool.        s
-00041710: 656c 662e 7265 736f 7572 6365 5f69 6420  elf.resource_id 
-00041720: 3d20 7265 736f 7572 6365 5f69 6420 2023  = resource_id  #
-00041730: 2074 7970 653a 206c 6973 745b 7374 725d   type: list[str]
-00041740: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00041750: 736f 7572 6365 5f74 7970 6520 3d20 7265  source_type = re
-00041760: 736f 7572 6365 5f74 7970 6520 2023 2074  source_type  # t
-00041770: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
-00041780: 2073 656c 662e 7461 675f 6b65 7920 3d20   self.tag_key = 
-00041790: 7461 675f 6b65 7920 2023 2074 7970 653a  tag_key  # type:
-000417a0: 206c 6973 745b 7374 725d 0a0a 2020 2020   list[str]..    
-000417b0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-000417c0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-000417d0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000417e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000417f0: 5f6d 6170 203d 2073 7570 6572 2855 6e74  _map = super(Unt
-00041800: 6167 5265 736f 7572 6365 7352 6571 7565  agResourcesReque
-00041810: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
-00041820: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00041830: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00041840: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00041850: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00041860: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00041870: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00041880: 2e61 6c6c 2069 7320 6e6f 7420 4e6f 6e65  .all is not None
-00041890: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000418a0: 7375 6c74 5b27 416c 6c27 5d20 3d20 7365  sult['All'] = se
-000418b0: 6c66 2e61 6c6c 0a20 2020 2020 2020 2069  lf.all.        i
-000418c0: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
-000418d0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-000418e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000418f0: 6c74 5b27 5265 736f 7572 6365 4964 275d  lt['ResourceId']
-00041900: 203d 2073 656c 662e 7265 736f 7572 6365   = self.resource
-00041910: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-00041920: 656c 662e 7265 736f 7572 6365 5f74 7970  elf.resource_typ
-00041930: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00041940: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00041950: 745b 2752 6573 6f75 7263 6554 7970 6527  t['ResourceType'
-00041960: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
-00041970: 655f 7479 7065 0a20 2020 2020 2020 2069  e_type.        i
-00041980: 6620 7365 6c66 2e74 6167 5f6b 6579 2069  f self.tag_key i
-00041990: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000419a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000419b0: 5461 674b 6579 275d 203d 2073 656c 662e  TagKey'] = self.
-000419c0: 7461 675f 6b65 790a 2020 2020 2020 2020  tag_key.        
-000419d0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000419e0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000419f0: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-00041a00: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00041a10: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00041a20: 6620 6d2e 6765 7428 2741 6c6c 2729 2069  f m.get('All') i
-00041a30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041a40: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00041a50: 203d 206d 2e67 6574 2827 416c 6c27 290a   = m.get('All').
-00041a60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00041a70: 2827 5265 736f 7572 6365 4964 2729 2069  ('ResourceId') i
-00041a80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041a90: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00041aa0: 6f75 7263 655f 6964 203d 206d 2e67 6574  ource_id = m.get
-00041ab0: 2827 5265 736f 7572 6365 4964 2729 0a20  ('ResourceId'). 
-00041ac0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00041ad0: 2752 6573 6f75 7263 6554 7970 6527 2920  'ResourceType') 
-00041ae0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00041af0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00041b00: 736f 7572 6365 5f74 7970 6520 3d20 6d2e  source_type = m.
-00041b10: 6765 7428 2752 6573 6f75 7263 6554 7970  get('ResourceTyp
-00041b20: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00041b30: 2e67 6574 2827 5461 674b 6579 2729 2069  .get('TagKey') i
-00041b40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041b50: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
-00041b60: 5f6b 6579 203d 206d 2e67 6574 2827 5461  _key = m.get('Ta
-00041b70: 674b 6579 2729 0a20 2020 2020 2020 2072  gKey').        r
-00041b80: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00041b90: 7373 2055 6e74 6167 5265 736f 7572 6365  ss UntagResource
-00041ba0: 7353 6872 696e 6b52 6571 7565 7374 2854  sShrinkRequest(T
-00041bb0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00041bc0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00041bd0: 2061 6c6c 3d4e 6f6e 652c 2072 6573 6f75   all=None, resou
-00041be0: 7263 655f 6964 5f73 6872 696e 6b3d 4e6f  rce_id_shrink=No
-00041bf0: 6e65 2c20 7265 736f 7572 6365 5f74 7970  ne, resource_typ
-00041c00: 653d 4e6f 6e65 2c20 7461 675f 6b65 795f  e=None, tag_key_
-00041c10: 7368 7269 6e6b 3d4e 6f6e 6529 3a0a 2020  shrink=None):.  
-00041c20: 2020 2020 2020 7365 6c66 2e61 6c6c 203d        self.all =
-00041c30: 2061 6c6c 2020 2320 7479 7065 3a20 626f   all  # type: bo
-00041c40: 6f6c 0a20 2020 2020 2020 2073 656c 662e  ol.        self.
-00041c50: 7265 736f 7572 6365 5f69 645f 7368 7269  resource_id_shri
-00041c60: 6e6b 203d 2072 6573 6f75 7263 655f 6964  nk = resource_id
-00041c70: 5f73 6872 696e 6b20 2023 2074 7970 653a  _shrink  # type:
-00041c80: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-00041c90: 662e 7265 736f 7572 6365 5f74 7970 6520  f.resource_type 
-00041ca0: 3d20 7265 736f 7572 6365 5f74 7970 6520  = resource_type 
-00041cb0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-00041cc0: 2020 2020 2073 656c 662e 7461 675f 6b65       self.tag_ke
-00041cd0: 795f 7368 7269 6e6b 203d 2074 6167 5f6b  y_shrink = tag_k
-00041ce0: 6579 5f73 6872 696e 6b20 2023 2074 7970  ey_shrink  # typ
-00041cf0: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
-00041d00: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00041d10: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00041d20: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00041d30: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00041d40: 203d 2073 7570 6572 2855 6e74 6167 5265   = super(UntagRe
-00041d50: 736f 7572 6365 7353 6872 696e 6b52 6571  sourcesShrinkReq
-00041d60: 7565 7374 2c20 7365 6c66 292e 746f 5f6d  uest, self).to_m
-00041d70: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00041d80: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00041d90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00041da0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00041db0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00041dc0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00041dd0: 6c66 2e61 6c6c 2069 7320 6e6f 7420 4e6f  lf.all is not No
-00041de0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00041df0: 7265 7375 6c74 5b27 416c 6c27 5d20 3d20  result['All'] = 
-00041e00: 7365 6c66 2e61 6c6c 0a20 2020 2020 2020  self.all.       
-00041e10: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
-00041e20: 655f 6964 5f73 6872 696e 6b20 6973 206e  e_id_shrink is n
-00041e30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00041e40: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
-00041e50: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
-00041e60: 2e72 6573 6f75 7263 655f 6964 5f73 6872  .resource_id_shr
-00041e70: 696e 6b0a 2020 2020 2020 2020 6966 2073  ink.        if s
-00041e80: 656c 662e 7265 736f 7572 6365 5f74 7970  elf.resource_typ
-00041e90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00041ea0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00041eb0: 745b 2752 6573 6f75 7263 6554 7970 6527  t['ResourceType'
-00041ec0: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
-00041ed0: 655f 7479 7065 0a20 2020 2020 2020 2069  e_type.        i
-00041ee0: 6620 7365 6c66 2e74 6167 5f6b 6579 5f73  f self.tag_key_s
-00041ef0: 6872 696e 6b20 6973 206e 6f74 204e 6f6e  hrink is not Non
-00041f00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00041f10: 6573 756c 745b 2754 6167 4b65 7927 5d20  esult['TagKey'] 
-00041f20: 3d20 7365 6c66 2e74 6167 5f6b 6579 5f73  = self.tag_key_s
-00041f30: 6872 696e 6b0a 2020 2020 2020 2020 7265  hrink.        re
-00041f40: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00041f50: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00041f60: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
-00041f70: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-00041f80: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00041f90: 6d2e 6765 7428 2741 6c6c 2729 2069 7320  m.get('All') is 
-00041fa0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00041fb0: 2020 2020 2020 7365 6c66 2e61 6c6c 203d        self.all =
-00041fc0: 206d 2e67 6574 2827 416c 6c27 290a 2020   m.get('All').  
-00041fd0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00041fe0: 5265 736f 7572 6365 4964 2729 2069 7320  ResourceId') is 
-00041ff0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00042000: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
-00042010: 7263 655f 6964 5f73 6872 696e 6b20 3d20  rce_id_shrink = 
-00042020: 6d2e 6765 7428 2752 6573 6f75 7263 6549  m.get('ResourceI
-00042030: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00042040: 2e67 6574 2827 5265 736f 7572 6365 5479  .get('ResourceTy
-00042050: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
-00042060: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00042070: 6c66 2e72 6573 6f75 7263 655f 7479 7065  lf.resource_type
-00042080: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
-00042090: 6365 5479 7065 2729 0a20 2020 2020 2020  ceType').       
-000420a0: 2069 6620 6d2e 6765 7428 2754 6167 4b65   if m.get('TagKe
-000420b0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-000420c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000420d0: 662e 7461 675f 6b65 795f 7368 7269 6e6b  f.tag_key_shrink
-000420e0: 203d 206d 2e67 6574 2827 5461 674b 6579   = m.get('TagKey
-000420f0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00042100: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-00042110: 6e74 6167 5265 736f 7572 6365 7352 6573  ntagResourcesRes
-00042120: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-00042130: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00042140: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
-00042150: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
-00042160: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
-00042170: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-00042180: 6865 6164 6572 7320 2023 2074 7970 653a  headers  # type:
-00042190: 2064 6963 745b 7374 722c 2073 7472 5d0a   dict[str, str].
-000421a0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-000421b0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
-000421c0: 735f 636f 6465 2020 2320 7479 7065 3a20  s_code  # type: 
-000421d0: 696e 740a 0a20 2020 2064 6566 2076 616c  int..    def val
-000421e0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000421f0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00042200: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00042210: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00042220: 7375 7065 7228 556e 7461 6752 6573 6f75  super(UntagResou
-00042230: 7263 6573 5265 7370 6f6e 7365 2c20 7365  rcesResponse, se
-00042240: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-00042250: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00042260: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00042270: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00042280: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00042290: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000422a0: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-000422b0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-000422c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000422d0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-000422e0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-000422f0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00042300: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-00042310: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00042320: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-00042330: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-00042340: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-00042350: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00042360: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00042370: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00042380: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00042390: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000423a0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-000423b0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-000423c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000423d0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-000423e0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-000423f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00042400: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00042410: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00042420: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00042430: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00042440: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00042450: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00042460: 0a0a 0a63 6c61 7373 2055 7064 6174 6541  ...class UpdateA
-00042470: 6c69 6173 5265 7175 6573 7428 5465 614d  liasRequest(TeaM
-00042480: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00042490: 5f69 6e69 745f 5f28 7365 6c66 2c20 626f  _init__(self, bo
-000424a0: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
-000424b0: 2020 2320 5468 6520 616c 6961 7320 696e    # The alias in
-000424c0: 666f 726d 6174 696f 6e20 746f 2062 6520  formation to be 
-000424d0: 7570 6461 7465 642e 0a20 2020 2020 2020  updated..       
-000424e0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-000424f0: 7920 2023 2074 7970 653a 2055 7064 6174  y  # type: Updat
-00042500: 6541 6c69 6173 496e 7075 740a 0a20 2020  eAliasInput..   
-00042510: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00042520: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00042530: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-00042540: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00042550: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-00042560: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00042570: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00042580: 3d20 7375 7065 7228 5570 6461 7465 416c  = super(UpdateAl
-00042590: 6961 7352 6571 7565 7374 2c20 7365 6c66  iasRequest, self
-000425a0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-000425b0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000425c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000425d0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000425e0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000425f0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00042600: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-00042610: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00042620: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00042630: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00042640: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-00042650: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00042660: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00042670: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
-00042680: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00042690: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000426a0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-000426b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000426c0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000426d0: 5f6d 6f64 656c 203d 2055 7064 6174 6541  _model = UpdateA
-000426e0: 6c69 6173 496e 7075 7428 290a 2020 2020  liasInput().    
-000426f0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00042700: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-00042710: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-00042720: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-00042730: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-00042740: 7064 6174 6541 6c69 6173 5265 7370 6f6e  pdateAliasRespon
-00042750: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-00042760: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00042770: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
-00042780: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
-00042790: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
-000427a0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-000427b0: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
-000427c0: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
-000427d0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
-000427e0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000427f0: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
-00042800: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
-00042810: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00042820: 626f 6479 2020 2320 7479 7065 3a20 416c  body  # type: Al
-00042830: 6961 730a 0a20 2020 2064 6566 2076 616c  ias..    def val
-00042840: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00042850: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00042860: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00042870: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-00042880: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-00042890: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-000428a0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-000428b0: 5570 6461 7465 416c 6961 7352 6573 706f  UpdateAliasRespo
-000428c0: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
-000428d0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-000428e0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-000428f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00042900: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00042910: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00042920: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00042930: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00042940: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00042950: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00042960: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00042970: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00042980: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00042990: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000429a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000429b0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-000429c0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000429d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000429e0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-000429f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00042a00: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00042a10: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00042a20: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00042a30: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00042a40: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00042a50: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-00042a60: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00042a70: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00042a80: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-00042a90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00042aa0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00042ab0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00042ac0: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00042ad0: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00042ae0: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00042af0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00042b00: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00042b10: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-00042b20: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-00042b30: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-00042b40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00042b50: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-00042b60: 656c 203d 2041 6c69 6173 2829 0a20 2020  el = Alias().   
-00042b70: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00042b80: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-00042b90: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-00042ba0: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-00042bb0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00042bc0: 5570 6461 7465 4375 7374 6f6d 446f 6d61  UpdateCustomDoma
-00042bd0: 696e 5265 7175 6573 7428 5465 614d 6f64  inRequest(TeaMod
-00042be0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00042bf0: 6e69 745f 5f28 7365 6c66 2c20 626f 6479  nit__(self, body
-00042c00: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00042c10: 2320 5468 6520 696e 666f 726d 6174 696f  # The informatio
-00042c20: 6e20 6162 6f75 7420 7468 6520 6375 7374  n about the cust
-00042c30: 6f6d 2064 6f6d 6169 6e20 6e61 6d65 2e0a  om domain name..
-00042c40: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00042c50: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
-00042c60: 3a20 5570 6461 7465 4375 7374 6f6d 446f  : UpdateCustomDo
-00042c70: 6d61 696e 496e 7075 740a 0a20 2020 2064  mainInput..    d
-00042c80: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00042c90: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00042ca0: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
-00042cb0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
-00042cc0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-00042cd0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00042ce0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00042cf0: 7375 7065 7228 5570 6461 7465 4375 7374  super(UpdateCust
-00042d00: 6f6d 446f 6d61 696e 5265 7175 6573 742c  omDomainRequest,
-00042d10: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-00042d20: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00042d30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00042d40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00042d50: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00042d60: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00042d70: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00042d80: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-00042d90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00042da0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-00042db0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-00042dc0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00042dd0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00042de0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
-00042df0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00042e00: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00042e10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00042e20: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-00042e30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042e40: 2074 656d 705f 6d6f 6465 6c20 3d20 5570   temp_model = Up
-00042e50: 6461 7465 4375 7374 6f6d 446f 6d61 696e  dateCustomDomain
-00042e60: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
-00042e70: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00042e80: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00042e90: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-00042ea0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00042eb0: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
-00042ec0: 6543 7573 746f 6d44 6f6d 6169 6e52 6573  eCustomDomainRes
-00042ed0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-00042ee0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00042ef0: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
-00042f00: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
-00042f10: 653d 4e6f 6e65 2c20 626f 6479 3d4e 6f6e  e=None, body=Non
-00042f20: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00042f30: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-00042f40: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
-00042f50: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
-00042f60: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00042f70: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-00042f80: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
-00042f90: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00042fa0: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
-00042fb0: 2043 7573 746f 6d44 6f6d 6169 6e0a 0a20   CustomDomain.. 
-00042fc0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00042fd0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00042fe0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-00042ff0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00043000: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-00043010: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00043020: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00043030: 7020 3d20 7375 7065 7228 5570 6461 7465  p = super(Update
-00043040: 4375 7374 6f6d 446f 6d61 696e 5265 7370  CustomDomainResp
-00043050: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
-00043060: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00043070: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00043080: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00043090: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-000430a0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-000430b0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-000430c0: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-000430d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000430e0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-000430f0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-00043100: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-00043110: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00043120: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00043130: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00043140: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-00043150: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00043160: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00043170: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-00043180: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00043190: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-000431a0: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-000431b0: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-000431c0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-000431d0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-000431e0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-000431f0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00043200: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00043210: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-00043220: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00043230: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00043240: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-00043250: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00043260: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00043270: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00043280: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00043290: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000432a0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-000432b0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-000432c0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-000432d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000432e0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000432f0: 6465 6c20 3d20 4375 7374 6f6d 446f 6d61  del = CustomDoma
-00043300: 696e 2829 0a20 2020 2020 2020 2020 2020  in().           
-00043310: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-00043320: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-00043330: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-00043340: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00043350: 0a0a 636c 6173 7320 5570 6461 7465 4675  ..class UpdateFu
-00043360: 6e63 7469 6f6e 5265 7175 6573 7428 5465  nctionRequest(Te
-00043370: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00043380: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00043390: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
-000433a0: 2020 2020 2320 5468 6520 6675 6e63 7469      # The functi
-000433b0: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 0a20  on information. 
-000433c0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-000433d0: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
-000433e0: 2055 7064 6174 6546 756e 6374 696f 6e49   UpdateFunctionI
-000433f0: 6e70 7574 0a0a 2020 2020 6465 6620 7661  nput..    def va
-00043400: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00043410: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00043420: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-00043430: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-00043440: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00043450: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00043460: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00043470: 2855 7064 6174 6546 756e 6374 696f 6e52  (UpdateFunctionR
-00043480: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
-00043490: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000434a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000434b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000434c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000434d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000434e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000434f0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-00043500: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00043510: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-00043520: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-00043530: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-00043540: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00043550: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00043560: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
-00043570: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00043580: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00043590: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-000435a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000435b0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-000435c0: 656c 203d 2055 7064 6174 6546 756e 6374  el = UpdateFunct
-000435d0: 696f 6e49 6e70 7574 2829 0a20 2020 2020  ionInput().     
-000435e0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-000435f0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-00043600: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-00043610: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00043620: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-00043630: 6461 7465 4675 6e63 7469 6f6e 5265 7370  dateFunctionResp
-00043640: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-00043650: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00043660: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
-00043670: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
-00043680: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
-00043690: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000436a0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-000436b0: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
-000436c0: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
-000436d0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-000436e0: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-000436f0: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
-00043700: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-00043710: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
-00043720: 4675 6e63 7469 6f6e 0a0a 2020 2020 6465  Function..    de
-00043730: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00043740: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00043750: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00043760: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00043770: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00043780: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00043790: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-000437a0: 7570 6572 2855 7064 6174 6546 756e 6374  uper(UpdateFunct
-000437b0: 696f 6e52 6573 706f 6e73 652c 2073 656c  ionResponse, sel
-000437c0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-000437d0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-000437e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000437f0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00043800: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00043810: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00043820: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-00043830: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00043840: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00043850: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-00043860: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-00043870: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00043880: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-00043890: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000438a0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-000438b0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-000438c0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-000438d0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-000438e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000438f0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00043900: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00043910: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-00043920: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00043930: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00043940: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
-00043950: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00043960: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00043970: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-00043980: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-00043990: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000439a0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-000439b0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-000439c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000439d0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-000439e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000439f0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00043a00: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-00043a10: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-00043a20: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00043a30: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-00043a40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00043a50: 7465 6d70 5f6d 6f64 656c 203d 2046 756e  temp_model = Fun
-00043a60: 6374 696f 6e28 290a 2020 2020 2020 2020  ction().        
-00043a70: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00043a80: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00043a90: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-00043aa0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00043ab0: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
-00043ac0: 6554 7269 6767 6572 5265 7175 6573 7428  eTriggerRequest(
-00043ad0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00043ae0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00043af0: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
-00043b00: 2020 2020 2020 2320 5468 6520 7472 6967        # The trig
-00043b10: 6765 7220 636f 6e66 6967 7572 6174 696f  ger configuratio
-00043b20: 6e73 2e0a 2020 2020 2020 2020 7365 6c66  ns..        self
-00043b30: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
-00043b40: 7479 7065 3a20 5570 6461 7465 5472 6967  type: UpdateTrig
-00043b50: 6765 7249 6e70 7574 0a0a 2020 2020 6465  gerInput..    de
-00043b60: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00043b70: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00043b80: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00043b90: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00043ba0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00043bb0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00043bc0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00043bd0: 7570 6572 2855 7064 6174 6554 7269 6767  uper(UpdateTrigg
-00043be0: 6572 5265 7175 6573 742c 2073 656c 6629  erRequest, self)
-00043bf0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00043c00: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00043c10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00043c20: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00043c30: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00043c40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00043c50: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00043c60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00043c70: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00043c80: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00043c90: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00043ca0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00043cb0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00043cc0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00043cd0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00043ce0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00043cf0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-00043d00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00043d10: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00043d20: 6d6f 6465 6c20 3d20 5570 6461 7465 5472  model = UpdateTr
-00043d30: 6967 6765 7249 6e70 7574 2829 0a20 2020  iggerInput().   
-00043d40: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00043d50: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-00043d60: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-00043d70: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-00043d80: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00043d90: 5570 6461 7465 5472 6967 6765 7252 6573  UpdateTriggerRes
-00043da0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-00043db0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00043dc0: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
-00043dd0: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
-00043de0: 653d 4e6f 6e65 2c20 626f 6479 3d4e 6f6e  e=None, body=Non
-00043df0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00043e00: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-00043e10: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
-00043e20: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
-00043e30: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00043e40: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-00043e50: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
-00043e60: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00043e70: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
-00043e80: 2054 7269 6767 6572 0a0a 2020 2020 6465   Trigger..    de
-00043e90: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00043ea0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00043eb0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00043ec0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00043ed0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00043ee0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00043ef0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00043f00: 7570 6572 2855 7064 6174 6554 7269 6767  uper(UpdateTrigg
-00043f10: 6572 5265 7370 6f6e 7365 2c20 7365 6c66  erResponse, self
-00043f20: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00043f30: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00043f40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00043f50: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00043f60: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00043f70: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00043f80: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00043f90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00043fa0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00043fb0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00043fc0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-00043fd0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00043fe0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00043ff0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00044000: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00044010: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00044020: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00044030: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00044040: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00044050: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00044060: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00044070: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00044080: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00044090: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-000440a0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-000440b0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000440c0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000440d0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-000440e0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-000440f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00044100: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-00044110: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-00044120: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00044130: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00044140: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00044150: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00044160: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00044170: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00044180: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00044190: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-000441a0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-000441b0: 656d 705f 6d6f 6465 6c20 3d20 5472 6967  emp_model = Trig
-000441c0: 6765 7228 290a 2020 2020 2020 2020 2020  ger().          
-000441d0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-000441e0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-000441f0: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-00044200: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00044210: 0a0a 0a                                  ...
+00032aa0: 636c 6173 7320 4765 7441 7379 6e63 5461  class GetAsyncTa
+00032ab0: 736b 5265 7175 6573 7428 5465 614d 6f64  skRequest(TeaMod
+00032ac0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00032ad0: 6e69 745f 5f28 7365 6c66 2c20 7175 616c  nit__(self, qual
+00032ae0: 6966 6965 723d 4e6f 6e65 293a 0a20 2020  ifier=None):.   
+00032af0: 2020 2020 2073 656c 662e 7175 616c 6966       self.qualif
+00032b00: 6965 7220 3d20 7175 616c 6966 6965 7220  ier = qualifier 
+00032b10: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
+00032b20: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00032b30: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00032b40: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+00032b50: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00032b60: 2020 5f6d 6170 203d 2073 7570 6572 2847    _map = super(G
+00032b70: 6574 4173 796e 6354 6173 6b52 6571 7565  etAsyncTaskReque
+00032b80: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
+00032b90: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00032ba0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00032bb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00032bc0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00032bd0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00032be0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00032bf0: 2e71 7561 6c69 6669 6572 2069 7320 6e6f  .qualifier is no
+00032c00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00032c10: 2020 2020 7265 7375 6c74 5b27 7175 616c      result['qual
+00032c20: 6966 6965 7227 5d20 3d20 7365 6c66 2e71  ifier'] = self.q
+00032c30: 7561 6c69 6669 6572 0a20 2020 2020 2020  ualifier.       
+00032c40: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00032c50: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00032c60: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+00032c70: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00032c80: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00032c90: 6966 206d 2e67 6574 2827 7175 616c 6966  if m.get('qualif
+00032ca0: 6965 7227 2920 6973 206e 6f74 204e 6f6e  ier') is not Non
+00032cb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00032cc0: 656c 662e 7175 616c 6966 6965 7220 3d20  elf.qualifier = 
+00032cd0: 6d2e 6765 7428 2771 7561 6c69 6669 6572  m.get('qualifier
+00032ce0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00032cf0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2047  n self...class G
+00032d00: 6574 4173 796e 6354 6173 6b52 6573 706f  etAsyncTaskRespo
+00032d10: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+00032d20: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00032d30: 7365 6c66 2c20 6865 6164 6572 733d 4e6f  self, headers=No
+00032d40: 6e65 2c20 7374 6174 7573 5f63 6f64 653d  ne, status_code=
+00032d50: 4e6f 6e65 2c20 626f 6479 3d4e 6f6e 6529  None, body=None)
+00032d60: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+00032d70: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+00032d80: 2020 2320 7479 7065 3a20 6469 6374 5b73    # type: dict[s
+00032d90: 7472 2c20 7374 725d 0a20 2020 2020 2020  tr, str].       
+00032da0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00032db0: 6520 3d20 7374 6174 7573 5f63 6f64 6520  e = status_code 
+00032dc0: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
+00032dd0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00032de0: 2062 6f64 7920 2023 2074 7970 653a 2041   body  # type: A
+00032df0: 7379 6e63 5461 736b 0a0a 2020 2020 6465  syncTask..    de
+00032e00: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00032e10: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00032e20: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+00032e30: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+00032e40: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00032e50: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00032e60: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00032e70: 7570 6572 2847 6574 4173 796e 6354 6173  uper(GetAsyncTas
+00032e80: 6b52 6573 706f 6e73 652c 2073 656c 6629  kResponse, self)
+00032e90: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00032ea0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00032eb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00032ec0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00032ed0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00032ee0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00032ef0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00032f00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00032f10: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00032f20: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00032f30: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00032f40: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00032f50: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00032f60: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00032f70: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00032f80: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00032f90: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00032fa0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00032fb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00032fc0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00032fd0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00032fe0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00032ff0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00033000: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00033010: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+00033020: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00033030: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00033040: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00033050: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00033060: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00033070: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00033080: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00033090: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+000330a0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+000330b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000330c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000330d0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+000330e0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+000330f0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00033100: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00033110: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00033120: 6d70 5f6d 6f64 656c 203d 2041 7379 6e63  mp_model = Async
+00033130: 5461 736b 2829 0a20 2020 2020 2020 2020  Task().         
+00033140: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+00033150: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+00033160: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+00033170: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00033180: 660a 0a0a 636c 6173 7320 4765 7443 6f6e  f...class GetCon
+00033190: 6375 7272 656e 6379 436f 6e66 6967 5265  currencyConfigRe
+000331a0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+000331b0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000331c0: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
+000331d0: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
+000331e0: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
+000331f0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00033200: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00033210: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
+00033220: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
+00033230: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00033240: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00033250: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
+00033260: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00033270: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
+00033280: 3a20 436f 6e63 7572 7265 6e63 7943 6f6e  : ConcurrencyCon
+00033290: 6669 670a 0a20 2020 2064 6566 2076 616c  fig..    def val
+000332a0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000332b0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+000332c0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+000332d0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+000332e0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+000332f0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00033300: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00033310: 4765 7443 6f6e 6375 7272 656e 6379 436f  GetConcurrencyCo
+00033320: 6e66 6967 5265 7370 6f6e 7365 2c20 7365  nfigResponse, se
+00033330: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+00033340: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00033350: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00033360: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00033370: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00033380: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00033390: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+000333a0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+000333b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000333c0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+000333d0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+000333e0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+000333f0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
+00033400: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00033410: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
+00033420: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
+00033430: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+00033440: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
+00033450: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033460: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00033470: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
+00033480: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
+00033490: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000334a0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000334b0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+000334c0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+000334d0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+000334e0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+000334f0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+00033500: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00033510: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+00033520: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+00033530: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00033540: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+00033550: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033560: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00033570: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+00033580: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+00033590: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000335a0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+000335b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000335c0: 2074 656d 705f 6d6f 6465 6c20 3d20 436f   temp_model = Co
+000335d0: 6e63 7572 7265 6e63 7943 6f6e 6669 6728  ncurrencyConfig(
+000335e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000335f0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
+00033600: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
+00033610: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
+00033620: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00033630: 6c61 7373 2047 6574 4375 7374 6f6d 446f  lass GetCustomDo
+00033640: 6d61 696e 5265 7370 6f6e 7365 2854 6561  mainResponse(Tea
+00033650: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00033660: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
+00033670: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
+00033680: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
+00033690: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
+000336a0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+000336b0: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
+000336c0: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
+000336d0: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
+000336e0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+000336f0: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
+00033700: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+00033710: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
+00033720: 2320 7479 7065 3a20 4375 7374 6f6d 446f  # type: CustomDo
+00033730: 6d61 696e 0a0a 2020 2020 6465 6620 7661  main..    def va
+00033740: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00033750: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00033760: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+00033770: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+00033780: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+00033790: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000337a0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000337b0: 2847 6574 4375 7374 6f6d 446f 6d61 696e  (GetCustomDomain
+000337c0: 5265 7370 6f6e 7365 2c20 7365 6c66 292e  Response, self).
+000337d0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000337e0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+000337f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00033800: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00033810: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00033820: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00033830: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+00033840: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033850: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00033860: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+00033870: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+00033880: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+00033890: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+000338a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000338b0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+000338c0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+000338d0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+000338e0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+000338f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00033900: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00033910: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00033920: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00033930: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00033940: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00033950: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
+00033960: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00033970: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00033980: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+00033990: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000339a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000339b0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+000339c0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+000339d0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+000339e0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+000339f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00033a00: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00033a10: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+00033a20: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+00033a30: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+00033a40: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+00033a50: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00033a60: 705f 6d6f 6465 6c20 3d20 4375 7374 6f6d  p_model = Custom
+00033a70: 446f 6d61 696e 2829 0a20 2020 2020 2020  Domain().       
+00033a80: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00033a90: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+00033aa0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+00033ab0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00033ac0: 656c 660a 0a0a 636c 6173 7320 4765 7446  elf...class GetF
+00033ad0: 756e 6374 696f 6e52 6571 7565 7374 2854  unctionRequest(T
+00033ae0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00033af0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00033b00: 2071 7561 6c69 6669 6572 3d4e 6f6e 6529   qualifier=None)
+00033b10: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
+00033b20: 7665 7273 696f 6e20 6f72 2061 6c69 6173  version or alias
+00033b30: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
+00033b40: 2e0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
+00033b50: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
+00033b60: 6669 6572 2020 2320 7479 7065 3a20 7374  fier  # type: st
+00033b70: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
+00033b80: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00033b90: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00033ba0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00033bb0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00033bc0: 7065 7228 4765 7446 756e 6374 696f 6e52  per(GetFunctionR
+00033bd0: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+00033be0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00033bf0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00033c00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00033c10: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00033c20: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00033c30: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00033c40: 7365 6c66 2e71 7561 6c69 6669 6572 2069  self.qualifier i
+00033c50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033c60: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00033c70: 7175 616c 6966 6965 7227 5d20 3d20 7365  qualifier'] = se
+00033c80: 6c66 2e71 7561 6c69 6669 6572 0a20 2020  lf.qualifier.   
+00033c90: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00033ca0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00033cb0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00033cc0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00033cd0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00033ce0: 2020 2020 6966 206d 2e67 6574 2827 7175      if m.get('qu
+00033cf0: 616c 6966 6965 7227 2920 6973 206e 6f74  alifier') is not
+00033d00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00033d10: 2020 2073 656c 662e 7175 616c 6966 6965     self.qualifie
+00033d20: 7220 3d20 6d2e 6765 7428 2771 7561 6c69  r = m.get('quali
+00033d30: 6669 6572 2729 0a20 2020 2020 2020 2072  fier').        r
+00033d40: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00033d50: 7373 2047 6574 4675 6e63 7469 6f6e 5265  ss GetFunctionRe
+00033d60: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00033d70: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00033d80: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
+00033d90: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
+00033da0: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
+00033db0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00033dc0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00033dd0: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
+00033de0: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
+00033df0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00033e00: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00033e10: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
+00033e20: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00033e30: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
+00033e40: 3a20 4675 6e63 7469 6f6e 0a0a 2020 2020  : Function..    
+00033e50: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00033e60: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00033e70: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+00033e80: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+00033e90: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00033ea0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00033eb0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00033ec0: 2073 7570 6572 2847 6574 4675 6e63 7469   super(GetFuncti
+00033ed0: 6f6e 5265 7370 6f6e 7365 2c20 7365 6c66  onResponse, self
+00033ee0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00033ef0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00033f00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00033f10: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00033f20: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00033f30: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00033f40: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+00033f50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00033f60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00033f70: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+00033f80: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+00033f90: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+00033fa0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+00033fb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00033fc0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+00033fd0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+00033fe0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00033ff0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+00034000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034010: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+00034020: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+00034030: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00034040: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00034050: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00034060: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00034070: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00034080: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00034090: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+000340a0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+000340b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000340c0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+000340d0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+000340e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000340f0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+00034100: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034110: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00034120: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00034130: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00034140: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00034150: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+00034160: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00034170: 656d 705f 6d6f 6465 6c20 3d20 4675 6e63  emp_model = Func
+00034180: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
+00034190: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+000341a0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+000341b0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+000341c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000341d0: 660a 0a0a 636c 6173 7320 4765 7446 756e  f...class GetFun
+000341e0: 6374 696f 6e43 6f64 6552 6571 7565 7374  ctionCodeRequest
+000341f0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00034200: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00034210: 662c 2071 7561 6c69 6669 6572 3d4e 6f6e  f, qualifier=Non
+00034220: 6529 3a0a 2020 2020 2020 2020 2320 5468  e):.        # Th
+00034230: 6520 7665 7273 696f 6e20 6f72 2061 6c69  e version or ali
+00034240: 6173 206f 6620 7468 6520 6675 6e63 7469  as of the functi
+00034250: 6f6e 2e0a 2020 2020 2020 2020 7365 6c66  on..        self
+00034260: 2e71 7561 6c69 6669 6572 203d 2071 7561  .qualifier = qua
+00034270: 6c69 6669 6572 2020 2320 7479 7065 3a20  lifier  # type: 
+00034280: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+00034290: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000342a0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000342b0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+000342c0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000342d0: 7375 7065 7228 4765 7446 756e 6374 696f  super(GetFunctio
+000342e0: 6e43 6f64 6552 6571 7565 7374 2c20 7365  nCodeRequest, se
+000342f0: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+00034300: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00034310: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034320: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00034330: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00034340: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00034350: 2020 2069 6620 7365 6c66 2e71 7561 6c69     if self.quali
+00034360: 6669 6572 2069 7320 6e6f 7420 4e6f 6e65  fier is not None
+00034370: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00034380: 7375 6c74 5b27 7175 616c 6966 6965 7227  sult['qualifier'
+00034390: 5d20 3d20 7365 6c66 2e71 7561 6c69 6669  ] = self.qualifi
+000343a0: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
+000343b0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000343c0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000343d0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+000343e0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000343f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00034400: 6574 2827 7175 616c 6966 6965 7227 2920  et('qualifier') 
+00034410: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00034420: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
+00034430: 616c 6966 6965 7220 3d20 6d2e 6765 7428  alifier = m.get(
+00034440: 2771 7561 6c69 6669 6572 2729 0a20 2020  'qualifier').   
+00034450: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00034460: 0a0a 0a63 6c61 7373 2047 6574 4675 6e63  ...class GetFunc
+00034470: 7469 6f6e 436f 6465 5265 7370 6f6e 7365  tionCodeResponse
+00034480: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00034490: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000344a0: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
+000344b0: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
+000344c0: 652c 2062 6f64 793d 4e6f 6e65 293a 0a20  e, body=None):. 
+000344d0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+000344e0: 6572 7320 3d20 6865 6164 6572 7320 2023  ers = headers  #
+000344f0: 2074 7970 653a 2064 6963 745b 7374 722c   type: dict[str,
+00034500: 2073 7472 5d0a 2020 2020 2020 2020 7365   str].        se
+00034510: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00034520: 2073 7461 7475 735f 636f 6465 2020 2320   status_code  # 
+00034530: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00034540: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+00034550: 6479 2020 2320 7479 7065 3a20 4f75 7470  dy  # type: Outp
+00034560: 7574 4675 6e63 436f 6465 0a0a 2020 2020  utFuncCode..    
+00034570: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00034580: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00034590: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+000345a0: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+000345b0: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+000345c0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000345d0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000345e0: 2073 7570 6572 2847 6574 4675 6e63 7469   super(GetFuncti
+000345f0: 6f6e 436f 6465 5265 7370 6f6e 7365 2c20  onCodeResponse, 
+00034600: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+00034610: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00034620: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00034630: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00034640: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00034650: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00034660: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00034670: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00034680: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00034690: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+000346a0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+000346b0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000346c0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+000346d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000346e0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+000346f0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+00034700: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00034710: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00034720: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00034730: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00034740: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00034750: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00034760: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00034770: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00034780: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00034790: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000347a0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000347b0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+000347c0: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+000347d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000347e0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+000347f0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00034800: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00034810: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00034820: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00034830: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00034840: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+00034850: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00034860: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00034870: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00034880: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00034890: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+000348a0: 4f75 7470 7574 4675 6e63 436f 6465 2829  OutputFuncCode()
+000348b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000348c0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+000348d0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+000348e0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+000348f0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00034900: 6173 7320 4765 744c 6179 6572 5665 7273  ass GetLayerVers
+00034910: 696f 6e52 6573 706f 6e73 6528 5465 614d  ionResponse(TeaM
+00034920: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00034930: 5f69 6e69 745f 5f28 7365 6c66 2c20 6865  _init__(self, he
+00034940: 6164 6572 733d 4e6f 6e65 2c20 7374 6174  aders=None, stat
+00034950: 7573 5f63 6f64 653d 4e6f 6e65 2c20 626f  us_code=None, bo
+00034960: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
+00034970: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00034980: 2068 6561 6465 7273 2020 2320 7479 7065   headers  # type
+00034990: 3a20 6469 6374 5b73 7472 2c20 7374 725d  : dict[str, str]
+000349a0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+000349b0: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+000349c0: 7573 5f63 6f64 6520 2023 2074 7970 653a  us_code  # type:
+000349d0: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
+000349e0: 662e 626f 6479 203d 2062 6f64 7920 2023  f.body = body  #
+000349f0: 2074 7970 653a 204c 6179 6572 0a0a 2020   type: Layer..  
+00034a00: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00034a10: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00034a20: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+00034a30: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00034a40: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+00034a50: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00034a60: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00034a70: 203d 2073 7570 6572 2847 6574 4c61 7965   = super(GetLaye
+00034a80: 7256 6572 7369 6f6e 5265 7370 6f6e 7365  rVersionResponse
+00034a90: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+00034aa0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00034ab0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00034ac0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00034ad0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00034ae0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00034af0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00034b00: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+00034b10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00034b20: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+00034b30: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+00034b40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00034b50: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+00034b60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034b70: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+00034b80: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+00034b90: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+00034ba0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00034bb0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+00034bc0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00034bd0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+00034be0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+00034bf0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00034c00: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00034c10: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+00034c20: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00034c30: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00034c40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00034c50: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+00034c60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00034c70: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00034c80: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+00034c90: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+00034ca0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00034cb0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00034cc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00034cd0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00034ce0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00034cf0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00034d00: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00034d10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00034d20: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+00034d30: 3d20 4c61 7965 7228 290a 2020 2020 2020  = Layer().      
+00034d40: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00034d50: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00034d60: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00034d70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00034d80: 7365 6c66 0a0a 0a63 6c61 7373 2047 6574  self...class Get
+00034d90: 4c61 7965 7256 6572 7369 6f6e 4279 4172  LayerVersionByAr
+00034da0: 6e52 6573 706f 6e73 6528 5465 614d 6f64  nResponse(TeaMod
+00034db0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00034dc0: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
+00034dd0: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
+00034de0: 5f63 6f64 653d 4e6f 6e65 2c20 626f 6479  _code=None, body
+00034df0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00034e00: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+00034e10: 6561 6465 7273 2020 2320 7479 7065 3a20  eaders  # type: 
+00034e20: 6469 6374 5b73 7472 2c20 7374 725d 0a20  dict[str, str]. 
+00034e30: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00034e40: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+00034e50: 5f63 6f64 6520 2023 2074 7970 653a 2069  _code  # type: i
+00034e60: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+00034e70: 626f 6479 203d 2062 6f64 7920 2023 2074  body = body  # t
+00034e80: 7970 653a 204c 6179 6572 0a0a 2020 2020  ype: Layer..    
+00034e90: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00034ea0: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00034eb0: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+00034ec0: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+00034ed0: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00034ee0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00034ef0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00034f00: 2073 7570 6572 2847 6574 4c61 7965 7256   super(GetLayerV
+00034f10: 6572 7369 6f6e 4279 4172 6e52 6573 706f  ersionByArnRespo
+00034f20: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
+00034f30: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00034f40: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00034f50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00034f60: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00034f70: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00034f80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00034f90: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+00034fa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00034fb0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+00034fc0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+00034fd0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+00034fe0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00034ff0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00035000: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00035010: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+00035020: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00035030: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00035040: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+00035050: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00035060: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+00035070: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+00035080: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00035090: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000350a0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000350b0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+000350c0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000350d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000350e0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+000350f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00035100: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00035110: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+00035120: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+00035130: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+00035140: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+00035150: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00035160: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00035170: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+00035180: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+00035190: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+000351a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000351b0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+000351c0: 656c 203d 204c 6179 6572 2829 0a20 2020  el = Layer().   
+000351d0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000351e0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+000351f0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+00035200: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+00035210: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00035220: 4765 7450 726f 7669 7369 6f6e 436f 6e66  GetProvisionConf
+00035230: 6967 5265 7175 6573 7428 5465 614d 6f64  igRequest(TeaMod
+00035240: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00035250: 6e69 745f 5f28 7365 6c66 2c20 7175 616c  nit__(self, qual
+00035260: 6966 6965 723d 4e6f 6e65 293a 0a20 2020  ifier=None):.   
+00035270: 2020 2020 2023 2054 6865 2066 756e 6374       # The funct
+00035280: 696f 6e20 616c 6961 7320 6f72 204c 4154  ion alias or LAT
+00035290: 4553 542e 0a20 2020 2020 2020 2073 656c  EST..        sel
+000352a0: 662e 7175 616c 6966 6965 7220 3d20 7175  f.qualifier = qu
+000352b0: 616c 6966 6965 7220 2023 2074 7970 653a  alifier  # type:
+000352c0: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
+000352d0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000352e0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000352f0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00035300: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00035310: 2073 7570 6572 2847 6574 5072 6f76 6973   super(GetProvis
+00035320: 696f 6e43 6f6e 6669 6752 6571 7565 7374  ionConfigRequest
+00035330: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+00035340: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00035350: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00035360: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00035370: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00035380: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00035390: 2020 2020 2020 2069 6620 7365 6c66 2e71         if self.q
+000353a0: 7561 6c69 6669 6572 2069 7320 6e6f 7420  ualifier is not 
+000353b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000353c0: 2020 7265 7375 6c74 5b27 7175 616c 6966    result['qualif
+000353d0: 6965 7227 5d20 3d20 7365 6c66 2e71 7561  ier'] = self.qua
+000353e0: 6c69 6669 6572 0a20 2020 2020 2020 2072  lifier.        r
+000353f0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00035400: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00035410: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+00035420: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00035430: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00035440: 206d 2e67 6574 2827 7175 616c 6966 6965   m.get('qualifie
+00035450: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
+00035460: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00035470: 662e 7175 616c 6966 6965 7220 3d20 6d2e  f.qualifier = m.
+00035480: 6765 7428 2771 7561 6c69 6669 6572 2729  get('qualifier')
+00035490: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000354a0: 7365 6c66 0a0a 0a63 6c61 7373 2047 6574  self...class Get
+000354b0: 5072 6f76 6973 696f 6e43 6f6e 6669 6752  ProvisionConfigR
+000354c0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+000354d0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000354e0: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
+000354f0: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
+00035500: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
+00035510: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+00035520: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+00035530: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
+00035540: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
+00035550: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00035560: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+00035570: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
+00035580: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+00035590: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
+000355a0: 653a 2050 726f 7669 7369 6f6e 436f 6e66  e: ProvisionConf
+000355b0: 6967 0a0a 2020 2020 6465 6620 7661 6c69  ig..    def vali
+000355c0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000355d0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000355e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000355f0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00035600: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00035610: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00035620: 2020 5f6d 6170 203d 2073 7570 6572 2847    _map = super(G
+00035630: 6574 5072 6f76 6973 696f 6e43 6f6e 6669  etProvisionConfi
+00035640: 6752 6573 706f 6e73 652c 2073 656c 6629  gResponse, self)
+00035650: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00035660: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00035670: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00035680: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00035690: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000356a0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000356b0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+000356c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000356d0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000356e0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+000356f0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00035700: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00035710: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00035720: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00035730: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00035740: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00035750: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00035760: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00035770: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00035780: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00035790: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+000357a0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000357b0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000357c0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000357d0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+000357e0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000357f0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00035800: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00035810: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00035820: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00035830: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00035840: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00035850: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+00035860: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+00035870: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00035880: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00035890: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+000358a0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+000358b0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+000358c0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+000358d0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+000358e0: 6d70 5f6d 6f64 656c 203d 2050 726f 7669  mp_model = Provi
+000358f0: 7369 6f6e 436f 6e66 6967 2829 0a20 2020  sionConfig().   
+00035900: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00035910: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+00035920: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+00035930: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+00035940: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00035950: 4765 7454 7269 6767 6572 5265 7370 6f6e  GetTriggerRespon
+00035960: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00035970: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00035980: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
+00035990: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
+000359a0: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
+000359b0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000359c0: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
+000359d0: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
+000359e0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
+000359f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00035a00: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
+00035a10: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
+00035a20: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00035a30: 626f 6479 2020 2320 7479 7065 3a20 5472  body  # type: Tr
+00035a40: 6967 6765 720a 0a20 2020 2064 6566 2076  igger..    def v
+00035a50: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00035a60: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00035a70: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+00035a80: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+00035a90: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+00035aa0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00035ab0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00035ac0: 7228 4765 7454 7269 6767 6572 5265 7370  r(GetTriggerResp
+00035ad0: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
+00035ae0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00035af0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00035b00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00035b10: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00035b20: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00035b30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00035b40: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00035b50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035b60: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00035b70: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00035b80: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+00035b90: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00035ba0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00035bb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00035bc0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+00035bd0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00035be0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00035bf0: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+00035c00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00035c10: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+00035c20: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+00035c30: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+00035c40: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00035c50: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00035c60: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00035c70: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00035c80: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00035c90: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+00035ca0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00035cb0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00035cc0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+00035cd0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+00035ce0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+00035cf0: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+00035d00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00035d10: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00035d20: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+00035d30: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
+00035d40: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
+00035d50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00035d60: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00035d70: 6465 6c20 3d20 5472 6967 6765 7228 290a  del = Trigger().
+00035d80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00035d90: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+00035da0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+00035db0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+00035dc0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00035dd0: 7373 2049 6e76 6f6b 6546 756e 6374 696f  ss InvokeFunctio
+00035de0: 6e48 6561 6465 7273 2854 6561 4d6f 6465  nHeaders(TeaMode
+00035df0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00035e00: 6974 5f5f 2873 656c 662c 2063 6f6d 6d6f  it__(self, commo
+00035e10: 6e5f 6865 6164 6572 733d 4e6f 6e65 2c20  n_headers=None, 
+00035e20: 785f 6663 5f61 7379 6e63 5f74 6173 6b5f  x_fc_async_task_
+00035e30: 6964 3d4e 6f6e 652c 2078 5f66 635f 696e  id=None, x_fc_in
+00035e40: 766f 6361 7469 6f6e 5f74 7970 653d 4e6f  vocation_type=No
+00035e50: 6e65 2c20 785f 6663 5f6c 6f67 5f74 7970  ne, x_fc_log_typ
+00035e60: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
+00035e70: 2073 656c 662e 636f 6d6d 6f6e 5f68 6561   self.common_hea
+00035e80: 6465 7273 203d 2063 6f6d 6d6f 6e5f 6865  ders = common_he
+00035e90: 6164 6572 7320 2023 2074 7970 653a 2064  aders  # type: d
+00035ea0: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
+00035eb0: 2020 2020 2020 7365 6c66 2e78 5f66 635f        self.x_fc_
+00035ec0: 6173 796e 635f 7461 736b 5f69 6420 3d20  async_task_id = 
+00035ed0: 785f 6663 5f61 7379 6e63 5f74 6173 6b5f  x_fc_async_task_
+00035ee0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+00035ef0: 2020 2020 2020 2020 2320 5468 6520 7479          # The ty
+00035f00: 7065 206f 6620 6675 6e63 7469 6f6e 2069  pe of function i
+00035f10: 6e76 6f63 6174 696f 6e2e 2056 616c 6964  nvocation. Valid
+00035f20: 2076 616c 7565 733a 2053 796e 6320 616e   values: Sync an
+00035f30: 6420 4173 796e 632e 0a20 2020 2020 2020  d Async..       
+00035f40: 2073 656c 662e 785f 6663 5f69 6e76 6f63   self.x_fc_invoc
+00035f50: 6174 696f 6e5f 7479 7065 203d 2078 5f66  ation_type = x_f
+00035f60: 635f 696e 766f 6361 7469 6f6e 5f74 7970  c_invocation_typ
+00035f70: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
+00035f80: 2020 2020 2020 2023 2054 6865 206c 6f67         # The log
+00035f90: 2074 7970 6520 6f66 2066 756e 6374 696f   type of functio
+00035fa0: 6e20 696e 766f 6361 7469 6f6e 2e20 5661  n invocation. Va
+00035fb0: 6c69 6420 7661 6c75 6573 3a20 4e6f 6e65  lid values: None
+00035fc0: 2061 6e64 2054 6169 6c2e 0a20 2020 2020   and Tail..     
+00035fd0: 2020 2073 656c 662e 785f 6663 5f6c 6f67     self.x_fc_log
+00035fe0: 5f74 7970 6520 3d20 785f 6663 5f6c 6f67  _type = x_fc_log
+00035ff0: 5f74 7970 6520 2023 2074 7970 653a 2073  _type  # type: s
+00036000: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
+00036010: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00036020: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00036030: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00036040: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00036050: 7570 6572 2849 6e76 6f6b 6546 756e 6374  uper(InvokeFunct
+00036060: 696f 6e48 6561 6465 7273 2c20 7365 6c66  ionHeaders, self
+00036070: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00036080: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00036090: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000360a0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000360b0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000360c0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000360d0: 2069 6620 7365 6c66 2e63 6f6d 6d6f 6e5f   if self.common_
+000360e0: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+000360f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00036100: 2072 6573 756c 745b 2763 6f6d 6d6f 6e48   result['commonH
+00036110: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+00036120: 636f 6d6d 6f6e 5f68 6561 6465 7273 0a20  common_headers. 
+00036130: 2020 2020 2020 2069 6620 7365 6c66 2e78         if self.x
+00036140: 5f66 635f 6173 796e 635f 7461 736b 5f69  _fc_async_task_i
+00036150: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00036160: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00036170: 745b 2778 2d66 632d 6173 796e 632d 7461  t['x-fc-async-ta
+00036180: 736b 2d69 6427 5d20 3d20 7365 6c66 2e78  sk-id'] = self.x
+00036190: 5f66 635f 6173 796e 635f 7461 736b 5f69  _fc_async_task_i
+000361a0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+000361b0: 662e 785f 6663 5f69 6e76 6f63 6174 696f  f.x_fc_invocatio
+000361c0: 6e5f 7479 7065 2069 7320 6e6f 7420 4e6f  n_type is not No
+000361d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000361e0: 7265 7375 6c74 5b27 782d 6663 2d69 6e76  result['x-fc-inv
+000361f0: 6f63 6174 696f 6e2d 7479 7065 275d 203d  ocation-type'] =
+00036200: 2073 656c 662e 785f 6663 5f69 6e76 6f63   self.x_fc_invoc
+00036210: 6174 696f 6e5f 7479 7065 0a20 2020 2020  ation_type.     
+00036220: 2020 2069 6620 7365 6c66 2e78 5f66 635f     if self.x_fc_
+00036230: 6c6f 675f 7479 7065 2069 7320 6e6f 7420  log_type is not 
+00036240: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00036250: 2020 7265 7375 6c74 5b27 782d 6663 2d6c    result['x-fc-l
+00036260: 6f67 2d74 7970 6527 5d20 3d20 7365 6c66  og-type'] = self
+00036270: 2e78 5f66 635f 6c6f 675f 7479 7065 0a20  .x_fc_log_type. 
+00036280: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00036290: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000362a0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+000362b0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+000362c0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+000362d0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000362e0: 636f 6d6d 6f6e 4865 6164 6572 7327 2920  commonHeaders') 
+000362f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00036300: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00036310: 6d6d 6f6e 5f68 6561 6465 7273 203d 206d  mmon_headers = m
+00036320: 2e67 6574 2827 636f 6d6d 6f6e 4865 6164  .get('commonHead
+00036330: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+00036340: 206d 2e67 6574 2827 782d 6663 2d61 7379   m.get('x-fc-asy
+00036350: 6e63 2d74 6173 6b2d 6964 2729 2069 7320  nc-task-id') is 
+00036360: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00036370: 2020 2020 2020 7365 6c66 2e78 5f66 635f        self.x_fc_
+00036380: 6173 796e 635f 7461 736b 5f69 6420 3d20  async_task_id = 
+00036390: 6d2e 6765 7428 2778 2d66 632d 6173 796e  m.get('x-fc-asyn
+000363a0: 632d 7461 736b 2d69 6427 290a 2020 2020  c-task-id').    
+000363b0: 2020 2020 6966 206d 2e67 6574 2827 782d      if m.get('x-
+000363c0: 6663 2d69 6e76 6f63 6174 696f 6e2d 7479  fc-invocation-ty
+000363d0: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
+000363e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000363f0: 6c66 2e78 5f66 635f 696e 766f 6361 7469  lf.x_fc_invocati
+00036400: 6f6e 5f74 7970 6520 3d20 6d2e 6765 7428  on_type = m.get(
+00036410: 2778 2d66 632d 696e 766f 6361 7469 6f6e  'x-fc-invocation
+00036420: 2d74 7970 6527 290a 2020 2020 2020 2020  -type').        
+00036430: 6966 206d 2e67 6574 2827 782d 6663 2d6c  if m.get('x-fc-l
+00036440: 6f67 2d74 7970 6527 2920 6973 206e 6f74  og-type') is not
+00036450: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00036460: 2020 2073 656c 662e 785f 6663 5f6c 6f67     self.x_fc_log
+00036470: 5f74 7970 6520 3d20 6d2e 6765 7428 2778  _type = m.get('x
+00036480: 2d66 632d 6c6f 672d 7479 7065 2729 0a20  -fc-log-type'). 
+00036490: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000364a0: 6c66 0a0a 0a63 6c61 7373 2049 6e76 6f6b  lf...class Invok
+000364b0: 6546 756e 6374 696f 6e52 6571 7565 7374  eFunctionRequest
+000364c0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000364d0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000364e0: 662c 2062 6f64 793d 4e6f 6e65 2c20 7175  f, body=None, qu
+000364f0: 616c 6966 6965 723d 4e6f 6e65 293a 0a20  alifier=None):. 
+00036500: 2020 2020 2020 2023 2054 6865 2072 6571         # The req
+00036510: 7565 7374 2070 6172 616d 6574 6572 7320  uest parameters 
+00036520: 6f66 2066 756e 6374 696f 6e20 696e 766f  of function invo
+00036530: 6361 7469 6f6e 2e0a 2020 2020 2020 2020  cation..        
+00036540: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00036550: 2020 2320 7479 7065 3a20 5245 4144 4142    # type: READAB
+00036560: 4c45 0a20 2020 2020 2020 2023 2054 6865  LE.        # The
+00036570: 2076 6572 7369 6f6e 206f 7220 616c 6961   version or alia
+00036580: 7320 6f66 2074 6865 2066 756e 6374 696f  s of the functio
+00036590: 6e2e 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+000365a0: 7175 616c 6966 6965 7220 3d20 7175 616c  qualifier = qual
+000365b0: 6966 6965 7220 2023 2074 7970 653a 2073  ifier  # type: s
+000365c0: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
+000365d0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000365e0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000365f0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00036600: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00036610: 7570 6572 2849 6e76 6f6b 6546 756e 6374  uper(InvokeFunct
+00036620: 696f 6e52 6571 7565 7374 2c20 7365 6c66  ionRequest, self
+00036630: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00036640: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00036650: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00036660: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00036670: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00036680: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00036690: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+000366a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000366b0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+000366c0: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+000366d0: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
+000366e0: 662e 7175 616c 6966 6965 7220 6973 206e  f.qualifier is n
+000366f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00036700: 2020 2020 2072 6573 756c 745b 2771 7561       result['qua
+00036710: 6c69 6669 6572 275d 203d 2073 656c 662e  lifier'] = self.
+00036720: 7175 616c 6966 6965 720a 2020 2020 2020  qualifier.      
+00036730: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00036740: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00036750: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00036760: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00036770: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00036780: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+00036790: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000367a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000367b0: 626f 6479 203d 206d 2e67 6574 2827 626f  body = m.get('bo
+000367c0: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
+000367d0: 6d2e 6765 7428 2771 7561 6c69 6669 6572  m.get('qualifier
+000367e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000367f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00036800: 2e71 7561 6c69 6669 6572 203d 206d 2e67  .qualifier = m.g
+00036810: 6574 2827 7175 616c 6966 6965 7227 290a  et('qualifier').
+00036820: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00036830: 656c 660a 0a0a 636c 6173 7320 496e 766f  elf...class Invo
+00036840: 6b65 4675 6e63 7469 6f6e 5265 7370 6f6e  keFunctionRespon
+00036850: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00036860: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00036870: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
+00036880: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
+00036890: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
+000368a0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000368b0: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
+000368c0: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
+000368d0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
+000368e0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000368f0: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
+00036900: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
+00036910: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00036920: 626f 6479 2020 2320 7479 7065 3a20 5245  body  # type: RE
+00036930: 4144 4142 4c45 0a0a 2020 2020 6465 6620  ADABLE..    def 
+00036940: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00036950: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00036960: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00036970: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00036980: 203d 2073 7570 6572 2849 6e76 6f6b 6546   = super(InvokeF
+00036990: 756e 6374 696f 6e52 6573 706f 6e73 652c  unctionResponse,
+000369a0: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+000369b0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000369c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000369d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000369e0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000369f0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00036a00: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+00036a10: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+00036a20: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00036a30: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+00036a40: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+00036a50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00036a60: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+00036a70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00036a80: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+00036a90: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+00036aa0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+00036ab0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00036ac0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+00036ad0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00036ae0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+00036af0: 2e62 6f64 790a 2020 2020 2020 2020 7265  .body.        re
+00036b00: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00036b10: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00036b20: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+00036b30: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00036b40: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00036b50: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00036b60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00036b70: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00036b80: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+00036b90: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00036ba0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+00036bb0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+00036bc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00036bd0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00036be0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+00036bf0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+00036c00: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+00036c10: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00036c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00036c30: 626f 6479 203d 206d 2e67 6574 2827 626f  body = m.get('bo
+00036c40: 6479 2729 0a20 2020 2020 2020 2072 6574  dy').        ret
+00036c50: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00036c60: 204c 6973 7441 6c69 6173 6573 5265 7175   ListAliasesRequ
+00036c70: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+00036c80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00036c90: 7365 6c66 2c20 6c69 6d69 743d 4e6f 6e65  self, limit=None
+00036ca0: 2c20 6e65 7874 5f74 6f6b 656e 3d4e 6f6e  , next_token=Non
+00036cb0: 652c 2070 7265 6669 783d 4e6f 6e65 293a  e, prefix=None):
+00036cc0: 0a20 2020 2020 2020 2023 2054 6865 206e  .        # The n
+00036cd0: 756d 6265 7220 6f66 2061 6c69 6173 6573  umber of aliases
+00036ce0: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
+00036cf0: 2020 2073 656c 662e 6c69 6d69 7420 3d20     self.limit = 
+00036d00: 6c69 6d69 7420 2023 2074 7970 653a 2069  limit  # type: i
+00036d10: 6e74 0a20 2020 2020 2020 2023 2054 6865  nt.        # The
+00036d20: 2070 6167 696e 6174 696f 6e20 746f 6b65   pagination toke
+00036d30: 6e20 7468 6174 2069 7320 7573 6564 2069  n that is used i
+00036d40: 6e20 7468 6520 6e65 7874 2072 6571 7565  n the next reque
+00036d50: 7374 2074 6f20 7265 7472 6965 7665 2061  st to retrieve a
+00036d60: 206e 6577 2070 6167 6520 6f66 2072 6573   new page of res
+00036d70: 756c 7473 2e0a 2020 2020 2020 2020 7365  ults..        se
+00036d80: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
+00036d90: 6e65 7874 5f74 6f6b 656e 2020 2320 7479  next_token  # ty
+00036da0: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+00036db0: 2320 5468 6520 616c 6961 7320 7072 6566  # The alias pref
+00036dc0: 6978 2e0a 2020 2020 2020 2020 7365 6c66  ix..        self
+00036dd0: 2e70 7265 6669 7820 3d20 7072 6566 6978  .prefix = prefix
+00036de0: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+00036df0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00036e00: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00036e10: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00036e20: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00036e30: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00036e40: 4c69 7374 416c 6961 7365 7352 6571 7565  ListAliasesReque
+00036e50: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
+00036e60: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00036e70: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00036e80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00036e90: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00036ea0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00036eb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00036ec0: 2e6c 696d 6974 2069 7320 6e6f 7420 4e6f  .limit is not No
+00036ed0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00036ee0: 7265 7375 6c74 5b27 6c69 6d69 7427 5d20  result['limit'] 
+00036ef0: 3d20 7365 6c66 2e6c 696d 6974 0a20 2020  = self.limit.   
+00036f00: 2020 2020 2069 6620 7365 6c66 2e6e 6578       if self.nex
+00036f10: 745f 746f 6b65 6e20 6973 206e 6f74 204e  t_token is not N
+00036f20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00036f30: 2072 6573 756c 745b 276e 6578 7454 6f6b   result['nextTok
+00036f40: 656e 275d 203d 2073 656c 662e 6e65 7874  en'] = self.next
+00036f50: 5f74 6f6b 656e 0a20 2020 2020 2020 2069  _token.        i
+00036f60: 6620 7365 6c66 2e70 7265 6669 7820 6973  f self.prefix is
+00036f70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00036f80: 2020 2020 2020 2072 6573 756c 745b 2770         result['p
+00036f90: 7265 6669 7827 5d20 3d20 7365 6c66 2e70  refix'] = self.p
+00036fa0: 7265 6669 780a 2020 2020 2020 2020 7265  refix.        re
+00036fb0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00036fc0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00036fd0: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+00036fe0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00036ff0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00037000: 6d2e 6765 7428 276c 696d 6974 2729 2069  m.get('limit') i
+00037010: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00037020: 2020 2020 2020 2020 7365 6c66 2e6c 696d          self.lim
+00037030: 6974 203d 206d 2e67 6574 2827 6c69 6d69  it = m.get('limi
+00037040: 7427 290a 2020 2020 2020 2020 6966 206d  t').        if m
+00037050: 2e67 6574 2827 6e65 7874 546f 6b65 6e27  .get('nextToken'
+00037060: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00037070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00037080: 6e65 7874 5f74 6f6b 656e 203d 206d 2e67  next_token = m.g
+00037090: 6574 2827 6e65 7874 546f 6b65 6e27 290a  et('nextToken').
+000370a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000370b0: 2827 7072 6566 6978 2729 2069 7320 6e6f  ('prefix') is no
+000370c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000370d0: 2020 2020 7365 6c66 2e70 7265 6669 7820      self.prefix 
+000370e0: 3d20 6d2e 6765 7428 2770 7265 6669 7827  = m.get('prefix'
+000370f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00037100: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
+00037110: 7374 416c 6961 7365 7352 6573 706f 6e73  stAliasesRespons
+00037120: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+00037130: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00037140: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
+00037150: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
+00037160: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
+00037170: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00037180: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
+00037190: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
+000371a0: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
+000371b0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+000371c0: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
+000371d0: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
+000371e0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+000371f0: 6f64 7920 2023 2074 7970 653a 204c 6973  ody  # type: Lis
+00037200: 7441 6c69 6173 6573 4f75 7470 7574 0a0a  tAliasesOutput..
+00037210: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00037220: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00037230: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00037240: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00037250: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00037260: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00037270: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00037280: 6170 203d 2073 7570 6572 284c 6973 7441  ap = super(ListA
+00037290: 6c69 6173 6573 5265 7370 6f6e 7365 2c20  liasesResponse, 
+000372a0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+000372b0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000372c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000372d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000372e0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000372f0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00037300: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00037310: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00037320: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00037330: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+00037340: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+00037350: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00037360: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+00037370: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00037380: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+00037390: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+000373a0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+000373b0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000373c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000373d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000373e0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+000373f0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00037400: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00037410: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00037420: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00037430: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00037440: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00037450: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+00037460: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+00037470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00037480: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00037490: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+000374a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000374b0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000374c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000374d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000374e0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+000374f0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00037500: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00037510: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00037520: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00037530: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00037540: 4c69 7374 416c 6961 7365 734f 7574 7075  ListAliasesOutpu
+00037550: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00037560: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+00037570: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+00037580: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+00037590: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+000375a0: 0a63 6c61 7373 204c 6973 7441 7379 6e63  .class ListAsync
+000375b0: 496e 766f 6b65 436f 6e66 6967 7352 6571  InvokeConfigsReq
+000375c0: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+000375d0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000375e0: 2873 656c 662c 2066 756e 6374 696f 6e5f  (self, function_
+000375f0: 6e61 6d65 3d4e 6f6e 652c 206c 696d 6974  name=None, limit
+00037600: 3d4e 6f6e 652c 206e 6578 745f 746f 6b65  =None, next_toke
+00037610: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+00037620: 2023 2054 6865 2066 756e 6374 696f 6e20   # The function 
+00037630: 6e61 6d65 2e20 4966 2079 6f75 2064 6f20  name. If you do 
+00037640: 6e6f 7420 636f 6e66 6967 7572 6520 7468  not configure th
+00037650: 6973 2070 6172 616d 6574 6572 2c20 7468  is parameter, th
+00037660: 6520 6173 796e 6368 726f 6e6f 7573 2069  e asynchronous i
+00037670: 6e76 6f63 6174 696f 6e20 636f 6e66 6967  nvocation config
+00037680: 7572 6174 696f 6e73 206f 6620 616c 6c20  urations of all 
+00037690: 6675 6e63 7469 6f6e 7320 6172 6520 6469  functions are di
+000376a0: 7370 6c61 7965 642e 0a20 2020 2020 2020  splayed..       
+000376b0: 2073 656c 662e 6675 6e63 7469 6f6e 5f6e   self.function_n
+000376c0: 616d 6520 3d20 6675 6e63 7469 6f6e 5f6e  ame = function_n
+000376d0: 616d 6520 2023 2074 7970 653a 2073 7472  ame  # type: str
+000376e0: 0a20 2020 2020 2020 2023 2054 6865 206d  .        # The m
+000376f0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00037700: 2065 6e74 7269 6573 2074 6f20 6265 2072   entries to be r
+00037710: 6574 7572 6e65 642e 0a20 2020 2020 2020  eturned..       
+00037720: 2073 656c 662e 6c69 6d69 7420 3d20 6c69   self.limit = li
+00037730: 6d69 7420 2023 2074 7970 653a 2069 6e74  mit  # type: int
+00037740: 0a20 2020 2020 2020 2023 2054 6865 2070  .        # The p
+00037750: 6167 696e 6720 696e 666f 726d 6174 696f  aging informatio
+00037760: 6e2e 2054 6869 7320 7061 7261 6d65 7465  n. This paramete
+00037770: 7220 7370 6563 6966 6965 7320 7468 6520  r specifies the 
+00037780: 7374 6172 7420 706f 696e 7420 6f66 2074  start point of t
+00037790: 6865 2071 7565 7279 2e0a 2020 2020 2020  he query..      
+000377a0: 2020 7365 6c66 2e6e 6578 745f 746f 6b65    self.next_toke
+000377b0: 6e20 3d20 6e65 7874 5f74 6f6b 656e 2020  n = next_token  
+000377c0: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
+000377d0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000377e0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000377f0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00037800: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00037810: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
+00037820: 7374 4173 796e 6349 6e76 6f6b 6543 6f6e  stAsyncInvokeCon
+00037830: 6669 6773 5265 7175 6573 742c 2073 656c  figsRequest, sel
+00037840: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+00037850: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00037860: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00037870: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00037880: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00037890: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000378a0: 2020 6966 2073 656c 662e 6675 6e63 7469    if self.functi
+000378b0: 6f6e 5f6e 616d 6520 6973 206e 6f74 204e  on_name is not N
+000378c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000378d0: 2072 6573 756c 745b 2766 756e 6374 696f   result['functio
+000378e0: 6e4e 616d 6527 5d20 3d20 7365 6c66 2e66  nName'] = self.f
+000378f0: 756e 6374 696f 6e5f 6e61 6d65 0a20 2020  unction_name.   
+00037900: 2020 2020 2069 6620 7365 6c66 2e6c 696d       if self.lim
+00037910: 6974 2069 7320 6e6f 7420 4e6f 6e65 3a0a  it is not None:.
+00037920: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00037930: 6c74 5b27 6c69 6d69 7427 5d20 3d20 7365  lt['limit'] = se
+00037940: 6c66 2e6c 696d 6974 0a20 2020 2020 2020  lf.limit.       
+00037950: 2069 6620 7365 6c66 2e6e 6578 745f 746f   if self.next_to
+00037960: 6b65 6e20 6973 206e 6f74 204e 6f6e 653a  ken is not None:
+00037970: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00037980: 756c 745b 276e 6578 7454 6f6b 656e 275d  ult['nextToken']
+00037990: 203d 2073 656c 662e 6e65 7874 5f74 6f6b   = self.next_tok
+000379a0: 656e 0a20 2020 2020 2020 2072 6574 7572  en.        retur
+000379b0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000379c0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000379d0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+000379e0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000379f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00037a00: 6574 2827 6675 6e63 7469 6f6e 4e61 6d65  et('functionName
+00037a10: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00037a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00037a30: 2e66 756e 6374 696f 6e5f 6e61 6d65 203d  .function_name =
+00037a40: 206d 2e67 6574 2827 6675 6e63 7469 6f6e   m.get('function
+00037a50: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
+00037a60: 6620 6d2e 6765 7428 276c 696d 6974 2729  f m.get('limit')
+00037a70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00037a80: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00037a90: 696d 6974 203d 206d 2e67 6574 2827 6c69  imit = m.get('li
+00037aa0: 6d69 7427 290a 2020 2020 2020 2020 6966  mit').        if
+00037ab0: 206d 2e67 6574 2827 6e65 7874 546f 6b65   m.get('nextToke
+00037ac0: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+00037ad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00037ae0: 662e 6e65 7874 5f74 6f6b 656e 203d 206d  f.next_token = m
+00037af0: 2e67 6574 2827 6e65 7874 546f 6b65 6e27  .get('nextToken'
+00037b00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00037b10: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
+00037b20: 7374 4173 796e 6349 6e76 6f6b 6543 6f6e  stAsyncInvokeCon
+00037b30: 6669 6773 5265 7370 6f6e 7365 2854 6561  figsResponse(Tea
+00037b40: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00037b50: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
+00037b60: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
+00037b70: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
+00037b80: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
+00037b90: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+00037ba0: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
+00037bb0: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
+00037bc0: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
+00037bd0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+00037be0: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
+00037bf0: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+00037c00: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
+00037c10: 2320 7479 7065 3a20 4c69 7374 4173 796e  # type: ListAsyn
+00037c20: 6349 6e76 6f6b 6543 6f6e 6669 674f 7574  cInvokeConfigOut
+00037c30: 7075 740a 0a20 2020 2064 6566 2076 616c  put..    def val
+00037c40: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00037c50: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00037c60: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00037c70: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00037c80: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00037c90: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00037ca0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00037cb0: 4c69 7374 4173 796e 6349 6e76 6f6b 6543  ListAsyncInvokeC
+00037cc0: 6f6e 6669 6773 5265 7370 6f6e 7365 2c20  onfigsResponse, 
+00037cd0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+00037ce0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00037cf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00037d00: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00037d10: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00037d20: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00037d30: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00037d40: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00037d50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00037d60: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+00037d70: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+00037d80: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00037d90: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+00037da0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00037db0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+00037dc0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+00037dd0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00037de0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00037df0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00037e00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00037e10: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00037e20: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00037e30: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00037e40: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00037e50: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00037e60: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00037e70: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00037e80: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+00037e90: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+00037ea0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00037eb0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00037ec0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00037ed0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00037ee0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00037ef0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00037f00: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00037f10: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+00037f20: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00037f30: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00037f40: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00037f50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00037f60: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00037f70: 4c69 7374 4173 796e 6349 6e76 6f6b 6543  ListAsyncInvokeC
+00037f80: 6f6e 6669 674f 7574 7075 7428 290a 2020  onfigOutput().  
+00037f90: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00037fa0: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+00037fb0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+00037fc0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+00037fd0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00037fe0: 204c 6973 7441 7379 6e63 5461 736b 7352   ListAsyncTasksR
+00037ff0: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+00038000: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00038010: 5f5f 2873 656c 662c 2069 6e63 6c75 6465  __(self, include
+00038020: 5f70 6179 6c6f 6164 3d4e 6f6e 652c 206c  _payload=None, l
+00038030: 696d 6974 3d4e 6f6e 652c 206e 6578 745f  imit=None, next_
+00038040: 746f 6b65 6e3d 4e6f 6e65 2c20 7072 6566  token=None, pref
+00038050: 6978 3d4e 6f6e 652c 2071 7561 6c69 6669  ix=None, qualifi
+00038060: 6572 3d4e 6f6e 652c 0a20 2020 2020 2020  er=None,.       
+00038070: 2020 2020 2020 2020 2020 736f 7274 5f6f            sort_o
+00038080: 7264 6572 5f62 795f 7469 6d65 3d4e 6f6e  rder_by_time=Non
+00038090: 652c 2073 7461 7274 6564 5f74 696d 655f  e, started_time_
+000380a0: 6265 6769 6e3d 4e6f 6e65 2c20 7374 6172  begin=None, star
+000380b0: 7465 645f 7469 6d65 5f65 6e64 3d4e 6f6e  ted_time_end=Non
+000380c0: 652c 2073 7461 7475 733d 4e6f 6e65 293a  e, status=None):
+000380d0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+000380e0: 636c 7564 655f 7061 796c 6f61 6420 3d20  clude_payload = 
+000380f0: 696e 636c 7564 655f 7061 796c 6f61 6420  include_payload 
+00038100: 2023 2074 7970 653a 2062 6f6f 6c0a 2020   # type: bool.  
+00038110: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
+00038120: 203d 206c 696d 6974 2020 2320 7479 7065   = limit  # type
+00038130: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+00038140: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
+00038150: 6e65 7874 5f74 6f6b 656e 2020 2320 7479  next_token  # ty
+00038160: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+00038170: 7365 6c66 2e70 7265 6669 7820 3d20 7072  self.prefix = pr
+00038180: 6566 6978 2020 2320 7479 7065 3a20 7374  efix  # type: st
+00038190: 720a 2020 2020 2020 2020 7365 6c66 2e71  r.        self.q
+000381a0: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
+000381b0: 6669 6572 2020 2320 7479 7065 3a20 7374  fier  # type: st
+000381c0: 720a 2020 2020 2020 2020 7365 6c66 2e73  r.        self.s
+000381d0: 6f72 745f 6f72 6465 725f 6279 5f74 696d  ort_order_by_tim
+000381e0: 6520 3d20 736f 7274 5f6f 7264 6572 5f62  e = sort_order_b
+000381f0: 795f 7469 6d65 2020 2320 7479 7065 3a20  y_time  # type: 
+00038200: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00038210: 2e73 7461 7274 6564 5f74 696d 655f 6265  .started_time_be
+00038220: 6769 6e20 3d20 7374 6172 7465 645f 7469  gin = started_ti
+00038230: 6d65 5f62 6567 696e 2020 2320 7479 7065  me_begin  # type
+00038240: 3a20 6c6f 6e67 0a20 2020 2020 2020 2073  : long.        s
+00038250: 656c 662e 7374 6172 7465 645f 7469 6d65  elf.started_time
+00038260: 5f65 6e64 203d 2073 7461 7274 6564 5f74  _end = started_t
+00038270: 696d 655f 656e 6420 2023 2074 7970 653a  ime_end  # type:
+00038280: 206c 6f6e 670a 2020 2020 2020 2020 7365   long.        se
+00038290: 6c66 2e73 7461 7475 7320 3d20 7374 6174  lf.status = stat
+000382a0: 7573 2020 2320 7479 7065 3a20 7374 720a  us  # type: str.
+000382b0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000382c0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000382d0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+000382e0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+000382f0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00038300: 7228 4c69 7374 4173 796e 6354 6173 6b73  r(ListAsyncTasks
+00038310: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
+00038320: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00038330: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00038340: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00038350: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00038360: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00038370: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00038380: 2073 656c 662e 696e 636c 7564 655f 7061   self.include_pa
+00038390: 796c 6f61 6420 6973 206e 6f74 204e 6f6e  yload is not Non
+000383a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000383b0: 6573 756c 745b 2769 6e63 6c75 6465 5061  esult['includePa
+000383c0: 796c 6f61 6427 5d20 3d20 7365 6c66 2e69  yload'] = self.i
+000383d0: 6e63 6c75 6465 5f70 6179 6c6f 6164 0a20  nclude_payload. 
+000383e0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+000383f0: 696d 6974 2069 7320 6e6f 7420 4e6f 6e65  imit is not None
+00038400: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00038410: 7375 6c74 5b27 6c69 6d69 7427 5d20 3d20  sult['limit'] = 
+00038420: 7365 6c66 2e6c 696d 6974 0a20 2020 2020  self.limit.     
+00038430: 2020 2069 6620 7365 6c66 2e6e 6578 745f     if self.next_
+00038440: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+00038450: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00038460: 6573 756c 745b 276e 6578 7454 6f6b 656e  esult['nextToken
+00038470: 275d 203d 2073 656c 662e 6e65 7874 5f74  '] = self.next_t
+00038480: 6f6b 656e 0a20 2020 2020 2020 2069 6620  oken.        if 
+00038490: 7365 6c66 2e70 7265 6669 7820 6973 206e  self.prefix is n
+000384a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000384b0: 2020 2020 2072 6573 756c 745b 2770 7265       result['pre
+000384c0: 6669 7827 5d20 3d20 7365 6c66 2e70 7265  fix'] = self.pre
+000384d0: 6669 780a 2020 2020 2020 2020 6966 2073  fix.        if s
+000384e0: 656c 662e 7175 616c 6966 6965 7220 6973  elf.qualifier is
+000384f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038500: 2020 2020 2020 2072 6573 756c 745b 2771         result['q
+00038510: 7561 6c69 6669 6572 275d 203d 2073 656c  ualifier'] = sel
+00038520: 662e 7175 616c 6966 6965 720a 2020 2020  f.qualifier.    
+00038530: 2020 2020 6966 2073 656c 662e 736f 7274      if self.sort
+00038540: 5f6f 7264 6572 5f62 795f 7469 6d65 2069  _order_by_time i
+00038550: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00038560: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00038570: 736f 7274 4f72 6465 7242 7954 696d 6527  sortOrderByTime'
+00038580: 5d20 3d20 7365 6c66 2e73 6f72 745f 6f72  ] = self.sort_or
+00038590: 6465 725f 6279 5f74 696d 650a 2020 2020  der_by_time.    
+000385a0: 2020 2020 6966 2073 656c 662e 7374 6172      if self.star
+000385b0: 7465 645f 7469 6d65 5f62 6567 696e 2069  ted_time_begin i
+000385c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000385d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000385e0: 7374 6172 7465 6454 696d 6542 6567 696e  startedTimeBegin
+000385f0: 275d 203d 2073 656c 662e 7374 6172 7465  '] = self.starte
+00038600: 645f 7469 6d65 5f62 6567 696e 0a20 2020  d_time_begin.   
+00038610: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+00038620: 7274 6564 5f74 696d 655f 656e 6420 6973  rted_time_end is
+00038630: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038640: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00038650: 7461 7274 6564 5469 6d65 456e 6427 5d20  tartedTimeEnd'] 
+00038660: 3d20 7365 6c66 2e73 7461 7274 6564 5f74  = self.started_t
+00038670: 696d 655f 656e 640a 2020 2020 2020 2020  ime_end.        
+00038680: 6966 2073 656c 662e 7374 6174 7573 2069  if self.status i
+00038690: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000386a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000386b0: 7374 6174 7573 275d 203d 2073 656c 662e  status'] = self.
+000386c0: 7374 6174 7573 0a20 2020 2020 2020 2072  status.        r
+000386d0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+000386e0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+000386f0: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+00038700: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00038710: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00038720: 206d 2e67 6574 2827 696e 636c 7564 6550   m.get('includeP
+00038730: 6179 6c6f 6164 2729 2069 7320 6e6f 7420  ayload') is not 
+00038740: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00038750: 2020 7365 6c66 2e69 6e63 6c75 6465 5f70    self.include_p
+00038760: 6179 6c6f 6164 203d 206d 2e67 6574 2827  ayload = m.get('
+00038770: 696e 636c 7564 6550 6179 6c6f 6164 2729  includePayload')
+00038780: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00038790: 7428 276c 696d 6974 2729 2069 7320 6e6f  t('limit') is no
+000387a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000387b0: 2020 2020 7365 6c66 2e6c 696d 6974 203d      self.limit =
+000387c0: 206d 2e67 6574 2827 6c69 6d69 7427 290a   m.get('limit').
+000387d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000387e0: 2827 6e65 7874 546f 6b65 6e27 2920 6973  ('nextToken') is
+000387f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038800: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
+00038810: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
+00038820: 6e65 7874 546f 6b65 6e27 290a 2020 2020  nextToken').    
+00038830: 2020 2020 6966 206d 2e67 6574 2827 7072      if m.get('pr
+00038840: 6566 6978 2729 2069 7320 6e6f 7420 4e6f  efix') is not No
+00038850: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00038860: 7365 6c66 2e70 7265 6669 7820 3d20 6d2e  self.prefix = m.
+00038870: 6765 7428 2770 7265 6669 7827 290a 2020  get('prefix').  
+00038880: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00038890: 7175 616c 6966 6965 7227 2920 6973 206e  qualifier') is n
+000388a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000388b0: 2020 2020 2073 656c 662e 7175 616c 6966       self.qualif
+000388c0: 6965 7220 3d20 6d2e 6765 7428 2771 7561  ier = m.get('qua
+000388d0: 6c69 6669 6572 2729 0a20 2020 2020 2020  lifier').       
+000388e0: 2069 6620 6d2e 6765 7428 2773 6f72 744f   if m.get('sortO
+000388f0: 7264 6572 4279 5469 6d65 2729 2069 7320  rderByTime') is 
+00038900: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038910: 2020 2020 2020 7365 6c66 2e73 6f72 745f        self.sort_
+00038920: 6f72 6465 725f 6279 5f74 696d 6520 3d20  order_by_time = 
+00038930: 6d2e 6765 7428 2773 6f72 744f 7264 6572  m.get('sortOrder
+00038940: 4279 5469 6d65 2729 0a20 2020 2020 2020  ByTime').       
+00038950: 2069 6620 6d2e 6765 7428 2773 7461 7274   if m.get('start
+00038960: 6564 5469 6d65 4265 6769 6e27 2920 6973  edTimeBegin') is
+00038970: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038980: 2020 2020 2020 2073 656c 662e 7374 6172         self.star
+00038990: 7465 645f 7469 6d65 5f62 6567 696e 203d  ted_time_begin =
+000389a0: 206d 2e67 6574 2827 7374 6172 7465 6454   m.get('startedT
+000389b0: 696d 6542 6567 696e 2729 0a20 2020 2020  imeBegin').     
+000389c0: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
+000389d0: 7274 6564 5469 6d65 456e 6427 2920 6973  rtedTimeEnd') is
+000389e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000389f0: 2020 2020 2020 2073 656c 662e 7374 6172         self.star
+00038a00: 7465 645f 7469 6d65 5f65 6e64 203d 206d  ted_time_end = m
+00038a10: 2e67 6574 2827 7374 6172 7465 6454 696d  .get('startedTim
+00038a20: 6545 6e64 2729 0a20 2020 2020 2020 2069  eEnd').        i
+00038a30: 6620 6d2e 6765 7428 2773 7461 7475 7327  f m.get('status'
+00038a40: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00038a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00038a60: 7374 6174 7573 203d 206d 2e67 6574 2827  status = m.get('
+00038a70: 7374 6174 7573 2729 0a20 2020 2020 2020  status').       
+00038a80: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00038a90: 6c61 7373 204c 6973 7441 7379 6e63 5461  lass ListAsyncTa
+00038aa0: 736b 7352 6573 706f 6e73 6528 5465 614d  sksResponse(TeaM
+00038ab0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00038ac0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6865  _init__(self, he
+00038ad0: 6164 6572 733d 4e6f 6e65 2c20 7374 6174  aders=None, stat
+00038ae0: 7573 5f63 6f64 653d 4e6f 6e65 2c20 626f  us_code=None, bo
+00038af0: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
+00038b00: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00038b10: 2068 6561 6465 7273 2020 2320 7479 7065   headers  # type
+00038b20: 3a20 6469 6374 5b73 7472 2c20 7374 725d  : dict[str, str]
+00038b30: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00038b40: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+00038b50: 7573 5f63 6f64 6520 2023 2074 7970 653a  us_code  # type:
+00038b60: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
+00038b70: 662e 626f 6479 203d 2062 6f64 7920 2023  f.body = body  #
+00038b80: 2074 7970 653a 204c 6973 7441 7379 6e63   type: ListAsync
+00038b90: 5461 736b 4f75 7470 7574 0a0a 2020 2020  TaskOutput..    
+00038ba0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00038bb0: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00038bc0: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+00038bd0: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+00038be0: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00038bf0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00038c00: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00038c10: 2073 7570 6572 284c 6973 7441 7379 6e63   super(ListAsync
+00038c20: 5461 736b 7352 6573 706f 6e73 652c 2073  TasksResponse, s
+00038c30: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+00038c40: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00038c50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038c60: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00038c70: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00038c80: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00038c90: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+00038ca0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+00038cb0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00038cc0: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+00038cd0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+00038ce0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00038cf0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+00038d00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00038d10: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+00038d20: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+00038d30: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00038d40: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00038d50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00038d60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00038d70: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00038d80: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00038d90: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00038da0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00038db0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00038dc0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00038dd0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00038de0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00038df0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00038e00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00038e10: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00038e20: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00038e30: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00038e40: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00038e50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00038e60: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00038e70: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00038e80: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+00038e90: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00038ea0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00038eb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00038ec0: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
+00038ed0: 6973 7441 7379 6e63 5461 736b 4f75 7470  istAsyncTaskOutp
+00038ee0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00038ef0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00038f00: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00038f10: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00038f20: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00038f30: 0a0a 636c 6173 7320 4c69 7374 436f 6e63  ..class ListConc
+00038f40: 7572 7265 6e63 7943 6f6e 6669 6773 5265  urrencyConfigsRe
+00038f50: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+00038f60: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00038f70: 5f28 7365 6c66 2c20 6675 6e63 7469 6f6e  _(self, function
+00038f80: 5f6e 616d 653d 4e6f 6e65 2c20 6c69 6d69  _name=None, limi
+00038f90: 743d 4e6f 6e65 2c20 6e65 7874 5f74 6f6b  t=None, next_tok
+00038fa0: 656e 3d4e 6f6e 6529 3a0a 2020 2020 2020  en=None):.      
+00038fb0: 2020 2320 5468 6520 6675 6e63 7469 6f6e    # The function
+00038fc0: 206e 616d 652e 2049 6620 796f 7520 6c65   name. If you le
+00038fd0: 6176 6520 7468 6973 2070 6172 616d 6574  ave this paramet
+00038fe0: 6572 2065 6d70 7479 2c20 7468 6520 636f  er empty, the co
+00038ff0: 6e63 7572 7265 6e63 7920 636f 6e66 6967  ncurrency config
+00039000: 7572 6174 696f 6e73 206f 6620 616c 6c20  urations of all 
+00039010: 6675 6e63 7469 6f6e 7320 6172 6520 7265  functions are re
+00039020: 7475 726e 6564 2e0a 2020 2020 2020 2020  turned..        
+00039030: 7365 6c66 2e66 756e 6374 696f 6e5f 6e61  self.function_na
+00039040: 6d65 203d 2066 756e 6374 696f 6e5f 6e61  me = function_na
+00039050: 6d65 2020 2320 7479 7065 3a20 7374 720a  me  # type: str.
+00039060: 2020 2020 2020 2020 2320 5468 6520 6d61          # The ma
+00039070: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
+00039080: 656e 7472 6965 7320 7265 7475 726e 6564  entries returned
+00039090: 2e0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000390a0: 696d 6974 203d 206c 696d 6974 2020 2320  imit = limit  # 
+000390b0: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+000390c0: 2020 2320 5468 6520 7061 6769 6e61 7469    # The paginati
+000390d0: 6f6e 2074 6f6b 656e 2074 6861 7420 6973  on token that is
+000390e0: 2075 7365 6420 696e 2074 6865 206e 6578   used in the nex
+000390f0: 7420 7265 7175 6573 7420 746f 2072 6574  t request to ret
+00039100: 7269 6576 6520 6120 6e65 7720 7061 6765  rieve a new page
+00039110: 206f 6620 7265 7375 6c74 732e 0a20 2020   of results..   
+00039120: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
+00039130: 6f6b 656e 203d 206e 6578 745f 746f 6b65  oken = next_toke
+00039140: 6e20 2023 2074 7970 653a 2073 7472 0a0a  n  # type: str..
+00039150: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00039160: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00039170: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+00039180: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00039190: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000391a0: 284c 6973 7443 6f6e 6375 7272 656e 6379  (ListConcurrency
+000391b0: 436f 6e66 6967 7352 6571 7565 7374 2c20  ConfigsRequest, 
+000391c0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+000391d0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000391e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000391f0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00039200: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00039210: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00039220: 2020 2020 2069 6620 7365 6c66 2e66 756e       if self.fun
+00039230: 6374 696f 6e5f 6e61 6d65 2069 7320 6e6f  ction_name is no
+00039240: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00039250: 2020 2020 7265 7375 6c74 5b27 6675 6e63      result['func
+00039260: 7469 6f6e 4e61 6d65 275d 203d 2073 656c  tionName'] = sel
+00039270: 662e 6675 6e63 7469 6f6e 5f6e 616d 650a  f.function_name.
+00039280: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00039290: 6c69 6d69 7420 6973 206e 6f74 204e 6f6e  limit is not Non
+000392a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000392b0: 6573 756c 745b 276c 696d 6974 275d 203d  esult['limit'] =
+000392c0: 2073 656c 662e 6c69 6d69 740a 2020 2020   self.limit.    
+000392d0: 2020 2020 6966 2073 656c 662e 6e65 7874      if self.next
+000392e0: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
+000392f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00039300: 7265 7375 6c74 5b27 6e65 7874 546f 6b65  result['nextToke
+00039310: 6e27 5d20 3d20 7365 6c66 2e6e 6578 745f  n'] = self.next_
+00039320: 746f 6b65 6e0a 2020 2020 2020 2020 7265  token.        re
+00039330: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00039340: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00039350: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+00039360: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00039370: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00039380: 6d2e 6765 7428 2766 756e 6374 696f 6e4e  m.get('functionN
+00039390: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
+000393a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000393b0: 656c 662e 6675 6e63 7469 6f6e 5f6e 616d  elf.function_nam
+000393c0: 6520 3d20 6d2e 6765 7428 2766 756e 6374  e = m.get('funct
+000393d0: 696f 6e4e 616d 6527 290a 2020 2020 2020  ionName').      
+000393e0: 2020 6966 206d 2e67 6574 2827 6c69 6d69    if m.get('limi
+000393f0: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
+00039400: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00039410: 662e 6c69 6d69 7420 3d20 6d2e 6765 7428  f.limit = m.get(
+00039420: 276c 696d 6974 2729 0a20 2020 2020 2020  'limit').       
+00039430: 2069 6620 6d2e 6765 7428 276e 6578 7454   if m.get('nextT
+00039440: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
+00039450: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00039460: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
+00039470: 3d20 6d2e 6765 7428 276e 6578 7454 6f6b  = m.get('nextTok
+00039480: 656e 2729 0a20 2020 2020 2020 2072 6574  en').        ret
+00039490: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+000394a0: 204c 6973 7443 6f6e 6375 7272 656e 6379   ListConcurrency
+000394b0: 436f 6e66 6967 7352 6573 706f 6e73 6528  ConfigsResponse(
+000394c0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+000394d0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000394e0: 2c20 6865 6164 6572 733d 4e6f 6e65 2c20  , headers=None, 
+000394f0: 7374 6174 7573 5f63 6f64 653d 4e6f 6e65  status_code=None
+00039500: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
+00039510: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00039520: 7273 203d 2068 6561 6465 7273 2020 2320  rs = headers  # 
+00039530: 7479 7065 3a20 6469 6374 5b73 7472 2c20  type: dict[str, 
+00039540: 7374 725d 0a20 2020 2020 2020 2073 656c  str].        sel
+00039550: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00039560: 7374 6174 7573 5f63 6f64 6520 2023 2074  status_code  # t
+00039570: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00039580: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+00039590: 7920 2023 2074 7970 653a 204c 6973 7443  y  # type: ListC
+000395a0: 6f6e 6375 7272 656e 6379 436f 6e66 6967  oncurrencyConfig
+000395b0: 734f 7574 7075 740a 0a20 2020 2064 6566  sOutput..    def
+000395c0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+000395d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000395e0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+000395f0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+00039600: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+00039610: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00039620: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00039630: 7065 7228 4c69 7374 436f 6e63 7572 7265  per(ListConcurre
+00039640: 6e63 7943 6f6e 6669 6773 5265 7370 6f6e  ncyConfigsRespon
+00039650: 7365 2c20 7365 6c66 292e 746f 5f6d 6170  se, self).to_map
+00039660: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00039670: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00039680: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00039690: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+000396a0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+000396b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000396c0: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+000396d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000396e0: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+000396f0: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+00039700: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+00039710: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+00039720: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00039730: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00039740: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+00039750: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+00039760: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00039770: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+00039780: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00039790: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+000397a0: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+000397b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000397c0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+000397d0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+000397e0: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+000397f0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00039800: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00039810: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+00039820: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00039830: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00039840: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+00039850: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+00039860: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00039870: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+00039880: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00039890: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000398a0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000398b0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+000398c0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+000398d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000398e0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000398f0: 6c20 3d20 4c69 7374 436f 6e63 7572 7265  l = ListConcurre
+00039900: 6e63 7943 6f6e 6669 6773 4f75 7470 7574  ncyConfigsOutput
+00039910: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00039920: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+00039930: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+00039940: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+00039950: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00039960: 636c 6173 7320 4c69 7374 4375 7374 6f6d  class ListCustom
+00039970: 446f 6d61 696e 7352 6571 7565 7374 2854  DomainsRequest(T
+00039980: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00039990: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+000399a0: 206c 696d 6974 3d4e 6f6e 652c 206e 6578   limit=None, nex
+000399b0: 745f 746f 6b65 6e3d 4e6f 6e65 2c20 7072  t_token=None, pr
+000399c0: 6566 6978 3d4e 6f6e 6529 3a0a 2020 2020  efix=None):.    
+000399d0: 2020 2020 2320 5468 6520 6e75 6d62 6572      # The number
+000399e0: 206f 6620 6375 7374 6f6d 2064 6f6d 6169   of custom domai
+000399f0: 6e20 6e61 6d65 7320 7265 7475 726e 6564  n names returned
+00039a00: 2e0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00039a10: 696d 6974 203d 206c 696d 6974 2020 2320  imit = limit  # 
+00039a20: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00039a30: 2020 2320 5468 6520 7061 6769 6e61 7469    # The paginati
+00039a40: 6f6e 2074 6f6b 656e 2074 6861 7420 6973  on token that is
+00039a50: 2075 7365 6420 696e 2074 6865 206e 6578   used in the nex
+00039a60: 7420 7265 7175 6573 7420 746f 2072 6574  t request to ret
+00039a70: 7269 6576 6520 6120 6e65 7720 7061 6765  rieve a new page
+00039a80: 206f 6620 7265 7375 6c74 732e 0a20 2020   of results..   
+00039a90: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
+00039aa0: 6f6b 656e 203d 206e 6578 745f 746f 6b65  oken = next_toke
+00039ab0: 6e20 2023 2074 7970 653a 2073 7472 0a20  n  # type: str. 
+00039ac0: 2020 2020 2020 2023 2054 6865 2064 6f6d         # The dom
+00039ad0: 6169 6e20 6e61 6d65 2070 7265 6669 782e  ain name prefix.
+00039ae0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+00039af0: 6566 6978 203d 2070 7265 6669 7820 2023  efix = prefix  #
+00039b00: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+00039b10: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00039b20: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00039b30: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00039b40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00039b50: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
+00039b60: 7443 7573 746f 6d44 6f6d 6169 6e73 5265  tCustomDomainsRe
+00039b70: 7175 6573 742c 2073 656c 6629 2e74 6f5f  quest, self).to_
+00039b80: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00039b90: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00039ba0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00039bb0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00039bc0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00039bd0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00039be0: 656c 662e 6c69 6d69 7420 6973 206e 6f74  elf.limit is not
+00039bf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00039c00: 2020 2072 6573 756c 745b 276c 696d 6974     result['limit
+00039c10: 275d 203d 2073 656c 662e 6c69 6d69 740a  '] = self.limit.
+00039c20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00039c30: 6e65 7874 5f74 6f6b 656e 2069 7320 6e6f  next_token is no
+00039c40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00039c50: 2020 2020 7265 7375 6c74 5b27 6e65 7874      result['next
+00039c60: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e6e  Token'] = self.n
+00039c70: 6578 745f 746f 6b65 6e0a 2020 2020 2020  ext_token.      
+00039c80: 2020 6966 2073 656c 662e 7072 6566 6978    if self.prefix
+00039c90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00039ca0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00039cb0: 5b27 7072 6566 6978 275d 203d 2073 656c  ['prefix'] = sel
+00039cc0: 662e 7072 6566 6978 0a20 2020 2020 2020  f.prefix.       
+00039cd0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00039ce0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00039cf0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+00039d00: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00039d10: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00039d20: 6966 206d 2e67 6574 2827 6c69 6d69 7427  if m.get('limit'
+00039d30: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00039d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00039d50: 6c69 6d69 7420 3d20 6d2e 6765 7428 276c  limit = m.get('l
+00039d60: 696d 6974 2729 0a20 2020 2020 2020 2069  imit').        i
+00039d70: 6620 6d2e 6765 7428 276e 6578 7454 6f6b  f m.get('nextTok
+00039d80: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
+00039d90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00039da0: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
+00039db0: 6d2e 6765 7428 276e 6578 7454 6f6b 656e  m.get('nextToken
+00039dc0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00039dd0: 6765 7428 2770 7265 6669 7827 2920 6973  get('prefix') is
+00039de0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00039df0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00039e00: 6978 203d 206d 2e67 6574 2827 7072 6566  ix = m.get('pref
+00039e10: 6978 2729 0a20 2020 2020 2020 2072 6574  ix').        ret
+00039e20: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00039e30: 204c 6973 7443 7573 746f 6d44 6f6d 6169   ListCustomDomai
+00039e40: 6e73 5265 7370 6f6e 7365 2854 6561 4d6f  nsResponse(TeaMo
+00039e50: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00039e60: 696e 6974 5f5f 2873 656c 662c 2068 6561  init__(self, hea
+00039e70: 6465 7273 3d4e 6f6e 652c 2073 7461 7475  ders=None, statu
+00039e80: 735f 636f 6465 3d4e 6f6e 652c 2062 6f64  s_code=None, bod
+00039e90: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
+00039ea0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00039eb0: 6865 6164 6572 7320 2023 2074 7970 653a  headers  # type:
+00039ec0: 2064 6963 745b 7374 722c 2073 7472 5d0a   dict[str, str].
+00039ed0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00039ee0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+00039ef0: 735f 636f 6465 2020 2320 7479 7065 3a20  s_code  # type: 
+00039f00: 696e 740a 2020 2020 2020 2020 7365 6c66  int.        self
+00039f10: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
+00039f20: 7479 7065 3a20 4c69 7374 4375 7374 6f6d  type: ListCustom
+00039f30: 446f 6d61 696e 4f75 7470 7574 0a0a 2020  DomainOutput..  
+00039f40: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00039f50: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00039f60: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+00039f70: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00039f80: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+00039f90: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00039fa0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00039fb0: 203d 2073 7570 6572 284c 6973 7443 7573   = super(ListCus
+00039fc0: 746f 6d44 6f6d 6169 6e73 5265 7370 6f6e  tomDomainsRespon
+00039fd0: 7365 2c20 7365 6c66 292e 746f 5f6d 6170  se, self).to_map
+00039fe0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00039ff0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0003a000: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0003a010: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0003a020: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0003a030: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003a040: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+0003a050: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003a060: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+0003a070: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+0003a080: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+0003a090: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+0003a0a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003a0b0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003a0c0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+0003a0d0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+0003a0e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003a0f0: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+0003a100: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003a110: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+0003a120: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+0003a130: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0003a140: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+0003a150: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+0003a160: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+0003a170: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0003a180: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003a190: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+0003a1a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003a1b0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+0003a1c0: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+0003a1d0: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+0003a1e0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+0003a1f0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+0003a200: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003a210: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+0003a220: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+0003a230: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+0003a240: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+0003a250: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003a260: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+0003a270: 6c20 3d20 4c69 7374 4375 7374 6f6d 446f  l = ListCustomDo
+0003a280: 6d61 696e 4f75 7470 7574 2829 0a20 2020  mainOutput().   
+0003a290: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+0003a2a0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+0003a2b0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+0003a2c0: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+0003a2d0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+0003a2e0: 4c69 7374 4675 6e63 7469 6f6e 5665 7273  ListFunctionVers
+0003a2f0: 696f 6e73 5265 7175 6573 7428 5465 614d  ionsRequest(TeaM
+0003a300: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0003a310: 5f69 6e69 745f 5f28 7365 6c66 2c20 6469  _init__(self, di
+0003a320: 7265 6374 696f 6e3d 4e6f 6e65 2c20 6c69  rection=None, li
+0003a330: 6d69 743d 4e6f 6e65 2c20 6e65 7874 5f74  mit=None, next_t
+0003a340: 6f6b 656e 3d4e 6f6e 6529 3a0a 2020 2020  oken=None):.    
+0003a350: 2020 2020 2320 5468 6520 736f 7274 696e      # The sortin
+0003a360: 6720 6d6f 6465 206f 6620 6675 6e63 7469  g mode of functi
+0003a370: 6f6e 2076 6572 7369 6f6e 732e 2056 616c  on versions. Val
+0003a380: 6964 2076 616c 7565 733a 2042 4143 4b57  id values: BACKW
+0003a390: 4152 4420 616e 6420 464f 5257 4152 442e  ARD and FORWARD.
+0003a3a0: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
+0003a3b0: 7265 6374 696f 6e20 3d20 6469 7265 6374  rection = direct
+0003a3c0: 696f 6e20 2023 2074 7970 653a 2073 7472  ion  # type: str
+0003a3d0: 0a20 2020 2020 2020 2023 2054 6865 206e  .        # The n
+0003a3e0: 756d 6265 7220 6f66 2066 756e 6374 696f  umber of functio
+0003a3f0: 6e20 7665 7273 696f 6e73 2074 6861 7420  n versions that 
+0003a400: 6172 6520 7265 7475 726e 6564 2e0a 2020  are returned..  
+0003a410: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
+0003a420: 203d 206c 696d 6974 2020 2320 7479 7065   = limit  # type
+0003a430: 3a20 696e 740a 2020 2020 2020 2020 2320  : int.        # 
+0003a440: 5468 6520 7061 6769 6e61 7469 6f6e 2074  The pagination t
+0003a450: 6f6b 656e 2074 6861 7420 6973 2075 7365  oken that is use
+0003a460: 6420 696e 2074 6865 206e 6578 7420 7265  d in the next re
+0003a470: 7175 6573 7420 746f 2072 6574 7269 6576  quest to retriev
+0003a480: 6520 6120 6e65 7720 7061 6765 206f 6620  e a new page of 
+0003a490: 7265 7375 6c74 732e 0a20 2020 2020 2020  results..       
+0003a4a0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003a4b0: 203d 206e 6578 745f 746f 6b65 6e20 2023   = next_token  #
+0003a4c0: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+0003a4d0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0003a4e0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0003a4f0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0003a500: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0003a510: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
+0003a520: 7446 756e 6374 696f 6e56 6572 7369 6f6e  tFunctionVersion
+0003a530: 7352 6571 7565 7374 2c20 7365 6c66 292e  sRequest, self).
+0003a540: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003a550: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0003a560: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003a570: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0003a580: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0003a590: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003a5a0: 6620 7365 6c66 2e64 6972 6563 7469 6f6e  f self.direction
+0003a5b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003a5c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003a5d0: 5b27 6469 7265 6374 696f 6e27 5d20 3d20  ['direction'] = 
+0003a5e0: 7365 6c66 2e64 6972 6563 7469 6f6e 0a20  self.direction. 
+0003a5f0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+0003a600: 696d 6974 2069 7320 6e6f 7420 4e6f 6e65  imit is not None
+0003a610: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003a620: 7375 6c74 5b27 6c69 6d69 7427 5d20 3d20  sult['limit'] = 
+0003a630: 7365 6c66 2e6c 696d 6974 0a20 2020 2020  self.limit.     
+0003a640: 2020 2069 6620 7365 6c66 2e6e 6578 745f     if self.next_
+0003a650: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+0003a660: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003a670: 6573 756c 745b 276e 6578 7454 6f6b 656e  esult['nextToken
+0003a680: 275d 203d 2073 656c 662e 6e65 7874 5f74  '] = self.next_t
+0003a690: 6f6b 656e 0a20 2020 2020 2020 2072 6574  oken.        ret
+0003a6a0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0003a6b0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0003a6c0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+0003a6d0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0003a6e0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0003a6f0: 2e67 6574 2827 6469 7265 6374 696f 6e27  .get('direction'
+0003a700: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003a710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003a720: 6469 7265 6374 696f 6e20 3d20 6d2e 6765  direction = m.ge
+0003a730: 7428 2764 6972 6563 7469 6f6e 2729 0a20  t('direction'). 
+0003a740: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003a750: 276c 696d 6974 2729 2069 7320 6e6f 7420  'limit') is not 
+0003a760: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003a770: 2020 7365 6c66 2e6c 696d 6974 203d 206d    self.limit = m
+0003a780: 2e67 6574 2827 6c69 6d69 7427 290a 2020  .get('limit').  
+0003a790: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003a7a0: 6e65 7874 546f 6b65 6e27 2920 6973 206e  nextToken') is n
+0003a7b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003a7c0: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
+0003a7d0: 6f6b 656e 203d 206d 2e67 6574 2827 6e65  oken = m.get('ne
+0003a7e0: 7874 546f 6b65 6e27 290a 2020 2020 2020  xtToken').      
+0003a7f0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0003a800: 636c 6173 7320 4c69 7374 4675 6e63 7469  class ListFuncti
+0003a810: 6f6e 5665 7273 696f 6e73 5265 7370 6f6e  onVersionsRespon
+0003a820: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+0003a830: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0003a840: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
+0003a850: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
+0003a860: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
+0003a870: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+0003a880: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
+0003a890: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
+0003a8a0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
+0003a8b0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0003a8c0: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
+0003a8d0: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
+0003a8e0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+0003a8f0: 626f 6479 2020 2320 7479 7065 3a20 4c69  body  # type: Li
+0003a900: 7374 5665 7273 696f 6e73 4f75 7470 7574  stVersionsOutput
+0003a910: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0003a920: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0003a930: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+0003a940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003a950: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+0003a960: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0003a970: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0003a980: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
+0003a990: 7446 756e 6374 696f 6e56 6572 7369 6f6e  tFunctionVersion
+0003a9a0: 7352 6573 706f 6e73 652c 2073 656c 6629  sResponse, self)
+0003a9b0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0003a9c0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0003a9d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003a9e0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0003a9f0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0003aa00: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0003aa10: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+0003aa20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003aa30: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0003aa40: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+0003aa50: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+0003aa60: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+0003aa70: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+0003aa80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003aa90: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+0003aaa0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+0003aab0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+0003aac0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+0003aad0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003aae0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+0003aaf0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+0003ab00: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003ab10: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0003ab20: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0003ab30: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+0003ab40: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0003ab50: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0003ab60: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+0003ab70: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+0003ab80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003ab90: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+0003aba0: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+0003abb0: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+0003abc0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+0003abd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003abe0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+0003abf0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+0003ac00: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+0003ac10: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+0003ac20: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+0003ac30: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+0003ac40: 6d70 5f6d 6f64 656c 203d 204c 6973 7456  mp_model = ListV
+0003ac50: 6572 7369 6f6e 734f 7574 7075 7428 290a  ersionsOutput().
+0003ac60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003ac70: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+0003ac80: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+0003ac90: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+0003aca0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0003acb0: 7373 204c 6973 7446 756e 6374 696f 6e73  ss ListFunctions
+0003acc0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+0003acd0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0003ace0: 745f 5f28 7365 6c66 2c20 6c69 6d69 743d  t__(self, limit=
+0003acf0: 4e6f 6e65 2c20 6e65 7874 5f74 6f6b 656e  None, next_token
+0003ad00: 3d4e 6f6e 652c 2070 7265 6669 783d 4e6f  =None, prefix=No
+0003ad10: 6e65 293a 0a20 2020 2020 2020 2023 2054  ne):.        # T
+0003ad20: 6865 206e 756d 6265 7220 6f66 2066 756e  he number of fun
+0003ad30: 6374 696f 6e73 2074 6f20 7265 7475 726e  ctions to return
+0003ad40: 2e20 5468 6520 6d69 6e69 6d75 6d20 7661  . The minimum va
+0003ad50: 6c75 6520 6973 2031 2061 6e64 2074 6865  lue is 1 and the
+0003ad60: 206d 6178 696d 756d 2076 616c 7565 2069   maximum value i
+0003ad70: 7320 3130 302e 0a20 2020 2020 2020 2073  s 100..        s
+0003ad80: 656c 662e 6c69 6d69 7420 3d20 6c69 6d69  elf.limit = limi
+0003ad90: 7420 2023 2074 7970 653a 2069 6e74 0a20  t  # type: int. 
+0003ada0: 2020 2020 2020 2023 2054 6865 2070 6167         # The pag
+0003adb0: 696e 6174 696f 6e20 746f 6b65 6e2e 0a20  ination token.. 
+0003adc0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
+0003add0: 5f74 6f6b 656e 203d 206e 6578 745f 746f  _token = next_to
+0003ade0: 6b65 6e20 2023 2074 7970 653a 2073 7472  ken  # type: str
+0003adf0: 0a20 2020 2020 2020 2023 2054 6865 2070  .        # The p
+0003ae00: 7265 6669 7820 6f66 2074 6865 2066 756e  refix of the fun
+0003ae10: 6374 696f 6e20 6e61 6d65 2e0a 2020 2020  ction name..    
+0003ae20: 2020 2020 7365 6c66 2e70 7265 6669 7820      self.prefix 
+0003ae30: 3d20 7072 6566 6978 2020 2320 7479 7065  = prefix  # type
+0003ae40: 3a20 7374 720a 0a20 2020 2064 6566 2076  : str..    def v
+0003ae50: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0003ae60: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0003ae70: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0003ae80: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0003ae90: 3d20 7375 7065 7228 4c69 7374 4675 6e63  = super(ListFunc
+0003aea0: 7469 6f6e 7352 6571 7565 7374 2c20 7365  tionsRequest, se
+0003aeb0: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+0003aec0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0003aed0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003aee0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0003aef0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0003af00: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0003af10: 2020 2069 6620 7365 6c66 2e6c 696d 6974     if self.limit
+0003af20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003af30: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003af40: 5b27 6c69 6d69 7427 5d20 3d20 7365 6c66  ['limit'] = self
+0003af50: 2e6c 696d 6974 0a20 2020 2020 2020 2069  .limit.        i
+0003af60: 6620 7365 6c66 2e6e 6578 745f 746f 6b65  f self.next_toke
+0003af70: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+0003af80: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003af90: 745b 276e 6578 7454 6f6b 656e 275d 203d  t['nextToken'] =
+0003afa0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003afb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003afc0: 2e70 7265 6669 7820 6973 206e 6f74 204e  .prefix is not N
+0003afd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003afe0: 2072 6573 756c 745b 2770 7265 6669 7827   result['prefix'
+0003aff0: 5d20 3d20 7365 6c66 2e70 7265 6669 780a  ] = self.prefix.
+0003b000: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003b010: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003b020: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0003b030: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0003b040: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0003b050: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003b060: 276c 696d 6974 2729 2069 7320 6e6f 7420  'limit') is not 
+0003b070: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003b080: 2020 7365 6c66 2e6c 696d 6974 203d 206d    self.limit = m
+0003b090: 2e67 6574 2827 6c69 6d69 7427 290a 2020  .get('limit').  
+0003b0a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003b0b0: 6e65 7874 546f 6b65 6e27 2920 6973 206e  nextToken') is n
+0003b0c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003b0d0: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
+0003b0e0: 6f6b 656e 203d 206d 2e67 6574 2827 6e65  oken = m.get('ne
+0003b0f0: 7874 546f 6b65 6e27 290a 2020 2020 2020  xtToken').      
+0003b100: 2020 6966 206d 2e67 6574 2827 7072 6566    if m.get('pref
+0003b110: 6978 2729 2069 7320 6e6f 7420 4e6f 6e65  ix') is not None
+0003b120: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003b130: 6c66 2e70 7265 6669 7820 3d20 6d2e 6765  lf.prefix = m.ge
+0003b140: 7428 2770 7265 6669 7827 290a 2020 2020  t('prefix').    
+0003b150: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0003b160: 0a0a 636c 6173 7320 4c69 7374 4675 6e63  ..class ListFunc
+0003b170: 7469 6f6e 7352 6573 706f 6e73 6528 5465  tionsResponse(Te
+0003b180: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0003b190: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0003b1a0: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
+0003b1b0: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
+0003b1c0: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
+0003b1d0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0003b1e0: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
+0003b1f0: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
+0003b200: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
+0003b210: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+0003b220: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
+0003b230: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
+0003b240: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
+0003b250: 2023 2074 7970 653a 204c 6973 7446 756e   # type: ListFun
+0003b260: 6374 696f 6e73 4f75 7470 7574 0a0a 2020  ctionsOutput..  
+0003b270: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0003b280: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+0003b290: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+0003b2a0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0003b2b0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+0003b2c0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0003b2d0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0003b2e0: 203d 2073 7570 6572 284c 6973 7446 756e   = super(ListFun
+0003b2f0: 6374 696f 6e73 5265 7370 6f6e 7365 2c20  ctionsResponse, 
+0003b300: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+0003b310: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0003b320: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003b330: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0003b340: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0003b350: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0003b360: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+0003b370: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+0003b380: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003b390: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+0003b3a0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+0003b3b0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0003b3c0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+0003b3d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003b3e0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+0003b3f0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+0003b400: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0003b410: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0003b420: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003b430: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003b440: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+0003b450: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+0003b460: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0003b470: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0003b480: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+0003b490: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+0003b4a0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+0003b4b0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+0003b4c0: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+0003b4d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003b4e0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+0003b4f0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+0003b500: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003b510: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+0003b520: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003b530: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0003b540: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+0003b550: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+0003b560: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003b570: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+0003b580: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003b590: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+0003b5a0: 4c69 7374 4675 6e63 7469 6f6e 734f 7574  ListFunctionsOut
+0003b5b0: 7075 7428 290a 2020 2020 2020 2020 2020  put().          
+0003b5c0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
+0003b5d0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+0003b5e0: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
+0003b5f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0003b600: 0a0a 0a63 6c61 7373 204c 6973 7449 6e73  ...class ListIns
+0003b610: 7461 6e63 6573 5265 7175 6573 7428 5465  tancesRequest(Te
+0003b620: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0003b630: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0003b640: 7175 616c 6966 6965 723d 4e6f 6e65 2c20  qualifier=None, 
+0003b650: 7769 7468 5f61 6c6c 5f61 6374 6976 653d  with_all_active=
+0003b660: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
+0003b670: 2054 6865 2066 756e 6374 696f 6e20 7665   The function ve
+0003b680: 7273 696f 6e20 6f72 2061 6c69 6173 2e0a  rsion or alias..
+0003b690: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
+0003b6a0: 6c69 6669 6572 203d 2071 7561 6c69 6669  lifier = qualifi
+0003b6b0: 6572 2020 2320 7479 7065 3a20 7374 720a  er  # type: str.
+0003b6c0: 2020 2020 2020 2020 2320 5370 6563 6966          # Specif
+0003b6d0: 6965 7320 7768 6574 6865 7220 746f 206c  ies whether to l
+0003b6e0: 6973 7420 616c 6c20 696e 7374 616e 6365  ist all instance
+0003b6f0: 732e 2056 616c 6964 2076 616c 7565 733a  s. Valid values:
+0003b700: 2074 7275 6520 616e 6420 6661 6c73 652e   true and false.
+0003b710: 0a20 2020 2020 2020 2073 656c 662e 7769  .        self.wi
+0003b720: 7468 5f61 6c6c 5f61 6374 6976 6520 3d20  th_all_active = 
+0003b730: 7769 7468 5f61 6c6c 5f61 6374 6976 6520  with_all_active 
+0003b740: 2023 2074 7970 653a 2062 6f6f 6c0a 0a20   # type: bool.. 
+0003b750: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0003b760: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0003b770: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+0003b780: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0003b790: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0003b7a0: 4c69 7374 496e 7374 616e 6365 7352 6571  ListInstancesReq
+0003b7b0: 7565 7374 2c20 7365 6c66 292e 746f 5f6d  uest, self).to_m
+0003b7c0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0003b7d0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0003b7e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003b7f0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0003b800: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0003b810: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0003b820: 6c66 2e71 7561 6c69 6669 6572 2069 7320  lf.qualifier is 
+0003b830: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003b840: 2020 2020 2020 7265 7375 6c74 5b27 7175        result['qu
+0003b850: 616c 6966 6965 7227 5d20 3d20 7365 6c66  alifier'] = self
+0003b860: 2e71 7561 6c69 6669 6572 0a20 2020 2020  .qualifier.     
+0003b870: 2020 2069 6620 7365 6c66 2e77 6974 685f     if self.with_
+0003b880: 616c 6c5f 6163 7469 7665 2069 7320 6e6f  all_active is no
+0003b890: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003b8a0: 2020 2020 7265 7375 6c74 5b27 7769 7468      result['with
+0003b8b0: 416c 6c41 6374 6976 6527 5d20 3d20 7365  AllActive'] = se
+0003b8c0: 6c66 2e77 6974 685f 616c 6c5f 6163 7469  lf.with_all_acti
+0003b8d0: 7665 0a20 2020 2020 2020 2072 6574 7572  ve.        retur
+0003b8e0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0003b8f0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0003b900: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+0003b910: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0003b920: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003b930: 6574 2827 7175 616c 6966 6965 7227 2920  et('qualifier') 
+0003b940: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003b950: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
+0003b960: 616c 6966 6965 7220 3d20 6d2e 6765 7428  alifier = m.get(
+0003b970: 2771 7561 6c69 6669 6572 2729 0a20 2020  'qualifier').   
+0003b980: 2020 2020 2069 6620 6d2e 6765 7428 2777       if m.get('w
+0003b990: 6974 6841 6c6c 4163 7469 7665 2729 2069  ithAllActive') i
+0003b9a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003b9b0: 2020 2020 2020 2020 7365 6c66 2e77 6974          self.wit
+0003b9c0: 685f 616c 6c5f 6163 7469 7665 203d 206d  h_all_active = m
+0003b9d0: 2e67 6574 2827 7769 7468 416c 6c41 6374  .get('withAllAct
+0003b9e0: 6976 6527 290a 2020 2020 2020 2020 7265  ive').        re
+0003b9f0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003ba00: 7320 4c69 7374 496e 7374 616e 6365 7352  s ListInstancesR
+0003ba10: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+0003ba20: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0003ba30: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
+0003ba40: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
+0003ba50: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
+0003ba60: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+0003ba70: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+0003ba80: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
+0003ba90: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
+0003baa0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+0003bab0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+0003bac0: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
+0003bad0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+0003bae0: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
+0003baf0: 653a 204c 6973 7449 6e73 7461 6e63 6573  e: ListInstances
+0003bb00: 4f75 7470 7574 0a0a 2020 2020 6465 6620  Output..    def 
+0003bb10: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0003bb20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003bb30: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+0003bb40: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+0003bb50: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+0003bb60: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0003bb70: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0003bb80: 6572 284c 6973 7449 6e73 7461 6e63 6573  er(ListInstances
+0003bb90: 5265 7370 6f6e 7365 2c20 7365 6c66 292e  Response, self).
+0003bba0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003bbb0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0003bbc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003bbd0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0003bbe0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0003bbf0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003bc00: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+0003bc10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003bc20: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003bc30: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+0003bc40: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+0003bc50: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+0003bc60: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+0003bc70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003bc80: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+0003bc90: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+0003bca0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+0003bcb0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+0003bcc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003bcd0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+0003bce0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+0003bcf0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0003bd00: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0003bd10: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0003bd20: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
+0003bd30: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003bd40: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003bd50: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+0003bd60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003bd70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003bd80: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+0003bd90: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+0003bda0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+0003bdb0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+0003bdc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003bdd0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0003bde0: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+0003bdf0: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+0003be00: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+0003be10: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0003be20: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0003be30: 705f 6d6f 6465 6c20 3d20 4c69 7374 496e  p_model = ListIn
+0003be40: 7374 616e 6365 734f 7574 7075 7428 290a  stancesOutput().
+0003be50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003be60: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+0003be70: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+0003be80: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+0003be90: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0003bea0: 7373 204c 6973 744c 6179 6572 5665 7273  ss ListLayerVers
+0003beb0: 696f 6e73 5265 7175 6573 7428 5465 614d  ionsRequest(TeaM
+0003bec0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0003bed0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6c69  _init__(self, li
+0003bee0: 6d69 743d 4e6f 6e65 2c20 7374 6172 745f  mit=None, start_
+0003bef0: 7665 7273 696f 6e3d 4e6f 6e65 293a 0a20  version=None):. 
+0003bf00: 2020 2020 2020 2023 2054 6865 206e 756d         # The num
+0003bf10: 6265 7220 6f66 2076 6572 7369 6f6e 7320  ber of versions 
+0003bf20: 746f 2062 6520 7265 7475 726e 6564 2e0a  to be returned..
+0003bf30: 2020 2020 2020 2020 7365 6c66 2e6c 696d          self.lim
+0003bf40: 6974 203d 206c 696d 6974 2020 2320 7479  it = limit  # ty
+0003bf50: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+0003bf60: 2320 5468 6520 696e 6974 6961 6c20 7665  # The initial ve
+0003bf70: 7273 696f 6e20 6f66 2074 6865 206c 6179  rsion of the lay
+0003bf80: 6572 2e0a 2020 2020 2020 2020 7365 6c66  er..        self
+0003bf90: 2e73 7461 7274 5f76 6572 7369 6f6e 203d  .start_version =
+0003bfa0: 2073 7461 7274 5f76 6572 7369 6f6e 2020   start_version  
+0003bfb0: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
+0003bfc0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0003bfd0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0003bfe0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+0003bff0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0003c000: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
+0003c010: 7374 4c61 7965 7256 6572 7369 6f6e 7352  stLayerVersionsR
+0003c020: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+0003c030: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0003c040: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0003c050: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003c060: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0003c070: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0003c080: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0003c090: 7365 6c66 2e6c 696d 6974 2069 7320 6e6f  self.limit is no
+0003c0a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003c0b0: 2020 2020 7265 7375 6c74 5b27 6c69 6d69      result['limi
+0003c0c0: 7427 5d20 3d20 7365 6c66 2e6c 696d 6974  t'] = self.limit
+0003c0d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003c0e0: 2e73 7461 7274 5f76 6572 7369 6f6e 2069  .start_version i
+0003c0f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003c100: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003c110: 7374 6172 7456 6572 7369 6f6e 275d 203d  startVersion'] =
+0003c120: 2073 656c 662e 7374 6172 745f 7665 7273   self.start_vers
+0003c130: 696f 6e0a 2020 2020 2020 2020 7265 7475  ion.        retu
+0003c140: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0003c150: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0003c160: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+0003c170: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+0003c180: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+0003c190: 6765 7428 276c 696d 6974 2729 2069 7320  get('limit') is 
+0003c1a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003c1b0: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
+0003c1c0: 203d 206d 2e67 6574 2827 6c69 6d69 7427   = m.get('limit'
+0003c1d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003c1e0: 6574 2827 7374 6172 7456 6572 7369 6f6e  et('startVersion
+0003c1f0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003c200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003c210: 2e73 7461 7274 5f76 6572 7369 6f6e 203d  .start_version =
+0003c220: 206d 2e67 6574 2827 7374 6172 7456 6572   m.get('startVer
+0003c230: 7369 6f6e 2729 0a20 2020 2020 2020 2072  sion').        r
+0003c240: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0003c250: 7373 204c 6973 744c 6179 6572 5665 7273  ss ListLayerVers
+0003c260: 696f 6e73 5265 7370 6f6e 7365 2854 6561  ionsResponse(Tea
+0003c270: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0003c280: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
+0003c290: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
+0003c2a0: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
+0003c2b0: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
+0003c2c0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0003c2d0: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
+0003c2e0: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
+0003c2f0: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
+0003c300: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+0003c310: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
+0003c320: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+0003c330: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
+0003c340: 2320 7479 7065 3a20 4c69 7374 4c61 7965  # type: ListLaye
+0003c350: 7256 6572 7369 6f6e 4f75 7470 7574 0a0a  rVersionOutput..
+0003c360: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0003c370: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0003c380: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+0003c390: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0003c3a0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+0003c3b0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+0003c3c0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+0003c3d0: 6170 203d 2073 7570 6572 284c 6973 744c  ap = super(ListL
+0003c3e0: 6179 6572 5665 7273 696f 6e73 5265 7370  ayerVersionsResp
+0003c3f0: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
+0003c400: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0003c410: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0003c420: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003c430: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0003c440: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0003c450: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0003c460: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+0003c470: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003c480: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+0003c490: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+0003c4a0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+0003c4b0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0003c4c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003c4d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003c4e0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+0003c4f0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+0003c500: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0003c510: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+0003c520: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003c530: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+0003c540: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+0003c550: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+0003c560: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0003c570: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0003c580: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+0003c590: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+0003c5a0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+0003c5b0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+0003c5c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003c5d0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0003c5e0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+0003c5f0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+0003c600: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+0003c610: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+0003c620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003c630: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0003c640: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+0003c650: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
+0003c660: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
+0003c670: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003c680: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+0003c690: 6465 6c20 3d20 4c69 7374 4c61 7965 7256  del = ListLayerV
+0003c6a0: 6572 7369 6f6e 4f75 7470 7574 2829 0a20  ersionOutput(). 
+0003c6b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003c6c0: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+0003c6d0: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+0003c6e0: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+0003c6f0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003c700: 7320 4c69 7374 4c61 7965 7273 5265 7175  s ListLayersRequ
+0003c710: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+0003c720: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0003c730: 7365 6c66 2c20 6c69 6d69 743d 4e6f 6e65  self, limit=None
+0003c740: 2c20 6e65 7874 5f74 6f6b 656e 3d4e 6f6e  , next_token=Non
+0003c750: 652c 206f 6666 6963 6961 6c3d 4e6f 6e65  e, official=None
+0003c760: 2c20 7072 6566 6978 3d4e 6f6e 652c 2070  , prefix=None, p
+0003c770: 7562 6c69 633d 4e6f 6e65 293a 0a20 2020  ublic=None):.   
+0003c780: 2020 2020 2023 2054 6865 206e 756d 6265       # The numbe
+0003c790: 7220 6f66 206c 6179 6572 7320 7468 6174  r of layers that
+0003c7a0: 2061 7265 2072 6574 7572 6e65 640a 2020   are returned.  
+0003c7b0: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
+0003c7c0: 203d 206c 696d 6974 2020 2320 7479 7065   = limit  # type
+0003c7d0: 3a20 696e 740a 2020 2020 2020 2020 2320  : int.        # 
+0003c7e0: 5468 6520 7061 6769 6e61 7469 6f6e 2074  The pagination t
+0003c7f0: 6f6b 656e 2074 6861 7420 6973 2075 7365  oken that is use
+0003c800: 6420 696e 2074 6865 206e 6578 7420 7265  d in the next re
+0003c810: 7175 6573 7420 746f 2072 6574 7269 6576  quest to retriev
+0003c820: 6520 6120 6e65 7720 7061 6765 206f 6620  e a new page of 
+0003c830: 7265 7375 6c74 732e 0a20 2020 2020 2020  results..       
+0003c840: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003c850: 203d 206e 6578 745f 746f 6b65 6e20 2023   = next_token  #
+0003c860: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+0003c870: 2020 2023 2053 7065 6369 6669 6573 2077     # Specifies w
+0003c880: 6865 7468 6572 2074 6865 206c 6179 6572  hether the layer
+0003c890: 2069 7320 6f66 6669 6369 616c 2e20 5661   is official. Va
+0003c8a0: 6c69 6420 7661 6c75 6573 3a20 7472 7565  lid values: true
+0003c8b0: 2061 6e64 2066 616c 7365 2e0a 2020 2020   and false..    
+0003c8c0: 2020 2020 7365 6c66 2e6f 6666 6963 6961      self.officia
+0003c8d0: 6c20 3d20 6f66 6669 6369 616c 2020 2320  l = official  # 
+0003c8e0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+0003c8f0: 2020 2320 5468 6520 6e61 6d65 2070 7265    # The name pre
+0003c900: 6669 7820 6f66 2074 6865 206c 6179 6572  fix of the layer
+0003c910: 2e0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+0003c920: 7265 6669 7820 3d20 7072 6566 6978 2020  refix = prefix  
+0003c930: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+0003c940: 2020 2020 2320 5370 6563 6966 6965 7320      # Specifies 
+0003c950: 7768 6574 6865 7220 7468 6520 6c61 7965  whether the laye
+0003c960: 7220 6973 2070 7562 6c69 632e 2056 616c  r is public. Val
+0003c970: 6964 2076 616c 7565 733a 2074 7275 6520  id values: true 
+0003c980: 616e 6420 6661 6c73 652e 0a20 2020 2020  and false..     
+0003c990: 2020 2073 656c 662e 7075 626c 6963 203d     self.public =
+0003c9a0: 2070 7562 6c69 6320 2023 2074 7970 653a   public  # type:
+0003c9b0: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
+0003c9c0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0003c9d0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0003c9e0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0003c9f0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0003ca00: 2073 7570 6572 284c 6973 744c 6179 6572   super(ListLayer
+0003ca10: 7352 6571 7565 7374 2c20 7365 6c66 292e  sRequest, self).
+0003ca20: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003ca30: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0003ca40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003ca50: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0003ca60: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0003ca70: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003ca80: 6620 7365 6c66 2e6c 696d 6974 2069 7320  f self.limit is 
+0003ca90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003caa0: 2020 2020 2020 7265 7375 6c74 5b27 6c69        result['li
+0003cab0: 6d69 7427 5d20 3d20 7365 6c66 2e6c 696d  mit'] = self.lim
+0003cac0: 6974 0a20 2020 2020 2020 2069 6620 7365  it.        if se
+0003cad0: 6c66 2e6e 6578 745f 746f 6b65 6e20 6973  lf.next_token is
+0003cae0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003caf0: 2020 2020 2020 2072 6573 756c 745b 276e         result['n
+0003cb00: 6578 7454 6f6b 656e 275d 203d 2073 656c  extToken'] = sel
+0003cb10: 662e 6e65 7874 5f74 6f6b 656e 0a20 2020  f.next_token.   
+0003cb20: 2020 2020 2069 6620 7365 6c66 2e6f 6666       if self.off
+0003cb30: 6963 6961 6c20 6973 206e 6f74 204e 6f6e  icial is not Non
+0003cb40: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003cb50: 6573 756c 745b 276f 6666 6963 6961 6c27  esult['official'
+0003cb60: 5d20 3d20 7365 6c66 2e6f 6666 6963 6961  ] = self.officia
+0003cb70: 6c0a 2020 2020 2020 2020 6966 2073 656c  l.        if sel
+0003cb80: 662e 7072 6566 6978 2069 7320 6e6f 7420  f.prefix is not 
+0003cb90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003cba0: 2020 7265 7375 6c74 5b27 7072 6566 6978    result['prefix
+0003cbb0: 275d 203d 2073 656c 662e 7072 6566 6978  '] = self.prefix
+0003cbc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003cbd0: 2e70 7562 6c69 6320 6973 206e 6f74 204e  .public is not N
+0003cbe0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003cbf0: 2072 6573 756c 745b 2770 7562 6c69 6327   result['public'
+0003cc00: 5d20 3d20 7365 6c66 2e70 7562 6c69 630a  ] = self.public.
+0003cc10: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003cc20: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003cc30: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0003cc40: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0003cc50: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0003cc60: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003cc70: 276c 696d 6974 2729 2069 7320 6e6f 7420  'limit') is not 
+0003cc80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003cc90: 2020 7365 6c66 2e6c 696d 6974 203d 206d    self.limit = m
+0003cca0: 2e67 6574 2827 6c69 6d69 7427 290a 2020  .get('limit').  
+0003ccb0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003ccc0: 6e65 7874 546f 6b65 6e27 2920 6973 206e  nextToken') is n
+0003ccd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003cce0: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
+0003ccf0: 6f6b 656e 203d 206d 2e67 6574 2827 6e65  oken = m.get('ne
+0003cd00: 7874 546f 6b65 6e27 290a 2020 2020 2020  xtToken').      
+0003cd10: 2020 6966 206d 2e67 6574 2827 6f66 6669    if m.get('offi
+0003cd20: 6369 616c 2729 2069 7320 6e6f 7420 4e6f  cial') is not No
+0003cd30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003cd40: 7365 6c66 2e6f 6666 6963 6961 6c20 3d20  self.official = 
+0003cd50: 6d2e 6765 7428 276f 6666 6963 6961 6c27  m.get('official'
+0003cd60: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003cd70: 6574 2827 7072 6566 6978 2729 2069 7320  et('prefix') is 
+0003cd80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003cd90: 2020 2020 2020 7365 6c66 2e70 7265 6669        self.prefi
+0003cda0: 7820 3d20 6d2e 6765 7428 2770 7265 6669  x = m.get('prefi
+0003cdb0: 7827 290a 2020 2020 2020 2020 6966 206d  x').        if m
+0003cdc0: 2e67 6574 2827 7075 626c 6963 2729 2069  .get('public') i
+0003cdd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003cde0: 2020 2020 2020 2020 7365 6c66 2e70 7562          self.pub
+0003cdf0: 6c69 6320 3d20 6d2e 6765 7428 2770 7562  lic = m.get('pub
+0003ce00: 6c69 6327 290a 2020 2020 2020 2020 7265  lic').        re
+0003ce10: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003ce20: 7320 4c69 7374 4c61 7965 7273 5265 7370  s ListLayersResp
+0003ce30: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+0003ce40: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0003ce50: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
+0003ce60: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
+0003ce70: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
+0003ce80: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0003ce90: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+0003cea0: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
+0003ceb0: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
+0003cec0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0003ced0: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+0003cee0: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+0003cef0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0003cf00: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
+0003cf10: 4c69 7374 4c61 7965 7273 4f75 7470 7574  ListLayersOutput
+0003cf20: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0003cf30: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0003cf40: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+0003cf50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003cf60: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+0003cf70: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0003cf80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0003cf90: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
+0003cfa0: 744c 6179 6572 7352 6573 706f 6e73 652c  tLayersResponse,
+0003cfb0: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+0003cfc0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0003cfd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003cfe0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0003cff0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0003d000: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0003d010: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+0003d020: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+0003d030: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003d040: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+0003d050: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+0003d060: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003d070: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+0003d080: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003d090: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+0003d0a0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+0003d0b0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+0003d0c0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+0003d0d0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0003d0e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003d0f0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+0003d100: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+0003d110: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0003d120: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0003d130: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+0003d140: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0003d150: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0003d160: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003d170: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+0003d180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003d190: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0003d1a0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+0003d1b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003d1c0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0003d1d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003d1e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003d1f0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+0003d200: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0003d210: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003d220: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+0003d230: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003d240: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+0003d250: 204c 6973 744c 6179 6572 734f 7574 7075   ListLayersOutpu
+0003d260: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+0003d270: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+0003d280: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+0003d290: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+0003d2a0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0003d2b0: 0a63 6c61 7373 204c 6973 7450 726f 7669  .class ListProvi
+0003d2c0: 7369 6f6e 436f 6e66 6967 7352 6571 7565  sionConfigsReque
+0003d2d0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+0003d2e0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0003d2f0: 656c 662c 2066 756e 6374 696f 6e5f 6e61  elf, function_na
+0003d300: 6d65 3d4e 6f6e 652c 206c 696d 6974 3d4e  me=None, limit=N
+0003d310: 6f6e 652c 206e 6578 745f 746f 6b65 6e3d  one, next_token=
+0003d320: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
+0003d330: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+0003d340: 2066 756e 6374 696f 6e2e 2049 6620 7468   function. If th
+0003d350: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
+0003d360: 6e6f 7420 7370 6563 6966 6965 642c 2074  not specified, t
+0003d370: 6865 2070 726f 7669 7369 6f6e 6564 2063  he provisioned c
+0003d380: 6f6e 6669 6775 7261 7469 6f6e 7320 6f66  onfigurations of
+0003d390: 2061 6c6c 2066 756e 6374 696f 6e73 2061   all functions a
+0003d3a0: 7265 206c 6973 7465 642e 0a20 2020 2020  re listed..     
+0003d3b0: 2020 2073 656c 662e 6675 6e63 7469 6f6e     self.function
+0003d3c0: 5f6e 616d 6520 3d20 6675 6e63 7469 6f6e  _name = function
+0003d3d0: 5f6e 616d 6520 2023 2074 7970 653a 2073  _name  # type: s
+0003d3e0: 7472 0a20 2020 2020 2020 2023 204e 756d  tr.        # Num
+0003d3f0: 6265 7220 6f66 2070 726f 7669 7369 6f6e  ber of provision
+0003d400: 6564 2063 6f6e 6669 6775 7261 7469 6f6e  ed configuration
+0003d410: 7320 746f 2072 6574 7572 6e2e 0a20 2020  s to return..   
+0003d420: 2020 2020 2073 656c 662e 6c69 6d69 7420       self.limit 
+0003d430: 3d20 6c69 6d69 7420 2023 2074 7970 653a  = limit  # type:
+0003d440: 2069 6e74 0a20 2020 2020 2020 2023 2041   int.        # A
+0003d450: 2070 6167 696e 6174 696f 6e20 746f 6b65   pagination toke
+0003d460: 6e2e 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+0003d470: 6e65 7874 5f74 6f6b 656e 203d 206e 6578  next_token = nex
+0003d480: 745f 746f 6b65 6e20 2023 2074 7970 653a  t_token  # type:
+0003d490: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
+0003d4a0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0003d4b0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0003d4c0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0003d4d0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0003d4e0: 2073 7570 6572 284c 6973 7450 726f 7669   super(ListProvi
+0003d4f0: 7369 6f6e 436f 6e66 6967 7352 6571 7565  sionConfigsReque
+0003d500: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
+0003d510: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0003d520: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0003d530: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0003d540: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0003d550: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0003d560: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003d570: 2e66 756e 6374 696f 6e5f 6e61 6d65 2069  .function_name i
+0003d580: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003d590: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003d5a0: 6675 6e63 7469 6f6e 4e61 6d65 275d 203d  functionName'] =
+0003d5b0: 2073 656c 662e 6675 6e63 7469 6f6e 5f6e   self.function_n
+0003d5c0: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
+0003d5d0: 656c 662e 6c69 6d69 7420 6973 206e 6f74  elf.limit is not
+0003d5e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003d5f0: 2020 2072 6573 756c 745b 276c 696d 6974     result['limit
+0003d600: 275d 203d 2073 656c 662e 6c69 6d69 740a  '] = self.limit.
+0003d610: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003d620: 6e65 7874 5f74 6f6b 656e 2069 7320 6e6f  next_token is no
+0003d630: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003d640: 2020 2020 7265 7375 6c74 5b27 6e65 7874      result['next
+0003d650: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e6e  Token'] = self.n
+0003d660: 6578 745f 746f 6b65 6e0a 2020 2020 2020  ext_token.      
+0003d670: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0003d680: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0003d690: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+0003d6a0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+0003d6b0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+0003d6c0: 2069 6620 6d2e 6765 7428 2766 756e 6374   if m.get('funct
+0003d6d0: 696f 6e4e 616d 6527 2920 6973 206e 6f74  ionName') is not
+0003d6e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003d6f0: 2020 2073 656c 662e 6675 6e63 7469 6f6e     self.function
+0003d700: 5f6e 616d 6520 3d20 6d2e 6765 7428 2766  _name = m.get('f
+0003d710: 756e 6374 696f 6e4e 616d 6527 290a 2020  unctionName').  
+0003d720: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003d730: 6c69 6d69 7427 2920 6973 206e 6f74 204e  limit') is not N
+0003d740: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003d750: 2073 656c 662e 6c69 6d69 7420 3d20 6d2e   self.limit = m.
+0003d760: 6765 7428 276c 696d 6974 2729 0a20 2020  get('limit').   
+0003d770: 2020 2020 2069 6620 6d2e 6765 7428 276e       if m.get('n
+0003d780: 6578 7454 6f6b 656e 2729 2069 7320 6e6f  extToken') is no
+0003d790: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003d7a0: 2020 2020 7365 6c66 2e6e 6578 745f 746f      self.next_to
+0003d7b0: 6b65 6e20 3d20 6d2e 6765 7428 276e 6578  ken = m.get('nex
+0003d7c0: 7454 6f6b 656e 2729 0a20 2020 2020 2020  tToken').       
+0003d7d0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+0003d7e0: 6c61 7373 204c 6973 7450 726f 7669 7369  lass ListProvisi
+0003d7f0: 6f6e 436f 6e66 6967 7352 6573 706f 6e73  onConfigsRespons
+0003d800: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+0003d810: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0003d820: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
+0003d830: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
+0003d840: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
+0003d850: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0003d860: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
+0003d870: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
+0003d880: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
+0003d890: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0003d8a0: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
+0003d8b0: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
+0003d8c0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+0003d8d0: 6f64 7920 2023 2074 7970 653a 204c 6973  ody  # type: Lis
+0003d8e0: 7450 726f 7669 7369 6f6e 436f 6e66 6967  tProvisionConfig
+0003d8f0: 734f 7574 7075 740a 0a20 2020 2064 6566  sOutput..    def
+0003d900: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0003d910: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003d920: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0003d930: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0003d940: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0003d950: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0003d960: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0003d970: 7065 7228 4c69 7374 5072 6f76 6973 696f  per(ListProvisio
+0003d980: 6e43 6f6e 6669 6773 5265 7370 6f6e 7365  nConfigsResponse
+0003d990: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+0003d9a0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0003d9b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003d9c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0003d9d0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0003d9e0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0003d9f0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0003da00: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0003da10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003da20: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0003da30: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0003da40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003da50: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0003da60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003da70: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0003da80: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0003da90: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0003daa0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0003dab0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0003dac0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003dad0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0003dae0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0003daf0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003db00: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003db10: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0003db20: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0003db30: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0003db40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003db50: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+0003db60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003db70: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0003db80: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+0003db90: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0003dba0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0003dbb0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003dbc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003dbd0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+0003dbe0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0003dbf0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003dc00: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+0003dc10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003dc20: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0003dc30: 3d20 4c69 7374 5072 6f76 6973 696f 6e43  = ListProvisionC
+0003dc40: 6f6e 6669 6773 4f75 7470 7574 2829 0a20  onfigsOutput(). 
+0003dc50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003dc60: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+0003dc70: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+0003dc80: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+0003dc90: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003dca0: 7320 4c69 7374 5461 6752 6573 6f75 7263  s ListTagResourc
+0003dcb0: 6573 5265 7175 6573 7454 6167 2854 6561  esRequestTag(Tea
+0003dcc0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0003dcd0: 5f5f 696e 6974 5f5f 2873 656c 662c 206b  __init__(self, k
+0003dce0: 6579 3d4e 6f6e 652c 2076 616c 7565 3d4e  ey=None, value=N
+0003dcf0: 6f6e 6529 3a0a 2020 2020 2020 2020 2320  one):.        # 
+0003dd00: 5468 6520 7461 6720 6b65 792e 0a20 2020  The tag key..   
+0003dd10: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+0003dd20: 2320 5468 6520 7461 6720 6b65 7920 6361  # The tag key ca
+0003dd30: 6e20 6265 2075 7020 746f 2036 3420 6368  n be up to 64 ch
+0003dd40: 6172 6163 7465 7273 2069 6e20 6c65 6e67  aracters in leng
+0003dd50: 7468 2c20 616e 6420 6361 6e6e 6f74 2063  th, and cannot c
+0003dd60: 6f6e 7461 696e 2060 6874 7470 3a2f 2f60  ontain `http://`
+0003dd70: 206f 7220 6068 7474 7073 3a2f 2f60 2e20   or `https://`. 
+0003dd80: 5468 6520 7461 6720 6b65 7920 6361 6e6e  The tag key cann
+0003dd90: 6f74 2073 7461 7274 2077 6974 6820 6061  ot start with `a
+0003dda0: 6c69 7975 6e60 206f 7220 6061 6373 3a60  liyun` or `acs:`
+0003ddb0: 2e0a 2020 2020 2020 2020 7365 6c66 2e6b  ..        self.k
+0003ddc0: 6579 203d 206b 6579 2020 2320 7479 7065  ey = key  # type
+0003ddd0: 3a20 7374 720a 2020 2020 2020 2020 2320  : str.        # 
+0003dde0: 5468 6520 7461 6720 7661 6c75 652e 0a20  The tag value.. 
+0003ddf0: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+0003de00: 2020 2320 5468 6520 7461 6720 7661 6c75    # The tag valu
+0003de10: 6520 6361 6e20 6265 2075 7020 746f 2031  e can be up to 1
+0003de20: 3238 2063 6861 7261 6374 6572 7320 696e  28 characters in
+0003de30: 206c 656e 6774 6820 616e 6420 6361 6e20   length and can 
+0003de40: 6265 2061 6e20 656d 7074 7920 7374 7269  be an empty stri
+0003de50: 6e67 2e0a 2020 2020 2020 2020 7365 6c66  ng..        self
+0003de60: 2e76 616c 7565 203d 2076 616c 7565 2020  .value = value  
+0003de70: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
+0003de80: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0003de90: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0003dea0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+0003deb0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0003dec0: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
+0003ded0: 7374 5461 6752 6573 6f75 7263 6573 5265  stTagResourcesRe
+0003dee0: 7175 6573 7454 6167 2c20 7365 6c66 292e  questTag, self).
+0003def0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003df00: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0003df10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003df20: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0003df30: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0003df40: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003df50: 6620 7365 6c66 2e6b 6579 2069 7320 6e6f  f self.key is no
+0003df60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003df70: 2020 2020 7265 7375 6c74 5b27 4b65 7927      result['Key'
+0003df80: 5d20 3d20 7365 6c66 2e6b 6579 0a20 2020  ] = self.key.   
+0003df90: 2020 2020 2069 6620 7365 6c66 2e76 616c       if self.val
+0003dfa0: 7565 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ue is not None:.
+0003dfb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003dfc0: 6c74 5b27 5661 6c75 6527 5d20 3d20 7365  lt['Value'] = se
+0003dfd0: 6c66 2e76 616c 7565 0a20 2020 2020 2020  lf.value.       
+0003dfe0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0003dff0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0003e000: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+0003e010: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0003e020: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0003e030: 6966 206d 2e67 6574 2827 4b65 7927 2920  if m.get('Key') 
+0003e040: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003e050: 2020 2020 2020 2020 2073 656c 662e 6b65           self.ke
+0003e060: 7920 3d20 6d2e 6765 7428 274b 6579 2729  y = m.get('Key')
+0003e070: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003e080: 7428 2756 616c 7565 2729 2069 7320 6e6f  t('Value') is no
+0003e090: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003e0a0: 2020 2020 7365 6c66 2e76 616c 7565 203d      self.value =
+0003e0b0: 206d 2e67 6574 2827 5661 6c75 6527 290a   m.get('Value').
+0003e0c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0003e0d0: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
+0003e0e0: 5461 6752 6573 6f75 7263 6573 5265 7175  TagResourcesRequ
+0003e0f0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+0003e100: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0003e110: 7365 6c66 2c20 6c69 6d69 743d 4e6f 6e65  self, limit=None
+0003e120: 2c20 6e65 7874 5f74 6f6b 656e 3d4e 6f6e  , next_token=Non
+0003e130: 652c 2072 6573 6f75 7263 655f 6964 3d4e  e, resource_id=N
+0003e140: 6f6e 652c 2072 6573 6f75 7263 655f 7479  one, resource_ty
+0003e150: 7065 3d4e 6f6e 652c 2074 6167 3d4e 6f6e  pe=None, tag=Non
+0003e160: 6529 3a0a 2020 2020 2020 2020 2320 5468  e):.        # Th
+0003e170: 6520 6e75 6d62 6572 206f 6620 7265 736f  e number of reso
+0003e180: 7572 6365 7320 746f 2072 6574 7572 6e2e  urces to return.
+0003e190: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+0003e1a0: 6d69 7420 3d20 6c69 6d69 7420 2023 2074  mit = limit  # t
+0003e1b0: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+0003e1c0: 2023 2054 6865 2070 6167 696e 6174 696f   # The paginatio
+0003e1d0: 6e20 746f 6b65 6e20 7468 6174 2069 7320  n token that is 
+0003e1e0: 7573 6564 2069 6e20 7468 6520 6e65 7874  used in the next
+0003e1f0: 2072 6571 7565 7374 2074 6f20 7265 7472   request to retr
+0003e200: 6965 7665 2061 206e 6577 2070 6167 6520  ieve a new page 
+0003e210: 6f66 2072 6573 756c 7473 2e0a 2020 2020  of results..    
+0003e220: 2020 2020 7365 6c66 2e6e 6578 745f 746f      self.next_to
+0003e230: 6b65 6e20 3d20 6e65 7874 5f74 6f6b 656e  ken = next_token
+0003e240: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0003e250: 2020 2020 2020 2320 5468 6520 7265 736f        # The reso
+0003e260: 7572 6365 2049 4473 2e0a 2020 2020 2020  urce IDs..      
+0003e270: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+0003e280: 6964 203d 2072 6573 6f75 7263 655f 6964  id = resource_id
+0003e290: 2020 2320 7479 7065 3a20 6c69 7374 5b73    # type: list[s
+0003e2a0: 7472 5d0a 2020 2020 2020 2020 2320 5468  tr].        # Th
+0003e2b0: 6520 7265 736f 7572 6365 2074 7970 652e  e resource type.
+0003e2c0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0003e2d0: 736f 7572 6365 5f74 7970 6520 3d20 7265  source_type = re
+0003e2e0: 736f 7572 6365 5f74 7970 6520 2023 2074  source_type  # t
+0003e2f0: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+0003e300: 2023 2054 6865 2074 6167 732e 0a20 2020   # The tags..   
+0003e310: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+0003e320: 2320 596f 7520 6361 6e20 7175 6572 7920  # You can query 
+0003e330: 7570 2074 6f20 3230 2074 6167 7320 6174  up to 20 tags at
+0003e340: 2061 2074 696d 652e 0a20 2020 2020 2020   a time..       
+0003e350: 2073 656c 662e 7461 6720 3d20 7461 6720   self.tag = tag 
+0003e360: 2023 2074 7970 653a 206c 6973 745b 4c69   # type: list[Li
+0003e370: 7374 5461 6752 6573 6f75 7263 6573 5265  stTagResourcesRe
+0003e380: 7175 6573 7454 6167 5d0a 0a20 2020 2064  questTag]..    d
+0003e390: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0003e3a0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+0003e3b0: 6c66 2e74 6167 3a0a 2020 2020 2020 2020  lf.tag:.        
+0003e3c0: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+0003e3d0: 662e 7461 673a 0a20 2020 2020 2020 2020  f.tag:.         
+0003e3e0: 2020 2020 2020 2069 6620 6b3a 0a20 2020         if k:.   
+0003e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e400: 206b 2e76 616c 6964 6174 6528 290a 0a20   k.validate().. 
+0003e410: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+0003e420: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+0003e430: 7020 3d20 7375 7065 7228 4c69 7374 5461  p = super(ListTa
+0003e440: 6752 6573 6f75 7263 6573 5265 7175 6573  gResourcesReques
+0003e450: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
+0003e460: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0003e470: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0003e480: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0003e490: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0003e4a0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0003e4b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003e4c0: 6c69 6d69 7420 6973 206e 6f74 204e 6f6e  limit is not Non
+0003e4d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003e4e0: 6573 756c 745b 274c 696d 6974 275d 203d  esult['Limit'] =
+0003e4f0: 2073 656c 662e 6c69 6d69 740a 2020 2020   self.limit.    
+0003e500: 2020 2020 6966 2073 656c 662e 6e65 7874      if self.next
+0003e510: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
+0003e520: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003e530: 7265 7375 6c74 5b27 4e65 7874 546f 6b65  result['NextToke
+0003e540: 6e27 5d20 3d20 7365 6c66 2e6e 6578 745f  n'] = self.next_
+0003e550: 746f 6b65 6e0a 2020 2020 2020 2020 6966  token.        if
+0003e560: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+0003e570: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0003e580: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003e590: 745b 2752 6573 6f75 7263 6549 6427 5d20  t['ResourceId'] 
+0003e5a0: 3d20 7365 6c66 2e72 6573 6f75 7263 655f  = self.resource_
+0003e5b0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0003e5c0: 6c66 2e72 6573 6f75 7263 655f 7479 7065  lf.resource_type
+0003e5d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003e5e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003e5f0: 5b27 5265 736f 7572 6365 5479 7065 275d  ['ResourceType']
+0003e600: 203d 2073 656c 662e 7265 736f 7572 6365   = self.resource
+0003e610: 5f74 7970 650a 2020 2020 2020 2020 7265  _type.        re
+0003e620: 7375 6c74 5b27 5461 6727 5d20 3d20 5b5d  sult['Tag'] = []
+0003e630: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003e640: 2e74 6167 2069 7320 6e6f 7420 4e6f 6e65  .tag is not None
+0003e650: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0003e660: 7220 6b20 696e 2073 656c 662e 7461 673a  r k in self.tag:
+0003e670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003e680: 2072 6573 756c 745b 2754 6167 275d 2e61   result['Tag'].a
+0003e690: 7070 656e 6428 6b2e 746f 5f6d 6170 2829  ppend(k.to_map()
+0003e6a0: 2069 6620 6b20 656c 7365 204e 6f6e 6529   if k else None)
+0003e6b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003e6c0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0003e6d0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0003e6e0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0003e6f0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+0003e700: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0003e710: 2827 4c69 6d69 7427 2920 6973 206e 6f74  ('Limit') is not
+0003e720: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003e730: 2020 2073 656c 662e 6c69 6d69 7420 3d20     self.limit = 
+0003e740: 6d2e 6765 7428 274c 696d 6974 2729 0a20  m.get('Limit'). 
+0003e750: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003e760: 274e 6578 7454 6f6b 656e 2729 2069 7320  'NextToken') is 
+0003e770: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003e780: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
+0003e790: 746f 6b65 6e20 3d20 6d2e 6765 7428 274e  token = m.get('N
+0003e7a0: 6578 7454 6f6b 656e 2729 0a20 2020 2020  extToken').     
+0003e7b0: 2020 2069 6620 6d2e 6765 7428 2752 6573     if m.get('Res
+0003e7c0: 6f75 7263 6549 6427 2920 6973 206e 6f74  ourceId') is not
+0003e7d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003e7e0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+0003e7f0: 5f69 6420 3d20 6d2e 6765 7428 2752 6573  _id = m.get('Res
+0003e800: 6f75 7263 6549 6427 290a 2020 2020 2020  ourceId').      
+0003e810: 2020 6966 206d 2e67 6574 2827 5265 736f    if m.get('Reso
+0003e820: 7572 6365 5479 7065 2729 2069 7320 6e6f  urceType') is no
+0003e830: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003e840: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
+0003e850: 655f 7479 7065 203d 206d 2e67 6574 2827  e_type = m.get('
+0003e860: 5265 736f 7572 6365 5479 7065 2729 0a20  ResourceType'). 
+0003e870: 2020 2020 2020 2073 656c 662e 7461 6720         self.tag 
+0003e880: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
+0003e890: 6d2e 6765 7428 2754 6167 2729 2069 7320  m.get('Tag') is 
+0003e8a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003e8b0: 2020 2020 2020 666f 7220 6b20 696e 206d        for k in m
+0003e8c0: 2e67 6574 2827 5461 6727 293a 0a20 2020  .get('Tag'):.   
+0003e8d0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0003e8e0: 705f 6d6f 6465 6c20 3d20 4c69 7374 5461  p_model = ListTa
+0003e8f0: 6752 6573 6f75 7263 6573 5265 7175 6573  gResourcesReques
+0003e900: 7454 6167 2829 0a20 2020 2020 2020 2020  tTag().         
+0003e910: 2020 2020 2020 2073 656c 662e 7461 672e         self.tag.
+0003e920: 6170 7065 6e64 2874 656d 705f 6d6f 6465  append(temp_mode
+0003e930: 6c2e 6672 6f6d 5f6d 6170 286b 2929 0a20  l.from_map(k)). 
+0003e940: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0003e950: 6c66 0a0a 0a63 6c61 7373 204c 6973 7454  lf...class ListT
+0003e960: 6167 5265 736f 7572 6365 7353 6872 696e  agResourcesShrin
+0003e970: 6b52 6571 7565 7374 2854 6561 4d6f 6465  kRequest(TeaMode
+0003e980: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+0003e990: 6974 5f5f 2873 656c 662c 206c 696d 6974  it__(self, limit
+0003e9a0: 3d4e 6f6e 652c 206e 6578 745f 746f 6b65  =None, next_toke
+0003e9b0: 6e3d 4e6f 6e65 2c20 7265 736f 7572 6365  n=None, resource
+0003e9c0: 5f69 645f 7368 7269 6e6b 3d4e 6f6e 652c  _id_shrink=None,
+0003e9d0: 2072 6573 6f75 7263 655f 7479 7065 3d4e   resource_type=N
+0003e9e0: 6f6e 652c 2074 6167 5f73 6872 696e 6b3d  one, tag_shrink=
+0003e9f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
+0003ea00: 2054 6865 206e 756d 6265 7220 6f66 2072   The number of r
+0003ea10: 6573 6f75 7263 6573 2074 6f20 7265 7475  esources to retu
+0003ea20: 726e 2e0a 2020 2020 2020 2020 7365 6c66  rn..        self
+0003ea30: 2e6c 696d 6974 203d 206c 696d 6974 2020  .limit = limit  
+0003ea40: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
+0003ea50: 2020 2020 2320 5468 6520 7061 6769 6e61      # The pagina
+0003ea60: 7469 6f6e 2074 6f6b 656e 2074 6861 7420  tion token that 
+0003ea70: 6973 2075 7365 6420 696e 2074 6865 206e  is used in the n
+0003ea80: 6578 7420 7265 7175 6573 7420 746f 2072  ext request to r
+0003ea90: 6574 7269 6576 6520 6120 6e65 7720 7061  etrieve a new pa
+0003eaa0: 6765 206f 6620 7265 7375 6c74 732e 0a20  ge of results.. 
+0003eab0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
+0003eac0: 5f74 6f6b 656e 203d 206e 6578 745f 746f  _token = next_to
+0003ead0: 6b65 6e20 2023 2074 7970 653a 2073 7472  ken  # type: str
+0003eae0: 0a20 2020 2020 2020 2023 2054 6865 2072  .        # The r
+0003eaf0: 6573 6f75 7263 6520 4944 732e 0a20 2020  esource IDs..   
+0003eb00: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+0003eb10: 6365 5f69 645f 7368 7269 6e6b 203d 2072  ce_id_shrink = r
+0003eb20: 6573 6f75 7263 655f 6964 5f73 6872 696e  esource_id_shrin
+0003eb30: 6b20 2023 2074 7970 653a 2073 7472 0a20  k  # type: str. 
+0003eb40: 2020 2020 2020 2023 2054 6865 2072 6573         # The res
+0003eb50: 6f75 7263 6520 7479 7065 2e0a 2020 2020  ource type..    
+0003eb60: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
+0003eb70: 655f 7479 7065 203d 2072 6573 6f75 7263  e_type = resourc
+0003eb80: 655f 7479 7065 2020 2320 7479 7065 3a20  e_type  # type: 
+0003eb90: 7374 720a 2020 2020 2020 2020 2320 5468  str.        # Th
+0003eba0: 6520 7461 6773 2e0a 2020 2020 2020 2020  e tags..        
+0003ebb0: 2320 0a20 2020 2020 2020 2023 2059 6f75  # .        # You
+0003ebc0: 2063 616e 2071 7565 7279 2075 7020 746f   can query up to
+0003ebd0: 2032 3020 7461 6773 2061 7420 6120 7469   20 tags at a ti
+0003ebe0: 6d65 2e0a 2020 2020 2020 2020 7365 6c66  me..        self
+0003ebf0: 2e74 6167 5f73 6872 696e 6b20 3d20 7461  .tag_shrink = ta
+0003ec00: 675f 7368 7269 6e6b 2020 2320 7479 7065  g_shrink  # type
+0003ec10: 3a20 7374 720a 0a20 2020 2064 6566 2076  : str..    def v
+0003ec20: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0003ec30: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0003ec40: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0003ec50: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0003ec60: 3d20 7375 7065 7228 4c69 7374 5461 6752  = super(ListTagR
+0003ec70: 6573 6f75 7263 6573 5368 7269 6e6b 5265  esourcesShrinkRe
+0003ec80: 7175 6573 742c 2073 656c 6629 2e74 6f5f  quest, self).to_
+0003ec90: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+0003eca0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+0003ecb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003ecc0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+0003ecd0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+0003ece0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0003ecf0: 656c 662e 6c69 6d69 7420 6973 206e 6f74  elf.limit is not
+0003ed00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003ed10: 2020 2072 6573 756c 745b 274c 696d 6974     result['Limit
+0003ed20: 275d 203d 2073 656c 662e 6c69 6d69 740a  '] = self.limit.
+0003ed30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003ed40: 6e65 7874 5f74 6f6b 656e 2069 7320 6e6f  next_token is no
+0003ed50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003ed60: 2020 2020 7265 7375 6c74 5b27 4e65 7874      result['Next
+0003ed70: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e6e  Token'] = self.n
+0003ed80: 6578 745f 746f 6b65 6e0a 2020 2020 2020  ext_token.      
+0003ed90: 2020 6966 2073 656c 662e 7265 736f 7572    if self.resour
+0003eda0: 6365 5f69 645f 7368 7269 6e6b 2069 7320  ce_id_shrink is 
+0003edb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003edc0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+0003edd0: 736f 7572 6365 4964 275d 203d 2073 656c  sourceId'] = sel
+0003ede0: 662e 7265 736f 7572 6365 5f69 645f 7368  f.resource_id_sh
+0003edf0: 7269 6e6b 0a20 2020 2020 2020 2069 6620  rink.        if 
+0003ee00: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
+0003ee10: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
+0003ee20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003ee30: 6c74 5b27 5265 736f 7572 6365 5479 7065  lt['ResourceType
+0003ee40: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+0003ee50: 6365 5f74 7970 650a 2020 2020 2020 2020  ce_type.        
+0003ee60: 6966 2073 656c 662e 7461 675f 7368 7269  if self.tag_shri
+0003ee70: 6e6b 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nk is not None:.
+0003ee80: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003ee90: 6c74 5b27 5461 6727 5d20 3d20 7365 6c66  lt['Tag'] = self
+0003eea0: 2e74 6167 5f73 6872 696e 6b0a 2020 2020  .tag_shrink.    
+0003eeb0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0003eec0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+0003eed0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+0003eee0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0003eef0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0003ef00: 2020 2069 6620 6d2e 6765 7428 274c 696d     if m.get('Lim
+0003ef10: 6974 2729 2069 7320 6e6f 7420 4e6f 6e65  it') is not None
+0003ef20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003ef30: 6c66 2e6c 696d 6974 203d 206d 2e67 6574  lf.limit = m.get
+0003ef40: 2827 4c69 6d69 7427 290a 2020 2020 2020  ('Limit').      
+0003ef50: 2020 6966 206d 2e67 6574 2827 4e65 7874    if m.get('Next
+0003ef60: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
+0003ef70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003ef80: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003ef90: 203d 206d 2e67 6574 2827 4e65 7874 546f   = m.get('NextTo
+0003efa0: 6b65 6e27 290a 2020 2020 2020 2020 6966  ken').        if
+0003efb0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+0003efc0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0003efd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003efe0: 6c66 2e72 6573 6f75 7263 655f 6964 5f73  lf.resource_id_s
+0003eff0: 6872 696e 6b20 3d20 6d2e 6765 7428 2752  hrink = m.get('R
+0003f000: 6573 6f75 7263 6549 6427 290a 2020 2020  esourceId').    
+0003f010: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+0003f020: 736f 7572 6365 5479 7065 2729 2069 7320  sourceType') is 
+0003f030: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003f040: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+0003f050: 7263 655f 7479 7065 203d 206d 2e67 6574  rce_type = m.get
+0003f060: 2827 5265 736f 7572 6365 5479 7065 2729  ('ResourceType')
+0003f070: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003f080: 7428 2754 6167 2729 2069 7320 6e6f 7420  t('Tag') is not 
+0003f090: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003f0a0: 2020 7365 6c66 2e74 6167 5f73 6872 696e    self.tag_shrin
+0003f0b0: 6b20 3d20 6d2e 6765 7428 2754 6167 2729  k = m.get('Tag')
+0003f0c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003f0d0: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+0003f0e0: 7454 6167 5265 736f 7572 6365 7352 6573  tTagResourcesRes
+0003f0f0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
+0003f100: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0003f110: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
+0003f120: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
+0003f130: 653d 4e6f 6e65 2c20 626f 6479 3d4e 6f6e  e=None, body=Non
+0003f140: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+0003f150: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+0003f160: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
+0003f170: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
+0003f180: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+0003f190: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+0003f1a0: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
+0003f1b0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0003f1c0: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
+0003f1d0: 204c 6973 7454 6167 5265 736f 7572 6365   ListTagResource
+0003f1e0: 734f 7574 7075 740a 0a20 2020 2064 6566  sOutput..    def
+0003f1f0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0003f200: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003f210: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0003f220: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0003f230: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0003f240: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0003f250: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0003f260: 7065 7228 4c69 7374 5461 6752 6573 6f75  per(ListTagResou
+0003f270: 7263 6573 5265 7370 6f6e 7365 2c20 7365  rcesResponse, se
+0003f280: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+0003f290: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0003f2a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003f2b0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0003f2c0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0003f2d0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0003f2e0: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+0003f2f0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+0003f300: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003f310: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+0003f320: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+0003f330: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+0003f340: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
+0003f350: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003f360: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
+0003f370: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
+0003f380: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+0003f390: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
+0003f3a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003f3b0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003f3c0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
+0003f3d0: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
+0003f3e0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0003f3f0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+0003f400: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+0003f410: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0003f420: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0003f430: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+0003f440: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+0003f450: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003f460: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+0003f470: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+0003f480: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0003f490: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+0003f4a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003f4b0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0003f4c0: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+0003f4d0: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+0003f4e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003f4f0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+0003f500: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003f510: 2074 656d 705f 6d6f 6465 6c20 3d20 4c69   temp_model = Li
+0003f520: 7374 5461 6752 6573 6f75 7263 6573 4f75  stTagResourcesOu
+0003f530: 7470 7574 2829 0a20 2020 2020 2020 2020  tput().         
+0003f540: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0003f550: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0003f560: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0003f570: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0003f580: 660a 0a0a 636c 6173 7320 4c69 7374 5472  f...class ListTr
+0003f590: 6967 6765 7273 5265 7175 6573 7428 5465  iggersRequest(Te
+0003f5a0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0003f5b0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0003f5c0: 6c69 6d69 743d 4e6f 6e65 2c20 6e65 7874  limit=None, next
+0003f5d0: 5f74 6f6b 656e 3d4e 6f6e 652c 2070 7265  _token=None, pre
+0003f5e0: 6669 783d 4e6f 6e65 293a 0a20 2020 2020  fix=None):.     
+0003f5f0: 2020 2023 2054 6865 206e 756d 6265 7220     # The number 
+0003f600: 6f66 2074 7269 6767 6572 7320 7265 7475  of triggers retu
+0003f610: 726e 6564 2e0a 2020 2020 2020 2020 7365  rned..        se
+0003f620: 6c66 2e6c 696d 6974 203d 206c 696d 6974  lf.limit = limit
+0003f630: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+0003f640: 2020 2020 2020 2320 5468 6520 746f 6b65        # The toke
+0003f650: 6e20 666f 7220 7468 6520 6e65 7874 2070  n for the next p
+0003f660: 6167 652e 0a20 2020 2020 2020 2073 656c  age..        sel
+0003f670: 662e 6e65 7874 5f74 6f6b 656e 203d 206e  f.next_token = n
+0003f680: 6578 745f 746f 6b65 6e20 2023 2074 7970  ext_token  # typ
+0003f690: 653a 2073 7472 0a20 2020 2020 2020 2023  e: str.        #
+0003f6a0: 2054 6865 2074 7269 6767 6572 206e 616d   The trigger nam
+0003f6b0: 6520 7072 6566 6978 2e0a 2020 2020 2020  e prefix..      
+0003f6c0: 2020 7365 6c66 2e70 7265 6669 7820 3d20    self.prefix = 
+0003f6d0: 7072 6566 6978 2020 2320 7479 7065 3a20  prefix  # type: 
+0003f6e0: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+0003f6f0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0003f700: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0003f710: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0003f720: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0003f730: 7375 7065 7228 4c69 7374 5472 6967 6765  super(ListTrigge
+0003f740: 7273 5265 7175 6573 742c 2073 656c 6629  rsRequest, self)
+0003f750: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0003f760: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0003f770: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003f780: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0003f790: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0003f7a0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0003f7b0: 6966 2073 656c 662e 6c69 6d69 7420 6973  if self.limit is
+0003f7c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003f7d0: 2020 2020 2020 2072 6573 756c 745b 276c         result['l
+0003f7e0: 696d 6974 275d 203d 2073 656c 662e 6c69  imit'] = self.li
+0003f7f0: 6d69 740a 2020 2020 2020 2020 6966 2073  mit.        if s
+0003f800: 656c 662e 6e65 7874 5f74 6f6b 656e 2069  elf.next_token i
+0003f810: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003f820: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003f830: 6e65 7874 546f 6b65 6e27 5d20 3d20 7365  nextToken'] = se
+0003f840: 6c66 2e6e 6578 745f 746f 6b65 6e0a 2020  lf.next_token.  
+0003f850: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0003f860: 6566 6978 2069 7320 6e6f 7420 4e6f 6e65  efix is not None
+0003f870: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003f880: 7375 6c74 5b27 7072 6566 6978 275d 203d  sult['prefix'] =
+0003f890: 2073 656c 662e 7072 6566 6978 0a20 2020   self.prefix.   
+0003f8a0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+0003f8b0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+0003f8c0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+0003f8d0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+0003f8e0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+0003f8f0: 2020 2020 6966 206d 2e67 6574 2827 6c69      if m.get('li
+0003f900: 6d69 7427 2920 6973 206e 6f74 204e 6f6e  mit') is not Non
+0003f910: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0003f920: 656c 662e 6c69 6d69 7420 3d20 6d2e 6765  elf.limit = m.ge
+0003f930: 7428 276c 696d 6974 2729 0a20 2020 2020  t('limit').     
+0003f940: 2020 2069 6620 6d2e 6765 7428 276e 6578     if m.get('nex
+0003f950: 7454 6f6b 656e 2729 2069 7320 6e6f 7420  tToken') is not 
+0003f960: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003f970: 2020 7365 6c66 2e6e 6578 745f 746f 6b65    self.next_toke
+0003f980: 6e20 3d20 6d2e 6765 7428 276e 6578 7454  n = m.get('nextT
+0003f990: 6f6b 656e 2729 0a20 2020 2020 2020 2069  oken').        i
+0003f9a0: 6620 6d2e 6765 7428 2770 7265 6669 7827  f m.get('prefix'
+0003f9b0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003f9c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003f9d0: 7072 6566 6978 203d 206d 2e67 6574 2827  prefix = m.get('
+0003f9e0: 7072 6566 6978 2729 0a20 2020 2020 2020  prefix').       
+0003f9f0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+0003fa00: 6c61 7373 204c 6973 7454 7269 6767 6572  lass ListTrigger
+0003fa10: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
+0003fa20: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0003fa30: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
+0003fa40: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
+0003fa50: 5f63 6f64 653d 4e6f 6e65 2c20 626f 6479  _code=None, body
+0003fa60: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0003fa70: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+0003fa80: 6561 6465 7273 2020 2320 7479 7065 3a20  eaders  # type: 
+0003fa90: 6469 6374 5b73 7472 2c20 7374 725d 0a20  dict[str, str]. 
+0003faa0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0003fab0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+0003fac0: 5f63 6f64 6520 2023 2074 7970 653a 2069  _code  # type: i
+0003fad0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+0003fae0: 626f 6479 203d 2062 6f64 7920 2023 2074  body = body  # t
+0003faf0: 7970 653a 204c 6973 7454 7269 6767 6572  ype: ListTrigger
+0003fb00: 734f 7574 7075 740a 0a20 2020 2064 6566  sOutput..    def
+0003fb10: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0003fb20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003fb30: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0003fb40: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0003fb50: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0003fb60: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0003fb70: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0003fb80: 7065 7228 4c69 7374 5472 6967 6765 7273  per(ListTriggers
+0003fb90: 5265 7370 6f6e 7365 2c20 7365 6c66 292e  Response, self).
+0003fba0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003fbb0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0003fbc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003fbd0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0003fbe0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0003fbf0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003fc00: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+0003fc10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003fc20: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003fc30: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+0003fc40: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+0003fc50: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+0003fc60: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+0003fc70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003fc80: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+0003fc90: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+0003fca0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+0003fcb0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+0003fcc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003fcd0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+0003fce0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+0003fcf0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0003fd00: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0003fd10: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0003fd20: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
+0003fd30: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003fd40: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003fd50: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+0003fd60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003fd70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003fd80: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+0003fd90: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+0003fda0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+0003fdb0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+0003fdc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003fdd0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0003fde0: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+0003fdf0: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+0003fe00: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+0003fe10: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0003fe20: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0003fe30: 705f 6d6f 6465 6c20 3d20 4c69 7374 5472  p_model = ListTr
+0003fe40: 6967 6765 7273 4f75 7470 7574 2829 0a20  iggersOutput(). 
+0003fe50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003fe60: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+0003fe70: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+0003fe80: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+0003fe90: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003fea0: 7320 4c69 7374 5670 6342 696e 6469 6e67  s ListVpcBinding
+0003feb0: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
+0003fec0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0003fed0: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
+0003fee0: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
+0003fef0: 5f63 6f64 653d 4e6f 6e65 2c20 626f 6479  _code=None, body
+0003ff00: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0003ff10: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+0003ff20: 6561 6465 7273 2020 2320 7479 7065 3a20  eaders  # type: 
+0003ff30: 6469 6374 5b73 7472 2c20 7374 725d 0a20  dict[str, str]. 
+0003ff40: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0003ff50: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+0003ff60: 5f63 6f64 6520 2023 2074 7970 653a 2069  _code  # type: i
+0003ff70: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+0003ff80: 626f 6479 203d 2062 6f64 7920 2023 2074  body = body  # t
+0003ff90: 7970 653a 204c 6973 7456 7063 4269 6e64  ype: ListVpcBind
+0003ffa0: 696e 6773 4f75 7470 7574 0a0a 2020 2020  ingsOutput..    
+0003ffb0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0003ffc0: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+0003ffd0: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+0003ffe0: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+0003fff0: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00040000: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00040010: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00040020: 2073 7570 6572 284c 6973 7456 7063 4269   super(ListVpcBi
+00040030: 6e64 696e 6773 5265 7370 6f6e 7365 2c20  ndingsResponse, 
+00040040: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+00040050: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00040060: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00040070: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00040080: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00040090: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000400a0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+000400b0: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+000400c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000400d0: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+000400e0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+000400f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00040100: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+00040110: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00040120: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+00040130: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+00040140: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00040150: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00040160: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00040170: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00040180: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00040190: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+000401a0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000401b0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000401c0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+000401d0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000401e0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000401f0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+00040200: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+00040210: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00040220: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00040230: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00040240: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00040250: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00040260: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00040270: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00040280: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+00040290: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000402a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000402b0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+000402c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000402d0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+000402e0: 4c69 7374 5670 6342 696e 6469 6e67 734f  ListVpcBindingsO
+000402f0: 7574 7075 7428 290a 2020 2020 2020 2020  utput().        
+00040300: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00040310: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+00040320: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+00040330: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00040340: 6c66 0a0a 0a63 6c61 7373 2050 7562 6c69  lf...class Publi
+00040350: 7368 4675 6e63 7469 6f6e 5665 7273 696f  shFunctionVersio
+00040360: 6e52 6571 7565 7374 2854 6561 4d6f 6465  nRequest(TeaMode
+00040370: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00040380: 6974 5f5f 2873 656c 662c 2062 6f64 793d  it__(self, body=
+00040390: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
+000403a0: 2054 6865 2069 6e66 6f72 6d61 7469 6f6e   The information
+000403b0: 2061 626f 7574 2074 6865 2066 756e 6374   about the funct
+000403c0: 696f 6e20 7665 7273 696f 6e2e 0a20 2020  ion version..   
+000403d0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+000403e0: 2062 6f64 7920 2023 2074 7970 653a 2050   body  # type: P
+000403f0: 7562 6c69 7368 5665 7273 696f 6e49 6e70  ublishVersionInp
+00040400: 7574 0a0a 2020 2020 6465 6620 7661 6c69  ut..    def vali
+00040410: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00040420: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00040430: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00040440: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00040450: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00040460: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00040470: 2020 5f6d 6170 203d 2073 7570 6572 2850    _map = super(P
+00040480: 7562 6c69 7368 4675 6e63 7469 6f6e 5665  ublishFunctionVe
+00040490: 7273 696f 6e52 6571 7565 7374 2c20 7365  rsionRequest, se
+000404a0: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+000404b0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+000404c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000404d0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+000404e0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+000404f0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00040500: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00040510: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00040520: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00040530: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00040540: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00040550: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00040560: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00040570: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00040580: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00040590: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000405a0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+000405b0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+000405c0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+000405d0: 6d70 5f6d 6f64 656c 203d 2050 7562 6c69  mp_model = Publi
+000405e0: 7368 5665 7273 696f 6e49 6e70 7574 2829  shVersionInput()
+000405f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00040600: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+00040610: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00040620: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+00040630: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00040640: 6173 7320 5075 626c 6973 6846 756e 6374  ass PublishFunct
+00040650: 696f 6e56 6572 7369 6f6e 5265 7370 6f6e  ionVersionRespon
+00040660: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00040670: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00040680: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
+00040690: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
+000406a0: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
+000406b0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000406c0: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
+000406d0: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
+000406e0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
+000406f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00040700: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
+00040710: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
+00040720: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00040730: 626f 6479 2020 2320 7479 7065 3a20 5665  body  # type: Ve
+00040740: 7273 696f 6e0a 0a20 2020 2064 6566 2076  rsion..    def v
+00040750: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00040760: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00040770: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+00040780: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+00040790: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+000407a0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+000407b0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+000407c0: 7228 5075 626c 6973 6846 756e 6374 696f  r(PublishFunctio
+000407d0: 6e56 6572 7369 6f6e 5265 7370 6f6e 7365  nVersionResponse
+000407e0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+000407f0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00040800: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00040810: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00040820: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00040830: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00040840: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00040850: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+00040860: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00040870: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+00040880: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+00040890: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000408a0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+000408b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000408c0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+000408d0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+000408e0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+000408f0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00040900: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+00040910: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00040920: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+00040930: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+00040940: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00040950: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00040960: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+00040970: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00040980: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00040990: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000409a0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+000409b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000409c0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000409d0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+000409e0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000409f0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00040a00: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00040a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00040a20: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00040a30: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00040a40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00040a50: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00040a60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00040a70: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+00040a80: 3d20 5665 7273 696f 6e28 290a 2020 2020  = Version().    
+00040a90: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00040aa0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+00040ab0: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+00040ac0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+00040ad0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2050  n self...class P
+00040ae0: 7574 4173 796e 6349 6e76 6f6b 6543 6f6e  utAsyncInvokeCon
+00040af0: 6669 6752 6571 7565 7374 2854 6561 4d6f  figRequest(TeaMo
+00040b00: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00040b10: 696e 6974 5f5f 2873 656c 662c 2062 6f64  init__(self, bod
+00040b20: 793d 4e6f 6e65 2c20 7175 616c 6966 6965  y=None, qualifie
+00040b30: 723d 4e6f 6e65 293a 0a20 2020 2020 2020  r=None):.       
+00040b40: 2023 2054 6865 2063 6f6e 6669 6775 7261   # The configura
+00040b50: 7469 6f6e 7320 6f66 2061 7379 6e63 6872  tions of asynchr
+00040b60: 6f6e 6f75 7320 6675 6e63 7469 6f6e 2069  onous function i
+00040b70: 6e76 6f63 6174 696f 6e2e 0a20 2020 2020  nvocation..     
+00040b80: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+00040b90: 6f64 7920 2023 2074 7970 653a 2050 7574  ody  # type: Put
+00040ba0: 4173 796e 6349 6e76 6f6b 6543 6f6e 6669  AsyncInvokeConfi
+00040bb0: 6749 6e70 7574 0a20 2020 2020 2020 2023  gInput.        #
+00040bc0: 2054 6865 2076 6572 7369 6f6e 206f 7220   The version or 
+00040bd0: 616c 6961 7320 6f66 2074 6865 2066 756e  alias of the fun
+00040be0: 6374 696f 6e2e 0a20 2020 2020 2020 2073  ction..        s
+00040bf0: 656c 662e 7175 616c 6966 6965 7220 3d20  elf.qualifier = 
+00040c00: 7175 616c 6966 6965 7220 2023 2074 7970  qualifier  # typ
+00040c10: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+00040c20: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00040c30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00040c40: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+00040c50: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+00040c60: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+00040c70: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00040c80: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00040c90: 6572 2850 7574 4173 796e 6349 6e76 6f6b  er(PutAsyncInvok
+00040ca0: 6543 6f6e 6669 6752 6571 7565 7374 2c20  eConfigRequest, 
+00040cb0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+00040cc0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00040cd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00040ce0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00040cf0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00040d00: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00040d10: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00040d20: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+00040d30: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00040d40: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+00040d50: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+00040d60: 2020 2020 2020 2069 6620 7365 6c66 2e71         if self.q
+00040d70: 7561 6c69 6669 6572 2069 7320 6e6f 7420  ualifier is not 
+00040d80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00040d90: 2020 7265 7375 6c74 5b27 7175 616c 6966    result['qualif
+00040da0: 6965 7227 5d20 3d20 7365 6c66 2e71 7561  ier'] = self.qua
+00040db0: 6c69 6669 6572 0a20 2020 2020 2020 2072  lifier.        r
+00040dc0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00040dd0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00040de0: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+00040df0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00040e00: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00040e10: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+00040e20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00040e30: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+00040e40: 656c 203d 2050 7574 4173 796e 6349 6e76  el = PutAsyncInv
+00040e50: 6f6b 6543 6f6e 6669 6749 6e70 7574 2829  okeConfigInput()
+00040e60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00040e70: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+00040e80: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00040e90: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+00040ea0: 6966 206d 2e67 6574 2827 7175 616c 6966  if m.get('qualif
+00040eb0: 6965 7227 2920 6973 206e 6f74 204e 6f6e  ier') is not Non
+00040ec0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00040ed0: 656c 662e 7175 616c 6966 6965 7220 3d20  elf.qualifier = 
+00040ee0: 6d2e 6765 7428 2771 7561 6c69 6669 6572  m.get('qualifier
+00040ef0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00040f00: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2050  n self...class P
+00040f10: 7574 4173 796e 6349 6e76 6f6b 6543 6f6e  utAsyncInvokeCon
+00040f20: 6669 6752 6573 706f 6e73 6528 5465 614d  figResponse(TeaM
+00040f30: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00040f40: 5f69 6e69 745f 5f28 7365 6c66 2c20 6865  _init__(self, he
+00040f50: 6164 6572 733d 4e6f 6e65 2c20 7374 6174  aders=None, stat
+00040f60: 7573 5f63 6f64 653d 4e6f 6e65 2c20 626f  us_code=None, bo
+00040f70: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
+00040f80: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00040f90: 2068 6561 6465 7273 2020 2320 7479 7065   headers  # type
+00040fa0: 3a20 6469 6374 5b73 7472 2c20 7374 725d  : dict[str, str]
+00040fb0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00040fc0: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+00040fd0: 7573 5f63 6f64 6520 2023 2074 7970 653a  us_code  # type:
+00040fe0: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
+00040ff0: 662e 626f 6479 203d 2062 6f64 7920 2023  f.body = body  #
+00041000: 2074 7970 653a 2041 7379 6e63 436f 6e66   type: AsyncConf
+00041010: 6967 0a0a 2020 2020 6465 6620 7661 6c69  ig..    def vali
+00041020: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00041030: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00041040: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00041050: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00041060: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00041070: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00041080: 2020 5f6d 6170 203d 2073 7570 6572 2850    _map = super(P
+00041090: 7574 4173 796e 6349 6e76 6f6b 6543 6f6e  utAsyncInvokeCon
+000410a0: 6669 6752 6573 706f 6e73 652c 2073 656c  figResponse, sel
+000410b0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+000410c0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000410d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000410e0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000410f0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00041100: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00041110: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+00041120: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00041130: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00041140: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+00041150: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+00041160: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00041170: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+00041180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00041190: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+000411a0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+000411b0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000411c0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+000411d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000411e0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+000411f0: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00041200: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00041210: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00041220: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00041230: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+00041240: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00041250: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00041260: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+00041270: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+00041280: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00041290: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000412a0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000412b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000412c0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+000412d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000412e0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000412f0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+00041300: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+00041310: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00041320: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+00041330: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00041340: 7465 6d70 5f6d 6f64 656c 203d 2041 7379  temp_model = Asy
+00041350: 6e63 436f 6e66 6967 2829 0a20 2020 2020  ncConfig().     
+00041360: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00041370: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00041380: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00041390: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000413a0: 2073 656c 660a 0a0a 636c 6173 7320 5075   self...class Pu
+000413b0: 7443 6f6e 6375 7272 656e 6379 436f 6e66  tConcurrencyConf
+000413c0: 6967 5265 7175 6573 7428 5465 614d 6f64  igRequest(TeaMod
+000413d0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000413e0: 6e69 745f 5f28 7365 6c66 2c20 626f 6479  nit__(self, body
+000413f0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00041400: 2320 5468 6520 636f 6e63 7572 7265 6e63  # The concurrenc
+00041410: 7920 636f 6e66 6967 7572 6174 696f 6e73  y configurations
+00041420: 2e0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00041430: 6f64 7920 3d20 626f 6479 2020 2320 7479  ody = body  # ty
+00041440: 7065 3a20 5075 7443 6f6e 6375 7272 656e  pe: PutConcurren
+00041450: 6379 496e 7075 740a 0a20 2020 2064 6566  cyInput..    def
+00041460: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00041470: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00041480: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+00041490: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+000414a0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+000414b0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000414c0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000414d0: 7065 7228 5075 7443 6f6e 6375 7272 656e  per(PutConcurren
+000414e0: 6379 436f 6e66 6967 5265 7175 6573 742c  cyConfigRequest,
+000414f0: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+00041500: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00041510: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00041520: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00041530: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00041540: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00041550: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00041560: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+00041570: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00041580: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+00041590: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+000415a0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000415b0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+000415c0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+000415d0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+000415e0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000415f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00041600: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+00041610: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00041620: 2074 656d 705f 6d6f 6465 6c20 3d20 5075   temp_model = Pu
+00041630: 7443 6f6e 6375 7272 656e 6379 496e 7075  tConcurrencyInpu
+00041640: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00041650: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+00041660: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+00041670: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+00041680: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00041690: 0a63 6c61 7373 2050 7574 436f 6e63 7572  .class PutConcur
+000416a0: 7265 6e63 7943 6f6e 6669 6752 6573 706f  rencyConfigRespo
+000416b0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+000416c0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000416d0: 7365 6c66 2c20 6865 6164 6572 733d 4e6f  self, headers=No
+000416e0: 6e65 2c20 7374 6174 7573 5f63 6f64 653d  ne, status_code=
+000416f0: 4e6f 6e65 2c20 626f 6479 3d4e 6f6e 6529  None, body=None)
+00041700: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+00041710: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+00041720: 2020 2320 7479 7065 3a20 6469 6374 5b73    # type: dict[s
+00041730: 7472 2c20 7374 725d 0a20 2020 2020 2020  tr, str].       
+00041740: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00041750: 6520 3d20 7374 6174 7573 5f63 6f64 6520  e = status_code 
+00041760: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
+00041770: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00041780: 2062 6f64 7920 2023 2074 7970 653a 2043   body  # type: C
+00041790: 6f6e 6375 7272 656e 6379 436f 6e66 6967  oncurrencyConfig
+000417a0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+000417b0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+000417c0: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+000417d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000417e0: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+000417f0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00041800: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00041810: 5f6d 6170 203d 2073 7570 6572 2850 7574  _map = super(Put
+00041820: 436f 6e63 7572 7265 6e63 7943 6f6e 6669  ConcurrencyConfi
+00041830: 6752 6573 706f 6e73 652c 2073 656c 6629  gResponse, self)
+00041840: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00041850: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00041860: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00041870: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00041880: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00041890: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000418a0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+000418b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000418c0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000418d0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+000418e0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+000418f0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00041900: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00041910: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00041920: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00041930: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00041940: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00041950: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00041960: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00041970: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00041980: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00041990: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000419a0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000419b0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000419c0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+000419d0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000419e0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000419f0: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00041a00: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00041a10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00041a20: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00041a30: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00041a40: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+00041a50: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+00041a60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00041a70: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00041a80: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+00041a90: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+00041aa0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00041ab0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00041ac0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00041ad0: 6d70 5f6d 6f64 656c 203d 2043 6f6e 6375  mp_model = Concu
+00041ae0: 7272 656e 6379 436f 6e66 6967 2829 0a20  rrencyConfig(). 
+00041af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00041b00: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+00041b10: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+00041b20: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+00041b30: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00041b40: 7320 5075 744c 6179 6572 4143 4c52 6571  s PutLayerACLReq
+00041b50: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+00041b60: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00041b70: 2873 656c 662c 2070 7562 6c69 633d 4e6f  (self, public=No
+00041b80: 6e65 293a 0a20 2020 2020 2020 2023 2053  ne):.        # S
+00041b90: 7065 6369 6669 6573 2077 6865 7468 6572  pecifies whether
+00041ba0: 2074 6865 206c 6179 6572 2069 7320 6120   the layer is a 
+00041bb0: 7075 626c 6963 206c 6179 6572 2e20 5661  public layer. Va
+00041bc0: 6c69 6420 7661 6c75 6573 3a20 7472 7565  lid values: true
+00041bd0: 2061 6e64 2066 616c 7365 2e0a 2020 2020   and false..    
+00041be0: 2020 2020 7365 6c66 2e70 7562 6c69 6320      self.public 
+00041bf0: 3d20 7075 626c 6963 2020 2320 7479 7065  = public  # type
+00041c00: 3a20 7374 720a 0a20 2020 2064 6566 2076  : str..    def v
+00041c10: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00041c20: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00041c30: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00041c40: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00041c50: 3d20 7375 7065 7228 5075 744c 6179 6572  = super(PutLayer
+00041c60: 4143 4c52 6571 7565 7374 2c20 7365 6c66  ACLRequest, self
+00041c70: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00041c80: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00041c90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00041ca0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00041cb0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00041cc0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00041cd0: 2069 6620 7365 6c66 2e70 7562 6c69 6320   if self.public 
+00041ce0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00041cf0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00041d00: 2770 7562 6c69 6327 5d20 3d20 7365 6c66  'public'] = self
+00041d10: 2e70 7562 6c69 630a 2020 2020 2020 2020  .public.        
+00041d20: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00041d30: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00041d40: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
+00041d50: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00041d60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00041d70: 6620 6d2e 6765 7428 2770 7562 6c69 6327  f m.get('public'
+00041d80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00041d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00041da0: 7075 626c 6963 203d 206d 2e67 6574 2827  public = m.get('
+00041db0: 7075 626c 6963 2729 0a20 2020 2020 2020  public').       
+00041dc0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00041dd0: 6c61 7373 2050 7574 4c61 7965 7241 434c  lass PutLayerACL
+00041de0: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+00041df0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00041e00: 6974 5f5f 2873 656c 662c 2068 6561 6465  it__(self, heade
+00041e10: 7273 3d4e 6f6e 652c 2073 7461 7475 735f  rs=None, status_
+00041e20: 636f 6465 3d4e 6f6e 6529 3a0a 2020 2020  code=None):.    
+00041e30: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00041e40: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
+00041e50: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
+00041e60: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
+00041e70: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+00041e80: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
+00041e90: 653a 2069 6e74 0a0a 2020 2020 6465 6620  e: int..    def 
+00041ea0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00041eb0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00041ec0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00041ed0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00041ee0: 203d 2073 7570 6572 2850 7574 4c61 7965   = super(PutLaye
+00041ef0: 7241 434c 5265 7370 6f6e 7365 2c20 7365  rACLResponse, se
+00041f00: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+00041f10: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00041f20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00041f30: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00041f40: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00041f50: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00041f60: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+00041f70: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+00041f80: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00041f90: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+00041fa0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+00041fb0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+00041fc0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
+00041fd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00041fe0: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
+00041ff0: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
+00042000: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+00042010: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00042020: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00042030: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00042040: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00042050: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00042060: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+00042070: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+00042080: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00042090: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+000420a0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+000420b0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000420c0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+000420d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000420e0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+000420f0: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00042100: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00042110: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00042120: 0a0a 0a63 6c61 7373 2050 7574 5072 6f76  ...class PutProv
+00042130: 6973 696f 6e43 6f6e 6669 6752 6571 7565  isionConfigReque
+00042140: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+00042150: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00042160: 656c 662c 2062 6f64 793d 4e6f 6e65 2c20  elf, body=None, 
+00042170: 7175 616c 6966 6965 723d 4e6f 6e65 293a  qualifier=None):
+00042180: 0a20 2020 2020 2020 2023 2054 6865 2069  .        # The i
+00042190: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+000421a0: 2074 6865 2070 726f 7669 7369 6f6e 6564   the provisioned
+000421b0: 2063 6f6e 6669 6775 7261 7469 6f6e 2e0a   configuration..
+000421c0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000421d0: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
+000421e0: 3a20 5075 7450 726f 7669 7369 6f6e 436f  : PutProvisionCo
+000421f0: 6e66 6967 496e 7075 740a 2020 2020 2020  nfigInput.      
+00042200: 2020 2320 5468 6520 6675 6e63 7469 6f6e    # The function
+00042210: 2061 6c69 6173 206f 7220 4c41 5445 5354   alias or LATEST
+00042220: 2e0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
+00042230: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
+00042240: 6669 6572 2020 2320 7479 7065 3a20 7374  fier  # type: st
+00042250: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
+00042260: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00042270: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+00042280: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00042290: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+000422a0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+000422b0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000422c0: 205f 6d61 7020 3d20 7375 7065 7228 5075   _map = super(Pu
+000422d0: 7450 726f 7669 7369 6f6e 436f 6e66 6967  tProvisionConfig
+000422e0: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
+000422f0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00042300: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00042310: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00042320: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00042330: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00042340: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00042350: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+00042360: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00042370: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00042380: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00042390: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000423a0: 6966 2073 656c 662e 7175 616c 6966 6965  if self.qualifie
+000423b0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+000423c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000423d0: 745b 2771 7561 6c69 6669 6572 275d 203d  t['qualifier'] =
+000423e0: 2073 656c 662e 7175 616c 6966 6965 720a   self.qualifier.
+000423f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00042400: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00042410: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+00042420: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00042430: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00042440: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00042450: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+00042460: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00042470: 2074 656d 705f 6d6f 6465 6c20 3d20 5075   temp_model = Pu
+00042480: 7450 726f 7669 7369 6f6e 436f 6e66 6967  tProvisionConfig
+00042490: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
+000424a0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+000424b0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+000424c0: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+000424d0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000424e0: 2771 7561 6c69 6669 6572 2729 2069 7320  'qualifier') is 
+000424f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00042500: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
+00042510: 6669 6572 203d 206d 2e67 6574 2827 7175  fier = m.get('qu
+00042520: 616c 6966 6965 7227 290a 2020 2020 2020  alifier').      
+00042530: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00042540: 636c 6173 7320 5075 7450 726f 7669 7369  class PutProvisi
+00042550: 6f6e 436f 6e66 6967 5265 7370 6f6e 7365  onConfigResponse
+00042560: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00042570: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00042580: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
+00042590: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
+000425a0: 652c 2062 6f64 793d 4e6f 6e65 293a 0a20  e, body=None):. 
+000425b0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+000425c0: 6572 7320 3d20 6865 6164 6572 7320 2023  ers = headers  #
+000425d0: 2074 7970 653a 2064 6963 745b 7374 722c   type: dict[str,
+000425e0: 2073 7472 5d0a 2020 2020 2020 2020 7365   str].        se
+000425f0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00042600: 2073 7461 7475 735f 636f 6465 2020 2320   status_code  # 
+00042610: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00042620: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+00042630: 6479 2020 2320 7479 7065 3a20 5072 6f76  dy  # type: Prov
+00042640: 6973 696f 6e43 6f6e 6669 670a 0a20 2020  isionConfig..   
+00042650: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00042660: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00042670: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+00042680: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00042690: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+000426a0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000426b0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000426c0: 3d20 7375 7065 7228 5075 7450 726f 7669  = super(PutProvi
+000426d0: 7369 6f6e 436f 6e66 6967 5265 7370 6f6e  sionConfigRespon
+000426e0: 7365 2c20 7365 6c66 292e 746f 5f6d 6170  se, self).to_map
+000426f0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00042700: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00042710: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00042720: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00042730: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00042740: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00042750: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+00042760: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00042770: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+00042780: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+00042790: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+000427a0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+000427b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000427c0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000427d0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+000427e0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+000427f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00042800: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+00042810: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00042820: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00042830: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00042840: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00042850: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00042860: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00042870: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00042880: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00042890: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000428a0: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+000428b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000428c0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+000428d0: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+000428e0: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+000428f0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00042900: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+00042910: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00042920: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00042930: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00042940: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+00042950: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+00042960: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00042970: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+00042980: 6c20 3d20 5072 6f76 6973 696f 6e43 6f6e  l = ProvisionCon
+00042990: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
+000429a0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
+000429b0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+000429c0: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
+000429d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000429e0: 0a0a 0a63 6c61 7373 2053 746f 7041 7379  ...class StopAsy
+000429f0: 6e63 5461 736b 5265 7175 6573 7428 5465  ncTaskRequest(Te
+00042a00: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00042a10: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00042a20: 7175 616c 6966 6965 723d 4e6f 6e65 293a  qualifier=None):
+00042a30: 0a20 2020 2020 2020 2073 656c 662e 7175  .        self.qu
+00042a40: 616c 6966 6965 7220 3d20 7175 616c 6966  alifier = qualif
+00042a50: 6965 7220 2023 2074 7970 653a 2073 7472  ier  # type: str
+00042a60: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00042a70: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00042a80: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00042a90: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00042aa0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00042ab0: 6572 2853 746f 7041 7379 6e63 5461 736b  er(StopAsyncTask
+00042ac0: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
+00042ad0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00042ae0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00042af0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00042b00: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00042b10: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00042b20: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00042b30: 2073 656c 662e 7175 616c 6966 6965 7220   self.qualifier 
+00042b40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00042b50: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00042b60: 2771 7561 6c69 6669 6572 275d 203d 2073  'qualifier'] = s
+00042b70: 656c 662e 7175 616c 6966 6965 720a 2020  elf.qualifier.  
+00042b80: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00042b90: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00042ba0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00042bb0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00042bc0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00042bd0: 2020 2020 2069 6620 6d2e 6765 7428 2771       if m.get('q
+00042be0: 7561 6c69 6669 6572 2729 2069 7320 6e6f  ualifier') is no
+00042bf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00042c00: 2020 2020 7365 6c66 2e71 7561 6c69 6669      self.qualifi
+00042c10: 6572 203d 206d 2e67 6574 2827 7175 616c  er = m.get('qual
+00042c20: 6966 6965 7227 290a 2020 2020 2020 2020  ifier').        
+00042c30: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00042c40: 6173 7320 5374 6f70 4173 796e 6354 6173  ass StopAsyncTas
+00042c50: 6b52 6573 706f 6e73 6528 5465 614d 6f64  kResponse(TeaMod
+00042c60: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00042c70: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
+00042c80: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
+00042c90: 5f63 6f64 653d 4e6f 6e65 293a 0a20 2020  _code=None):.   
+00042ca0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00042cb0: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
+00042cc0: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
+00042cd0: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
+00042ce0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+00042cf0: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
+00042d00: 7065 3a20 696e 740a 0a20 2020 2064 6566  pe: int..    def
+00042d10: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00042d20: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00042d30: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00042d40: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00042d50: 7020 3d20 7375 7065 7228 5374 6f70 4173  p = super(StopAs
+00042d60: 796e 6354 6173 6b52 6573 706f 6e73 652c  yncTaskResponse,
+00042d70: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+00042d80: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00042d90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00042da0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00042db0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00042dc0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00042dd0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+00042de0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+00042df0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00042e00: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+00042e10: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+00042e20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00042e30: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+00042e40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00042e50: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+00042e60: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+00042e70: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+00042e80: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00042e90: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00042ea0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00042eb0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00042ec0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00042ed0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00042ee0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00042ef0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00042f00: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00042f10: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00042f20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00042f30: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00042f40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00042f50: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00042f60: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00042f70: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+00042f80: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00042f90: 656c 660a 0a0a 636c 6173 7320 5461 6752  elf...class TagR
+00042fa0: 6573 6f75 7263 6573 5265 7175 6573 7428  esourcesRequest(
+00042fb0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00042fc0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00042fd0: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
+00042fe0: 2020 2020 2020 2320 5468 6520 636f 6e66        # The conf
+00042ff0: 6967 7572 6174 696f 6e20 6f66 2074 6865  iguration of the
+00043000: 2072 6573 6f75 7263 6520 7461 672e 0a20   resource tag.. 
+00043010: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00043020: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
+00043030: 2054 6167 5265 736f 7572 6365 7349 6e70   TagResourcesInp
+00043040: 7574 0a0a 2020 2020 6465 6620 7661 6c69  ut..    def vali
+00043050: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00043060: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00043070: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00043080: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00043090: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+000430a0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+000430b0: 2020 5f6d 6170 203d 2073 7570 6572 2854    _map = super(T
+000430c0: 6167 5265 736f 7572 6365 7352 6571 7565  agResourcesReque
+000430d0: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
+000430e0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000430f0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00043100: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00043110: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00043120: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00043130: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00043140: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+00043150: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00043160: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+00043170: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+00043180: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00043190: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000431a0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000431b0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+000431c0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000431d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000431e0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+000431f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00043200: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+00043210: 2054 6167 5265 736f 7572 6365 7349 6e70   TagResourcesInp
+00043220: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00043230: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00043240: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00043250: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00043260: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00043270: 0a0a 636c 6173 7320 5461 6752 6573 6f75  ..class TagResou
+00043280: 7263 6573 5265 7370 6f6e 7365 2854 6561  rcesResponse(Tea
+00043290: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000432a0: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
+000432b0: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
+000432c0: 7475 735f 636f 6465 3d4e 6f6e 6529 3a0a  tus_code=None):.
+000432d0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000432e0: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
+000432f0: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
+00043300: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
+00043310: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00043320: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
+00043330: 2074 7970 653a 2069 6e74 0a0a 2020 2020   type: int..    
+00043340: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00043350: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00043360: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00043370: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00043380: 5f6d 6170 203d 2073 7570 6572 2854 6167  _map = super(Tag
+00043390: 5265 736f 7572 6365 7352 6573 706f 6e73  ResourcesRespons
+000433a0: 652c 2073 656c 6629 2e74 6f5f 6d61 7028  e, self).to_map(
+000433b0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000433c0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000433d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000433e0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000433f0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00043400: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00043410: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+00043420: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043430: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+00043440: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+00043450: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00043460: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+00043470: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00043480: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00043490: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+000434a0: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+000434b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000434c0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000434d0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+000434e0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+000434f0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00043500: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00043510: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+00043520: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00043530: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+00043540: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+00043550: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00043560: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+00043570: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00043580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00043590: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+000435a0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+000435b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000435c0: 2073 656c 660a 0a0a 636c 6173 7320 556e   self...class Un
+000435d0: 7461 6752 6573 6f75 7263 6573 5265 7175  tagResourcesRequ
+000435e0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+000435f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00043600: 7365 6c66 2c20 616c 6c3d 4e6f 6e65 2c20  self, all=None, 
+00043610: 7265 736f 7572 6365 5f69 643d 4e6f 6e65  resource_id=None
+00043620: 2c20 7265 736f 7572 6365 5f74 7970 653d  , resource_type=
+00043630: 4e6f 6e65 2c20 7461 675f 6b65 793d 4e6f  None, tag_key=No
+00043640: 6e65 293a 0a20 2020 2020 2020 2023 2053  ne):.        # S
+00043650: 7065 6369 6669 6573 2077 6865 7468 6572  pecifies whether
+00043660: 2074 6f20 6465 6c65 7465 2061 6c6c 2074   to delete all t
+00043670: 6167 732e 0a20 2020 2020 2020 2073 656c  ags..        sel
+00043680: 662e 616c 6c20 3d20 616c 6c20 2023 2074  f.all = all  # t
+00043690: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+000436a0: 2020 2320 5468 6520 7265 736f 7572 6365    # The resource
+000436b0: 2069 6465 6e74 6966 6965 7273 2e0a 2020   identifiers..  
+000436c0: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+000436d0: 7263 655f 6964 203d 2072 6573 6f75 7263  rce_id = resourc
+000436e0: 655f 6964 2020 2320 7479 7065 3a20 6c69  e_id  # type: li
+000436f0: 7374 5b73 7472 5d0a 2020 2020 2020 2020  st[str].        
+00043700: 2320 5468 6520 7265 736f 7572 6365 2074  # The resource t
+00043710: 7970 652e 0a20 2020 2020 2020 2073 656c  ype..        sel
+00043720: 662e 7265 736f 7572 6365 5f74 7970 6520  f.resource_type 
+00043730: 3d20 7265 736f 7572 6365 5f74 7970 6520  = resource_type 
+00043740: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00043750: 2020 2020 2023 2054 6865 2074 6167 2074       # The tag t
+00043760: 6f20 7265 6d6f 7665 2e20 596f 7520 6361  o remove. You ca
+00043770: 6e20 7370 6563 6966 7920 6120 6d61 7869  n specify a maxi
+00043780: 6d75 6d20 6f66 2035 3020 7461 6773 2e0a  mum of 50 tags..
+00043790: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
+000437a0: 5f6b 6579 203d 2074 6167 5f6b 6579 2020  _key = tag_key  
+000437b0: 2320 7479 7065 3a20 6c69 7374 5b73 7472  # type: list[str
+000437c0: 5d0a 0a20 2020 2064 6566 2076 616c 6964  ]..    def valid
+000437d0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000437e0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000437f0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00043800: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00043810: 7065 7228 556e 7461 6752 6573 6f75 7263  per(UntagResourc
+00043820: 6573 5265 7175 6573 742c 2073 656c 6629  esRequest, self)
+00043830: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00043840: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00043850: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00043860: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00043870: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00043880: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00043890: 6966 2073 656c 662e 616c 6c20 6973 206e  if self.all is n
+000438a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000438b0: 2020 2020 2072 6573 756c 745b 2741 6c6c       result['All
+000438c0: 275d 203d 2073 656c 662e 616c 6c0a 2020  '] = self.all.  
+000438d0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+000438e0: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
+000438f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00043900: 2020 2072 6573 756c 745b 2752 6573 6f75     result['Resou
+00043910: 7263 6549 6427 5d20 3d20 7365 6c66 2e72  rceId'] = self.r
+00043920: 6573 6f75 7263 655f 6964 0a20 2020 2020  esource_id.     
+00043930: 2020 2069 6620 7365 6c66 2e72 6573 6f75     if self.resou
+00043940: 7263 655f 7479 7065 2069 7320 6e6f 7420  rce_type is not 
+00043950: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00043960: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
+00043970: 6365 5479 7065 275d 203d 2073 656c 662e  ceType'] = self.
+00043980: 7265 736f 7572 6365 5f74 7970 650a 2020  resource_type.  
+00043990: 2020 2020 2020 6966 2073 656c 662e 7461        if self.ta
+000439a0: 675f 6b65 7920 6973 206e 6f74 204e 6f6e  g_key is not Non
+000439b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000439c0: 6573 756c 745b 2754 6167 4b65 7927 5d20  esult['TagKey'] 
+000439d0: 3d20 7365 6c66 2e74 6167 5f6b 6579 0a20  = self.tag_key. 
+000439e0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000439f0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00043a00: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+00043a10: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00043a20: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00043a30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00043a40: 416c 6c27 2920 6973 206e 6f74 204e 6f6e  All') is not Non
+00043a50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00043a60: 656c 662e 616c 6c20 3d20 6d2e 6765 7428  elf.all = m.get(
+00043a70: 2741 6c6c 2729 0a20 2020 2020 2020 2069  'All').        i
+00043a80: 6620 6d2e 6765 7428 2752 6573 6f75 7263  f m.get('Resourc
+00043a90: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+00043aa0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00043ab0: 656c 662e 7265 736f 7572 6365 5f69 6420  elf.resource_id 
+00043ac0: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
+00043ad0: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
+00043ae0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+00043af0: 5479 7065 2729 2069 7320 6e6f 7420 4e6f  Type') is not No
+00043b00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00043b10: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
+00043b20: 7065 203d 206d 2e67 6574 2827 5265 736f  pe = m.get('Reso
+00043b30: 7572 6365 5479 7065 2729 0a20 2020 2020  urceType').     
+00043b40: 2020 2069 6620 6d2e 6765 7428 2754 6167     if m.get('Tag
+00043b50: 4b65 7927 2920 6973 206e 6f74 204e 6f6e  Key') is not Non
+00043b60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00043b70: 656c 662e 7461 675f 6b65 7920 3d20 6d2e  elf.tag_key = m.
+00043b80: 6765 7428 2754 6167 4b65 7927 290a 2020  get('TagKey').  
+00043b90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00043ba0: 660a 0a0a 636c 6173 7320 556e 7461 6752  f...class UntagR
+00043bb0: 6573 6f75 7263 6573 5368 7269 6e6b 5265  esourcesShrinkRe
+00043bc0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+00043bd0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00043be0: 5f28 7365 6c66 2c20 616c 6c3d 4e6f 6e65  _(self, all=None
+00043bf0: 2c20 7265 736f 7572 6365 5f69 645f 7368  , resource_id_sh
+00043c00: 7269 6e6b 3d4e 6f6e 652c 2072 6573 6f75  rink=None, resou
+00043c10: 7263 655f 7479 7065 3d4e 6f6e 652c 2074  rce_type=None, t
+00043c20: 6167 5f6b 6579 5f73 6872 696e 6b3d 4e6f  ag_key_shrink=No
+00043c30: 6e65 293a 0a20 2020 2020 2020 2023 2053  ne):.        # S
+00043c40: 7065 6369 6669 6573 2077 6865 7468 6572  pecifies whether
+00043c50: 2074 6f20 6465 6c65 7465 2061 6c6c 2074   to delete all t
+00043c60: 6167 732e 0a20 2020 2020 2020 2073 656c  ags..        sel
+00043c70: 662e 616c 6c20 3d20 616c 6c20 2023 2074  f.all = all  # t
+00043c80: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00043c90: 2020 2320 5468 6520 7265 736f 7572 6365    # The resource
+00043ca0: 2069 6465 6e74 6966 6965 7273 2e0a 2020   identifiers..  
+00043cb0: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+00043cc0: 7263 655f 6964 5f73 6872 696e 6b20 3d20  rce_id_shrink = 
+00043cd0: 7265 736f 7572 6365 5f69 645f 7368 7269  resource_id_shri
+00043ce0: 6e6b 2020 2320 7479 7065 3a20 7374 720a  nk  # type: str.
+00043cf0: 2020 2020 2020 2020 2320 5468 6520 7265          # The re
+00043d00: 736f 7572 6365 2074 7970 652e 0a20 2020  source type..   
+00043d10: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00043d20: 6365 5f74 7970 6520 3d20 7265 736f 7572  ce_type = resour
+00043d30: 6365 5f74 7970 6520 2023 2074 7970 653a  ce_type  # type:
+00043d40: 2073 7472 0a20 2020 2020 2020 2023 2054   str.        # T
+00043d50: 6865 2074 6167 2074 6f20 7265 6d6f 7665  he tag to remove
+00043d60: 2e20 596f 7520 6361 6e20 7370 6563 6966  . You can specif
+00043d70: 7920 6120 6d61 7869 6d75 6d20 6f66 2035  y a maximum of 5
+00043d80: 3020 7461 6773 2e0a 2020 2020 2020 2020  0 tags..        
+00043d90: 7365 6c66 2e74 6167 5f6b 6579 5f73 6872  self.tag_key_shr
+00043da0: 696e 6b20 3d20 7461 675f 6b65 795f 7368  ink = tag_key_sh
+00043db0: 7269 6e6b 2020 2320 7479 7065 3a20 7374  rink  # type: st
+00043dc0: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
+00043dd0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00043de0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00043df0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00043e00: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00043e10: 7065 7228 556e 7461 6752 6573 6f75 7263  per(UntagResourc
+00043e20: 6573 5368 7269 6e6b 5265 7175 6573 742c  esShrinkRequest,
+00043e30: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+00043e40: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00043e50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00043e60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00043e70: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00043e80: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00043e90: 2020 2020 2020 6966 2073 656c 662e 616c        if self.al
+00043ea0: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
+00043eb0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00043ec0: 745b 2741 6c6c 275d 203d 2073 656c 662e  t['All'] = self.
+00043ed0: 616c 6c0a 2020 2020 2020 2020 6966 2073  all.        if s
+00043ee0: 656c 662e 7265 736f 7572 6365 5f69 645f  elf.resource_id_
+00043ef0: 7368 7269 6e6b 2069 7320 6e6f 7420 4e6f  shrink is not No
+00043f00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00043f10: 7265 7375 6c74 5b27 5265 736f 7572 6365  result['Resource
+00043f20: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
+00043f30: 7572 6365 5f69 645f 7368 7269 6e6b 0a20  urce_id_shrink. 
+00043f40: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00043f50: 6573 6f75 7263 655f 7479 7065 2069 7320  esource_type is 
+00043f60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00043f70: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+00043f80: 736f 7572 6365 5479 7065 275d 203d 2073  sourceType'] = s
+00043f90: 656c 662e 7265 736f 7572 6365 5f74 7970  elf.resource_typ
+00043fa0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00043fb0: 662e 7461 675f 6b65 795f 7368 7269 6e6b  f.tag_key_shrink
+00043fc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00043fd0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00043fe0: 5b27 5461 674b 6579 275d 203d 2073 656c  ['TagKey'] = sel
+00043ff0: 662e 7461 675f 6b65 795f 7368 7269 6e6b  f.tag_key_shrink
+00044000: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00044010: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00044020: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00044030: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00044040: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00044050: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00044060: 2827 416c 6c27 2920 6973 206e 6f74 204e  ('All') is not N
+00044070: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00044080: 2073 656c 662e 616c 6c20 3d20 6d2e 6765   self.all = m.ge
+00044090: 7428 2741 6c6c 2729 0a20 2020 2020 2020  t('All').       
+000440a0: 2069 6620 6d2e 6765 7428 2752 6573 6f75   if m.get('Resou
+000440b0: 7263 6549 6427 2920 6973 206e 6f74 204e  rceId') is not N
+000440c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000440d0: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+000440e0: 645f 7368 7269 6e6b 203d 206d 2e67 6574  d_shrink = m.get
+000440f0: 2827 5265 736f 7572 6365 4964 2729 0a20  ('ResourceId'). 
+00044100: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00044110: 2752 6573 6f75 7263 6554 7970 6527 2920  'ResourceType') 
+00044120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00044130: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00044140: 736f 7572 6365 5f74 7970 6520 3d20 6d2e  source_type = m.
+00044150: 6765 7428 2752 6573 6f75 7263 6554 7970  get('ResourceTyp
+00044160: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00044170: 2e67 6574 2827 5461 674b 6579 2729 2069  .get('TagKey') i
+00044180: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00044190: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
+000441a0: 5f6b 6579 5f73 6872 696e 6b20 3d20 6d2e  _key_shrink = m.
+000441b0: 6765 7428 2754 6167 4b65 7927 290a 2020  get('TagKey').  
+000441c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000441d0: 660a 0a0a 636c 6173 7320 556e 7461 6752  f...class UntagR
+000441e0: 6573 6f75 7263 6573 5265 7370 6f6e 7365  esourcesResponse
+000441f0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00044200: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00044210: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
+00044220: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
+00044230: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00044240: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+00044250: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
+00044260: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
+00044270: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+00044280: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+00044290: 6520 2023 2074 7970 653a 2069 6e74 0a0a  e  # type: int..
+000442a0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000442b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000442c0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+000442d0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000442e0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000442f0: 2855 6e74 6167 5265 736f 7572 6365 7352  (UntagResourcesR
+00044300: 6573 706f 6e73 652c 2073 656c 6629 2e74  esponse, self).t
+00044310: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00044320: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00044330: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00044340: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00044350: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00044360: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00044370: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+00044380: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044390: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+000443a0: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+000443b0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+000443c0: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+000443d0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+000443e0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000443f0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+00044400: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+00044410: 636f 6465 0a20 2020 2020 2020 2072 6574  code.        ret
+00044420: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00044430: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00044440: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+00044450: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00044460: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00044470: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+00044480: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00044490: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000444a0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+000444b0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+000444c0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+000444d0: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+000444e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000444f0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00044500: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+00044510: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+00044520: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00044530: 6173 7320 5570 6461 7465 416c 6961 7352  ass UpdateAliasR
+00044540: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+00044550: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00044560: 5f5f 2873 656c 662c 2062 6f64 793d 4e6f  __(self, body=No
+00044570: 6e65 293a 0a20 2020 2020 2020 2023 2054  ne):.        # T
+00044580: 6865 2061 6c69 6173 2069 6e66 6f72 6d61  he alias informa
+00044590: 7469 6f6e 2074 6f20 6265 2075 7064 6174  tion to be updat
+000445a0: 6564 2e0a 2020 2020 2020 2020 7365 6c66  ed..        self
+000445b0: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
+000445c0: 7479 7065 3a20 5570 6461 7465 416c 6961  type: UpdateAlia
+000445d0: 7349 6e70 7574 0a0a 2020 2020 6465 6620  sInput..    def 
+000445e0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000445f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00044600: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+00044610: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+00044620: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+00044630: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00044640: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00044650: 6572 2855 7064 6174 6541 6c69 6173 5265  er(UpdateAliasRe
+00044660: 7175 6573 742c 2073 656c 6629 2e74 6f5f  quest, self).to_
+00044670: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00044680: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00044690: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000446a0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000446b0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000446c0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000446d0: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+000446e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000446f0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+00044700: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+00044710: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+00044720: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00044730: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00044740: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+00044750: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00044760: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00044770: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+00044780: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044790: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000447a0: 6c20 3d20 5570 6461 7465 416c 6961 7349  l = UpdateAliasI
+000447b0: 6e70 7574 2829 0a20 2020 2020 2020 2020  nput().         
+000447c0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+000447d0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+000447e0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+000447f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00044800: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
+00044810: 416c 6961 7352 6573 706f 6e73 6528 5465  AliasResponse(Te
+00044820: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00044830: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00044840: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
+00044850: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
+00044860: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
+00044870: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00044880: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
+00044890: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
+000448a0: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
+000448b0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+000448c0: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
+000448d0: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
+000448e0: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
+000448f0: 2023 2074 7970 653a 2041 6c69 6173 0a0a   # type: Alias..
+00044900: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00044910: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00044920: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00044930: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00044940: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00044950: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00044960: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00044970: 6170 203d 2073 7570 6572 2855 7064 6174  ap = super(Updat
+00044980: 6541 6c69 6173 5265 7370 6f6e 7365 2c20  eAliasResponse, 
+00044990: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+000449a0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000449b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000449c0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000449d0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000449e0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000449f0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00044a00: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00044a10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00044a20: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+00044a30: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+00044a40: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00044a50: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+00044a60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00044a70: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+00044a80: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+00044a90: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00044aa0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00044ab0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00044ac0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00044ad0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00044ae0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00044af0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00044b00: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00044b10: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00044b20: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00044b30: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00044b40: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+00044b50: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+00044b60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00044b70: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00044b80: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00044b90: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00044ba0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00044bb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00044bc0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00044bd0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+00044be0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00044bf0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00044c00: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00044c10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00044c20: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00044c30: 416c 6961 7328 290a 2020 2020 2020 2020  Alias().        
+00044c40: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00044c50: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+00044c60: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+00044c70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00044c80: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
+00044c90: 6543 7573 746f 6d44 6f6d 6169 6e52 6571  eCustomDomainReq
+00044ca0: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+00044cb0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00044cc0: 2873 656c 662c 2062 6f64 793d 4e6f 6e65  (self, body=None
+00044cd0: 293a 0a20 2020 2020 2020 2023 2054 6865  ):.        # The
+00044ce0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
+00044cf0: 7574 2074 6865 2063 7573 746f 6d20 646f  ut the custom do
+00044d00: 6d61 696e 206e 616d 652e 0a20 2020 2020  main name..     
+00044d10: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+00044d20: 6f64 7920 2023 2074 7970 653a 2055 7064  ody  # type: Upd
+00044d30: 6174 6543 7573 746f 6d44 6f6d 6169 6e49  ateCustomDomainI
+00044d40: 6e70 7574 0a0a 2020 2020 6465 6620 7661  nput..    def va
+00044d50: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00044d60: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00044d70: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+00044d80: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+00044d90: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+00044da0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00044db0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00044dc0: 2855 7064 6174 6543 7573 746f 6d44 6f6d  (UpdateCustomDom
+00044dd0: 6169 6e52 6571 7565 7374 2c20 7365 6c66  ainRequest, self
+00044de0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00044df0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00044e00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00044e10: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00044e20: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00044e30: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00044e40: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+00044e50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044e60: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+00044e70: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00044e80: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00044e90: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00044ea0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00044eb0: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+00044ec0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00044ed0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00044ee0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+00044ef0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00044f00: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00044f10: 5f6d 6f64 656c 203d 2055 7064 6174 6543  _model = UpdateC
+00044f20: 7573 746f 6d44 6f6d 6169 6e49 6e70 7574  ustomDomainInput
+00044f30: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00044f40: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+00044f50: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+00044f60: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+00044f70: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00044f80: 636c 6173 7320 5570 6461 7465 4375 7374  class UpdateCust
+00044f90: 6f6d 446f 6d61 696e 5265 7370 6f6e 7365  omDomainResponse
+00044fa0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00044fb0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00044fc0: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
+00044fd0: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
+00044fe0: 652c 2062 6f64 793d 4e6f 6e65 293a 0a20  e, body=None):. 
+00044ff0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00045000: 6572 7320 3d20 6865 6164 6572 7320 2023  ers = headers  #
+00045010: 2074 7970 653a 2064 6963 745b 7374 722c   type: dict[str,
+00045020: 2073 7472 5d0a 2020 2020 2020 2020 7365   str].        se
+00045030: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00045040: 2073 7461 7475 735f 636f 6465 2020 2320   status_code  # 
+00045050: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00045060: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+00045070: 6479 2020 2320 7479 7065 3a20 4375 7374  dy  # type: Cust
+00045080: 6f6d 446f 6d61 696e 0a0a 2020 2020 6465  omDomain..    de
+00045090: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000450a0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000450b0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+000450c0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+000450d0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+000450e0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000450f0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00045100: 7570 6572 2855 7064 6174 6543 7573 746f  uper(UpdateCusto
+00045110: 6d44 6f6d 6169 6e52 6573 706f 6e73 652c  mDomainResponse,
+00045120: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+00045130: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00045140: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00045150: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00045160: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00045170: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00045180: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+00045190: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+000451a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000451b0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+000451c0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+000451d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000451e0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+000451f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00045200: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+00045210: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+00045220: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+00045230: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00045240: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+00045250: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00045260: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+00045270: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+00045280: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00045290: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000452a0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+000452b0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+000452c0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+000452d0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000452e0: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+000452f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00045300: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+00045310: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+00045320: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00045330: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+00045340: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00045350: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00045360: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+00045370: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+00045380: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00045390: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+000453a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000453b0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+000453c0: 2043 7573 746f 6d44 6f6d 6169 6e28 290a   CustomDomain().
+000453d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000453e0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+000453f0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+00045400: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+00045410: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00045420: 7373 2055 7064 6174 6546 756e 6374 696f  ss UpdateFunctio
+00045430: 6e52 6571 7565 7374 2854 6561 4d6f 6465  nRequest(TeaMode
+00045440: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00045450: 6974 5f5f 2873 656c 662c 2062 6f64 793d  it__(self, body=
+00045460: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
+00045470: 2054 6865 2066 756e 6374 696f 6e20 696e   The function in
+00045480: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
+00045490: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+000454a0: 6479 2020 2320 7479 7065 3a20 5570 6461  dy  # type: Upda
+000454b0: 7465 4675 6e63 7469 6f6e 496e 7075 740a  teFunctionInput.
+000454c0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000454d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000454e0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+000454f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00045500: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+00045510: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00045520: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00045530: 6d61 7020 3d20 7375 7065 7228 5570 6461  map = super(Upda
+00045540: 7465 4675 6e63 7469 6f6e 5265 7175 6573  teFunctionReques
+00045550: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
+00045560: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00045570: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00045580: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00045590: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000455a0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000455b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000455c0: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+000455d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000455e0: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+000455f0: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00045600: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00045610: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00045620: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00045630: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00045640: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00045650: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00045660: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00045670: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00045680: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00045690: 5570 6461 7465 4675 6e63 7469 6f6e 496e  UpdateFunctionIn
+000456a0: 7075 7428 290a 2020 2020 2020 2020 2020  put().          
+000456b0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
+000456c0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+000456d0: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
+000456e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000456f0: 0a0a 0a63 6c61 7373 2055 7064 6174 6546  ...class UpdateF
+00045700: 756e 6374 696f 6e52 6573 706f 6e73 6528  unctionResponse(
+00045710: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00045720: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00045730: 2c20 6865 6164 6572 733d 4e6f 6e65 2c20  , headers=None, 
+00045740: 7374 6174 7573 5f63 6f64 653d 4e6f 6e65  status_code=None
+00045750: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
+00045760: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00045770: 7273 203d 2068 6561 6465 7273 2020 2320  rs = headers  # 
+00045780: 7479 7065 3a20 6469 6374 5b73 7472 2c20  type: dict[str, 
+00045790: 7374 725d 0a20 2020 2020 2020 2073 656c  str].        sel
+000457a0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+000457b0: 7374 6174 7573 5f63 6f64 6520 2023 2074  status_code  # t
+000457c0: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+000457d0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+000457e0: 7920 2023 2074 7970 653a 2046 756e 6374  y  # type: Funct
+000457f0: 696f 6e0a 0a20 2020 2064 6566 2076 616c  ion..    def val
+00045800: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00045810: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00045820: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00045830: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00045840: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00045850: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00045860: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00045870: 5570 6461 7465 4675 6e63 7469 6f6e 5265  UpdateFunctionRe
+00045880: 7370 6f6e 7365 2c20 7365 6c66 292e 746f  sponse, self).to
+00045890: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000458a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000458b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000458c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000458d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000458e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000458f0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+00045900: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00045910: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+00045920: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+00045930: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+00045940: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+00045950: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+00045960: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00045970: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+00045980: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+00045990: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+000459a0: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+000459b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000459c0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+000459d0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+000459e0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+000459f0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00045a00: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00045a10: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+00045a20: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00045a30: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00045a40: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00045a50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00045a60: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00045a70: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+00045a80: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00045a90: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+00045aa0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+00045ab0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00045ac0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00045ad0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+00045ae0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+00045af0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+00045b00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00045b10: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00045b20: 6d6f 6465 6c20 3d20 4675 6e63 7469 6f6e  model = Function
+00045b30: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00045b40: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+00045b50: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+00045b60: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+00045b70: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00045b80: 636c 6173 7320 5570 6461 7465 5472 6967  class UpdateTrig
+00045b90: 6765 7252 6571 7565 7374 2854 6561 4d6f  gerRequest(TeaMo
+00045ba0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00045bb0: 696e 6974 5f5f 2873 656c 662c 2062 6f64  init__(self, bod
+00045bc0: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
+00045bd0: 2023 2054 6865 2074 7269 6767 6572 2063   # The trigger c
+00045be0: 6f6e 6669 6775 7261 7469 6f6e 732e 0a20  onfigurations.. 
+00045bf0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00045c00: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
+00045c10: 2055 7064 6174 6554 7269 6767 6572 496e   UpdateTriggerIn
+00045c20: 7075 740a 0a20 2020 2064 6566 2076 616c  put..    def val
+00045c30: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00045c40: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00045c50: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00045c60: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00045c70: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00045c80: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00045c90: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00045ca0: 5570 6461 7465 5472 6967 6765 7252 6571  UpdateTriggerReq
+00045cb0: 7565 7374 2c20 7365 6c66 292e 746f 5f6d  uest, self).to_m
+00045cc0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00045cd0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00045ce0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00045cf0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00045d00: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00045d10: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00045d20: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+00045d30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00045d40: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+00045d50: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+00045d60: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+00045d70: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00045d80: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00045d90: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+00045da0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00045db0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00045dc0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00045dd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00045de0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00045df0: 203d 2055 7064 6174 6554 7269 6767 6572   = UpdateTrigger
+00045e00: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
+00045e10: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00045e20: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+00045e30: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+00045e40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00045e50: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
+00045e60: 6554 7269 6767 6572 5265 7370 6f6e 7365  eTriggerResponse
+00045e70: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00045e80: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00045e90: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
+00045ea0: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
+00045eb0: 652c 2062 6f64 793d 4e6f 6e65 293a 0a20  e, body=None):. 
+00045ec0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00045ed0: 6572 7320 3d20 6865 6164 6572 7320 2023  ers = headers  #
+00045ee0: 2074 7970 653a 2064 6963 745b 7374 722c   type: dict[str,
+00045ef0: 2073 7472 5d0a 2020 2020 2020 2020 7365   str].        se
+00045f00: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00045f10: 2073 7461 7475 735f 636f 6465 2020 2320   status_code  # 
+00045f20: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00045f30: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+00045f40: 6479 2020 2320 7479 7065 3a20 5472 6967  dy  # type: Trig
+00045f50: 6765 720a 0a20 2020 2064 6566 2076 616c  ger..    def val
+00045f60: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00045f70: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00045f80: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00045f90: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00045fa0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00045fb0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00045fc0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00045fd0: 5570 6461 7465 5472 6967 6765 7252 6573  UpdateTriggerRes
+00045fe0: 706f 6e73 652c 2073 656c 6629 2e74 6f5f  ponse, self).to_
+00045ff0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00046000: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00046010: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00046020: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00046030: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00046040: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00046050: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+00046060: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00046070: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+00046080: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+00046090: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000460a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000460b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000460c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000460d0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000460e0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000460f0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+00046100: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+00046110: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00046120: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+00046130: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+00046140: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+00046150: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00046160: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00046170: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+00046180: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00046190: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+000461a0: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+000461b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000461c0: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000461d0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+000461e0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+000461f0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+00046200: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+00046210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00046220: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00046230: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+00046240: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+00046250: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+00046260: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00046270: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00046280: 6f64 656c 203d 2054 7269 6767 6572 2829  odel = Trigger()
+00046290: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000462a0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+000462b0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+000462c0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+000462d0: 7265 7475 726e 2073 656c 660a 0a0a       return self...
```

### Comparing `alibabacloud_fc20230330_py2-4.0.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO` & `alibabacloud_fc20230330_py2-4.1.0/alibabacloud_fc20230330_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-fc20230330-py2
-Version: 4.0.0
+Version: 4.1.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330_py2-4.0.0/setup.py` & `alibabacloud_fc20230330_py2-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_fc20230330_py2.
 
-Created on 15/04/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_fc20230330"
 NAME = "alibabacloud_fc20230330_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Function Compute (20230330) SDK Library for Python2"
```

