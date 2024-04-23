# Comparing `tmp/alibabacloud_fc20230330-4.0.0.tar.gz` & `tmp/alibabacloud_fc20230330-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_fc20230330-4.0.0.tar", last modified: Mon Apr 15 08:40:29 2024, max compression
+gzip compressed data, was "dist/alibabacloud_fc20230330-4.1.0.tar", last modified: Tue Apr 23 06:21:49 2024, max compression
```

## Comparing `alibabacloud_fc20230330-4.0.0.tar` & `alibabacloud_fc20230330-4.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/
--rw-r--r--   0 root         (0) root         (0)     4489 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330/__init__.py
--rw-r--r--   0 root         (0) root         (0)   151117 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330/client.py
--rw-r--r--   0 root         (0) root         (0)   279312 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 08:40:29.000000 alibabacloud_fc20230330-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2024-04-15 08:40:28.000000 alibabacloud_fc20230330-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)     4694 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   162189 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330/client.py
+-rw-r--r--   0 root         (0) root         (0)   287705 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2620 2024-04-23 06:21:49.000000 alibabacloud_fc20230330-4.1.0/setup.py
```

### Comparing `alibabacloud_fc20230330-4.0.0/ChangeLog.md` & `alibabacloud_fc20230330-4.1.0/ChangeLog.md`

 * *Files 11% similar despite different names*

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

### Comparing `alibabacloud_fc20230330-4.0.0/LICENSE` & `alibabacloud_fc20230330-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330-4.0.0/PKG-INFO` & `alibabacloud_fc20230330-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_fc20230330
-Version: 4.0.0
+Version: 4.1.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330-4.0.0/README-CN.md` & `alibabacloud_fc20230330-4.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330-4.0.0/README.md` & `alibabacloud_fc20230330-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330/client.py` & `alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1331,14 +1331,98 @@
         function_name: str,
         request: fc20230330_models.GetAsyncInvokeConfigRequest,
     ) -> fc20230330_models.GetAsyncInvokeConfigResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_async_invoke_config_with_options_async(function_name, request, headers, runtime)
 
+    def get_async_task_with_options(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.GetAsyncTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fc20230330_models.GetAsyncTaskResponse:
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
+            pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-tasks/{OpenApiUtilClient.get_encode_param(task_id)}',
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
+    async def get_async_task_with_options_async(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.GetAsyncTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fc20230330_models.GetAsyncTaskResponse:
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
+            pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-tasks/{OpenApiUtilClient.get_encode_param(task_id)}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            fc20230330_models.GetAsyncTaskResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_async_task(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.GetAsyncTaskRequest,
+    ) -> fc20230330_models.GetAsyncTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_async_task_with_options(function_name, task_id, request, headers, runtime)
+
+    async def get_async_task_async(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.GetAsyncTaskRequest,
+    ) -> fc20230330_models.GetAsyncTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_async_task_with_options_async(function_name, task_id, request, headers, runtime)
+
     def get_concurrency_config_with_options(
         self,
         function_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> fc20230330_models.GetConcurrencyConfigResponse:
         req = open_api_models.OpenApiRequest(
@@ -2199,14 +2283,126 @@
         self,
         request: fc20230330_models.ListAsyncInvokeConfigsRequest,
     ) -> fc20230330_models.ListAsyncInvokeConfigsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_async_invoke_configs_with_options_async(request, headers, runtime)
 
+    def list_async_tasks_with_options(
+        self,
+        function_name: str,
+        request: fc20230330_models.ListAsyncTasksRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fc20230330_models.ListAsyncTasksResponse:
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
+            pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-tasks',
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
+    async def list_async_tasks_with_options_async(
+        self,
+        function_name: str,
+        request: fc20230330_models.ListAsyncTasksRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fc20230330_models.ListAsyncTasksResponse:
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
+            pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-tasks',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            fc20230330_models.ListAsyncTasksResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_async_tasks(
+        self,
+        function_name: str,
+        request: fc20230330_models.ListAsyncTasksRequest,
+    ) -> fc20230330_models.ListAsyncTasksResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_async_tasks_with_options(function_name, request, headers, runtime)
+
+    async def list_async_tasks_async(
+        self,
+        function_name: str,
+        request: fc20230330_models.ListAsyncTasksRequest,
+    ) -> fc20230330_models.ListAsyncTasksResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_async_tasks_with_options_async(function_name, request, headers, runtime)
+
     def list_concurrency_configs_with_options(
         self,
         request: fc20230330_models.ListConcurrencyConfigsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> fc20230330_models.ListConcurrencyConfigsResponse:
         UtilClient.validate_model(request)
@@ -3533,14 +3729,98 @@
         function_name: str,
         request: fc20230330_models.PutProvisionConfigRequest,
     ) -> fc20230330_models.PutProvisionConfigResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.put_provision_config_with_options_async(function_name, request, headers, runtime)
 
+    def stop_async_task_with_options(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.StopAsyncTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fc20230330_models.StopAsyncTaskResponse:
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
+            pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-tasks/{OpenApiUtilClient.get_encode_param(task_id)}/stop',
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
+    async def stop_async_task_with_options_async(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.StopAsyncTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fc20230330_models.StopAsyncTaskResponse:
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
+            pathname=f'/2023-03-30/functions/{OpenApiUtilClient.get_encode_param(function_name)}/async-tasks/{OpenApiUtilClient.get_encode_param(task_id)}/stop',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            fc20230330_models.StopAsyncTaskResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def stop_async_task(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.StopAsyncTaskRequest,
+    ) -> fc20230330_models.StopAsyncTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.stop_async_task_with_options(function_name, task_id, request, headers, runtime)
+
+    async def stop_async_task_async(
+        self,
+        function_name: str,
+        task_id: str,
+        request: fc20230330_models.StopAsyncTaskRequest,
+    ) -> fc20230330_models.StopAsyncTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.stop_async_task_with_options_async(function_name, task_id, request, headers, runtime)
+
     def tag_resources_with_options(
         self,
         request: fc20230330_models.TagResourcesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> fc20230330_models.TagResourcesResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330/models.py` & `alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12984,4474 +12984,4999 @@
 00032b70: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
 00032b80: 5f6d 6f64 656c 203d 2041 7379 6e63 436f  _model = AsyncCo
 00032b90: 6e66 6967 2829 0a20 2020 2020 2020 2020  nfig().         
 00032ba0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
 00032bb0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
 00032bc0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
 00032bd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00032be0: 660a 0a0a 636c 6173 7320 4765 7443 6f6e  f...class GetCon
-00032bf0: 6375 7272 656e 6379 436f 6e66 6967 5265  currencyConfigRe
-00032c00: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-00032c10: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00032c20: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00032c30: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-00032c40: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-00032c50: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00032c60: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-00032c70: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-00032c80: 2020 2062 6f64 793a 2043 6f6e 6375 7272     body: Concurr
-00032c90: 656e 6379 436f 6e66 6967 203d 204e 6f6e  encyConfig = Non
-00032ca0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00032cb0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00032cc0: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-00032cd0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00032ce0: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-00032cf0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00032d00: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-00032d10: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00032d20: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00032d30: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00032d40: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00032d50: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00032d60: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00032d70: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00032d80: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-00032d90: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00032da0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00032db0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00032dc0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00032dd0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00032de0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-00032df0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-00032e00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00032e10: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-00032e20: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-00032e30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00032e40: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-00032e50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00032e60: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-00032e70: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-00032e80: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-00032e90: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00032ea0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00032eb0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00032ec0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-00032ed0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-00032ee0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00032ef0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00032f00: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00032f10: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00032f20: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00032f30: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00032f40: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00032f50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00032f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00032f70: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00032f80: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00032f90: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00032fa0: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00032fb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00032fc0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00032fd0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-00032fe0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-00032ff0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-00033000: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00033010: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00033020: 5f6d 6f64 656c 203d 2043 6f6e 6375 7272  _model = Concurr
-00033030: 656e 6379 436f 6e66 6967 2829 0a20 2020  encyConfig().   
-00033040: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00033050: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-00033060: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-00033070: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-00033080: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00033090: 4765 7443 7573 746f 6d44 6f6d 6169 6e52  GetCustomDomainR
-000330a0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-000330b0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-000330c0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000330d0: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-000330e0: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-000330f0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00033100: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-00033110: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00033120: 2020 2020 626f 6479 3a20 4375 7374 6f6d      body: Custom
-00033130: 446f 6d61 696e 203d 204e 6f6e 652c 0a20  Domain = None,. 
-00033140: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00033150: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-00033160: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
-00033170: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-00033180: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-00033190: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-000331a0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
-000331b0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000331c0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-000331d0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-000331e0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-000331f0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00033200: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00033210: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00033220: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00033230: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00033240: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00033250: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00033260: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00033270: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00033280: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-00033290: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-000332a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000332b0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-000332c0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-000332d0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-000332e0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-000332f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00033300: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-00033310: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-00033320: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00033330: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-00033340: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00033350: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00033360: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00033370: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-00033380: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00033390: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000333a0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000333b0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000333c0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000333d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000333e0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-000333f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00033400: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00033410: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00033420: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00033430: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00033440: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00033450: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00033460: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00033470: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-00033480: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-00033490: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-000334a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000334b0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-000334c0: 656c 203d 2043 7573 746f 6d44 6f6d 6169  el = CustomDomai
-000334d0: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-000334e0: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-000334f0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00033500: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00033510: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00033520: 0a63 6c61 7373 2047 6574 4675 6e63 7469  .class GetFuncti
-00033530: 6f6e 5265 7175 6573 7428 5465 614d 6f64  onRequest(TeaMod
-00033540: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00033550: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00033560: 656c 662c 0a20 2020 2020 2020 2071 7561  elf,.        qua
-00033570: 6c69 6669 6572 3a20 7374 7220 3d20 4e6f  lifier: str = No
-00033580: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00033590: 2020 2023 2054 6865 2076 6572 7369 6f6e     # The version
-000335a0: 206f 7220 616c 6961 7320 6f66 2074 6865   or alias of the
-000335b0: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
-000335c0: 2020 2073 656c 662e 7175 616c 6966 6965     self.qualifie
-000335d0: 7220 3d20 7175 616c 6966 6965 720a 0a20  r = qualifier.. 
-000335e0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-000335f0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00033600: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00033610: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00033620: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00033630: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00033640: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00033650: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00033660: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00033670: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00033680: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00033690: 2069 6620 7365 6c66 2e71 7561 6c69 6669   if self.qualifi
-000336a0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-000336b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000336c0: 6c74 5b27 7175 616c 6966 6965 7227 5d20  lt['qualifier'] 
-000336d0: 3d20 7365 6c66 2e71 7561 6c69 6669 6572  = self.qualifier
-000336e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000336f0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00033700: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00033710: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-00033720: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00033730: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00033740: 6966 206d 2e67 6574 2827 7175 616c 6966  if m.get('qualif
-00033750: 6965 7227 2920 6973 206e 6f74 204e 6f6e  ier') is not Non
-00033760: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00033770: 656c 662e 7175 616c 6966 6965 7220 3d20  elf.qualifier = 
-00033780: 6d2e 6765 7428 2771 7561 6c69 6669 6572  m.get('qualifier
-00033790: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-000337a0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2047  n self...class G
-000337b0: 6574 4675 6e63 7469 6f6e 5265 7370 6f6e  etFunctionRespon
-000337c0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-000337d0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000337e0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000337f0: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-00033800: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-00033810: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00033820: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
-00033830: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
-00033840: 6f64 793a 2046 756e 6374 696f 6e20 3d20  ody: Function = 
-00033850: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00033860: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00033870: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-00033880: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-00033890: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-000338a0: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
-000338b0: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
-000338c0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000338d0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-000338e0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-000338f0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00033900: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-00033910: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00033920: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00033930: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-00033940: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00033950: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00033960: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00033970: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00033980: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00033990: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000339a0: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
-000339b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000339c0: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
-000339d0: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
-000339e0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
-000339f0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
-00033a00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00033a10: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00033a20: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
-00033a30: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
-00033a40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00033a50: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
-00033a60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00033a70: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
-00033a80: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
-00033a90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00033aa0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00033ab0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00033ac0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-00033ad0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00033ae0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00033af0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-00033b00: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-00033b10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00033b20: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-00033b30: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-00033b40: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00033b50: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00033b60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00033b70: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00033b80: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00033b90: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00033ba0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00033bb0: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-00033bc0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00033bd0: 656d 705f 6d6f 6465 6c20 3d20 4675 6e63  emp_model = Func
-00033be0: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
-00033bf0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-00033c00: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-00033c10: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-00033c20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00033c30: 660a 0a0a 636c 6173 7320 4765 7446 756e  f...class GetFun
-00033c40: 6374 696f 6e43 6f64 6552 6571 7565 7374  ctionCodeRequest
-00033c50: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00033c60: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00033c70: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00033c80: 2020 2020 7175 616c 6966 6965 723a 2073      qualifier: s
-00033c90: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
-00033ca0: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
-00033cb0: 7665 7273 696f 6e20 6f72 2061 6c69 6173  version or alias
-00033cc0: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
-00033cd0: 2e0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
-00033ce0: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
-00033cf0: 6669 6572 0a0a 2020 2020 6465 6620 7661  fier..    def va
-00033d00: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00033d10: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00033d20: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-00033d30: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-00033d40: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-00033d50: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-00033d60: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-00033d70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00033d80: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-00033d90: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-00033da0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00033db0: 7175 616c 6966 6965 7220 6973 206e 6f74  qualifier is not
-00033dc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00033dd0: 2020 2072 6573 756c 745b 2771 7561 6c69     result['quali
-00033de0: 6669 6572 275d 203d 2073 656c 662e 7175  fier'] = self.qu
-00033df0: 616c 6966 6965 720a 2020 2020 2020 2020  alifier.        
-00033e00: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00033e10: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00033e20: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00033e30: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00033e40: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00033e50: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00033e60: 2771 7561 6c69 6669 6572 2729 2069 7320  'qualifier') is 
-00033e70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00033e80: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
-00033e90: 6669 6572 203d 206d 2e67 6574 2827 7175  fier = m.get('qu
-00033ea0: 616c 6966 6965 7227 290a 2020 2020 2020  alifier').      
-00033eb0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00033ec0: 636c 6173 7320 4765 7446 756e 6374 696f  class GetFunctio
-00033ed0: 6e43 6f64 6552 6573 706f 6e73 6528 5465  nCodeResponse(Te
-00033ee0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00033ef0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00033f00: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00033f10: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
-00033f20: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
-00033f30: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
-00033f40: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
-00033f50: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-00033f60: 4f75 7470 7574 4675 6e63 436f 6465 203d  OutputFuncCode =
-00033f70: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-00033f80: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00033f90: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-00033fa0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00033fb0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-00033fc0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-00033fd0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-00033fe0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00033ff0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00034000: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-00034010: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00034020: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-00034030: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00034040: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00034050: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00034060: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00034070: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00034080: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00034090: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-000340a0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-000340b0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000340c0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-000340d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000340e0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-000340f0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00034100: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00034110: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00034120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00034130: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00034140: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-00034150: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00034160: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00034170: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00034180: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00034190: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-000341a0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-000341b0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-000341c0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000341d0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000341e0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000341f0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00034200: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00034210: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-00034220: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-00034230: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00034240: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-00034250: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-00034260: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00034270: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-00034280: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00034290: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000342a0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-000342b0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-000342c0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000342d0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-000342e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000342f0: 7465 6d70 5f6d 6f64 656c 203d 204f 7574  temp_model = Out
-00034300: 7075 7446 756e 6343 6f64 6528 290a 2020  putFuncCode().  
-00034310: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00034320: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-00034330: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-00034340: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-00034350: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00034360: 2047 6574 4c61 7965 7256 6572 7369 6f6e   GetLayerVersion
-00034370: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00034380: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00034390: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-000343a0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-000343b0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-000343c0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-000343d0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-000343e0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-000343f0: 2020 2020 2062 6f64 793a 204c 6179 6572       body: Layer
-00034400: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-00034410: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00034420: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-00034430: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00034440: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-00034450: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-00034460: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-00034470: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00034480: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00034490: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-000344a0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000344b0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-000344c0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000344d0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000344e0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000344f0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00034500: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00034510: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00034520: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00034530: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00034540: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00034550: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-00034560: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00034570: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-00034580: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-00034590: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-000345a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000345b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000345c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000345d0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-000345e0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-000345f0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-00034600: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-00034610: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00034620: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-00034630: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-00034640: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-00034650: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00034660: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00034670: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00034680: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00034690: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000346a0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-000346b0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-000346c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000346d0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-000346e0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000346f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00034700: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-00034710: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00034720: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00034730: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-00034740: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-00034750: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00034760: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-00034770: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00034780: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
-00034790: 6179 6572 2829 0a20 2020 2020 2020 2020  ayer().         
-000347a0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-000347b0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-000347c0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-000347d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000347e0: 660a 0a0a 636c 6173 7320 4765 744c 6179  f...class GetLay
-000347f0: 6572 5665 7273 696f 6e42 7941 726e 5265  erVersionByArnRe
-00034800: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-00034810: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00034820: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00034830: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-00034840: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-00034850: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00034860: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-00034870: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-00034880: 2020 2062 6f64 793a 204c 6179 6572 203d     body: Layer =
-00034890: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-000348a0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-000348b0: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-000348c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000348d0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-000348e0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-000348f0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-00034900: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00034910: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00034920: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-00034930: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00034940: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-00034950: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00034960: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00034970: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00034980: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00034990: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-000349a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000349b0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-000349c0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-000349d0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000349e0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-000349f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00034a00: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00034a10: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00034a20: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00034a30: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00034a40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00034a50: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00034a60: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-00034a70: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00034a80: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00034a90: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00034aa0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00034ab0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00034ac0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00034ad0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00034ae0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00034af0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00034b00: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-00034b10: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00034b20: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00034b30: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-00034b40: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-00034b50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00034b60: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-00034b70: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-00034b80: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00034b90: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-00034ba0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00034bb0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00034bc0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-00034bd0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-00034be0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00034bf0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-00034c00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00034c10: 7465 6d70 5f6d 6f64 656c 203d 204c 6179  temp_model = Lay
-00034c20: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-00034c30: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-00034c40: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-00034c50: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-00034c60: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00034c70: 0a0a 636c 6173 7320 4765 7450 726f 7669  ..class GetProvi
-00034c80: 7369 6f6e 436f 6e66 6967 5265 7175 6573  sionConfigReques
-00034c90: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
-00034ca0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00034cb0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00034cc0: 2020 2020 2071 7561 6c69 6669 6572 3a20       qualifier: 
-00034cd0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00034ce0: 293a 0a20 2020 2020 2020 2023 2054 6865  ):.        # The
-00034cf0: 2066 756e 6374 696f 6e20 616c 6961 7320   function alias 
-00034d00: 6f72 204c 4154 4553 542e 0a20 2020 2020  or LATEST..     
-00034d10: 2020 2073 656c 662e 7175 616c 6966 6965     self.qualifie
-00034d20: 7220 3d20 7175 616c 6966 6965 720a 0a20  r = qualifier.. 
-00034d30: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00034d40: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00034d50: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00034d60: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00034d70: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00034d80: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00034d90: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00034da0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00034db0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00034dc0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00034dd0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00034de0: 2069 6620 7365 6c66 2e71 7561 6c69 6669   if self.qualifi
-00034df0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00034e00: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00034e10: 6c74 5b27 7175 616c 6966 6965 7227 5d20  lt['qualifier'] 
-00034e20: 3d20 7365 6c66 2e71 7561 6c69 6669 6572  = self.qualifier
-00034e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00034e40: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00034e50: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00034e60: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-00034e70: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00034e80: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00034e90: 6966 206d 2e67 6574 2827 7175 616c 6966  if m.get('qualif
-00034ea0: 6965 7227 2920 6973 206e 6f74 204e 6f6e  ier') is not Non
-00034eb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00034ec0: 656c 662e 7175 616c 6966 6965 7220 3d20  elf.qualifier = 
-00034ed0: 6d2e 6765 7428 2771 7561 6c69 6669 6572  m.get('qualifier
-00034ee0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00034ef0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2047  n self...class G
-00034f00: 6574 5072 6f76 6973 696f 6e43 6f6e 6669  etProvisionConfi
-00034f10: 6752 6573 706f 6e73 6528 5465 614d 6f64  gResponse(TeaMod
-00034f20: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00034f30: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00034f40: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
-00034f50: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
-00034f60: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00034f70: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
-00034f80: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-00034f90: 2020 2020 2020 626f 6479 3a20 5072 6f76        body: Prov
-00034fa0: 6973 696f 6e43 6f6e 6669 6720 3d20 4e6f  isionConfig = No
-00034fb0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00034fc0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00034fd0: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-00034fe0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00034ff0: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-00035000: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-00035010: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-00035020: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00035030: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00035040: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
-00035050: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
-00035060: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-00035070: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00035080: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00035090: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-000350a0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-000350b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000350c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000350d0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-000350e0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-000350f0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00035100: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-00035110: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00035120: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-00035130: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-00035140: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00035150: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-00035160: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00035170: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-00035180: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-00035190: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-000351a0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-000351b0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-000351c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000351d0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-000351e0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-000351f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00035200: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00035210: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00035220: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00035230: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00035240: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00035250: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-00035260: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00035270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035280: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-00035290: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-000352a0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-000352b0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-000352c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000352d0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-000352e0: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-000352f0: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-00035300: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
-00035310: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-00035320: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00035330: 705f 6d6f 6465 6c20 3d20 5072 6f76 6973  p_model = Provis
-00035340: 696f 6e43 6f6e 6669 6728 290a 2020 2020  ionConfig().    
-00035350: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00035360: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-00035370: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-00035380: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-00035390: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2047  n self...class G
-000353a0: 6574 5472 6967 6765 7252 6573 706f 6e73  etTriggerRespons
-000353b0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-000353c0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-000353d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000353e0: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
-000353f0: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
-00035400: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
-00035410: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
-00035420: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
-00035430: 6479 3a20 5472 6967 6765 7220 3d20 4e6f  dy: Trigger = No
-00035440: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00035450: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00035460: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-00035470: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00035480: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-00035490: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-000354a0: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-000354b0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000354c0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-000354d0: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
-000354e0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
-000354f0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-00035500: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00035510: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00035520: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00035530: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00035540: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00035550: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00035560: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00035570: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00035580: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00035590: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-000355a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000355b0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-000355c0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-000355d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000355e0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-000355f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00035600: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-00035610: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-00035620: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-00035630: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00035640: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-00035650: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00035660: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-00035670: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-00035680: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00035690: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-000356a0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-000356b0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-000356c0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-000356d0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000356e0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-000356f0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00035700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035710: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-00035720: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-00035730: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-00035740: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-00035750: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00035760: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-00035770: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-00035780: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-00035790: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
-000357a0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-000357b0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-000357c0: 705f 6d6f 6465 6c20 3d20 5472 6967 6765  p_model = Trigge
-000357d0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-000357e0: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-000357f0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00035800: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00035810: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00035820: 0a63 6c61 7373 2049 6e76 6f6b 6546 756e  .class InvokeFun
-00035830: 6374 696f 6e48 6561 6465 7273 2854 6561  ctionHeaders(Tea
-00035840: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00035850: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00035860: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00035870: 636f 6d6d 6f6e 5f68 6561 6465 7273 3a20  common_headers: 
-00035880: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-00035890: 204e 6f6e 652c 0a20 2020 2020 2020 2078   None,.        x
-000358a0: 5f66 635f 6173 796e 635f 7461 736b 5f69  _fc_async_task_i
-000358b0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-000358c0: 2020 2020 2020 2078 5f66 635f 696e 766f         x_fc_invo
-000358d0: 6361 7469 6f6e 5f74 7970 653a 2073 7472  cation_type: str
-000358e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000358f0: 2078 5f66 635f 6c6f 675f 7479 7065 3a20   x_fc_log_type: 
-00035900: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00035910: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00035920: 636f 6d6d 6f6e 5f68 6561 6465 7273 203d  common_headers =
-00035930: 2063 6f6d 6d6f 6e5f 6865 6164 6572 730a   common_headers.
-00035940: 2020 2020 2020 2020 7365 6c66 2e78 5f66          self.x_f
-00035950: 635f 6173 796e 635f 7461 736b 5f69 6420  c_async_task_id 
-00035960: 3d20 785f 6663 5f61 7379 6e63 5f74 6173  = x_fc_async_tas
-00035970: 6b5f 6964 0a20 2020 2020 2020 2023 2054  k_id.        # T
-00035980: 6865 2074 7970 6520 6f66 2066 756e 6374  he type of funct
-00035990: 696f 6e20 696e 766f 6361 7469 6f6e 2e20  ion invocation. 
-000359a0: 5661 6c69 6420 7661 6c75 6573 3a20 5379  Valid values: Sy
-000359b0: 6e63 2061 6e64 2041 7379 6e63 2e0a 2020  nc and Async..  
-000359c0: 2020 2020 2020 7365 6c66 2e78 5f66 635f        self.x_fc_
-000359d0: 696e 766f 6361 7469 6f6e 5f74 7970 6520  invocation_type 
-000359e0: 3d20 785f 6663 5f69 6e76 6f63 6174 696f  = x_fc_invocatio
-000359f0: 6e5f 7479 7065 0a20 2020 2020 2020 2023  n_type.        #
-00035a00: 2054 6865 206c 6f67 2074 7970 6520 6f66   The log type of
-00035a10: 2066 756e 6374 696f 6e20 696e 766f 6361   function invoca
-00035a20: 7469 6f6e 2e20 5661 6c69 6420 7661 6c75  tion. Valid valu
-00035a30: 6573 3a20 4e6f 6e65 2061 6e64 2054 6169  es: None and Tai
-00035a40: 6c2e 0a20 2020 2020 2020 2073 656c 662e  l..        self.
-00035a50: 785f 6663 5f6c 6f67 5f74 7970 6520 3d20  x_fc_log_type = 
-00035a60: 785f 6663 5f6c 6f67 5f74 7970 650a 0a20  x_fc_log_type.. 
-00035a70: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00035a80: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00035a90: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00035aa0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00035ab0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00035ac0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00035ad0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00035ae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00035af0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00035b00: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00035b10: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00035b20: 2069 6620 7365 6c66 2e63 6f6d 6d6f 6e5f   if self.common_
-00035b30: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
-00035b40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00035b50: 2072 6573 756c 745b 2763 6f6d 6d6f 6e48   result['commonH
-00035b60: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-00035b70: 636f 6d6d 6f6e 5f68 6561 6465 7273 0a20  common_headers. 
-00035b80: 2020 2020 2020 2069 6620 7365 6c66 2e78         if self.x
-00035b90: 5f66 635f 6173 796e 635f 7461 736b 5f69  _fc_async_task_i
-00035ba0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00035bb0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00035bc0: 745b 2778 2d66 632d 6173 796e 632d 7461  t['x-fc-async-ta
-00035bd0: 736b 2d69 6427 5d20 3d20 7365 6c66 2e78  sk-id'] = self.x
-00035be0: 5f66 635f 6173 796e 635f 7461 736b 5f69  _fc_async_task_i
-00035bf0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00035c00: 662e 785f 6663 5f69 6e76 6f63 6174 696f  f.x_fc_invocatio
-00035c10: 6e5f 7479 7065 2069 7320 6e6f 7420 4e6f  n_type is not No
-00035c20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00035c30: 7265 7375 6c74 5b27 782d 6663 2d69 6e76  result['x-fc-inv
-00035c40: 6f63 6174 696f 6e2d 7479 7065 275d 203d  ocation-type'] =
-00035c50: 2073 656c 662e 785f 6663 5f69 6e76 6f63   self.x_fc_invoc
-00035c60: 6174 696f 6e5f 7479 7065 0a20 2020 2020  ation_type.     
-00035c70: 2020 2069 6620 7365 6c66 2e78 5f66 635f     if self.x_fc_
-00035c80: 6c6f 675f 7479 7065 2069 7320 6e6f 7420  log_type is not 
-00035c90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00035ca0: 2020 7265 7375 6c74 5b27 782d 6663 2d6c    result['x-fc-l
-00035cb0: 6f67 2d74 7970 6527 5d20 3d20 7365 6c66  og-type'] = self
-00035cc0: 2e78 5f66 635f 6c6f 675f 7479 7065 0a20  .x_fc_log_type. 
-00035cd0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00035ce0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00035cf0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00035d00: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00035d10: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00035d20: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00035d30: 206d 2e67 6574 2827 636f 6d6d 6f6e 4865   m.get('commonHe
-00035d40: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-00035d50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00035d60: 2073 656c 662e 636f 6d6d 6f6e 5f68 6561   self.common_hea
-00035d70: 6465 7273 203d 206d 2e67 6574 2827 636f  ders = m.get('co
-00035d80: 6d6d 6f6e 4865 6164 6572 7327 290a 2020  mmonHeaders').  
-00035d90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00035da0: 782d 6663 2d61 7379 6e63 2d74 6173 6b2d  x-fc-async-task-
-00035db0: 6964 2729 2069 7320 6e6f 7420 4e6f 6e65  id') is not None
-00035dc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00035dd0: 6c66 2e78 5f66 635f 6173 796e 635f 7461  lf.x_fc_async_ta
-00035de0: 736b 5f69 6420 3d20 6d2e 6765 7428 2778  sk_id = m.get('x
-00035df0: 2d66 632d 6173 796e 632d 7461 736b 2d69  -fc-async-task-i
-00035e00: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00035e10: 2e67 6574 2827 782d 6663 2d69 6e76 6f63  .get('x-fc-invoc
-00035e20: 6174 696f 6e2d 7479 7065 2729 2069 7320  ation-type') is 
-00035e30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00035e40: 2020 2020 2020 7365 6c66 2e78 5f66 635f        self.x_fc_
-00035e50: 696e 766f 6361 7469 6f6e 5f74 7970 6520  invocation_type 
-00035e60: 3d20 6d2e 6765 7428 2778 2d66 632d 696e  = m.get('x-fc-in
-00035e70: 766f 6361 7469 6f6e 2d74 7970 6527 290a  vocation-type').
-00035e80: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00035e90: 2827 782d 6663 2d6c 6f67 2d74 7970 6527  ('x-fc-log-type'
-00035ea0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00035eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00035ec0: 785f 6663 5f6c 6f67 5f74 7970 6520 3d20  x_fc_log_type = 
-00035ed0: 6d2e 6765 7428 2778 2d66 632d 6c6f 672d  m.get('x-fc-log-
-00035ee0: 7479 7065 2729 0a20 2020 2020 2020 2072  type').        r
-00035ef0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00035f00: 7373 2049 6e76 6f6b 6546 756e 6374 696f  ss InvokeFunctio
-00035f10: 6e52 6571 7565 7374 2854 6561 4d6f 6465  nRequest(TeaMode
-00035f20: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00035f30: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00035f40: 6c66 2c0a 2020 2020 2020 2020 626f 6479  lf,.        body
-00035f50: 3a20 4269 6e61 7279 494f 203d 204e 6f6e  : BinaryIO = Non
-00035f60: 652c 0a20 2020 2020 2020 2071 7561 6c69  e,.        quali
-00035f70: 6669 6572 3a20 7374 7220 3d20 4e6f 6e65  fier: str = None
-00035f80: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00035f90: 2023 2054 6865 2072 6571 7565 7374 2070   # The request p
-00035fa0: 6172 616d 6574 6572 7320 6f66 2066 756e  arameters of fun
-00035fb0: 6374 696f 6e20 696e 766f 6361 7469 6f6e  ction invocation
-00035fc0: 2e0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-00035fd0: 6f64 7920 3d20 626f 6479 0a20 2020 2020  ody = body.     
-00035fe0: 2020 2023 2054 6865 2076 6572 7369 6f6e     # The version
-00035ff0: 206f 7220 616c 6961 7320 6f66 2074 6865   or alias of the
-00036000: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
-00036010: 2020 2073 656c 662e 7175 616c 6966 6965     self.qualifie
-00036020: 7220 3d20 7175 616c 6966 6965 720a 0a20  r = qualifier.. 
-00036030: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00036040: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00036050: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00036060: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00036070: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00036080: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00036090: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000360a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000360b0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000360c0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000360d0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000360e0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-000360f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00036100: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00036110: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00036120: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
-00036130: 662e 7175 616c 6966 6965 7220 6973 206e  f.qualifier is n
-00036140: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00036150: 2020 2020 2072 6573 756c 745b 2771 7561       result['qua
-00036160: 6c69 6669 6572 275d 203d 2073 656c 662e  lifier'] = self.
-00036170: 7175 616c 6966 6965 720a 2020 2020 2020  qualifier.      
-00036180: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00036190: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-000361a0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-000361b0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-000361c0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-000361d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000361e0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-000361f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00036200: 2020 2073 656c 662e 626f 6479 203d 206d     self.body = m
-00036210: 2e67 6574 2827 626f 6479 2729 0a20 2020  .get('body').   
-00036220: 2020 2020 2069 6620 6d2e 6765 7428 2771       if m.get('q
-00036230: 7561 6c69 6669 6572 2729 2069 7320 6e6f  ualifier') is no
-00036240: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036250: 2020 2020 7365 6c66 2e71 7561 6c69 6669      self.qualifi
-00036260: 6572 203d 206d 2e67 6574 2827 7175 616c  er = m.get('qual
-00036270: 6966 6965 7227 290a 2020 2020 2020 2020  ifier').        
-00036280: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00036290: 6173 7320 496e 766f 6b65 4675 6e63 7469  ass InvokeFuncti
-000362a0: 6f6e 5265 7370 6f6e 7365 2854 6561 4d6f  onResponse(TeaMo
-000362b0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-000362c0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000362d0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
-000362e0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
-000362f0: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
-00036300: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
-00036310: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
-00036320: 2020 2020 2020 2062 6f64 793a 2042 696e         body: Bin
-00036330: 6172 7949 4f20 3d20 4e6f 6e65 2c0a 2020  aryIO = None,.  
-00036340: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00036350: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-00036360: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-00036370: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-00036380: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-00036390: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-000363a0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-000363b0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000363c0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000363d0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000363e0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-000363f0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00036400: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00036410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00036420: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00036430: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00036440: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00036450: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00036460: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-00036470: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00036480: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-00036490: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-000364a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000364b0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-000364c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000364d0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-000364e0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-000364f0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-00036500: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00036510: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-00036520: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00036530: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-00036540: 662e 626f 6479 0a20 2020 2020 2020 2072  f.body.        r
-00036550: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00036560: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00036570: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00036580: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00036590: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000365a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000365b0: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-000365c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000365d0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-000365e0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-000365f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00036600: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-00036610: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00036620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00036630: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-00036640: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-00036650: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00036660: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-00036670: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036680: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00036690: 6d2e 6765 7428 2762 6f64 7927 290a 2020  m.get('body').  
-000366a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000366b0: 660a 0a0a 636c 6173 7320 4c69 7374 416c  f...class ListAl
-000366c0: 6961 7365 7352 6571 7565 7374 2854 6561  iasesRequest(Tea
-000366d0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-000366e0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-000366f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00036700: 6c69 6d69 743a 2069 6e74 203d 204e 6f6e  limit: int = Non
-00036710: 652c 0a20 2020 2020 2020 206e 6578 745f  e,.        next_
-00036720: 746f 6b65 6e3a 2073 7472 203d 204e 6f6e  token: str = Non
-00036730: 652c 0a20 2020 2020 2020 2070 7265 6669  e,.        prefi
-00036740: 783a 2073 7472 203d 204e 6f6e 652c 0a20  x: str = None,. 
-00036750: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-00036760: 5468 6520 6e75 6d62 6572 206f 6620 616c  The number of al
-00036770: 6961 7365 7320 7265 7475 726e 6564 2e0a  iases returned..
-00036780: 2020 2020 2020 2020 7365 6c66 2e6c 696d          self.lim
-00036790: 6974 203d 206c 696d 6974 0a20 2020 2020  it = limit.     
-000367a0: 2020 2023 2054 6865 2070 6167 696e 6174     # The paginat
-000367b0: 696f 6e20 746f 6b65 6e20 7468 6174 2069  ion token that i
-000367c0: 7320 7573 6564 2069 6e20 7468 6520 6e65  s used in the ne
-000367d0: 7874 2072 6571 7565 7374 2074 6f20 7265  xt request to re
-000367e0: 7472 6965 7665 2061 206e 6577 2070 6167  trieve a new pag
-000367f0: 6520 6f66 2072 6573 756c 7473 2e0a 2020  e of results..  
-00036800: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
-00036810: 746f 6b65 6e20 3d20 6e65 7874 5f74 6f6b  token = next_tok
-00036820: 656e 0a20 2020 2020 2020 2023 2054 6865  en.        # The
-00036830: 2061 6c69 6173 2070 7265 6669 782e 0a20   alias prefix.. 
-00036840: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00036850: 6978 203d 2070 7265 6669 780a 0a20 2020  ix = prefix..   
-00036860: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00036870: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-00036880: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-00036890: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000368a0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000368b0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000368c0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000368d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000368e0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000368f0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00036900: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00036910: 6620 7365 6c66 2e6c 696d 6974 2069 7320  f self.limit is 
-00036920: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00036930: 2020 2020 2020 7265 7375 6c74 5b27 6c69        result['li
-00036940: 6d69 7427 5d20 3d20 7365 6c66 2e6c 696d  mit'] = self.lim
-00036950: 6974 0a20 2020 2020 2020 2069 6620 7365  it.        if se
-00036960: 6c66 2e6e 6578 745f 746f 6b65 6e20 6973  lf.next_token is
-00036970: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00036980: 2020 2020 2020 2072 6573 756c 745b 276e         result['n
-00036990: 6578 7454 6f6b 656e 275d 203d 2073 656c  extToken'] = sel
-000369a0: 662e 6e65 7874 5f74 6f6b 656e 0a20 2020  f.next_token.   
-000369b0: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-000369c0: 6669 7820 6973 206e 6f74 204e 6f6e 653a  fix is not None:
-000369d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000369e0: 756c 745b 2770 7265 6669 7827 5d20 3d20  ult['prefix'] = 
-000369f0: 7365 6c66 2e70 7265 6669 780a 2020 2020  self.prefix.    
-00036a00: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00036a10: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00036a20: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00036a30: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00036a40: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00036a50: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00036a60: 6765 7428 276c 696d 6974 2729 2069 7320  get('limit') is 
-00036a70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00036a80: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
-00036a90: 203d 206d 2e67 6574 2827 6c69 6d69 7427   = m.get('limit'
-00036aa0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00036ab0: 6574 2827 6e65 7874 546f 6b65 6e27 2920  et('nextToken') 
-00036ac0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00036ad0: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-00036ae0: 7874 5f74 6f6b 656e 203d 206d 2e67 6574  xt_token = m.get
-00036af0: 2827 6e65 7874 546f 6b65 6e27 290a 2020  ('nextToken').  
-00036b00: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00036b10: 7072 6566 6978 2729 2069 7320 6e6f 7420  prefix') is not 
-00036b20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00036b30: 2020 7365 6c66 2e70 7265 6669 7820 3d20    self.prefix = 
-00036b40: 6d2e 6765 7428 2770 7265 6669 7827 290a  m.get('prefix').
-00036b50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00036b60: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
-00036b70: 416c 6961 7365 7352 6573 706f 6e73 6528  AliasesResponse(
-00036b80: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00036b90: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00036ba0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00036bb0: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
-00036bc0: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-00036bd0: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
-00036be0: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
-00036bf0: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
-00036c00: 3a20 4c69 7374 416c 6961 7365 734f 7574  : ListAliasesOut
-00036c10: 7075 7420 3d20 4e6f 6e65 2c0a 2020 2020  put = None,.    
-00036c20: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00036c30: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-00036c40: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-00036c50: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-00036c60: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00036c70: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-00036c80: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-00036c90: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00036ca0: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-00036cb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00036cc0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-00036cd0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-00036ce0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00036cf0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-00036d00: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00036d10: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00036d20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00036d30: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00036d40: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00036d50: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00036d60: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-00036d70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00036d80: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00036d90: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-00036da0: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-00036db0: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-00036dc0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-00036dd0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00036de0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-00036df0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-00036e00: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-00036e10: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-00036e20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036e30: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-00036e40: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-00036e50: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00036e60: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00036e70: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00036e80: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00036e90: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00036ea0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00036eb0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00036ec0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-00036ed0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036ee0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00036ef0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-00036f00: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-00036f10: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00036f20: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00036f30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00036f40: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-00036f50: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00036f60: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00036f70: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-00036f80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00036f90: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-00036fa0: 3d20 4c69 7374 416c 6961 7365 734f 7574  = ListAliasesOut
-00036fb0: 7075 7428 290a 2020 2020 2020 2020 2020  put().          
-00036fc0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-00036fd0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-00036fe0: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-00036ff0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00037000: 0a0a 0a63 6c61 7373 204c 6973 7441 7379  ...class ListAsy
-00037010: 6e63 496e 766f 6b65 436f 6e66 6967 7352  ncInvokeConfigsR
-00037020: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-00037030: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00037040: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00037050: 2c0a 2020 2020 2020 2020 6675 6e63 7469  ,.        functi
-00037060: 6f6e 5f6e 616d 653a 2073 7472 203d 204e  on_name: str = N
-00037070: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
-00037080: 6974 3a20 696e 7420 3d20 4e6f 6e65 2c0a  it: int = None,.
-00037090: 2020 2020 2020 2020 6e65 7874 5f74 6f6b          next_tok
-000370a0: 656e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  en: str = None,.
-000370b0: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
-000370c0: 2054 6865 2066 756e 6374 696f 6e20 6e61   The function na
-000370d0: 6d65 2e20 4966 2079 6f75 2064 6f20 6e6f  me. If you do no
-000370e0: 7420 636f 6e66 6967 7572 6520 7468 6973  t configure this
-000370f0: 2070 6172 616d 6574 6572 2c20 7468 6520   parameter, the 
-00037100: 6173 796e 6368 726f 6e6f 7573 2069 6e76  asynchronous inv
-00037110: 6f63 6174 696f 6e20 636f 6e66 6967 7572  ocation configur
-00037120: 6174 696f 6e73 206f 6620 616c 6c20 6675  ations of all fu
-00037130: 6e63 7469 6f6e 7320 6172 6520 6469 7370  nctions are disp
-00037140: 6c61 7965 642e 0a20 2020 2020 2020 2073  layed..        s
-00037150: 656c 662e 6675 6e63 7469 6f6e 5f6e 616d  elf.function_nam
-00037160: 6520 3d20 6675 6e63 7469 6f6e 5f6e 616d  e = function_nam
-00037170: 650a 2020 2020 2020 2020 2320 5468 6520  e.        # The 
-00037180: 6d61 7869 6d75 6d20 6e75 6d62 6572 206f  maximum number o
-00037190: 6620 656e 7472 6965 7320 746f 2062 6520  f entries to be 
-000371a0: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
-000371b0: 2020 7365 6c66 2e6c 696d 6974 203d 206c    self.limit = l
-000371c0: 696d 6974 0a20 2020 2020 2020 2023 2054  imit.        # T
-000371d0: 6865 2070 6167 696e 6720 696e 666f 726d  he paging inform
-000371e0: 6174 696f 6e2e 2054 6869 7320 7061 7261  ation. This para
-000371f0: 6d65 7465 7220 7370 6563 6966 6965 7320  meter specifies 
-00037200: 7468 6520 7374 6172 7420 706f 696e 7420  the start point 
-00037210: 6f66 2074 6865 2071 7565 7279 2e0a 2020  of the query..  
-00037220: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
-00037230: 746f 6b65 6e20 3d20 6e65 7874 5f74 6f6b  token = next_tok
-00037240: 656e 0a0a 2020 2020 6465 6620 7661 6c69  en..    def vali
-00037250: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00037260: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00037270: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00037280: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00037290: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-000372a0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-000372b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000372c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000372d0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-000372e0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-000372f0: 2020 2020 2020 6966 2073 656c 662e 6675        if self.fu
-00037300: 6e63 7469 6f6e 5f6e 616d 6520 6973 206e  nction_name is n
-00037310: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00037320: 2020 2020 2072 6573 756c 745b 2766 756e       result['fun
-00037330: 6374 696f 6e4e 616d 6527 5d20 3d20 7365  ctionName'] = se
-00037340: 6c66 2e66 756e 6374 696f 6e5f 6e61 6d65  lf.function_name
-00037350: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00037360: 2e6c 696d 6974 2069 7320 6e6f 7420 4e6f  .limit is not No
-00037370: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00037380: 7265 7375 6c74 5b27 6c69 6d69 7427 5d20  result['limit'] 
-00037390: 3d20 7365 6c66 2e6c 696d 6974 0a20 2020  = self.limit.   
-000373a0: 2020 2020 2069 6620 7365 6c66 2e6e 6578       if self.nex
-000373b0: 745f 746f 6b65 6e20 6973 206e 6f74 204e  t_token is not N
-000373c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000373d0: 2072 6573 756c 745b 276e 6578 7454 6f6b   result['nextTok
-000373e0: 656e 275d 203d 2073 656c 662e 6e65 7874  en'] = self.next
-000373f0: 5f74 6f6b 656e 0a20 2020 2020 2020 2072  _token.        r
-00037400: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00037410: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00037420: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00037430: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00037440: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00037450: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00037460: 6675 6e63 7469 6f6e 4e61 6d65 2729 2069  functionName') i
-00037470: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00037480: 2020 2020 2020 2020 7365 6c66 2e66 756e          self.fun
-00037490: 6374 696f 6e5f 6e61 6d65 203d 206d 2e67  ction_name = m.g
-000374a0: 6574 2827 6675 6e63 7469 6f6e 4e61 6d65  et('functionName
-000374b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000374c0: 6765 7428 276c 696d 6974 2729 2069 7320  get('limit') is 
-000374d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000374e0: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
-000374f0: 203d 206d 2e67 6574 2827 6c69 6d69 7427   = m.get('limit'
-00037500: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00037510: 6574 2827 6e65 7874 546f 6b65 6e27 2920  et('nextToken') 
-00037520: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00037530: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-00037540: 7874 5f74 6f6b 656e 203d 206d 2e67 6574  xt_token = m.get
-00037550: 2827 6e65 7874 546f 6b65 6e27 290a 2020  ('nextToken').  
-00037560: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00037570: 660a 0a0a 636c 6173 7320 4c69 7374 4173  f...class ListAs
-00037580: 796e 6349 6e76 6f6b 6543 6f6e 6669 6773  yncInvokeConfigs
-00037590: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-000375a0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000375b0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-000375c0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-000375d0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-000375e0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-000375f0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-00037600: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00037610: 2020 2020 2062 6f64 793a 204c 6973 7441       body: ListA
-00037620: 7379 6e63 496e 766f 6b65 436f 6e66 6967  syncInvokeConfig
-00037630: 4f75 7470 7574 203d 204e 6f6e 652c 0a20  Output = None,. 
-00037640: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00037650: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-00037660: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
-00037670: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-00037680: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-00037690: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-000376a0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
-000376b0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000376c0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-000376d0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-000376e0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-000376f0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00037700: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00037710: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00037720: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00037730: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00037740: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00037750: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00037760: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00037770: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00037780: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-00037790: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-000377a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000377b0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-000377c0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-000377d0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-000377e0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-000377f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00037800: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-00037810: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-00037820: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00037830: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-00037840: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00037850: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00037860: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00037870: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-00037880: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00037890: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000378a0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000378b0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000378c0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000378d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000378e0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-000378f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00037900: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00037910: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00037920: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00037930: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00037940: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00037950: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00037960: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00037970: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-00037980: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-00037990: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-000379a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000379b0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-000379c0: 656c 203d 204c 6973 7441 7379 6e63 496e  el = ListAsyncIn
-000379d0: 766f 6b65 436f 6e66 6967 4f75 7470 7574  vokeConfigOutput
-000379e0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000379f0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00037a00: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00037a10: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00037a20: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00037a30: 636c 6173 7320 4c69 7374 436f 6e63 7572  class ListConcur
-00037a40: 7265 6e63 7943 6f6e 6669 6773 5265 7175  rencyConfigsRequ
-00037a50: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-00037a60: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00037a70: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00037a80: 2020 2020 2020 2066 756e 6374 696f 6e5f         function_
-00037a90: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-00037aa0: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
-00037ab0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00037ac0: 2020 2020 206e 6578 745f 746f 6b65 6e3a       next_token:
-00037ad0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00037ae0: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
-00037af0: 6520 6675 6e63 7469 6f6e 206e 616d 652e  e function name.
-00037b00: 2049 6620 796f 7520 6c65 6176 6520 7468   If you leave th
-00037b10: 6973 2070 6172 616d 6574 6572 2065 6d70  is parameter emp
-00037b20: 7479 2c20 7468 6520 636f 6e63 7572 7265  ty, the concurre
-00037b30: 6e63 7920 636f 6e66 6967 7572 6174 696f  ncy configuratio
-00037b40: 6e73 206f 6620 616c 6c20 6675 6e63 7469  ns of all functi
-00037b50: 6f6e 7320 6172 6520 7265 7475 726e 6564  ons are returned
-00037b60: 2e0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
-00037b70: 756e 6374 696f 6e5f 6e61 6d65 203d 2066  unction_name = f
-00037b80: 756e 6374 696f 6e5f 6e61 6d65 0a20 2020  unction_name.   
-00037b90: 2020 2020 2023 2054 6865 206d 6178 696d       # The maxim
-00037ba0: 756d 206e 756d 6265 7220 6f66 2065 6e74  um number of ent
-00037bb0: 7269 6573 2072 6574 7572 6e65 642e 0a20  ries returned.. 
-00037bc0: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
-00037bd0: 7420 3d20 6c69 6d69 740a 2020 2020 2020  t = limit.      
-00037be0: 2020 2320 5468 6520 7061 6769 6e61 7469    # The paginati
-00037bf0: 6f6e 2074 6f6b 656e 2074 6861 7420 6973  on token that is
-00037c00: 2075 7365 6420 696e 2074 6865 206e 6578   used in the nex
-00037c10: 7420 7265 7175 6573 7420 746f 2072 6574  t request to ret
-00037c20: 7269 6576 6520 6120 6e65 7720 7061 6765  rieve a new page
-00037c30: 206f 6620 7265 7375 6c74 732e 0a20 2020   of results..   
-00037c40: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
-00037c50: 6f6b 656e 203d 206e 6578 745f 746f 6b65  oken = next_toke
-00037c60: 6e0a 0a20 2020 2064 6566 2076 616c 6964  n..    def valid
-00037c70: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00037c80: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00037c90: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00037ca0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00037cb0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00037cc0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00037cd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00037ce0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00037cf0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00037d00: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00037d10: 2020 2020 2069 6620 7365 6c66 2e66 756e       if self.fun
-00037d20: 6374 696f 6e5f 6e61 6d65 2069 7320 6e6f  ction_name is no
-00037d30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00037d40: 2020 2020 7265 7375 6c74 5b27 6675 6e63      result['func
-00037d50: 7469 6f6e 4e61 6d65 275d 203d 2073 656c  tionName'] = sel
-00037d60: 662e 6675 6e63 7469 6f6e 5f6e 616d 650a  f.function_name.
-00037d70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00037d80: 6c69 6d69 7420 6973 206e 6f74 204e 6f6e  limit is not Non
-00037d90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00037da0: 6573 756c 745b 276c 696d 6974 275d 203d  esult['limit'] =
-00037db0: 2073 656c 662e 6c69 6d69 740a 2020 2020   self.limit.    
-00037dc0: 2020 2020 6966 2073 656c 662e 6e65 7874      if self.next
-00037dd0: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
-00037de0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00037df0: 7265 7375 6c74 5b27 6e65 7874 546f 6b65  result['nextToke
-00037e00: 6e27 5d20 3d20 7365 6c66 2e6e 6578 745f  n'] = self.next_
-00037e10: 746f 6b65 6e0a 2020 2020 2020 2020 7265  token.        re
-00037e20: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00037e30: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00037e40: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-00037e50: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00037e60: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00037e70: 2020 2020 2069 6620 6d2e 6765 7428 2766       if m.get('f
-00037e80: 756e 6374 696f 6e4e 616d 6527 2920 6973  unctionName') is
-00037e90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00037ea0: 2020 2020 2020 2073 656c 662e 6675 6e63         self.func
-00037eb0: 7469 6f6e 5f6e 616d 6520 3d20 6d2e 6765  tion_name = m.ge
-00037ec0: 7428 2766 756e 6374 696f 6e4e 616d 6527  t('functionName'
-00037ed0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00037ee0: 6574 2827 6c69 6d69 7427 2920 6973 206e  et('limit') is n
-00037ef0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00037f00: 2020 2020 2073 656c 662e 6c69 6d69 7420       self.limit 
-00037f10: 3d20 6d2e 6765 7428 276c 696d 6974 2729  = m.get('limit')
-00037f20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00037f30: 7428 276e 6578 7454 6f6b 656e 2729 2069  t('nextToken') i
-00037f40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00037f50: 2020 2020 2020 2020 7365 6c66 2e6e 6578          self.nex
-00037f60: 745f 746f 6b65 6e20 3d20 6d2e 6765 7428  t_token = m.get(
-00037f70: 276e 6578 7454 6f6b 656e 2729 0a20 2020  'nextToken').   
-00037f80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00037f90: 0a0a 0a63 6c61 7373 204c 6973 7443 6f6e  ...class ListCon
-00037fa0: 6375 7272 656e 6379 436f 6e66 6967 7352  currencyConfigsR
-00037fb0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00037fc0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00037fd0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00037fe0: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-00037ff0: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-00038000: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00038010: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-00038020: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00038030: 2020 2020 626f 6479 3a20 4c69 7374 436f      body: ListCo
-00038040: 6e63 7572 7265 6e63 7943 6f6e 6669 6773  ncurrencyConfigs
-00038050: 4f75 7470 7574 203d 204e 6f6e 652c 0a20  Output = None,. 
-00038060: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00038070: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-00038080: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
-00038090: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-000380a0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-000380b0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-000380c0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
-000380d0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000380e0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-000380f0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-00038100: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-00038110: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00038120: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00038130: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00038140: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00038150: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00038160: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00038170: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00038180: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00038190: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000381a0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-000381b0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-000381c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000381d0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-000381e0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-000381f0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00038200: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-00038210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00038220: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-00038230: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-00038240: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00038250: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-00038260: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00038270: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00038280: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00038290: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-000382a0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000382b0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000382c0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000382d0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000382e0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000382f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00038300: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-00038310: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00038320: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00038330: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00038340: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00038350: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00038360: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00038370: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00038380: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00038390: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-000383a0: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-000383b0: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-000383c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000383d0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-000383e0: 656c 203d 204c 6973 7443 6f6e 6375 7272  el = ListConcurr
-000383f0: 656e 6379 436f 6e66 6967 734f 7574 7075  encyConfigsOutpu
-00038400: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00038410: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-00038420: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00038430: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00038440: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00038450: 0a63 6c61 7373 204c 6973 7443 7573 746f  .class ListCusto
-00038460: 6d44 6f6d 6169 6e73 5265 7175 6573 7428  mDomainsRequest(
-00038470: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00038480: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00038490: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000384a0: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
-000384b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6e65  None,.        ne
-000384c0: 7874 5f74 6f6b 656e 3a20 7374 7220 3d20  xt_token: str = 
-000384d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
-000384e0: 6566 6978 3a20 7374 7220 3d20 4e6f 6e65  efix: str = None
-000384f0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00038500: 2023 2054 6865 206e 756d 6265 7220 6f66   # The number of
-00038510: 2063 7573 746f 6d20 646f 6d61 696e 206e   custom domain n
-00038520: 616d 6573 2072 6574 7572 6e65 642e 0a20  ames returned.. 
-00038530: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
-00038540: 7420 3d20 6c69 6d69 740a 2020 2020 2020  t = limit.      
-00038550: 2020 2320 5468 6520 7061 6769 6e61 7469    # The paginati
-00038560: 6f6e 2074 6f6b 656e 2074 6861 7420 6973  on token that is
-00038570: 2075 7365 6420 696e 2074 6865 206e 6578   used in the nex
-00038580: 7420 7265 7175 6573 7420 746f 2072 6574  t request to ret
-00038590: 7269 6576 6520 6120 6e65 7720 7061 6765  rieve a new page
-000385a0: 206f 6620 7265 7375 6c74 732e 0a20 2020   of results..   
-000385b0: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
-000385c0: 6f6b 656e 203d 206e 6578 745f 746f 6b65  oken = next_toke
-000385d0: 6e0a 2020 2020 2020 2020 2320 5468 6520  n.        # The 
-000385e0: 646f 6d61 696e 206e 616d 6520 7072 6566  domain name pref
-000385f0: 6978 2e0a 2020 2020 2020 2020 7365 6c66  ix..        self
-00038600: 2e70 7265 6669 7820 3d20 7072 6566 6978  .prefix = prefix
-00038610: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00038620: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00038630: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00038640: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00038650: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00038660: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00038670: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00032be0: 660a 0a0a 636c 6173 7320 4765 7441 7379  f...class GetAsy
+00032bf0: 6e63 5461 736b 5265 7175 6573 7428 5465  ncTaskRequest(Te
+00032c00: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00032c10: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00032c20: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00032c30: 2071 7561 6c69 6669 6572 3a20 7374 7220   qualifier: str 
+00032c40: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00032c50: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
+00032c60: 6966 6965 7220 3d20 7175 616c 6966 6965  ifier = qualifie
+00032c70: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
+00032c80: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00032c90: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00032ca0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00032cb0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00032cc0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00032cd0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00032ce0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00032cf0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00032d00: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00032d10: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00032d20: 2020 2020 2069 6620 7365 6c66 2e71 7561       if self.qua
+00032d30: 6c69 6669 6572 2069 7320 6e6f 7420 4e6f  lifier is not No
+00032d40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00032d50: 7265 7375 6c74 5b27 7175 616c 6966 6965  result['qualifie
+00032d60: 7227 5d20 3d20 7365 6c66 2e71 7561 6c69  r'] = self.quali
+00032d70: 6669 6572 0a20 2020 2020 2020 2072 6574  fier.        ret
+00032d80: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00032d90: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00032da0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00032db0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00032dc0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00032dd0: 2020 2020 6966 206d 2e67 6574 2827 7175      if m.get('qu
+00032de0: 616c 6966 6965 7227 2920 6973 206e 6f74  alifier') is not
+00032df0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00032e00: 2020 2073 656c 662e 7175 616c 6966 6965     self.qualifie
+00032e10: 7220 3d20 6d2e 6765 7428 2771 7561 6c69  r = m.get('quali
+00032e20: 6669 6572 2729 0a20 2020 2020 2020 2072  fier').        r
+00032e30: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00032e40: 7373 2047 6574 4173 796e 6354 6173 6b52  ss GetAsyncTaskR
+00032e50: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+00032e60: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00032e70: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00032e80: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
+00032e90: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
+00032ea0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00032eb0: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
+00032ec0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+00032ed0: 2020 2020 626f 6479 3a20 4173 796e 6354      body: AsyncT
+00032ee0: 6173 6b20 3d20 4e6f 6e65 2c0a 2020 2020  ask = None,.    
+00032ef0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00032f00: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+00032f10: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+00032f20: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+00032f30: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+00032f40: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+00032f50: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+00032f60: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00032f70: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+00032f80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00032f90: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+00032fa0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+00032fb0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00032fc0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00032fd0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00032fe0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00032ff0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00033000: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00033010: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00033020: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00033030: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+00033040: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033050: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00033060: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+00033070: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+00033080: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+00033090: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+000330a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000330b0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+000330c0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+000330d0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+000330e0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+000330f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00033100: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00033110: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00033120: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00033130: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00033140: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00033150: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00033160: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00033170: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00033180: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00033190: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+000331a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000331b0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000331c0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+000331d0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000331e0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+000331f0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00033200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00033210: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00033220: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00033230: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00033240: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00033250: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00033260: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+00033270: 3d20 4173 796e 6354 6173 6b28 290a 2020  = AsyncTask().  
+00033280: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00033290: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+000332a0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+000332b0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+000332c0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+000332d0: 2047 6574 436f 6e63 7572 7265 6e63 7943   GetConcurrencyC
+000332e0: 6f6e 6669 6752 6573 706f 6e73 6528 5465  onfigResponse(Te
+000332f0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00033300: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00033310: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00033320: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
+00033330: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
+00033340: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
+00033350: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
+00033360: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
+00033370: 436f 6e63 7572 7265 6e63 7943 6f6e 6669  ConcurrencyConfi
+00033380: 6720 3d20 4e6f 6e65 2c0a 2020 2020 293a  g = None,.    ):
+00033390: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000333a0: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+000333b0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000333c0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+000333d0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+000333e0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+000333f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00033400: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00033410: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+00033420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033430: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+00033440: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00033450: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00033460: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00033470: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00033480: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00033490: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000334a0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000334b0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000334c0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000334d0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+000334e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000334f0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+00033500: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+00033510: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+00033520: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+00033530: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+00033540: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00033550: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+00033560: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+00033570: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+00033580: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+00033590: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000335a0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+000335b0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+000335c0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+000335d0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000335e0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000335f0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00033600: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00033610: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00033620: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+00033630: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+00033640: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00033650: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00033660: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00033670: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00033680: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00033690: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000336a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000336b0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+000336c0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000336d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000336e0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+000336f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00033700: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00033710: 436f 6e63 7572 7265 6e63 7943 6f6e 6669  ConcurrencyConfi
+00033720: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+00033730: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+00033740: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+00033750: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+00033760: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00033770: 0a63 6c61 7373 2047 6574 4375 7374 6f6d  .class GetCustom
+00033780: 446f 6d61 696e 5265 7370 6f6e 7365 2854  DomainResponse(T
+00033790: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000337a0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000337b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000337c0: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+000337d0: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+000337e0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+000337f0: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+00033800: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+00033810: 2043 7573 746f 6d44 6f6d 6169 6e20 3d20   CustomDomain = 
+00033820: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00033830: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00033840: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+00033850: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00033860: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00033870: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
+00033880: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+00033890: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000338a0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+000338b0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+000338c0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000338d0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+000338e0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000338f0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00033900: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00033910: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00033920: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00033930: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00033940: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00033950: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00033960: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00033970: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+00033980: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00033990: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+000339a0: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+000339b0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+000339c0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+000339d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000339e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000339f0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+00033a00: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+00033a10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00033a20: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+00033a30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00033a40: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00033a50: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00033a60: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00033a70: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00033a80: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00033a90: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00033aa0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00033ab0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00033ac0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+00033ad0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+00033ae0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00033af0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+00033b00: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+00033b10: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00033b20: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+00033b30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00033b40: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00033b50: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00033b60: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00033b70: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00033b80: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+00033b90: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00033ba0: 656d 705f 6d6f 6465 6c20 3d20 4375 7374  emp_model = Cust
+00033bb0: 6f6d 446f 6d61 696e 2829 0a20 2020 2020  omDomain().     
+00033bc0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00033bd0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00033be0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00033bf0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00033c00: 2073 656c 660a 0a0a 636c 6173 7320 4765   self...class Ge
+00033c10: 7446 756e 6374 696f 6e52 6571 7565 7374  tFunctionRequest
+00033c20: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00033c30: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00033c40: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00033c50: 2020 2020 7175 616c 6966 6965 723a 2073      qualifier: s
+00033c60: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+00033c70: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
+00033c80: 7665 7273 696f 6e20 6f72 2061 6c69 6173  version or alias
+00033c90: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
+00033ca0: 2e0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
+00033cb0: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
+00033cc0: 6669 6572 0a0a 2020 2020 6465 6620 7661  fier..    def va
+00033cd0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00033ce0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00033cf0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00033d00: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00033d10: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00033d20: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00033d30: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00033d40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00033d50: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00033d60: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00033d70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00033d80: 7175 616c 6966 6965 7220 6973 206e 6f74  qualifier is not
+00033d90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00033da0: 2020 2072 6573 756c 745b 2771 7561 6c69     result['quali
+00033db0: 6669 6572 275d 203d 2073 656c 662e 7175  fier'] = self.qu
+00033dc0: 616c 6966 6965 720a 2020 2020 2020 2020  alifier.        
+00033dd0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00033de0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00033df0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00033e00: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00033e10: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00033e20: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00033e30: 2771 7561 6c69 6669 6572 2729 2069 7320  'qualifier') is 
+00033e40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00033e50: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
+00033e60: 6669 6572 203d 206d 2e67 6574 2827 7175  fier = m.get('qu
+00033e70: 616c 6966 6965 7227 290a 2020 2020 2020  alifier').      
+00033e80: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00033e90: 636c 6173 7320 4765 7446 756e 6374 696f  class GetFunctio
+00033ea0: 6e52 6573 706f 6e73 6528 5465 614d 6f64  nResponse(TeaMod
+00033eb0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00033ec0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00033ed0: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+00033ee0: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+00033ef0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00033f00: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+00033f10: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00033f20: 2020 2020 2020 626f 6479 3a20 4675 6e63        body: Func
+00033f30: 7469 6f6e 203d 204e 6f6e 652c 0a20 2020  tion = None,.   
+00033f40: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00033f50: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+00033f60: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+00033f70: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+00033f80: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+00033f90: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+00033fa0: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+00033fb0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00033fc0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00033fd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00033fe0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00033ff0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00034000: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00034010: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00034020: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00034030: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00034040: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00034050: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00034060: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00034070: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00034080: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00034090: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000340a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000340b0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+000340c0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+000340d0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+000340e0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+000340f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00034100: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00034110: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00034120: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00034130: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00034140: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00034150: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00034160: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00034170: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00034180: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00034190: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000341a0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+000341b0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+000341c0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+000341d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000341e0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+000341f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00034200: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00034210: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00034220: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00034230: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00034240: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00034250: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00034260: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00034270: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00034280: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00034290: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+000342a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000342b0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+000342c0: 203d 2046 756e 6374 696f 6e28 290a 2020   = Function().  
+000342d0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000342e0: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+000342f0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+00034300: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+00034310: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00034320: 2047 6574 4675 6e63 7469 6f6e 436f 6465   GetFunctionCode
+00034330: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00034340: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00034350: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00034360: 662c 0a20 2020 2020 2020 2071 7561 6c69  f,.        quali
+00034370: 6669 6572 3a20 7374 7220 3d20 4e6f 6e65  fier: str = None
+00034380: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00034390: 2023 2054 6865 2076 6572 7369 6f6e 206f   # The version o
+000343a0: 7220 616c 6961 7320 6f66 2074 6865 2066  r alias of the f
+000343b0: 756e 6374 696f 6e2e 0a20 2020 2020 2020  unction..       
+000343c0: 2073 656c 662e 7175 616c 6966 6965 7220   self.qualifier 
+000343d0: 3d20 7175 616c 6966 6965 720a 0a20 2020  = qualifier..   
+000343e0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000343f0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00034400: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00034410: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00034420: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00034430: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00034440: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00034450: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00034460: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00034470: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00034480: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00034490: 6620 7365 6c66 2e71 7561 6c69 6669 6572  f self.qualifier
+000344a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000344b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000344c0: 5b27 7175 616c 6966 6965 7227 5d20 3d20  ['qualifier'] = 
+000344d0: 7365 6c66 2e71 7561 6c69 6669 6572 0a20  self.qualifier. 
+000344e0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000344f0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00034500: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+00034510: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+00034520: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00034530: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00034540: 206d 2e67 6574 2827 7175 616c 6966 6965   m.get('qualifie
+00034550: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
+00034560: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00034570: 662e 7175 616c 6966 6965 7220 3d20 6d2e  f.qualifier = m.
+00034580: 6765 7428 2771 7561 6c69 6669 6572 2729  get('qualifier')
+00034590: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000345a0: 7365 6c66 0a0a 0a63 6c61 7373 2047 6574  self...class Get
+000345b0: 4675 6e63 7469 6f6e 436f 6465 5265 7370  FunctionCodeResp
+000345c0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+000345d0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000345e0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000345f0: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+00034600: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
+00034610: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00034620: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
+00034630: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00034640: 2062 6f64 793a 204f 7574 7075 7446 756e   body: OutputFun
+00034650: 6343 6f64 6520 3d20 4e6f 6e65 2c0a 2020  cCode = None,.  
+00034660: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00034670: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00034680: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+00034690: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000346a0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000346b0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+000346c0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+000346d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000346e0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+000346f0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00034700: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00034710: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00034720: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00034730: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00034740: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00034750: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00034760: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00034770: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00034780: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00034790: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000347a0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+000347b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000347c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000347d0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+000347e0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+000347f0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+00034800: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+00034810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00034820: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+00034830: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+00034840: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00034850: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+00034860: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034870: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+00034880: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+00034890: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000348a0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000348b0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000348c0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000348d0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+000348e0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+000348f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00034900: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+00034910: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034920: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00034930: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+00034940: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+00034950: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00034960: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+00034970: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00034980: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00034990: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000349a0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+000349b0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+000349c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000349d0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000349e0: 6c20 3d20 4f75 7470 7574 4675 6e63 436f  l = OutputFuncCo
+000349f0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00034a00: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00034a10: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00034a20: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00034a30: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00034a40: 0a0a 636c 6173 7320 4765 744c 6179 6572  ..class GetLayer
+00034a50: 5665 7273 696f 6e52 6573 706f 6e73 6528  VersionResponse(
+00034a60: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00034a70: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00034a80: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00034a90: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
+00034aa0: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+00034ab0: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
+00034ac0: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
+00034ad0: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+00034ae0: 3a20 4c61 7965 7220 3d20 4e6f 6e65 2c0a  : Layer = None,.
+00034af0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00034b00: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+00034b10: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
+00034b20: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00034b30: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
+00034b40: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00034b50: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
+00034b60: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00034b70: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00034b80: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+00034b90: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+00034ba0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+00034bb0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00034bc0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00034bd0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00034be0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00034bf0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034c00: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00034c10: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00034c20: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00034c30: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+00034c40: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+00034c50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00034c60: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+00034c70: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+00034c80: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+00034c90: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
+00034ca0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00034cb0: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
+00034cc0: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
+00034cd0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+00034ce0: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
+00034cf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00034d00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00034d10: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
+00034d20: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
+00034d30: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00034d40: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00034d50: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00034d60: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00034d70: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00034d80: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00034d90: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+00034da0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00034db0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00034dc0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+00034dd0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+00034de0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+00034df0: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+00034e00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00034e10: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00034e20: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+00034e30: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
+00034e40: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
+00034e50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00034e60: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00034e70: 6465 6c20 3d20 4c61 7965 7228 290a 2020  del = Layer().  
+00034e80: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00034e90: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+00034ea0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+00034eb0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+00034ec0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00034ed0: 2047 6574 4c61 7965 7256 6572 7369 6f6e   GetLayerVersion
+00034ee0: 4279 4172 6e52 6573 706f 6e73 6528 5465  ByArnResponse(Te
+00034ef0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00034f00: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00034f10: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00034f20: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
+00034f30: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
+00034f40: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
+00034f50: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
+00034f60: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
+00034f70: 4c61 7965 7220 3d20 4e6f 6e65 2c0a 2020  Layer = None,.  
+00034f80: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00034f90: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00034fa0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+00034fb0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+00034fc0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00034fd0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+00034fe0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+00034ff0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00035000: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00035010: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00035020: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00035030: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00035040: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00035050: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00035060: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00035070: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00035080: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035090: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000350a0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000350b0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000350c0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+000350d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000350e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000350f0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+00035100: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+00035110: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+00035120: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+00035130: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00035140: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+00035150: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+00035160: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00035170: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+00035180: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00035190: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+000351a0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+000351b0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000351c0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000351d0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000351e0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000351f0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+00035200: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00035210: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00035220: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+00035230: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00035240: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00035250: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+00035260: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+00035270: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00035280: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+00035290: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000352a0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000352b0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000352c0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+000352d0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+000352e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000352f0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+00035300: 6c20 3d20 4c61 7965 7228 290a 2020 2020  l = Layer().    
+00035310: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00035320: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+00035330: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+00035340: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+00035350: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2047  n self...class G
+00035360: 6574 5072 6f76 6973 696f 6e43 6f6e 6669  etProvisionConfi
+00035370: 6752 6571 7565 7374 2854 6561 4d6f 6465  gRequest(TeaMode
+00035380: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00035390: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000353a0: 6c66 2c0a 2020 2020 2020 2020 7175 616c  lf,.        qual
+000353b0: 6966 6965 723a 2073 7472 203d 204e 6f6e  ifier: str = Non
+000353c0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000353d0: 2020 2320 5468 6520 6675 6e63 7469 6f6e    # The function
+000353e0: 2061 6c69 6173 206f 7220 4c41 5445 5354   alias or LATEST
+000353f0: 2e0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
+00035400: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
+00035410: 6669 6572 0a0a 2020 2020 6465 6620 7661  fier..    def va
+00035420: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00035430: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00035440: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00035450: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00035460: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00035470: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00035480: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00035490: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000354a0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000354b0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000354c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000354d0: 7175 616c 6966 6965 7220 6973 206e 6f74  qualifier is not
+000354e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000354f0: 2020 2072 6573 756c 745b 2771 7561 6c69     result['quali
+00035500: 6669 6572 275d 203d 2073 656c 662e 7175  fier'] = self.qu
+00035510: 616c 6966 6965 720a 2020 2020 2020 2020  alifier.        
+00035520: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00035530: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00035540: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00035550: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00035560: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00035570: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00035580: 2771 7561 6c69 6669 6572 2729 2069 7320  'qualifier') is 
+00035590: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000355a0: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
+000355b0: 6669 6572 203d 206d 2e67 6574 2827 7175  fier = m.get('qu
+000355c0: 616c 6966 6965 7227 290a 2020 2020 2020  alifier').      
+000355d0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+000355e0: 636c 6173 7320 4765 7450 726f 7669 7369  class GetProvisi
+000355f0: 6f6e 436f 6e66 6967 5265 7370 6f6e 7365  onConfigResponse
+00035600: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00035610: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00035620: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00035630: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+00035640: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+00035650: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+00035660: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+00035670: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+00035680: 793a 2050 726f 7669 7369 6f6e 436f 6e66  y: ProvisionConf
+00035690: 6967 203d 204e 6f6e 652c 0a20 2020 2029  ig = None,.    )
+000356a0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+000356b0: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+000356c0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+000356d0: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+000356e0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+000356f0: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00035700: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00035710: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00035720: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+00035730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00035740: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+00035750: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00035760: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00035770: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00035780: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00035790: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000357a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000357b0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+000357c0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+000357d0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000357e0: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+000357f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00035800: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+00035810: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+00035820: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00035830: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+00035840: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+00035850: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00035860: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+00035870: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+00035880: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
+00035890: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+000358a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000358b0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
+000358c0: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
+000358d0: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
+000358e0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+000358f0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00035900: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00035910: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00035920: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00035930: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00035940: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+00035950: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00035960: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+00035970: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+00035980: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00035990: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+000359a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000359b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000359c0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+000359d0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+000359e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000359f0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+00035a00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035a10: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+00035a20: 2050 726f 7669 7369 6f6e 436f 6e66 6967   ProvisionConfig
+00035a30: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00035a40: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+00035a50: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+00035a60: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+00035a70: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00035a80: 636c 6173 7320 4765 7454 7269 6767 6572  class GetTrigger
+00035a90: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+00035aa0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00035ab0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00035ac0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
+00035ad0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
+00035ae0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00035af0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
+00035b00: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+00035b10: 2020 2020 2062 6f64 793a 2054 7269 6767       body: Trigg
+00035b20: 6572 203d 204e 6f6e 652c 0a20 2020 2029  er = None,.    )
+00035b30: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+00035b40: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+00035b50: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00035b60: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+00035b70: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00035b80: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00035b90: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00035ba0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00035bb0: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+00035bc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00035bd0: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+00035be0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00035bf0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00035c00: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00035c10: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00035c20: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00035c30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00035c40: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00035c50: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00035c60: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00035c70: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+00035c80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00035c90: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+00035ca0: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+00035cb0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00035cc0: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+00035cd0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+00035ce0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00035cf0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+00035d00: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+00035d10: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
+00035d20: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+00035d30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00035d40: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
+00035d50: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
+00035d60: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
+00035d70: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00035d80: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00035d90: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00035da0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00035db0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00035dc0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00035dd0: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+00035de0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00035df0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+00035e00: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+00035e10: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00035e20: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+00035e30: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00035e40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00035e50: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+00035e60: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+00035e70: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00035e80: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+00035e90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035ea0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+00035eb0: 2054 7269 6767 6572 2829 0a20 2020 2020   Trigger().     
+00035ec0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00035ed0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00035ee0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00035ef0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00035f00: 2073 656c 660a 0a0a 636c 6173 7320 496e   self...class In
+00035f10: 766f 6b65 4675 6e63 7469 6f6e 4865 6164  vokeFunctionHead
+00035f20: 6572 7328 5465 614d 6f64 656c 293a 0a20  ers(TeaModel):. 
+00035f30: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00035f40: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00035f50: 2020 2020 2020 2063 6f6d 6d6f 6e5f 6865         common_he
+00035f60: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00035f70: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00035f80: 2020 2020 2020 785f 6663 5f61 7379 6e63        x_fc_async
+00035f90: 5f74 6173 6b5f 6964 3a20 7374 7220 3d20  _task_id: str = 
+00035fa0: 4e6f 6e65 2c0a 2020 2020 2020 2020 785f  None,.        x_
+00035fb0: 6663 5f69 6e76 6f63 6174 696f 6e5f 7479  fc_invocation_ty
+00035fc0: 7065 3a20 7374 7220 3d20 4e6f 6e65 2c0a  pe: str = None,.
+00035fd0: 2020 2020 2020 2020 785f 6663 5f6c 6f67          x_fc_log
+00035fe0: 5f74 7970 653a 2073 7472 203d 204e 6f6e  _type: str = Non
+00035ff0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00036000: 2020 7365 6c66 2e63 6f6d 6d6f 6e5f 6865    self.common_he
+00036010: 6164 6572 7320 3d20 636f 6d6d 6f6e 5f68  aders = common_h
+00036020: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
+00036030: 656c 662e 785f 6663 5f61 7379 6e63 5f74  elf.x_fc_async_t
+00036040: 6173 6b5f 6964 203d 2078 5f66 635f 6173  ask_id = x_fc_as
+00036050: 796e 635f 7461 736b 5f69 640a 2020 2020  ync_task_id.    
+00036060: 2020 2020 2320 5468 6520 7479 7065 206f      # The type o
+00036070: 6620 6675 6e63 7469 6f6e 2069 6e76 6f63  f function invoc
+00036080: 6174 696f 6e2e 2056 616c 6964 2076 616c  ation. Valid val
+00036090: 7565 733a 2053 796e 6320 616e 6420 4173  ues: Sync and As
+000360a0: 796e 632e 0a20 2020 2020 2020 2073 656c  ync..        sel
+000360b0: 662e 785f 6663 5f69 6e76 6f63 6174 696f  f.x_fc_invocatio
+000360c0: 6e5f 7479 7065 203d 2078 5f66 635f 696e  n_type = x_fc_in
+000360d0: 766f 6361 7469 6f6e 5f74 7970 650a 2020  vocation_type.  
+000360e0: 2020 2020 2020 2320 5468 6520 6c6f 6720        # The log 
+000360f0: 7479 7065 206f 6620 6675 6e63 7469 6f6e  type of function
+00036100: 2069 6e76 6f63 6174 696f 6e2e 2056 616c   invocation. Val
+00036110: 6964 2076 616c 7565 733a 204e 6f6e 6520  id values: None 
+00036120: 616e 6420 5461 696c 2e0a 2020 2020 2020  and Tail..      
+00036130: 2020 7365 6c66 2e78 5f66 635f 6c6f 675f    self.x_fc_log_
+00036140: 7479 7065 203d 2078 5f66 635f 6c6f 675f  type = x_fc_log_
+00036150: 7479 7065 0a0a 2020 2020 6465 6620 7661  type..    def va
+00036160: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00036170: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00036180: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00036190: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000361a0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+000361b0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000361c0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000361d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000361e0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000361f0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00036200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00036210: 636f 6d6d 6f6e 5f68 6561 6465 7273 2069  common_headers i
+00036220: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00036230: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00036240: 636f 6d6d 6f6e 4865 6164 6572 7327 5d20  commonHeaders'] 
+00036250: 3d20 7365 6c66 2e63 6f6d 6d6f 6e5f 6865  = self.common_he
+00036260: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+00036270: 2073 656c 662e 785f 6663 5f61 7379 6e63   self.x_fc_async
+00036280: 5f74 6173 6b5f 6964 2069 7320 6e6f 7420  _task_id is not 
+00036290: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000362a0: 2020 7265 7375 6c74 5b27 782d 6663 2d61    result['x-fc-a
+000362b0: 7379 6e63 2d74 6173 6b2d 6964 275d 203d  sync-task-id'] =
+000362c0: 2073 656c 662e 785f 6663 5f61 7379 6e63   self.x_fc_async
+000362d0: 5f74 6173 6b5f 6964 0a20 2020 2020 2020  _task_id.       
+000362e0: 2069 6620 7365 6c66 2e78 5f66 635f 696e   if self.x_fc_in
+000362f0: 766f 6361 7469 6f6e 5f74 7970 6520 6973  vocation_type is
+00036300: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00036310: 2020 2020 2020 2072 6573 756c 745b 2778         result['x
+00036320: 2d66 632d 696e 766f 6361 7469 6f6e 2d74  -fc-invocation-t
+00036330: 7970 6527 5d20 3d20 7365 6c66 2e78 5f66  ype'] = self.x_f
+00036340: 635f 696e 766f 6361 7469 6f6e 5f74 7970  c_invocation_typ
+00036350: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00036360: 662e 785f 6663 5f6c 6f67 5f74 7970 6520  f.x_fc_log_type 
+00036370: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00036380: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00036390: 2778 2d66 632d 6c6f 672d 7479 7065 275d  'x-fc-log-type']
+000363a0: 203d 2073 656c 662e 785f 6663 5f6c 6f67   = self.x_fc_log
+000363b0: 5f74 7970 650a 2020 2020 2020 2020 7265  _type.        re
+000363c0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000363d0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000363e0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000363f0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00036400: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00036410: 2020 2020 2069 6620 6d2e 6765 7428 2763       if m.get('c
+00036420: 6f6d 6d6f 6e48 6561 6465 7273 2729 2069  ommonHeaders') i
+00036430: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00036440: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+00036450: 6d6f 6e5f 6865 6164 6572 7320 3d20 6d2e  mon_headers = m.
+00036460: 6765 7428 2763 6f6d 6d6f 6e48 6561 6465  get('commonHeade
+00036470: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00036480: 6d2e 6765 7428 2778 2d66 632d 6173 796e  m.get('x-fc-asyn
+00036490: 632d 7461 736b 2d69 6427 2920 6973 206e  c-task-id') is n
+000364a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000364b0: 2020 2020 2073 656c 662e 785f 6663 5f61       self.x_fc_a
+000364c0: 7379 6e63 5f74 6173 6b5f 6964 203d 206d  sync_task_id = m
+000364d0: 2e67 6574 2827 782d 6663 2d61 7379 6e63  .get('x-fc-async
+000364e0: 2d74 6173 6b2d 6964 2729 0a20 2020 2020  -task-id').     
+000364f0: 2020 2069 6620 6d2e 6765 7428 2778 2d66     if m.get('x-f
+00036500: 632d 696e 766f 6361 7469 6f6e 2d74 7970  c-invocation-typ
+00036510: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00036520: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00036530: 662e 785f 6663 5f69 6e76 6f63 6174 696f  f.x_fc_invocatio
+00036540: 6e5f 7479 7065 203d 206d 2e67 6574 2827  n_type = m.get('
+00036550: 782d 6663 2d69 6e76 6f63 6174 696f 6e2d  x-fc-invocation-
+00036560: 7479 7065 2729 0a20 2020 2020 2020 2069  type').        i
+00036570: 6620 6d2e 6765 7428 2778 2d66 632d 6c6f  f m.get('x-fc-lo
+00036580: 672d 7479 7065 2729 2069 7320 6e6f 7420  g-type') is not 
+00036590: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000365a0: 2020 7365 6c66 2e78 5f66 635f 6c6f 675f    self.x_fc_log_
+000365b0: 7479 7065 203d 206d 2e67 6574 2827 782d  type = m.get('x-
+000365c0: 6663 2d6c 6f67 2d74 7970 6527 290a 2020  fc-log-type').  
+000365d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000365e0: 660a 0a0a 636c 6173 7320 496e 766f 6b65  f...class Invoke
+000365f0: 4675 6e63 7469 6f6e 5265 7175 6573 7428  FunctionRequest(
+00036600: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00036610: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00036620: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00036630: 2020 2062 6f64 793a 2042 696e 6172 7949     body: BinaryI
+00036640: 4f20 3d20 4e6f 6e65 2c0a 2020 2020 2020  O = None,.      
+00036650: 2020 7175 616c 6966 6965 723a 2073 7472    qualifier: str
+00036660: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00036670: 2020 2020 2020 2020 2320 5468 6520 7265          # The re
+00036680: 7175 6573 7420 7061 7261 6d65 7465 7273  quest parameters
+00036690: 206f 6620 6675 6e63 7469 6f6e 2069 6e76   of function inv
+000366a0: 6f63 6174 696f 6e2e 0a20 2020 2020 2020  ocation..       
+000366b0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+000366c0: 790a 2020 2020 2020 2020 2320 5468 6520  y.        # The 
+000366d0: 7665 7273 696f 6e20 6f72 2061 6c69 6173  version or alias
+000366e0: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
+000366f0: 2e0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
+00036700: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
+00036710: 6669 6572 0a0a 2020 2020 6465 6620 7661  fier..    def va
+00036720: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00036730: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00036740: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00036750: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00036760: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00036770: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00036780: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00036790: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000367a0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000367b0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000367c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000367d0: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+000367e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000367f0: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00036800: 656c 662e 626f 6479 0a20 2020 2020 2020  elf.body.       
+00036810: 2069 6620 7365 6c66 2e71 7561 6c69 6669   if self.qualifi
+00036820: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+00036830: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00036840: 6c74 5b27 7175 616c 6966 6965 7227 5d20  lt['qualifier'] 
+00036850: 3d20 7365 6c66 2e71 7561 6c69 6669 6572  = self.qualifier
+00036860: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00036870: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00036880: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00036890: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000368a0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000368b0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000368c0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+000368d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000368e0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000368f0: 6f64 7920 3d20 6d2e 6765 7428 2762 6f64  ody = m.get('bod
+00036900: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
+00036910: 2e67 6574 2827 7175 616c 6966 6965 7227  .get('qualifier'
+00036920: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00036930: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00036940: 7175 616c 6966 6965 7220 3d20 6d2e 6765  qualifier = m.ge
+00036950: 7428 2771 7561 6c69 6669 6572 2729 0a20  t('qualifier'). 
+00036960: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00036970: 6c66 0a0a 0a63 6c61 7373 2049 6e76 6f6b  lf...class Invok
+00036980: 6546 756e 6374 696f 6e52 6573 706f 6e73  eFunctionRespons
+00036990: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+000369a0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000369b0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000369c0: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+000369d0: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+000369e0: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+000369f0: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+00036a00: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+00036a10: 6479 3a20 4269 6e61 7279 494f 203d 204e  dy: BinaryIO = N
+00036a20: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00036a30: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00036a40: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+00036a50: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+00036a60: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+00036a70: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
+00036a80: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
+00036a90: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00036aa0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00036ab0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00036ac0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00036ad0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00036ae0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00036af0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00036b00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00036b10: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00036b20: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00036b30: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00036b40: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+00036b50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00036b60: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+00036b70: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+00036b80: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00036b90: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+00036ba0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+00036bb0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00036bc0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+00036bd0: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+00036be0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
+00036bf0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+00036c00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00036c10: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
+00036c20: 5d20 3d20 7365 6c66 2e62 6f64 790a 2020  ] = self.body.  
+00036c30: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00036c40: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00036c50: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00036c60: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00036c70: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00036c80: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00036c90: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00036ca0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00036cb0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00036cc0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+00036cd0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00036ce0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+00036cf0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+00036d00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00036d10: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00036d20: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+00036d30: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+00036d40: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+00036d50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00036d60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00036d70: 626f 6479 203d 206d 2e67 6574 2827 626f  body = m.get('bo
+00036d80: 6479 2729 0a20 2020 2020 2020 2072 6574  dy').        ret
+00036d90: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00036da0: 204c 6973 7441 6c69 6173 6573 5265 7175   ListAliasesRequ
+00036db0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+00036dc0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00036dd0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00036de0: 2020 2020 2020 206c 696d 6974 3a20 696e         limit: in
+00036df0: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+00036e00: 2020 6e65 7874 5f74 6f6b 656e 3a20 7374    next_token: st
+00036e10: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00036e20: 2020 7072 6566 6978 3a20 7374 7220 3d20    prefix: str = 
+00036e30: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00036e40: 2020 2020 2023 2054 6865 206e 756d 6265       # The numbe
+00036e50: 7220 6f66 2061 6c69 6173 6573 2072 6574  r of aliases ret
+00036e60: 7572 6e65 642e 0a20 2020 2020 2020 2073  urned..        s
+00036e70: 656c 662e 6c69 6d69 7420 3d20 6c69 6d69  elf.limit = limi
+00036e80: 740a 2020 2020 2020 2020 2320 5468 6520  t.        # The 
+00036e90: 7061 6769 6e61 7469 6f6e 2074 6f6b 656e  pagination token
+00036ea0: 2074 6861 7420 6973 2075 7365 6420 696e   that is used in
+00036eb0: 2074 6865 206e 6578 7420 7265 7175 6573   the next reques
+00036ec0: 7420 746f 2072 6574 7269 6576 6520 6120  t to retrieve a 
+00036ed0: 6e65 7720 7061 6765 206f 6620 7265 7375  new page of resu
+00036ee0: 6c74 732e 0a20 2020 2020 2020 2073 656c  lts..        sel
+00036ef0: 662e 6e65 7874 5f74 6f6b 656e 203d 206e  f.next_token = n
+00036f00: 6578 745f 746f 6b65 6e0a 2020 2020 2020  ext_token.      
+00036f10: 2020 2320 5468 6520 616c 6961 7320 7072    # The alias pr
+00036f20: 6566 6978 2e0a 2020 2020 2020 2020 7365  efix..        se
+00036f30: 6c66 2e70 7265 6669 7820 3d20 7072 6566  lf.prefix = pref
+00036f40: 6978 0a0a 2020 2020 6465 6620 7661 6c69  ix..    def vali
+00036f50: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00036f60: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00036f70: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00036f80: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00036f90: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+00036fa0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00036fb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00036fc0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00036fd0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00036fe0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00036ff0: 2020 2020 2020 6966 2073 656c 662e 6c69        if self.li
+00037000: 6d69 7420 6973 206e 6f74 204e 6f6e 653a  mit is not None:
+00037010: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00037020: 756c 745b 276c 696d 6974 275d 203d 2073  ult['limit'] = s
+00037030: 656c 662e 6c69 6d69 740a 2020 2020 2020  elf.limit.      
+00037040: 2020 6966 2073 656c 662e 6e65 7874 5f74    if self.next_t
+00037050: 6f6b 656e 2069 7320 6e6f 7420 4e6f 6e65  oken is not None
+00037060: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00037070: 7375 6c74 5b27 6e65 7874 546f 6b65 6e27  sult['nextToken'
+00037080: 5d20 3d20 7365 6c66 2e6e 6578 745f 746f  ] = self.next_to
+00037090: 6b65 6e0a 2020 2020 2020 2020 6966 2073  ken.        if s
+000370a0: 656c 662e 7072 6566 6978 2069 7320 6e6f  elf.prefix is no
+000370b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000370c0: 2020 2020 7265 7375 6c74 5b27 7072 6566      result['pref
+000370d0: 6978 275d 203d 2073 656c 662e 7072 6566  ix'] = self.pref
+000370e0: 6978 0a20 2020 2020 2020 2072 6574 7572  ix.        retur
+000370f0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00037100: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00037110: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00037120: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00037130: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00037140: 2020 6966 206d 2e67 6574 2827 6c69 6d69    if m.get('limi
+00037150: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
+00037160: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00037170: 662e 6c69 6d69 7420 3d20 6d2e 6765 7428  f.limit = m.get(
+00037180: 276c 696d 6974 2729 0a20 2020 2020 2020  'limit').       
+00037190: 2069 6620 6d2e 6765 7428 276e 6578 7454   if m.get('nextT
+000371a0: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
+000371b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000371c0: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
+000371d0: 3d20 6d2e 6765 7428 276e 6578 7454 6f6b  = m.get('nextTok
+000371e0: 656e 2729 0a20 2020 2020 2020 2069 6620  en').        if 
+000371f0: 6d2e 6765 7428 2770 7265 6669 7827 2920  m.get('prefix') 
+00037200: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00037210: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00037220: 6566 6978 203d 206d 2e67 6574 2827 7072  efix = m.get('pr
+00037230: 6566 6978 2729 0a20 2020 2020 2020 2072  efix').        r
+00037240: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00037250: 7373 204c 6973 7441 6c69 6173 6573 5265  ss ListAliasesRe
+00037260: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00037270: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00037280: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00037290: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+000372a0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+000372b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+000372c0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+000372d0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+000372e0: 2020 2062 6f64 793a 204c 6973 7441 6c69     body: ListAli
+000372f0: 6173 6573 4f75 7470 7574 203d 204e 6f6e  asesOutput = Non
+00037300: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00037310: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00037320: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+00037330: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00037340: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
+00037350: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00037360: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
+00037370: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00037380: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00037390: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+000373a0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+000373b0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+000373c0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000373d0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000373e0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000373f0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00037400: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00037410: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00037420: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00037430: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00037440: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+00037450: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+00037460: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00037470: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+00037480: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+00037490: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000374a0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+000374b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000374c0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+000374d0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+000374e0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+000374f0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00037500: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+00037510: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00037520: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+00037530: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+00037540: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00037550: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00037560: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+00037570: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+00037580: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00037590: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000375a0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+000375b0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000375c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000375d0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+000375e0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+000375f0: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
+00037600: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
+00037610: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00037620: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+00037630: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
+00037640: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
+00037650: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+00037660: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00037670: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00037680: 5f6d 6f64 656c 203d 204c 6973 7441 6c69  _model = ListAli
+00037690: 6173 6573 4f75 7470 7574 2829 0a20 2020  asesOutput().   
+000376a0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000376b0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+000376c0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+000376d0: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+000376e0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000376f0: 4c69 7374 4173 796e 6349 6e76 6f6b 6543  ListAsyncInvokeC
+00037700: 6f6e 6669 6773 5265 7175 6573 7428 5465  onfigsRequest(Te
+00037710: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00037720: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00037730: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00037740: 2066 756e 6374 696f 6e5f 6e61 6d65 3a20   function_name: 
+00037750: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00037760: 2020 2020 6c69 6d69 743a 2069 6e74 203d      limit: int =
+00037770: 204e 6f6e 652c 0a20 2020 2020 2020 206e   None,.        n
+00037780: 6578 745f 746f 6b65 6e3a 2073 7472 203d  ext_token: str =
+00037790: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000377a0: 2020 2020 2020 2320 5468 6520 6675 6e63        # The func
+000377b0: 7469 6f6e 206e 616d 652e 2049 6620 796f  tion name. If yo
+000377c0: 7520 646f 206e 6f74 2063 6f6e 6669 6775  u do not configu
+000377d0: 7265 2074 6869 7320 7061 7261 6d65 7465  re this paramete
+000377e0: 722c 2074 6865 2061 7379 6e63 6872 6f6e  r, the asynchron
+000377f0: 6f75 7320 696e 766f 6361 7469 6f6e 2063  ous invocation c
+00037800: 6f6e 6669 6775 7261 7469 6f6e 7320 6f66  onfigurations of
+00037810: 2061 6c6c 2066 756e 6374 696f 6e73 2061   all functions a
+00037820: 7265 2064 6973 706c 6179 6564 2e0a 2020  re displayed..  
+00037830: 2020 2020 2020 7365 6c66 2e66 756e 6374        self.funct
+00037840: 696f 6e5f 6e61 6d65 203d 2066 756e 6374  ion_name = funct
+00037850: 696f 6e5f 6e61 6d65 0a20 2020 2020 2020  ion_name.       
+00037860: 2023 2054 6865 206d 6178 696d 756d 206e   # The maximum n
+00037870: 756d 6265 7220 6f66 2065 6e74 7269 6573  umber of entries
+00037880: 2074 6f20 6265 2072 6574 7572 6e65 642e   to be returned.
+00037890: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000378a0: 6d69 7420 3d20 6c69 6d69 740a 2020 2020  mit = limit.    
+000378b0: 2020 2020 2320 5468 6520 7061 6769 6e67      # The paging
+000378c0: 2069 6e66 6f72 6d61 7469 6f6e 2e20 5468   information. Th
+000378d0: 6973 2070 6172 616d 6574 6572 2073 7065  is parameter spe
+000378e0: 6369 6669 6573 2074 6865 2073 7461 7274  cifies the start
+000378f0: 2070 6f69 6e74 206f 6620 7468 6520 7175   point of the qu
+00037900: 6572 792e 0a20 2020 2020 2020 2073 656c  ery..        sel
+00037910: 662e 6e65 7874 5f74 6f6b 656e 203d 206e  f.next_token = n
+00037920: 6578 745f 746f 6b65 6e0a 0a20 2020 2064  ext_token..    d
+00037930: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00037940: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00037950: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00037960: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00037970: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00037980: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00037990: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000379a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000379b0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000379c0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000379d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000379e0: 7365 6c66 2e66 756e 6374 696f 6e5f 6e61  self.function_na
+000379f0: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+00037a00: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00037a10: 6c74 5b27 6675 6e63 7469 6f6e 4e61 6d65  lt['functionName
+00037a20: 275d 203d 2073 656c 662e 6675 6e63 7469  '] = self.functi
+00037a30: 6f6e 5f6e 616d 650a 2020 2020 2020 2020  on_name.        
+00037a40: 6966 2073 656c 662e 6c69 6d69 7420 6973  if self.limit is
+00037a50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00037a60: 2020 2020 2020 2072 6573 756c 745b 276c         result['l
+00037a70: 696d 6974 275d 203d 2073 656c 662e 6c69  imit'] = self.li
+00037a80: 6d69 740a 2020 2020 2020 2020 6966 2073  mit.        if s
+00037a90: 656c 662e 6e65 7874 5f74 6f6b 656e 2069  elf.next_token i
+00037aa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00037ab0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00037ac0: 6e65 7874 546f 6b65 6e27 5d20 3d20 7365  nextToken'] = se
+00037ad0: 6c66 2e6e 6578 745f 746f 6b65 6e0a 2020  lf.next_token.  
+00037ae0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00037af0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00037b00: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00037b10: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00037b20: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00037b30: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00037b40: 6d2e 6765 7428 2766 756e 6374 696f 6e4e  m.get('functionN
+00037b50: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
+00037b60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00037b70: 656c 662e 6675 6e63 7469 6f6e 5f6e 616d  elf.function_nam
+00037b80: 6520 3d20 6d2e 6765 7428 2766 756e 6374  e = m.get('funct
+00037b90: 696f 6e4e 616d 6527 290a 2020 2020 2020  ionName').      
+00037ba0: 2020 6966 206d 2e67 6574 2827 6c69 6d69    if m.get('limi
+00037bb0: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
+00037bc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00037bd0: 662e 6c69 6d69 7420 3d20 6d2e 6765 7428  f.limit = m.get(
+00037be0: 276c 696d 6974 2729 0a20 2020 2020 2020  'limit').       
+00037bf0: 2069 6620 6d2e 6765 7428 276e 6578 7454   if m.get('nextT
+00037c00: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
+00037c10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00037c20: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
+00037c30: 3d20 6d2e 6765 7428 276e 6578 7454 6f6b  = m.get('nextTok
+00037c40: 656e 2729 0a20 2020 2020 2020 2072 6574  en').        ret
+00037c50: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00037c60: 204c 6973 7441 7379 6e63 496e 766f 6b65   ListAsyncInvoke
+00037c70: 436f 6e66 6967 7352 6573 706f 6e73 6528  ConfigsResponse(
+00037c80: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00037c90: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00037ca0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00037cb0: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
+00037cc0: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+00037cd0: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
+00037ce0: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
+00037cf0: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+00037d00: 3a20 4c69 7374 4173 796e 6349 6e76 6f6b  : ListAsyncInvok
+00037d10: 6543 6f6e 6669 674f 7574 7075 7420 3d20  eConfigOutput = 
+00037d20: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00037d30: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00037d40: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+00037d50: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00037d60: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00037d70: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
+00037d80: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+00037d90: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00037da0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00037db0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+00037dc0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00037dd0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+00037de0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00037df0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00037e00: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00037e10: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00037e20: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00037e30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00037e40: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00037e50: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00037e60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00037e70: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+00037e80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00037e90: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+00037ea0: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+00037eb0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+00037ec0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+00037ed0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00037ee0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00037ef0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+00037f00: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+00037f10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00037f20: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+00037f30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00037f40: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00037f50: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00037f60: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00037f70: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00037f80: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00037f90: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00037fa0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00037fb0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00037fc0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+00037fd0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+00037fe0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00037ff0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+00038000: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+00038010: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00038020: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+00038030: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038040: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00038050: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00038060: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00038070: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00038080: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+00038090: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+000380a0: 656d 705f 6d6f 6465 6c20 3d20 4c69 7374  emp_model = List
+000380b0: 4173 796e 6349 6e76 6f6b 6543 6f6e 6669  AsyncInvokeConfi
+000380c0: 674f 7574 7075 7428 290a 2020 2020 2020  gOutput().      
+000380d0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+000380e0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+000380f0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00038100: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00038110: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+00038120: 7441 7379 6e63 5461 736b 7352 6571 7565  tAsyncTasksReque
+00038130: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+00038140: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00038150: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00038160: 2020 2020 2020 696e 636c 7564 655f 7061        include_pa
+00038170: 796c 6f61 643a 2062 6f6f 6c20 3d20 4e6f  yload: bool = No
+00038180: 6e65 2c0a 2020 2020 2020 2020 6c69 6d69  ne,.        limi
+00038190: 743a 2069 6e74 203d 204e 6f6e 652c 0a20  t: int = None,. 
+000381a0: 2020 2020 2020 206e 6578 745f 746f 6b65         next_toke
+000381b0: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
+000381c0: 2020 2020 2020 2070 7265 6669 783a 2073         prefix: s
+000381d0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000381e0: 2020 2071 7561 6c69 6669 6572 3a20 7374     qualifier: st
+000381f0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00038200: 2020 736f 7274 5f6f 7264 6572 5f62 795f    sort_order_by_
+00038210: 7469 6d65 3a20 7374 7220 3d20 4e6f 6e65  time: str = None
+00038220: 2c0a 2020 2020 2020 2020 7374 6172 7465  ,.        starte
+00038230: 645f 7469 6d65 5f62 6567 696e 3a20 696e  d_time_begin: in
+00038240: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+00038250: 2020 7374 6172 7465 645f 7469 6d65 5f65    started_time_e
+00038260: 6e64 3a20 696e 7420 3d20 4e6f 6e65 2c0a  nd: int = None,.
+00038270: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
+00038280: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00038290: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000382a0: 696e 636c 7564 655f 7061 796c 6f61 6420  include_payload 
+000382b0: 3d20 696e 636c 7564 655f 7061 796c 6f61  = include_payloa
+000382c0: 640a 2020 2020 2020 2020 7365 6c66 2e6c  d.        self.l
+000382d0: 696d 6974 203d 206c 696d 6974 0a20 2020  imit = limit.   
+000382e0: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
+000382f0: 6f6b 656e 203d 206e 6578 745f 746f 6b65  oken = next_toke
+00038300: 6e0a 2020 2020 2020 2020 7365 6c66 2e70  n.        self.p
+00038310: 7265 6669 7820 3d20 7072 6566 6978 0a20  refix = prefix. 
+00038320: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
+00038330: 6966 6965 7220 3d20 7175 616c 6966 6965  ifier = qualifie
+00038340: 720a 2020 2020 2020 2020 7365 6c66 2e73  r.        self.s
+00038350: 6f72 745f 6f72 6465 725f 6279 5f74 696d  ort_order_by_tim
+00038360: 6520 3d20 736f 7274 5f6f 7264 6572 5f62  e = sort_order_b
+00038370: 795f 7469 6d65 0a20 2020 2020 2020 2073  y_time.        s
+00038380: 656c 662e 7374 6172 7465 645f 7469 6d65  elf.started_time
+00038390: 5f62 6567 696e 203d 2073 7461 7274 6564  _begin = started
+000383a0: 5f74 696d 655f 6265 6769 6e0a 2020 2020  _time_begin.    
+000383b0: 2020 2020 7365 6c66 2e73 7461 7274 6564      self.started
+000383c0: 5f74 696d 655f 656e 6420 3d20 7374 6172  _time_end = star
+000383d0: 7465 645f 7469 6d65 5f65 6e64 0a20 2020  ted_time_end.   
+000383e0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000383f0: 203d 2073 7461 7475 730a 0a20 2020 2064   = status..    d
+00038400: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00038410: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00038420: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00038430: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00038440: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00038450: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00038460: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00038470: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00038480: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00038490: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000384a0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000384b0: 7365 6c66 2e69 6e63 6c75 6465 5f70 6179  self.include_pay
+000384c0: 6c6f 6164 2069 7320 6e6f 7420 4e6f 6e65  load is not None
+000384d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000384e0: 7375 6c74 5b27 696e 636c 7564 6550 6179  sult['includePay
+000384f0: 6c6f 6164 275d 203d 2073 656c 662e 696e  load'] = self.in
+00038500: 636c 7564 655f 7061 796c 6f61 640a 2020  clude_payload.  
+00038510: 2020 2020 2020 6966 2073 656c 662e 6c69        if self.li
+00038520: 6d69 7420 6973 206e 6f74 204e 6f6e 653a  mit is not None:
+00038530: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00038540: 756c 745b 276c 696d 6974 275d 203d 2073  ult['limit'] = s
+00038550: 656c 662e 6c69 6d69 740a 2020 2020 2020  elf.limit.      
+00038560: 2020 6966 2073 656c 662e 6e65 7874 5f74    if self.next_t
+00038570: 6f6b 656e 2069 7320 6e6f 7420 4e6f 6e65  oken is not None
+00038580: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00038590: 7375 6c74 5b27 6e65 7874 546f 6b65 6e27  sult['nextToken'
+000385a0: 5d20 3d20 7365 6c66 2e6e 6578 745f 746f  ] = self.next_to
+000385b0: 6b65 6e0a 2020 2020 2020 2020 6966 2073  ken.        if s
+000385c0: 656c 662e 7072 6566 6978 2069 7320 6e6f  elf.prefix is no
+000385d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000385e0: 2020 2020 7265 7375 6c74 5b27 7072 6566      result['pref
+000385f0: 6978 275d 203d 2073 656c 662e 7072 6566  ix'] = self.pref
+00038600: 6978 0a20 2020 2020 2020 2069 6620 7365  ix.        if se
+00038610: 6c66 2e71 7561 6c69 6669 6572 2069 7320  lf.qualifier is 
+00038620: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038630: 2020 2020 2020 7265 7375 6c74 5b27 7175        result['qu
+00038640: 616c 6966 6965 7227 5d20 3d20 7365 6c66  alifier'] = self
+00038650: 2e71 7561 6c69 6669 6572 0a20 2020 2020  .qualifier.     
+00038660: 2020 2069 6620 7365 6c66 2e73 6f72 745f     if self.sort_
+00038670: 6f72 6465 725f 6279 5f74 696d 6520 6973  order_by_time is
 00038680: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00038690: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000386a0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000386b0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000386c0: 2020 2020 6966 2073 656c 662e 6c69 6d69      if self.limi
-000386d0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-000386e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000386f0: 745b 276c 696d 6974 275d 203d 2073 656c  t['limit'] = sel
-00038700: 662e 6c69 6d69 740a 2020 2020 2020 2020  f.limit.        
-00038710: 6966 2073 656c 662e 6e65 7874 5f74 6f6b  if self.next_tok
-00038720: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
-00038730: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00038740: 6c74 5b27 6e65 7874 546f 6b65 6e27 5d20  lt['nextToken'] 
-00038750: 3d20 7365 6c66 2e6e 6578 745f 746f 6b65  = self.next_toke
-00038760: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-00038770: 662e 7072 6566 6978 2069 7320 6e6f 7420  f.prefix is not 
-00038780: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00038790: 2020 7265 7375 6c74 5b27 7072 6566 6978    result['prefix
-000387a0: 275d 203d 2073 656c 662e 7072 6566 6978  '] = self.prefix
-000387b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000387c0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-000387d0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-000387e0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-000387f0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00038800: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00038810: 6966 206d 2e67 6574 2827 6c69 6d69 7427  if m.get('limit'
-00038820: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00038830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00038840: 6c69 6d69 7420 3d20 6d2e 6765 7428 276c  limit = m.get('l
-00038850: 696d 6974 2729 0a20 2020 2020 2020 2069  imit').        i
-00038860: 6620 6d2e 6765 7428 276e 6578 7454 6f6b  f m.get('nextTok
-00038870: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
-00038880: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00038890: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
-000388a0: 6d2e 6765 7428 276e 6578 7454 6f6b 656e  m.get('nextToken
-000388b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000388c0: 6765 7428 2770 7265 6669 7827 2920 6973  get('prefix') is
-000388d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000388e0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-000388f0: 6978 203d 206d 2e67 6574 2827 7072 6566  ix = m.get('pref
-00038900: 6978 2729 0a20 2020 2020 2020 2072 6574  ix').        ret
-00038910: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00038920: 204c 6973 7443 7573 746f 6d44 6f6d 6169   ListCustomDomai
-00038930: 6e73 5265 7370 6f6e 7365 2854 6561 4d6f  nsResponse(TeaMo
-00038940: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00038950: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00038960: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
-00038970: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
-00038980: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
-00038990: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
-000389a0: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
-000389b0: 2020 2020 2020 2062 6f64 793a 204c 6973         body: Lis
-000389c0: 7443 7573 746f 6d44 6f6d 6169 6e4f 7574  tCustomDomainOut
-000389d0: 7075 7420 3d20 4e6f 6e65 2c0a 2020 2020  put = None,.    
-000389e0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000389f0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-00038a00: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-00038a10: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-00038a20: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00038a30: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-00038a40: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-00038a50: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00038a60: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-00038a70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00038a80: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-00038a90: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-00038aa0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00038ab0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-00038ac0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00038ad0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00038ae0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00038af0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00038b00: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00038b10: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00038b20: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-00038b30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00038b40: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00038b50: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-00038b60: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-00038b70: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-00038b80: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-00038b90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00038ba0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-00038bb0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-00038bc0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-00038bd0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-00038be0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00038bf0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-00038c00: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-00038c10: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00038c20: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00038c30: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00038c40: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00038c50: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00038c60: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00038c70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00038c80: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-00038c90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00038ca0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00038cb0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-00038cc0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-00038cd0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00038ce0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00038cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00038d00: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-00038d10: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00038d20: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00038d30: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-00038d40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00038d50: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-00038d60: 3d20 4c69 7374 4375 7374 6f6d 446f 6d61  = ListCustomDoma
-00038d70: 696e 4f75 7470 7574 2829 0a20 2020 2020  inOutput().     
-00038d80: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00038d90: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-00038da0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-00038db0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00038dc0: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
-00038dd0: 7374 4675 6e63 7469 6f6e 5665 7273 696f  stFunctionVersio
-00038de0: 6e73 5265 7175 6573 7428 5465 614d 6f64  nsRequest(TeaMod
-00038df0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00038e00: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00038e10: 656c 662c 0a20 2020 2020 2020 2064 6972  elf,.        dir
-00038e20: 6563 7469 6f6e 3a20 7374 7220 3d20 4e6f  ection: str = No
-00038e30: 6e65 2c0a 2020 2020 2020 2020 6c69 6d69  ne,.        limi
-00038e40: 743a 2069 6e74 203d 204e 6f6e 652c 0a20  t: int = None,. 
-00038e50: 2020 2020 2020 206e 6578 745f 746f 6b65         next_toke
-00038e60: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
-00038e70: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-00038e80: 5468 6520 736f 7274 696e 6720 6d6f 6465  The sorting mode
-00038e90: 206f 6620 6675 6e63 7469 6f6e 2076 6572   of function ver
-00038ea0: 7369 6f6e 732e 2056 616c 6964 2076 616c  sions. Valid val
-00038eb0: 7565 733a 2042 4143 4b57 4152 4420 616e  ues: BACKWARD an
-00038ec0: 6420 464f 5257 4152 442e 0a20 2020 2020  d FORWARD..     
-00038ed0: 2020 2073 656c 662e 6469 7265 6374 696f     self.directio
-00038ee0: 6e20 3d20 6469 7265 6374 696f 6e0a 2020  n = direction.  
-00038ef0: 2020 2020 2020 2320 5468 6520 6e75 6d62        # The numb
-00038f00: 6572 206f 6620 6675 6e63 7469 6f6e 2076  er of function v
-00038f10: 6572 7369 6f6e 7320 7468 6174 2061 7265  ersions that are
-00038f20: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
-00038f30: 2020 2073 656c 662e 6c69 6d69 7420 3d20     self.limit = 
-00038f40: 6c69 6d69 740a 2020 2020 2020 2020 2320  limit.        # 
-00038f50: 5468 6520 7061 6769 6e61 7469 6f6e 2074  The pagination t
-00038f60: 6f6b 656e 2074 6861 7420 6973 2075 7365  oken that is use
-00038f70: 6420 696e 2074 6865 206e 6578 7420 7265  d in the next re
-00038f80: 7175 6573 7420 746f 2072 6574 7269 6576  quest to retriev
-00038f90: 6520 6120 6e65 7720 7061 6765 206f 6620  e a new page of 
-00038fa0: 7265 7375 6c74 732e 0a20 2020 2020 2020  results..       
-00038fb0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
-00038fc0: 203d 206e 6578 745f 746f 6b65 6e0a 0a20   = next_token.. 
-00038fd0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00038fe0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00038ff0: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00039000: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00039010: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00039020: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00039030: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00039040: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00039050: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00039060: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00039070: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00039080: 2069 6620 7365 6c66 2e64 6972 6563 7469   if self.directi
-00039090: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-000390a0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000390b0: 6c74 5b27 6469 7265 6374 696f 6e27 5d20  lt['direction'] 
-000390c0: 3d20 7365 6c66 2e64 6972 6563 7469 6f6e  = self.direction
-000390d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000390e0: 2e6c 696d 6974 2069 7320 6e6f 7420 4e6f  .limit is not No
-000390f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00039100: 7265 7375 6c74 5b27 6c69 6d69 7427 5d20  result['limit'] 
-00039110: 3d20 7365 6c66 2e6c 696d 6974 0a20 2020  = self.limit.   
-00039120: 2020 2020 2069 6620 7365 6c66 2e6e 6578       if self.nex
-00039130: 745f 746f 6b65 6e20 6973 206e 6f74 204e  t_token is not N
-00039140: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00039150: 2072 6573 756c 745b 276e 6578 7454 6f6b   result['nextTok
-00039160: 656e 275d 203d 2073 656c 662e 6e65 7874  en'] = self.next
-00039170: 5f74 6f6b 656e 0a20 2020 2020 2020 2072  _token.        r
-00039180: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00039190: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000391a0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000391b0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000391c0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000391d0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000391e0: 6469 7265 6374 696f 6e27 2920 6973 206e  direction') is n
-000391f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00039200: 2020 2020 2073 656c 662e 6469 7265 6374       self.direct
-00039210: 696f 6e20 3d20 6d2e 6765 7428 2764 6972  ion = m.get('dir
-00039220: 6563 7469 6f6e 2729 0a20 2020 2020 2020  ection').       
-00039230: 2069 6620 6d2e 6765 7428 276c 696d 6974   if m.get('limit
-00039240: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00039250: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00039260: 2e6c 696d 6974 203d 206d 2e67 6574 2827  .limit = m.get('
-00039270: 6c69 6d69 7427 290a 2020 2020 2020 2020  limit').        
-00039280: 6966 206d 2e67 6574 2827 6e65 7874 546f  if m.get('nextTo
-00039290: 6b65 6e27 2920 6973 206e 6f74 204e 6f6e  ken') is not Non
-000392a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000392b0: 656c 662e 6e65 7874 5f74 6f6b 656e 203d  elf.next_token =
-000392c0: 206d 2e67 6574 2827 6e65 7874 546f 6b65   m.get('nextToke
-000392d0: 6e27 290a 2020 2020 2020 2020 7265 7475  n').        retu
-000392e0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000392f0: 4c69 7374 4675 6e63 7469 6f6e 5665 7273  ListFunctionVers
-00039300: 696f 6e73 5265 7370 6f6e 7365 2854 6561  ionsResponse(Tea
-00039310: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00039320: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00039330: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00039340: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
-00039350: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
-00039360: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
-00039370: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
-00039380: 0a20 2020 2020 2020 2062 6f64 793a 204c  .        body: L
-00039390: 6973 7456 6572 7369 6f6e 734f 7574 7075  istVersionsOutpu
-000393a0: 7420 3d20 4e6f 6e65 2c0a 2020 2020 293a  t = None,.    ):
-000393b0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-000393c0: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
-000393d0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-000393e0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
-000393f0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
-00039400: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
-00039410: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00039420: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00039430: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00039440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00039450: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-00039460: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00039470: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00039480: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-00039490: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000394a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000394b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000394c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000394d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000394e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000394f0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-00039500: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00039510: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-00039520: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-00039530: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-00039540: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-00039550: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-00039560: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00039570: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-00039580: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-00039590: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-000395a0: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-000395b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000395c0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-000395d0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-000395e0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-000395f0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00039600: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00039610: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-00039620: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00039630: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00039640: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-00039650: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-00039660: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00039670: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00039680: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00039690: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000396a0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-000396b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000396c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000396d0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
-000396e0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-000396f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00039700: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-00039710: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00039720: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-00039730: 4c69 7374 5665 7273 696f 6e73 4f75 7470  ListVersionsOutp
-00039740: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-00039750: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-00039760: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-00039770: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-00039780: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00039790: 0a0a 636c 6173 7320 4c69 7374 4675 6e63  ..class ListFunc
-000397a0: 7469 6f6e 7352 6571 7565 7374 2854 6561  tionsRequest(Tea
-000397b0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-000397c0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-000397d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000397e0: 6c69 6d69 743a 2069 6e74 203d 204e 6f6e  limit: int = Non
-000397f0: 652c 0a20 2020 2020 2020 206e 6578 745f  e,.        next_
-00039800: 746f 6b65 6e3a 2073 7472 203d 204e 6f6e  token: str = Non
-00039810: 652c 0a20 2020 2020 2020 2070 7265 6669  e,.        prefi
-00039820: 783a 2073 7472 203d 204e 6f6e 652c 0a20  x: str = None,. 
-00039830: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-00039840: 5468 6520 6e75 6d62 6572 206f 6620 6675  The number of fu
-00039850: 6e63 7469 6f6e 7320 746f 2072 6574 7572  nctions to retur
-00039860: 6e2e 2054 6865 206d 696e 696d 756d 2076  n. The minimum v
-00039870: 616c 7565 2069 7320 3120 616e 6420 7468  alue is 1 and th
-00039880: 6520 6d61 7869 6d75 6d20 7661 6c75 6520  e maximum value 
-00039890: 6973 2031 3030 2e0a 2020 2020 2020 2020  is 100..        
-000398a0: 7365 6c66 2e6c 696d 6974 203d 206c 696d  self.limit = lim
-000398b0: 6974 0a20 2020 2020 2020 2023 2054 6865  it.        # The
-000398c0: 2070 6167 696e 6174 696f 6e20 746f 6b65   pagination toke
-000398d0: 6e2e 0a20 2020 2020 2020 2073 656c 662e  n..        self.
-000398e0: 6e65 7874 5f74 6f6b 656e 203d 206e 6578  next_token = nex
-000398f0: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
-00039900: 2320 5468 6520 7072 6566 6978 206f 6620  # The prefix of 
-00039910: 7468 6520 6675 6e63 7469 6f6e 206e 616d  the function nam
-00039920: 652e 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00039930: 7072 6566 6978 203d 2070 7265 6669 780a  prefix = prefix.
-00039940: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00039950: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00039960: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00039970: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00039980: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00039990: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-000399a0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000399b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000399c0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000399d0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000399e0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000399f0: 2020 2069 6620 7365 6c66 2e6c 696d 6974     if self.limit
-00039a00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00039a10: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00039a20: 5b27 6c69 6d69 7427 5d20 3d20 7365 6c66  ['limit'] = self
-00039a30: 2e6c 696d 6974 0a20 2020 2020 2020 2069  .limit.        i
-00039a40: 6620 7365 6c66 2e6e 6578 745f 746f 6b65  f self.next_toke
-00039a50: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00039a60: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00039a70: 745b 276e 6578 7454 6f6b 656e 275d 203d  t['nextToken'] =
-00039a80: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
-00039a90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00039aa0: 2e70 7265 6669 7820 6973 206e 6f74 204e  .prefix is not N
-00039ab0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00039ac0: 2072 6573 756c 745b 2770 7265 6669 7827   result['prefix'
-00039ad0: 5d20 3d20 7365 6c66 2e70 7265 6669 780a  ] = self.prefix.
-00039ae0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00039af0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00039b00: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00039b10: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00039b20: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00039b30: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00039b40: 6620 6d2e 6765 7428 276c 696d 6974 2729  f m.get('limit')
-00039b50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00039b60: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00039b70: 696d 6974 203d 206d 2e67 6574 2827 6c69  imit = m.get('li
-00039b80: 6d69 7427 290a 2020 2020 2020 2020 6966  mit').        if
-00039b90: 206d 2e67 6574 2827 6e65 7874 546f 6b65   m.get('nextToke
-00039ba0: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
-00039bb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00039bc0: 662e 6e65 7874 5f74 6f6b 656e 203d 206d  f.next_token = m
-00039bd0: 2e67 6574 2827 6e65 7874 546f 6b65 6e27  .get('nextToken'
-00039be0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00039bf0: 6574 2827 7072 6566 6978 2729 2069 7320  et('prefix') is 
-00039c00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00039c10: 2020 2020 2020 7365 6c66 2e70 7265 6669        self.prefi
-00039c20: 7820 3d20 6d2e 6765 7428 2770 7265 6669  x = m.get('prefi
-00039c30: 7827 290a 2020 2020 2020 2020 7265 7475  x').        retu
-00039c40: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00039c50: 4c69 7374 4675 6e63 7469 6f6e 7352 6573  ListFunctionsRes
-00039c60: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-00039c70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00039c80: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00039c90: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-00039ca0: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-00039cb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00039cc0: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-00039cd0: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-00039ce0: 2020 626f 6479 3a20 4c69 7374 4675 6e63    body: ListFunc
-00039cf0: 7469 6f6e 734f 7574 7075 7420 3d20 4e6f  tionsOutput = No
-00039d00: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00039d10: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00039d20: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-00039d30: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00039d40: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-00039d50: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-00039d60: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-00039d70: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00039d80: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00039d90: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
-00039da0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
-00039db0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-00039dc0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00039dd0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00039de0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00039df0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00039e00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00039e10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00039e20: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00039e30: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00039e40: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00039e50: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-00039e60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00039e70: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-00039e80: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-00039e90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00039ea0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-00039eb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00039ec0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-00039ed0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-00039ee0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-00039ef0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00039f00: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-00039f10: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00039f20: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-00039f30: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-00039f40: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00039f50: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00039f60: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00039f70: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00039f80: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00039f90: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00039fa0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-00039fb0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00039fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00039fd0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-00039fe0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-00039ff0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-0003a000: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-0003a010: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003a020: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-0003a030: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-0003a040: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-0003a050: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
-0003a060: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-0003a070: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-0003a080: 705f 6d6f 6465 6c20 3d20 4c69 7374 4675  p_model = ListFu
-0003a090: 6e63 7469 6f6e 734f 7574 7075 7428 290a  nctionsOutput().
-0003a0a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003a0b0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-0003a0c0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-0003a0d0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-0003a0e0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0003a0f0: 7373 204c 6973 7449 6e73 7461 6e63 6573  ss ListInstances
-0003a100: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-0003a110: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0003a120: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-0003a130: 662c 0a20 2020 2020 2020 2071 7561 6c69  f,.        quali
-0003a140: 6669 6572 3a20 7374 7220 3d20 4e6f 6e65  fier: str = None
-0003a150: 2c0a 2020 2020 2020 2020 7769 7468 5f61  ,.        with_a
-0003a160: 6c6c 5f61 6374 6976 653a 2062 6f6f 6c20  ll_active: bool 
-0003a170: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0003a180: 2020 2020 2020 2023 2054 6865 2066 756e         # The fun
-0003a190: 6374 696f 6e20 7665 7273 696f 6e20 6f72  ction version or
-0003a1a0: 2061 6c69 6173 2e0a 2020 2020 2020 2020   alias..        
-0003a1b0: 7365 6c66 2e71 7561 6c69 6669 6572 203d  self.qualifier =
-0003a1c0: 2071 7561 6c69 6669 6572 0a20 2020 2020   qualifier.     
-0003a1d0: 2020 2023 2053 7065 6369 6669 6573 2077     # Specifies w
-0003a1e0: 6865 7468 6572 2074 6f20 6c69 7374 2061  hether to list a
-0003a1f0: 6c6c 2069 6e73 7461 6e63 6573 2e20 5661  ll instances. Va
-0003a200: 6c69 6420 7661 6c75 6573 3a20 7472 7565  lid values: true
-0003a210: 2061 6e64 2066 616c 7365 2e0a 2020 2020   and false..    
-0003a220: 2020 2020 7365 6c66 2e77 6974 685f 616c      self.with_al
-0003a230: 6c5f 6163 7469 7665 203d 2077 6974 685f  l_active = with_
-0003a240: 616c 6c5f 6163 7469 7665 0a0a 2020 2020  all_active..    
-0003a250: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0003a260: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0003a270: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0003a280: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0003a290: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-0003a2a0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0003a2b0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0003a2c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003a2d0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0003a2e0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0003a2f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0003a300: 2073 656c 662e 7175 616c 6966 6965 7220   self.qualifier 
-0003a310: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003a320: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003a330: 2771 7561 6c69 6669 6572 275d 203d 2073  'qualifier'] = s
-0003a340: 656c 662e 7175 616c 6966 6965 720a 2020  elf.qualifier.  
-0003a350: 2020 2020 2020 6966 2073 656c 662e 7769        if self.wi
-0003a360: 7468 5f61 6c6c 5f61 6374 6976 6520 6973  th_all_active is
-0003a370: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003a380: 2020 2020 2020 2072 6573 756c 745b 2777         result['w
-0003a390: 6974 6841 6c6c 4163 7469 7665 275d 203d  ithAllActive'] =
-0003a3a0: 2073 656c 662e 7769 7468 5f61 6c6c 5f61   self.with_all_a
-0003a3b0: 6374 6976 650a 2020 2020 2020 2020 7265  ctive.        re
-0003a3c0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0003a3d0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0003a3e0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-0003a3f0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0003a400: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0003a410: 2020 2020 2069 6620 6d2e 6765 7428 2771       if m.get('q
-0003a420: 7561 6c69 6669 6572 2729 2069 7320 6e6f  ualifier') is no
-0003a430: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003a440: 2020 2020 7365 6c66 2e71 7561 6c69 6669      self.qualifi
-0003a450: 6572 203d 206d 2e67 6574 2827 7175 616c  er = m.get('qual
-0003a460: 6966 6965 7227 290a 2020 2020 2020 2020  ifier').        
-0003a470: 6966 206d 2e67 6574 2827 7769 7468 416c  if m.get('withAl
-0003a480: 6c41 6374 6976 6527 2920 6973 206e 6f74  lActive') is not
-0003a490: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003a4a0: 2020 2073 656c 662e 7769 7468 5f61 6c6c     self.with_all
-0003a4b0: 5f61 6374 6976 6520 3d20 6d2e 6765 7428  _active = m.get(
-0003a4c0: 2777 6974 6841 6c6c 4163 7469 7665 2729  'withAllActive')
-0003a4d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0003a4e0: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-0003a4f0: 7449 6e73 7461 6e63 6573 5265 7370 6f6e  tInstancesRespon
-0003a500: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-0003a510: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-0003a520: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0003a530: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-0003a540: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-0003a550: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-0003a560: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
-0003a570: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
-0003a580: 6f64 793a 204c 6973 7449 6e73 7461 6e63  ody: ListInstanc
-0003a590: 6573 4f75 7470 7574 203d 204e 6f6e 652c  esOutput = None,
-0003a5a0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0003a5b0: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
-0003a5c0: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
-0003a5d0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0003a5e0: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
-0003a5f0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0003a600: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
-0003a610: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0003a620: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003a630: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-0003a640: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-0003a650: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-0003a660: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0003a670: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0003a680: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-0003a690: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003a6a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003a6b0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003a6c0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003a6d0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003a6e0: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-0003a6f0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-0003a700: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003a710: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-0003a720: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-0003a730: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0003a740: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-0003a750: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003a760: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-0003a770: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-0003a780: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0003a790: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0003a7a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003a7b0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003a7c0: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0003a7d0: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0003a7e0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0003a7f0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0003a800: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-0003a810: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-0003a820: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0003a830: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0003a840: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-0003a850: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003a860: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-0003a870: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-0003a880: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-0003a890: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-0003a8a0: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-0003a8b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003a8c0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003a8d0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-0003a8e0: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-0003a8f0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-0003a900: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003a910: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-0003a920: 6f64 656c 203d 204c 6973 7449 6e73 7461  odel = ListInsta
-0003a930: 6e63 6573 4f75 7470 7574 2829 0a20 2020  ncesOutput().   
-0003a940: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003a950: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-0003a960: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-0003a970: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-0003a980: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0003a990: 4c69 7374 4c61 7965 7256 6572 7369 6f6e  ListLayerVersion
-0003a9a0: 7352 6571 7565 7374 2854 6561 4d6f 6465  sRequest(TeaMode
-0003a9b0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0003a9c0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0003a9d0: 6c66 2c0a 2020 2020 2020 2020 6c69 6d69  lf,.        limi
-0003a9e0: 743a 2069 6e74 203d 204e 6f6e 652c 0a20  t: int = None,. 
-0003a9f0: 2020 2020 2020 2073 7461 7274 5f76 6572         start_ver
-0003aa00: 7369 6f6e 3a20 7374 7220 3d20 4e6f 6e65  sion: str = None
-0003aa10: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0003aa20: 2023 2054 6865 206e 756d 6265 7220 6f66   # The number of
-0003aa30: 2076 6572 7369 6f6e 7320 746f 2062 6520   versions to be 
-0003aa40: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
-0003aa50: 2020 7365 6c66 2e6c 696d 6974 203d 206c    self.limit = l
-0003aa60: 696d 6974 0a20 2020 2020 2020 2023 2054  imit.        # T
-0003aa70: 6865 2069 6e69 7469 616c 2076 6572 7369  he initial versi
-0003aa80: 6f6e 206f 6620 7468 6520 6c61 7965 722e  on of the layer.
-0003aa90: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0003aaa0: 6172 745f 7665 7273 696f 6e20 3d20 7374  art_version = st
-0003aab0: 6172 745f 7665 7273 696f 6e0a 0a20 2020  art_version..   
-0003aac0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0003aad0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-0003aae0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-0003aaf0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0003ab00: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-0003ab10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0003ab20: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-0003ab30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003ab40: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-0003ab50: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0003ab60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0003ab70: 6620 7365 6c66 2e6c 696d 6974 2069 7320  f self.limit is 
-0003ab80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003ab90: 2020 2020 2020 7265 7375 6c74 5b27 6c69        result['li
-0003aba0: 6d69 7427 5d20 3d20 7365 6c66 2e6c 696d  mit'] = self.lim
-0003abb0: 6974 0a20 2020 2020 2020 2069 6620 7365  it.        if se
-0003abc0: 6c66 2e73 7461 7274 5f76 6572 7369 6f6e  lf.start_version
-0003abd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003abe0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003abf0: 5b27 7374 6172 7456 6572 7369 6f6e 275d  ['startVersion']
-0003ac00: 203d 2073 656c 662e 7374 6172 745f 7665   = self.start_ve
-0003ac10: 7273 696f 6e0a 2020 2020 2020 2020 7265  rsion.        re
-0003ac20: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0003ac30: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0003ac40: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-0003ac50: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0003ac60: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0003ac70: 2020 2020 2069 6620 6d2e 6765 7428 276c       if m.get('l
-0003ac80: 696d 6974 2729 2069 7320 6e6f 7420 4e6f  imit') is not No
-0003ac90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003aca0: 7365 6c66 2e6c 696d 6974 203d 206d 2e67  self.limit = m.g
-0003acb0: 6574 2827 6c69 6d69 7427 290a 2020 2020  et('limit').    
-0003acc0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-0003acd0: 6172 7456 6572 7369 6f6e 2729 2069 7320  artVersion') is 
-0003ace0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003acf0: 2020 2020 2020 7365 6c66 2e73 7461 7274        self.start
-0003ad00: 5f76 6572 7369 6f6e 203d 206d 2e67 6574  _version = m.get
-0003ad10: 2827 7374 6172 7456 6572 7369 6f6e 2729  ('startVersion')
-0003ad20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0003ad30: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-0003ad40: 744c 6179 6572 5665 7273 696f 6e73 5265  tLayerVersionsRe
-0003ad50: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-0003ad60: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003ad70: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0003ad80: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-0003ad90: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-0003ada0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0003adb0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-0003adc0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-0003add0: 2020 2062 6f64 793a 204c 6973 744c 6179     body: ListLay
-0003ade0: 6572 5665 7273 696f 6e4f 7574 7075 7420  erVersionOutput 
-0003adf0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0003ae00: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0003ae10: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-0003ae20: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0003ae30: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0003ae40: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-0003ae50: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-0003ae60: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0003ae70: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0003ae80: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-0003ae90: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003aea0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-0003aeb0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0003aec0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0003aed0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0003aee0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0003aef0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0003af00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003af10: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0003af20: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0003af30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0003af40: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-0003af50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003af60: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-0003af70: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-0003af80: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-0003af90: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003afa0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003afb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003afc0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-0003afd0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003afe0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0003aff0: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-0003b000: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003b010: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-0003b020: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-0003b030: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0003b040: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0003b050: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0003b060: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0003b070: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0003b080: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0003b090: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-0003b0a0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-0003b0b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003b0c0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-0003b0d0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-0003b0e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003b0f0: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-0003b100: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003b110: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0003b120: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-0003b130: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-0003b140: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003b150: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-0003b160: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003b170: 2074 656d 705f 6d6f 6465 6c20 3d20 4c69   temp_model = Li
-0003b180: 7374 4c61 7965 7256 6572 7369 6f6e 4f75  stLayerVersionOu
-0003b190: 7470 7574 2829 0a20 2020 2020 2020 2020  tput().         
-0003b1a0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-0003b1b0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-0003b1c0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-0003b1d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0003b1e0: 660a 0a0a 636c 6173 7320 4c69 7374 4c61  f...class ListLa
-0003b1f0: 7965 7273 5265 7175 6573 7428 5465 614d  yersRequest(TeaM
-0003b200: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0003b210: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0003b220: 2073 656c 662c 0a20 2020 2020 2020 206c   self,.        l
-0003b230: 696d 6974 3a20 696e 7420 3d20 4e6f 6e65  imit: int = None
-0003b240: 2c0a 2020 2020 2020 2020 6e65 7874 5f74  ,.        next_t
-0003b250: 6f6b 656e 3a20 7374 7220 3d20 4e6f 6e65  oken: str = None
-0003b260: 2c0a 2020 2020 2020 2020 6f66 6669 6369  ,.        offici
-0003b270: 616c 3a20 7374 7220 3d20 4e6f 6e65 2c0a  al: str = None,.
-0003b280: 2020 2020 2020 2020 7072 6566 6978 3a20          prefix: 
-0003b290: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0003b2a0: 2020 2020 7075 626c 6963 3a20 7374 7220      public: str 
-0003b2b0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0003b2c0: 2020 2020 2020 2023 2054 6865 206e 756d         # The num
-0003b2d0: 6265 7220 6f66 206c 6179 6572 7320 7468  ber of layers th
-0003b2e0: 6174 2061 7265 2072 6574 7572 6e65 640a  at are returned.
-0003b2f0: 2020 2020 2020 2020 7365 6c66 2e6c 696d          self.lim
-0003b300: 6974 203d 206c 696d 6974 0a20 2020 2020  it = limit.     
-0003b310: 2020 2023 2054 6865 2070 6167 696e 6174     # The paginat
-0003b320: 696f 6e20 746f 6b65 6e20 7468 6174 2069  ion token that i
-0003b330: 7320 7573 6564 2069 6e20 7468 6520 6e65  s used in the ne
-0003b340: 7874 2072 6571 7565 7374 2074 6f20 7265  xt request to re
-0003b350: 7472 6965 7665 2061 206e 6577 2070 6167  trieve a new pag
-0003b360: 6520 6f66 2072 6573 756c 7473 2e0a 2020  e of results..  
-0003b370: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
-0003b380: 746f 6b65 6e20 3d20 6e65 7874 5f74 6f6b  token = next_tok
-0003b390: 656e 0a20 2020 2020 2020 2023 2053 7065  en.        # Spe
-0003b3a0: 6369 6669 6573 2077 6865 7468 6572 2074  cifies whether t
-0003b3b0: 6865 206c 6179 6572 2069 7320 6f66 6669  he layer is offi
-0003b3c0: 6369 616c 2e20 5661 6c69 6420 7661 6c75  cial. Valid valu
-0003b3d0: 6573 3a20 7472 7565 2061 6e64 2066 616c  es: true and fal
-0003b3e0: 7365 2e0a 2020 2020 2020 2020 7365 6c66  se..        self
-0003b3f0: 2e6f 6666 6963 6961 6c20 3d20 6f66 6669  .official = offi
-0003b400: 6369 616c 0a20 2020 2020 2020 2023 2054  cial.        # T
-0003b410: 6865 206e 616d 6520 7072 6566 6978 206f  he name prefix o
-0003b420: 6620 7468 6520 6c61 7965 722e 0a20 2020  f the layer..   
-0003b430: 2020 2020 2073 656c 662e 7072 6566 6978       self.prefix
-0003b440: 203d 2070 7265 6669 780a 2020 2020 2020   = prefix.      
-0003b450: 2020 2320 5370 6563 6966 6965 7320 7768    # Specifies wh
-0003b460: 6574 6865 7220 7468 6520 6c61 7965 7220  ether the layer 
-0003b470: 6973 2070 7562 6c69 632e 2056 616c 6964  is public. Valid
-0003b480: 2076 616c 7565 733a 2074 7275 6520 616e   values: true an
-0003b490: 6420 6661 6c73 652e 0a20 2020 2020 2020  d false..       
-0003b4a0: 2073 656c 662e 7075 626c 6963 203d 2070   self.public = p
-0003b4b0: 7562 6c69 630a 0a20 2020 2064 6566 2076  ublic..    def v
-0003b4c0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0003b4d0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-0003b4e0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-0003b4f0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-0003b500: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-0003b510: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-0003b520: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-0003b530: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0003b540: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-0003b550: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-0003b560: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0003b570: 2e6c 696d 6974 2069 7320 6e6f 7420 4e6f  .limit is not No
-0003b580: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003b590: 7265 7375 6c74 5b27 6c69 6d69 7427 5d20  result['limit'] 
-0003b5a0: 3d20 7365 6c66 2e6c 696d 6974 0a20 2020  = self.limit.   
-0003b5b0: 2020 2020 2069 6620 7365 6c66 2e6e 6578       if self.nex
-0003b5c0: 745f 746f 6b65 6e20 6973 206e 6f74 204e  t_token is not N
-0003b5d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003b5e0: 2072 6573 756c 745b 276e 6578 7454 6f6b   result['nextTok
-0003b5f0: 656e 275d 203d 2073 656c 662e 6e65 7874  en'] = self.next
-0003b600: 5f74 6f6b 656e 0a20 2020 2020 2020 2069  _token.        i
-0003b610: 6620 7365 6c66 2e6f 6666 6963 6961 6c20  f self.official 
-0003b620: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003b630: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003b640: 276f 6666 6963 6961 6c27 5d20 3d20 7365  'official'] = se
-0003b650: 6c66 2e6f 6666 6963 6961 6c0a 2020 2020  lf.official.    
-0003b660: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-0003b670: 6978 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ix is not None:.
-0003b680: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0003b690: 6c74 5b27 7072 6566 6978 275d 203d 2073  lt['prefix'] = s
-0003b6a0: 656c 662e 7072 6566 6978 0a20 2020 2020  elf.prefix.     
-0003b6b0: 2020 2069 6620 7365 6c66 2e70 7562 6c69     if self.publi
-0003b6c0: 6320 6973 206e 6f74 204e 6f6e 653a 0a20  c is not None:. 
-0003b6d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003b6e0: 745b 2770 7562 6c69 6327 5d20 3d20 7365  t['public'] = se
-0003b6f0: 6c66 2e70 7562 6c69 630a 2020 2020 2020  lf.public.      
-0003b700: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0003b710: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0003b720: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0003b730: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0003b740: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0003b750: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003b760: 7428 276c 696d 6974 2729 2069 7320 6e6f  t('limit') is no
-0003b770: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003b780: 2020 2020 7365 6c66 2e6c 696d 6974 203d      self.limit =
-0003b790: 206d 2e67 6574 2827 6c69 6d69 7427 290a   m.get('limit').
-0003b7a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003b7b0: 2827 6e65 7874 546f 6b65 6e27 2920 6973  ('nextToken') is
-0003b7c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003b7d0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
-0003b7e0: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
-0003b7f0: 6e65 7874 546f 6b65 6e27 290a 2020 2020  nextToken').    
-0003b800: 2020 2020 6966 206d 2e67 6574 2827 6f66      if m.get('of
-0003b810: 6669 6369 616c 2729 2069 7320 6e6f 7420  ficial') is not 
-0003b820: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003b830: 2020 7365 6c66 2e6f 6666 6963 6961 6c20    self.official 
-0003b840: 3d20 6d2e 6765 7428 276f 6666 6963 6961  = m.get('officia
-0003b850: 6c27 290a 2020 2020 2020 2020 6966 206d  l').        if m
-0003b860: 2e67 6574 2827 7072 6566 6978 2729 2069  .get('prefix') i
-0003b870: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003b880: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-0003b890: 6669 7820 3d20 6d2e 6765 7428 2770 7265  fix = m.get('pre
-0003b8a0: 6669 7827 290a 2020 2020 2020 2020 6966  fix').        if
-0003b8b0: 206d 2e67 6574 2827 7075 626c 6963 2729   m.get('public')
-0003b8c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003b8d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0003b8e0: 7562 6c69 6320 3d20 6d2e 6765 7428 2770  ublic = m.get('p
-0003b8f0: 7562 6c69 6327 290a 2020 2020 2020 2020  ublic').        
-0003b900: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0003b910: 6173 7320 4c69 7374 4c61 7965 7273 5265  ass ListLayersRe
-0003b920: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-0003b930: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003b940: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0003b950: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-0003b960: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-0003b970: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0003b980: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-0003b990: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-0003b9a0: 2020 2062 6f64 793a 204c 6973 744c 6179     body: ListLay
-0003b9b0: 6572 734f 7574 7075 7420 3d20 4e6f 6e65  ersOutput = None
-0003b9c0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0003b9d0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0003b9e0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-0003b9f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003ba00: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
-0003ba10: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0003ba20: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
-0003ba30: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0003ba40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0003ba50: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-0003ba60: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-0003ba70: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-0003ba80: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0003ba90: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0003baa0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-0003bab0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0003bac0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003bad0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0003bae0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0003baf0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0003bb00: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-0003bb10: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-0003bb20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003bb30: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-0003bb40: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-0003bb50: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0003bb60: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-0003bb70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003bb80: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-0003bb90: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-0003bba0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-0003bbb0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0003bbc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003bbd0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003bbe0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-0003bbf0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-0003bc00: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0003bc10: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0003bc20: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-0003bc30: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-0003bc40: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-0003bc50: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0003bc60: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0003bc70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003bc80: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-0003bc90: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-0003bca0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0003bcb0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-0003bcc0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-0003bcd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003bce0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0003bcf0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-0003bd00: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-0003bd10: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-0003bd20: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003bd30: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-0003bd40: 6d6f 6465 6c20 3d20 4c69 7374 4c61 7965  model = ListLaye
-0003bd50: 7273 4f75 7470 7574 2829 0a20 2020 2020  rsOutput().     
-0003bd60: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0003bd70: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-0003bd80: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-0003bd90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0003bda0: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
-0003bdb0: 7374 5072 6f76 6973 696f 6e43 6f6e 6669  stProvisionConfi
-0003bdc0: 6773 5265 7175 6573 7428 5465 614d 6f64  gsRequest(TeaMod
-0003bdd0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0003bde0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0003bdf0: 656c 662c 0a20 2020 2020 2020 2066 756e  elf,.        fun
-0003be00: 6374 696f 6e5f 6e61 6d65 3a20 7374 7220  ction_name: str 
-0003be10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0003be20: 6c69 6d69 743a 2069 6e74 203d 204e 6f6e  limit: int = Non
-0003be30: 652c 0a20 2020 2020 2020 206e 6578 745f  e,.        next_
-0003be40: 746f 6b65 6e3a 2073 7472 203d 204e 6f6e  token: str = Non
-0003be50: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0003be60: 2020 2320 5468 6520 6e61 6d65 206f 6620    # The name of 
-0003be70: 7468 6520 6675 6e63 7469 6f6e 2e20 4966  the function. If
-0003be80: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
-0003be90: 6973 206e 6f74 2073 7065 6369 6669 6564  is not specified
-0003bea0: 2c20 7468 6520 7072 6f76 6973 696f 6e65  , the provisione
-0003beb0: 6420 636f 6e66 6967 7572 6174 696f 6e73  d configurations
-0003bec0: 206f 6620 616c 6c20 6675 6e63 7469 6f6e   of all function
-0003bed0: 7320 6172 6520 6c69 7374 6564 2e0a 2020  s are listed..  
-0003bee0: 2020 2020 2020 7365 6c66 2e66 756e 6374        self.funct
-0003bef0: 696f 6e5f 6e61 6d65 203d 2066 756e 6374  ion_name = funct
-0003bf00: 696f 6e5f 6e61 6d65 0a20 2020 2020 2020  ion_name.       
-0003bf10: 2023 204e 756d 6265 7220 6f66 2070 726f   # Number of pro
-0003bf20: 7669 7369 6f6e 6564 2063 6f6e 6669 6775  visioned configu
-0003bf30: 7261 7469 6f6e 7320 746f 2072 6574 7572  rations to retur
-0003bf40: 6e2e 0a20 2020 2020 2020 2073 656c 662e  n..        self.
-0003bf50: 6c69 6d69 7420 3d20 6c69 6d69 740a 2020  limit = limit.  
-0003bf60: 2020 2020 2020 2320 4120 7061 6769 6e61        # A pagina
-0003bf70: 7469 6f6e 2074 6f6b 656e 2e0a 2020 2020  tion token..    
-0003bf80: 2020 2020 7365 6c66 2e6e 6578 745f 746f      self.next_to
-0003bf90: 6b65 6e20 3d20 6e65 7874 5f74 6f6b 656e  ken = next_token
-0003bfa0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0003bfb0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0003bfc0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0003bfd0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0003bfe0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0003bff0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-0003c000: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003c010: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003c020: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003c030: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003c040: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003c050: 2020 2020 6966 2073 656c 662e 6675 6e63      if self.func
-0003c060: 7469 6f6e 5f6e 616d 6520 6973 206e 6f74  tion_name is not
-0003c070: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003c080: 2020 2072 6573 756c 745b 2766 756e 6374     result['funct
-0003c090: 696f 6e4e 616d 6527 5d20 3d20 7365 6c66  ionName'] = self
-0003c0a0: 2e66 756e 6374 696f 6e5f 6e61 6d65 0a20  .function_name. 
-0003c0b0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
-0003c0c0: 696d 6974 2069 7320 6e6f 7420 4e6f 6e65  imit is not None
-0003c0d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003c0e0: 7375 6c74 5b27 6c69 6d69 7427 5d20 3d20  sult['limit'] = 
-0003c0f0: 7365 6c66 2e6c 696d 6974 0a20 2020 2020  self.limit.     
-0003c100: 2020 2069 6620 7365 6c66 2e6e 6578 745f     if self.next_
-0003c110: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
-0003c120: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003c130: 6573 756c 745b 276e 6578 7454 6f6b 656e  esult['nextToken
-0003c140: 275d 203d 2073 656c 662e 6e65 7874 5f74  '] = self.next_t
-0003c150: 6f6b 656e 0a20 2020 2020 2020 2072 6574  oken.        ret
-0003c160: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0003c170: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0003c180: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-0003c190: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0003c1a0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0003c1b0: 2020 2020 6966 206d 2e67 6574 2827 6675      if m.get('fu
-0003c1c0: 6e63 7469 6f6e 4e61 6d65 2729 2069 7320  nctionName') is 
-0003c1d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003c1e0: 2020 2020 2020 7365 6c66 2e66 756e 6374        self.funct
-0003c1f0: 696f 6e5f 6e61 6d65 203d 206d 2e67 6574  ion_name = m.get
-0003c200: 2827 6675 6e63 7469 6f6e 4e61 6d65 2729  ('functionName')
-0003c210: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003c220: 7428 276c 696d 6974 2729 2069 7320 6e6f  t('limit') is no
-0003c230: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003c240: 2020 2020 7365 6c66 2e6c 696d 6974 203d      self.limit =
-0003c250: 206d 2e67 6574 2827 6c69 6d69 7427 290a   m.get('limit').
-0003c260: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003c270: 2827 6e65 7874 546f 6b65 6e27 2920 6973  ('nextToken') is
-0003c280: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003c290: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
-0003c2a0: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
-0003c2b0: 6e65 7874 546f 6b65 6e27 290a 2020 2020  nextToken').    
-0003c2c0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0003c2d0: 0a0a 636c 6173 7320 4c69 7374 5072 6f76  ..class ListProv
-0003c2e0: 6973 696f 6e43 6f6e 6669 6773 5265 7370  isionConfigsResp
-0003c2f0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-0003c300: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0003c310: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0003c320: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-0003c330: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-0003c340: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0003c350: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-0003c360: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0003c370: 2062 6f64 793a 204c 6973 7450 726f 7669   body: ListProvi
-0003c380: 7369 6f6e 436f 6e66 6967 734f 7574 7075  sionConfigsOutpu
-0003c390: 7420 3d20 4e6f 6e65 2c0a 2020 2020 293a  t = None,.    ):
-0003c3a0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-0003c3b0: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
-0003c3c0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0003c3d0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
-0003c3e0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
-0003c3f0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
-0003c400: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0003c410: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0003c420: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-0003c430: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003c440: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-0003c450: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0003c460: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0003c470: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-0003c480: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0003c490: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0003c4a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003c4b0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0003c4c0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0003c4d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0003c4e0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-0003c4f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003c500: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-0003c510: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-0003c520: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-0003c530: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-0003c540: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-0003c550: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0003c560: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-0003c570: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-0003c580: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-0003c590: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-0003c5a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003c5b0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-0003c5c0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-0003c5d0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-0003c5e0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0003c5f0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0003c600: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-0003c610: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0003c620: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0003c630: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-0003c640: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-0003c650: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003c660: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0003c670: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0003c680: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003c690: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0003c6a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003c6b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0003c6c0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
-0003c6d0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0003c6e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003c6f0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-0003c700: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003c710: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-0003c720: 4c69 7374 5072 6f76 6973 696f 6e43 6f6e  ListProvisionCon
-0003c730: 6669 6773 4f75 7470 7574 2829 0a20 2020  figsOutput().   
-0003c740: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003c750: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-0003c760: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-0003c770: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-0003c780: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0003c790: 4c69 7374 5461 6752 6573 6f75 7263 6573  ListTagResources
-0003c7a0: 5265 7175 6573 7454 6167 2854 6561 4d6f  RequestTag(TeaMo
-0003c7b0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0003c7c0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0003c7d0: 7365 6c66 2c0a 2020 2020 2020 2020 6b65  self,.        ke
-0003c7e0: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
-0003c7f0: 2020 2020 2020 2076 616c 7565 3a20 7374         value: st
-0003c800: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
-0003c810: 0a20 2020 2020 2020 2023 20e6 a087 e7ad  .        # .....
-0003c820: bee5 908d 0a20 2020 2020 2020 2073 656c  .....        sel
-0003c830: 662e 6b65 7920 3d20 6b65 790a 2020 2020  f.key = key.    
-0003c840: 2020 2020 2320 e6a0 87e7 adbe e580 bc0a      # ..........
-0003c850: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-0003c860: 7565 203d 2076 616c 7565 0a0a 2020 2020  ue = value..    
-0003c870: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0003c880: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0003c890: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0003c8a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0003c8b0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-0003c8c0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0003c8d0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0003c8e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003c8f0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0003c900: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0003c910: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0003c920: 2073 656c 662e 6b65 7920 6973 206e 6f74   self.key is not
-0003c930: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003c940: 2020 2072 6573 756c 745b 274b 6579 275d     result['Key']
-0003c950: 203d 2073 656c 662e 6b65 790a 2020 2020   = self.key.    
-0003c960: 2020 2020 6966 2073 656c 662e 7661 6c75      if self.valu
-0003c970: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0003c980: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003c990: 745b 2756 616c 7565 275d 203d 2073 656c  t['Value'] = sel
-0003c9a0: 662e 7661 6c75 650a 2020 2020 2020 2020  f.value.        
-0003c9b0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0003c9c0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0003c9d0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0003c9e0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0003c9f0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0003ca00: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003ca10: 274b 6579 2729 2069 7320 6e6f 7420 4e6f  'Key') is not No
-0003ca20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003ca30: 7365 6c66 2e6b 6579 203d 206d 2e67 6574  self.key = m.get
-0003ca40: 2827 4b65 7927 290a 2020 2020 2020 2020  ('Key').        
-0003ca50: 6966 206d 2e67 6574 2827 5661 6c75 6527  if m.get('Value'
-0003ca60: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003ca70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003ca80: 7661 6c75 6520 3d20 6d2e 6765 7428 2756  value = m.get('V
-0003ca90: 616c 7565 2729 0a20 2020 2020 2020 2072  alue').        r
-0003caa0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0003cab0: 7373 204c 6973 7454 6167 5265 736f 7572  ss ListTagResour
-0003cac0: 6365 7352 6571 7565 7374 2854 6561 4d6f  cesRequest(TeaMo
-0003cad0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0003cae0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0003caf0: 7365 6c66 2c0a 2020 2020 2020 2020 6c69  self,.        li
-0003cb00: 6d69 743a 2069 6e74 203d 204e 6f6e 652c  mit: int = None,
-0003cb10: 0a20 2020 2020 2020 206e 6578 745f 746f  .        next_to
-0003cb20: 6b65 6e3a 2073 7472 203d 204e 6f6e 652c  ken: str = None,
-0003cb30: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
-0003cb40: 655f 6964 3a20 4c69 7374 5b73 7472 5d20  e_id: List[str] 
-0003cb50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0003cb60: 7265 736f 7572 6365 5f74 7970 653a 2073  resource_type: s
-0003cb70: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0003cb80: 2020 2074 6167 3a20 4c69 7374 5b4c 6973     tag: List[Lis
-0003cb90: 7454 6167 5265 736f 7572 6365 7352 6571  tTagResourcesReq
-0003cba0: 7565 7374 5461 675d 203d 204e 6f6e 652c  uestTag] = None,
-0003cbb0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0003cbc0: 7365 6c66 2e6c 696d 6974 203d 206c 696d  self.limit = lim
-0003cbd0: 6974 0a20 2020 2020 2020 2073 656c 662e  it.        self.
-0003cbe0: 6e65 7874 5f74 6f6b 656e 203d 206e 6578  next_token = nex
-0003cbf0: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
-0003cc00: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
-0003cc10: 203d 2072 6573 6f75 7263 655f 6964 0a20   = resource_id. 
-0003cc20: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-0003cc30: 7572 6365 5f74 7970 6520 3d20 7265 736f  urce_type = reso
-0003cc40: 7572 6365 5f74 7970 650a 2020 2020 2020  urce_type.      
-0003cc50: 2020 7365 6c66 2e74 6167 203d 2074 6167    self.tag = tag
-0003cc60: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0003cc70: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0003cc80: 2020 6966 2073 656c 662e 7461 673a 0a20    if self.tag:. 
-0003cc90: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0003cca0: 2069 6e20 7365 6c66 2e74 6167 3a0a 2020   in self.tag:.  
-0003ccb0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0003ccc0: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
-0003ccd0: 2020 2020 2020 2020 6b2e 7661 6c69 6461          k.valida
-0003cce0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-0003ccf0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0003cd00: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0003cd10: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0003cd20: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0003cd30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003cd40: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0003cd50: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0003cd60: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0003cd70: 2020 6966 2073 656c 662e 6c69 6d69 7420    if self.limit 
-0003cd80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003cd90: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003cda0: 274c 696d 6974 275d 203d 2073 656c 662e  'Limit'] = self.
-0003cdb0: 6c69 6d69 740a 2020 2020 2020 2020 6966  limit.        if
-0003cdc0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
-0003cdd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003cde0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003cdf0: 5b27 4e65 7874 546f 6b65 6e27 5d20 3d20  ['NextToken'] = 
-0003ce00: 7365 6c66 2e6e 6578 745f 746f 6b65 6e0a  self.next_token.
-0003ce10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003ce20: 7265 736f 7572 6365 5f69 6420 6973 206e  resource_id is n
-0003ce30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003ce40: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
-0003ce50: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
-0003ce60: 2e72 6573 6f75 7263 655f 6964 0a20 2020  .resource_id.   
-0003ce70: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
-0003ce80: 6f75 7263 655f 7479 7065 2069 7320 6e6f  ource_type is no
-0003ce90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003cea0: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
-0003ceb0: 7572 6365 5479 7065 275d 203d 2073 656c  urceType'] = sel
-0003cec0: 662e 7265 736f 7572 6365 5f74 7970 650a  f.resource_type.
-0003ced0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003cee0: 5461 6727 5d20 3d20 5b5d 0a20 2020 2020  Tag'] = [].     
-0003cef0: 2020 2069 6620 7365 6c66 2e74 6167 2069     if self.tag i
-0003cf00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003cf10: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-0003cf20: 2073 656c 662e 7461 673a 0a20 2020 2020   self.tag:.     
-0003cf30: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003cf40: 745b 2754 6167 275d 2e61 7070 656e 6428  t['Tag'].append(
-0003cf50: 6b2e 746f 5f6d 6170 2829 2069 6620 6b20  k.to_map() if k 
-0003cf60: 656c 7365 204e 6f6e 6529 0a20 2020 2020  else None).     
-0003cf70: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0003cf80: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-0003cf90: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-0003cfa0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-0003cfb0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0003cfc0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003cfd0: 6574 2827 4c69 6d69 7427 2920 6973 206e  et('Limit') is n
-0003cfe0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003cff0: 2020 2020 2073 656c 662e 6c69 6d69 7420       self.limit 
-0003d000: 3d20 6d2e 6765 7428 274c 696d 6974 2729  = m.get('Limit')
-0003d010: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003d020: 7428 274e 6578 7454 6f6b 656e 2729 2069  t('NextToken') i
-0003d030: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003d040: 2020 2020 2020 2020 7365 6c66 2e6e 6578          self.nex
-0003d050: 745f 746f 6b65 6e20 3d20 6d2e 6765 7428  t_token = m.get(
-0003d060: 274e 6578 7454 6f6b 656e 2729 0a20 2020  'NextToken').   
-0003d070: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-0003d080: 6573 6f75 7263 6549 6427 2920 6973 206e  esourceId') is n
-0003d090: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003d0a0: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
-0003d0b0: 6365 5f69 6420 3d20 6d2e 6765 7428 2752  ce_id = m.get('R
-0003d0c0: 6573 6f75 7263 6549 6427 290a 2020 2020  esourceId').    
-0003d0d0: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-0003d0e0: 736f 7572 6365 5479 7065 2729 2069 7320  sourceType') is 
-0003d0f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003d100: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
-0003d110: 7263 655f 7479 7065 203d 206d 2e67 6574  rce_type = m.get
-0003d120: 2827 5265 736f 7572 6365 5479 7065 2729  ('ResourceType')
-0003d130: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0003d140: 6720 3d20 5b5d 0a20 2020 2020 2020 2069  g = [].        i
-0003d150: 6620 6d2e 6765 7428 2754 6167 2729 2069  f m.get('Tag') i
-0003d160: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003d170: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-0003d180: 206d 2e67 6574 2827 5461 6727 293a 0a20   m.get('Tag'):. 
-0003d190: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0003d1a0: 656d 705f 6d6f 6465 6c20 3d20 4c69 7374  emp_model = List
-0003d1b0: 5461 6752 6573 6f75 7263 6573 5265 7175  TagResourcesRequ
-0003d1c0: 6573 7454 6167 2829 0a20 2020 2020 2020  estTag().       
-0003d1d0: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-0003d1e0: 672e 6170 7065 6e64 2874 656d 705f 6d6f  g.append(temp_mo
-0003d1f0: 6465 6c2e 6672 6f6d 5f6d 6170 286b 2929  del.from_map(k))
-0003d200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0003d210: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-0003d220: 7454 6167 5265 736f 7572 6365 7353 6872  tTagResourcesShr
-0003d230: 696e 6b52 6571 7565 7374 2854 6561 4d6f  inkRequest(TeaMo
-0003d240: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0003d250: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0003d260: 7365 6c66 2c0a 2020 2020 2020 2020 6c69  self,.        li
-0003d270: 6d69 743a 2069 6e74 203d 204e 6f6e 652c  mit: int = None,
-0003d280: 0a20 2020 2020 2020 206e 6578 745f 746f  .        next_to
-0003d290: 6b65 6e3a 2073 7472 203d 204e 6f6e 652c  ken: str = None,
-0003d2a0: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
-0003d2b0: 655f 6964 5f73 6872 696e 6b3a 2073 7472  e_id_shrink: str
-0003d2c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0003d2d0: 2072 6573 6f75 7263 655f 7479 7065 3a20   resource_type: 
-0003d2e0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0003d2f0: 2020 2020 7461 675f 7368 7269 6e6b 3a20      tag_shrink: 
-0003d300: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0003d310: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0003d320: 6c69 6d69 7420 3d20 6c69 6d69 740a 2020  limit = limit.  
-0003d330: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
-0003d340: 746f 6b65 6e20 3d20 6e65 7874 5f74 6f6b  token = next_tok
-0003d350: 656e 0a20 2020 2020 2020 2073 656c 662e  en.        self.
-0003d360: 7265 736f 7572 6365 5f69 645f 7368 7269  resource_id_shri
-0003d370: 6e6b 203d 2072 6573 6f75 7263 655f 6964  nk = resource_id
-0003d380: 5f73 6872 696e 6b0a 2020 2020 2020 2020  _shrink.        
-0003d390: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
-0003d3a0: 7065 203d 2072 6573 6f75 7263 655f 7479  pe = resource_ty
-0003d3b0: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-0003d3c0: 7461 675f 7368 7269 6e6b 203d 2074 6167  tag_shrink = tag
-0003d3d0: 5f73 6872 696e 6b0a 0a20 2020 2064 6566  _shrink..    def
-0003d3e0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0003d3f0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0003d400: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0003d410: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0003d420: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0003d430: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0003d440: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0003d450: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003d460: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0003d470: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0003d480: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0003d490: 6c66 2e6c 696d 6974 2069 7320 6e6f 7420  lf.limit is not 
-0003d4a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003d4b0: 2020 7265 7375 6c74 5b27 4c69 6d69 7427    result['Limit'
-0003d4c0: 5d20 3d20 7365 6c66 2e6c 696d 6974 0a20  ] = self.limit. 
-0003d4d0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-0003d4e0: 6578 745f 746f 6b65 6e20 6973 206e 6f74  ext_token is not
-0003d4f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003d500: 2020 2072 6573 756c 745b 274e 6578 7454     result['NextT
-0003d510: 6f6b 656e 275d 203d 2073 656c 662e 6e65  oken'] = self.ne
-0003d520: 7874 5f74 6f6b 656e 0a20 2020 2020 2020  xt_token.       
-0003d530: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
-0003d540: 655f 6964 5f73 6872 696e 6b20 6973 206e  e_id_shrink is n
-0003d550: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003d560: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
-0003d570: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
-0003d580: 2e72 6573 6f75 7263 655f 6964 5f73 6872  .resource_id_shr
-0003d590: 696e 6b0a 2020 2020 2020 2020 6966 2073  ink.        if s
-0003d5a0: 656c 662e 7265 736f 7572 6365 5f74 7970  elf.resource_typ
-0003d5b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0003d5c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003d5d0: 745b 2752 6573 6f75 7263 6554 7970 6527  t['ResourceType'
-0003d5e0: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
-0003d5f0: 655f 7479 7065 0a20 2020 2020 2020 2069  e_type.        i
-0003d600: 6620 7365 6c66 2e74 6167 5f73 6872 696e  f self.tag_shrin
-0003d610: 6b20 6973 206e 6f74 204e 6f6e 653a 0a20  k is not None:. 
-0003d620: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003d630: 745b 2754 6167 275d 203d 2073 656c 662e  t['Tag'] = self.
-0003d640: 7461 675f 7368 7269 6e6b 0a20 2020 2020  tag_shrink.     
-0003d650: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0003d660: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-0003d670: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-0003d680: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-0003d690: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0003d6a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003d6b0: 6574 2827 4c69 6d69 7427 2920 6973 206e  et('Limit') is n
-0003d6c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003d6d0: 2020 2020 2073 656c 662e 6c69 6d69 7420       self.limit 
-0003d6e0: 3d20 6d2e 6765 7428 274c 696d 6974 2729  = m.get('Limit')
-0003d6f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003d700: 7428 274e 6578 7454 6f6b 656e 2729 2069  t('NextToken') i
-0003d710: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003d720: 2020 2020 2020 2020 7365 6c66 2e6e 6578          self.nex
-0003d730: 745f 746f 6b65 6e20 3d20 6d2e 6765 7428  t_token = m.get(
-0003d740: 274e 6578 7454 6f6b 656e 2729 0a20 2020  'NextToken').   
-0003d750: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-0003d760: 6573 6f75 7263 6549 6427 2920 6973 206e  esourceId') is n
-0003d770: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003d780: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
-0003d790: 6365 5f69 645f 7368 7269 6e6b 203d 206d  ce_id_shrink = m
-0003d7a0: 2e67 6574 2827 5265 736f 7572 6365 4964  .get('ResourceId
-0003d7b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0003d7c0: 6765 7428 2752 6573 6f75 7263 6554 7970  get('ResourceTyp
-0003d7d0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0003d7e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0003d7f0: 662e 7265 736f 7572 6365 5f74 7970 6520  f.resource_type 
-0003d800: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
-0003d810: 6554 7970 6527 290a 2020 2020 2020 2020  eType').        
-0003d820: 6966 206d 2e67 6574 2827 5461 6727 2920  if m.get('Tag') 
-0003d830: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003d840: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-0003d850: 675f 7368 7269 6e6b 203d 206d 2e67 6574  g_shrink = m.get
-0003d860: 2827 5461 6727 290a 2020 2020 2020 2020  ('Tag').        
-0003d870: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0003d880: 6173 7320 4c69 7374 5461 6752 6573 6f75  ass ListTagResou
-0003d890: 7263 6573 5265 7370 6f6e 7365 2854 6561  rcesResponse(Tea
-0003d8a0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0003d8b0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0003d8c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0003d8d0: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
-0003d8e0: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
-0003d8f0: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
-0003d900: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
-0003d910: 0a20 2020 2020 2020 2062 6f64 793a 204c  .        body: L
-0003d920: 6973 7454 6167 5265 736f 7572 6365 734f  istTagResourcesO
-0003d930: 7574 7075 7420 3d20 4e6f 6e65 2c0a 2020  utput = None,.  
-0003d940: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-0003d950: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-0003d960: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-0003d970: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-0003d980: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0003d990: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-0003d9a0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-0003d9b0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0003d9c0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0003d9d0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0003d9e0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-0003d9f0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0003da00: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0003da10: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0003da20: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0003da30: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0003da40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003da50: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0003da60: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0003da70: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0003da80: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-0003da90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003daa0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003dab0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-0003dac0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-0003dad0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-0003dae0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-0003daf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003db00: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-0003db10: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-0003db20: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-0003db30: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-0003db40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003db50: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-0003db60: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-0003db70: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0003db80: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0003db90: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0003dba0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0003dbb0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0003dbc0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0003dbd0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003dbe0: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
-0003dbf0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003dc00: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-0003dc10: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
-0003dc20: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
-0003dc30: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-0003dc40: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
-0003dc50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0003dc60: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-0003dc70: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-0003dc80: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
-0003dc90: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-0003dca0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003dcb0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-0003dcc0: 6c20 3d20 4c69 7374 5461 6752 6573 6f75  l = ListTagResou
-0003dcd0: 7263 6573 4f75 7470 7574 2829 0a20 2020  rcesOutput().   
-0003dce0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003dcf0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-0003dd00: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-0003dd10: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-0003dd20: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0003dd30: 4c69 7374 5472 6967 6765 7273 5265 7175  ListTriggersRequ
-0003dd40: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-0003dd50: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0003dd60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0003dd70: 2020 2020 2020 206c 696d 6974 3a20 696e         limit: in
-0003dd80: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-0003dd90: 2020 6e65 7874 5f74 6f6b 656e 3a20 7374    next_token: st
-0003dda0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0003ddb0: 2020 7072 6566 6978 3a20 7374 7220 3d20    prefix: str = 
-0003ddc0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0003ddd0: 2020 2020 2023 2054 6865 206e 756d 6265       # The numbe
-0003dde0: 7220 6f66 2074 7269 6767 6572 7320 7265  r of triggers re
-0003ddf0: 7475 726e 6564 2e0a 2020 2020 2020 2020  turned..        
-0003de00: 7365 6c66 2e6c 696d 6974 203d 206c 696d  self.limit = lim
-0003de10: 6974 0a20 2020 2020 2020 2023 2054 6865  it.        # The
-0003de20: 2074 6f6b 656e 2066 6f72 2074 6865 206e   token for the n
-0003de30: 6578 7420 7061 6765 2e0a 2020 2020 2020  ext page..      
-0003de40: 2020 7365 6c66 2e6e 6578 745f 746f 6b65    self.next_toke
-0003de50: 6e20 3d20 6e65 7874 5f74 6f6b 656e 0a20  n = next_token. 
-0003de60: 2020 2020 2020 2023 2054 6865 2074 7269         # The tri
-0003de70: 6767 6572 206e 616d 6520 7072 6566 6978  gger name prefix
-0003de80: 2e0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-0003de90: 7265 6669 7820 3d20 7072 6566 6978 0a0a  refix = prefix..
-0003dea0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0003deb0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0003dec0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-0003ded0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0003dee0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0003def0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0003df00: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0003df10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003df20: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0003df30: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0003df40: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0003df50: 2020 6966 2073 656c 662e 6c69 6d69 7420    if self.limit 
-0003df60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003df70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003df80: 276c 696d 6974 275d 203d 2073 656c 662e  'limit'] = self.
-0003df90: 6c69 6d69 740a 2020 2020 2020 2020 6966  limit.        if
-0003dfa0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
-0003dfb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003dfc0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003dfd0: 5b27 6e65 7874 546f 6b65 6e27 5d20 3d20  ['nextToken'] = 
-0003dfe0: 7365 6c66 2e6e 6578 745f 746f 6b65 6e0a  self.next_token.
-0003dff0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003e000: 7072 6566 6978 2069 7320 6e6f 7420 4e6f  prefix is not No
-0003e010: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003e020: 7265 7375 6c74 5b27 7072 6566 6978 275d  result['prefix']
-0003e030: 203d 2073 656c 662e 7072 6566 6978 0a20   = self.prefix. 
-0003e040: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0003e050: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0003e060: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0003e070: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0003e080: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0003e090: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0003e0a0: 206d 2e67 6574 2827 6c69 6d69 7427 2920   m.get('limit') 
-0003e0b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003e0c0: 2020 2020 2020 2020 2073 656c 662e 6c69           self.li
-0003e0d0: 6d69 7420 3d20 6d2e 6765 7428 276c 696d  mit = m.get('lim
-0003e0e0: 6974 2729 0a20 2020 2020 2020 2069 6620  it').        if 
-0003e0f0: 6d2e 6765 7428 276e 6578 7454 6f6b 656e  m.get('nextToken
-0003e100: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0003e110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003e120: 2e6e 6578 745f 746f 6b65 6e20 3d20 6d2e  .next_token = m.
-0003e130: 6765 7428 276e 6578 7454 6f6b 656e 2729  get('nextToken')
-0003e140: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003e150: 7428 2770 7265 6669 7827 2920 6973 206e  t('prefix') is n
-0003e160: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003e170: 2020 2020 2073 656c 662e 7072 6566 6978       self.prefix
-0003e180: 203d 206d 2e67 6574 2827 7072 6566 6978   = m.get('prefix
-0003e190: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0003e1a0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
-0003e1b0: 6973 7454 7269 6767 6572 7352 6573 706f  istTriggersRespo
-0003e1c0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-0003e1d0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0003e1e0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0003e1f0: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-0003e200: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-0003e210: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0003e220: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
-0003e230: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0003e240: 626f 6479 3a20 4c69 7374 5472 6967 6765  body: ListTrigge
-0003e250: 7273 4f75 7470 7574 203d 204e 6f6e 652c  rsOutput = None,
-0003e260: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0003e270: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
-0003e280: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
-0003e290: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0003e2a0: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
-0003e2b0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0003e2c0: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
-0003e2d0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0003e2e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003e2f0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-0003e300: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-0003e310: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-0003e320: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0003e330: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0003e340: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-0003e350: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003e360: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003e370: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003e380: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003e390: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003e3a0: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-0003e3b0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-0003e3c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003e3d0: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-0003e3e0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-0003e3f0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0003e400: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-0003e410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003e420: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-0003e430: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-0003e440: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0003e450: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0003e460: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003e470: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003e480: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0003e490: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0003e4a0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0003e4b0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0003e4c0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-0003e4d0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-0003e4e0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0003e4f0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0003e500: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-0003e510: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003e520: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-0003e530: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-0003e540: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-0003e550: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-0003e560: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-0003e570: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003e580: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003e590: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-0003e5a0: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-0003e5b0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-0003e5c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003e5d0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-0003e5e0: 6f64 656c 203d 204c 6973 7454 7269 6767  odel = ListTrigg
-0003e5f0: 6572 734f 7574 7075 7428 290a 2020 2020  ersOutput().    
-0003e600: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0003e610: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-0003e620: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-0003e630: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-0003e640: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
-0003e650: 6973 7456 7063 4269 6e64 696e 6773 5265  istVpcBindingsRe
-0003e660: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-0003e670: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003e680: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0003e690: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-0003e6a0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-0003e6b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0003e6c0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-0003e6d0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-0003e6e0: 2020 2062 6f64 793a 204c 6973 7456 7063     body: ListVpc
-0003e6f0: 4269 6e64 696e 6773 4f75 7470 7574 203d  BindingsOutput =
-0003e700: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0003e710: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-0003e720: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-0003e730: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0003e740: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-0003e750: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-0003e760: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-0003e770: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0003e780: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-0003e790: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-0003e7a0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0003e7b0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-0003e7c0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0003e7d0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0003e7e0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0003e7f0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0003e800: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0003e810: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0003e820: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0003e830: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0003e840: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0003e850: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-0003e860: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003e870: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-0003e880: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-0003e890: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-0003e8a0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0003e8b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003e8c0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003e8d0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-0003e8e0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003e8f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0003e900: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-0003e910: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003e920: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-0003e930: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-0003e940: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-0003e950: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0003e960: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0003e970: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0003e980: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0003e990: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0003e9a0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-0003e9b0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-0003e9c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0003e9d0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-0003e9e0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-0003e9f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003ea00: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-0003ea10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003ea20: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0003ea30: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-0003ea40: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-0003ea50: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0003ea60: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-0003ea70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003ea80: 7465 6d70 5f6d 6f64 656c 203d 204c 6973  temp_model = Lis
-0003ea90: 7456 7063 4269 6e64 696e 6773 4f75 7470  tVpcBindingsOutp
-0003eaa0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-0003eab0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-0003eac0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-0003ead0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-0003eae0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0003eaf0: 0a0a 636c 6173 7320 5075 626c 6973 6846  ..class PublishF
-0003eb00: 756e 6374 696f 6e56 6572 7369 6f6e 5265  unctionVersionRe
-0003eb10: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-0003eb20: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0003eb30: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0003eb40: 0a20 2020 2020 2020 2062 6f64 793a 2050  .        body: P
-0003eb50: 7562 6c69 7368 5665 7273 696f 6e49 6e70  ublishVersionInp
-0003eb60: 7574 203d 204e 6f6e 652c 0a20 2020 2029  ut = None,.    )
-0003eb70: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
-0003eb80: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
-0003eb90: 7420 7468 6520 6675 6e63 7469 6f6e 2076  t the function v
-0003eba0: 6572 7369 6f6e 2e0a 2020 2020 2020 2020  ersion..        
-0003ebb0: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-0003ebc0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0003ebd0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0003ebe0: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-0003ebf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003ec00: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-0003ec10: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0003ec20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0003ec30: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-0003ec40: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0003ec50: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0003ec60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003ec70: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0003ec80: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0003ec90: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0003eca0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-0003ecb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003ecc0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-0003ecd0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-0003ece0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0003ecf0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0003ed00: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0003ed10: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0003ed20: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0003ed30: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0003ed40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003ed50: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-0003ed60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003ed70: 2074 656d 705f 6d6f 6465 6c20 3d20 5075   temp_model = Pu
-0003ed80: 626c 6973 6856 6572 7369 6f6e 496e 7075  blishVersionInpu
-0003ed90: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0003eda0: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-0003edb0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-0003edc0: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-0003edd0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0003ede0: 0a63 6c61 7373 2050 7562 6c69 7368 4675  .class PublishFu
-0003edf0: 6e63 7469 6f6e 5665 7273 696f 6e52 6573  nctionVersionRes
-0003ee00: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-0003ee10: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0003ee20: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0003ee30: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-0003ee40: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-0003ee50: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0003ee60: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-0003ee70: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-0003ee80: 2020 626f 6479 3a20 5665 7273 696f 6e20    body: Version 
-0003ee90: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0003eea0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0003eeb0: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-0003eec0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0003eed0: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0003eee0: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-0003eef0: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-0003ef00: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0003ef10: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0003ef20: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-0003ef30: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003ef40: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-0003ef50: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0003ef60: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0003ef70: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0003ef80: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0003ef90: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0003efa0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003efb0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0003efc0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0003efd0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0003efe0: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-0003eff0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003f000: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-0003f010: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-0003f020: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-0003f030: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003f040: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003f050: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003f060: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-0003f070: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003f080: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0003f090: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-0003f0a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003f0b0: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-0003f0c0: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-0003f0d0: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0003f0e0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0003f0f0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0003f100: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0003f110: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0003f120: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0003f130: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-0003f140: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-0003f150: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003f160: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-0003f170: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-0003f180: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003f190: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-0003f1a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003f1b0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0003f1c0: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-0003f1d0: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-0003f1e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003f1f0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-0003f200: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003f210: 2074 656d 705f 6d6f 6465 6c20 3d20 5665   temp_model = Ve
-0003f220: 7273 696f 6e28 290a 2020 2020 2020 2020  rsion().        
-0003f230: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0003f240: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-0003f250: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-0003f260: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0003f270: 6c66 0a0a 0a63 6c61 7373 2050 7574 4173  lf...class PutAs
-0003f280: 796e 6349 6e76 6f6b 6543 6f6e 6669 6752  yncInvokeConfigR
-0003f290: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-0003f2a0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003f2b0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0003f2c0: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-0003f2d0: 5075 7441 7379 6e63 496e 766f 6b65 436f  PutAsyncInvokeCo
-0003f2e0: 6e66 6967 496e 7075 7420 3d20 4e6f 6e65  nfigInput = None
-0003f2f0: 2c0a 2020 2020 2020 2020 7175 616c 6966  ,.        qualif
-0003f300: 6965 723a 2073 7472 203d 204e 6f6e 652c  ier: str = None,
-0003f310: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0003f320: 2320 5468 6520 636f 6e66 6967 7572 6174  # The configurat
-0003f330: 696f 6e73 206f 6620 6173 796e 6368 726f  ions of asynchro
-0003f340: 6e6f 7573 2066 756e 6374 696f 6e20 696e  nous function in
-0003f350: 766f 6361 7469 6f6e 2e0a 2020 2020 2020  vocation..      
-0003f360: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-0003f370: 6479 0a20 2020 2020 2020 2023 2054 6865  dy.        # The
-0003f380: 2076 6572 7369 6f6e 206f 7220 616c 6961   version or alia
-0003f390: 7320 6f66 2074 6865 2066 756e 6374 696f  s of the functio
-0003f3a0: 6e2e 0a20 2020 2020 2020 2073 656c 662e  n..        self.
-0003f3b0: 7175 616c 6966 6965 7220 3d20 7175 616c  qualifier = qual
-0003f3c0: 6966 6965 720a 0a20 2020 2064 6566 2076  ifier..    def v
-0003f3d0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0003f3e0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0003f3f0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-0003f400: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-0003f410: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-0003f420: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0003f430: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0003f440: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-0003f450: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0003f460: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003f470: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0003f480: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0003f490: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0003f4a0: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0003f4b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003f4c0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0003f4d0: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0003f4e0: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0003f4f0: 2020 2020 2069 6620 7365 6c66 2e71 7561       if self.qua
-0003f500: 6c69 6669 6572 2069 7320 6e6f 7420 4e6f  lifier is not No
-0003f510: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003f520: 7265 7375 6c74 5b27 7175 616c 6966 6965  result['qualifie
-0003f530: 7227 5d20 3d20 7365 6c66 2e71 7561 6c69  r'] = self.quali
-0003f540: 6669 6572 0a20 2020 2020 2020 2072 6574  fier.        ret
-0003f550: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0003f560: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0003f570: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-0003f580: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0003f590: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0003f5a0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-0003f5b0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-0003f5c0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-0003f5d0: 6d70 5f6d 6f64 656c 203d 2050 7574 4173  mp_model = PutAs
-0003f5e0: 796e 6349 6e76 6f6b 6543 6f6e 6669 6749  yncInvokeConfigI
-0003f5f0: 6e70 7574 2829 0a20 2020 2020 2020 2020  nput().         
-0003f600: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-0003f610: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-0003f620: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-0003f630: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0003f640: 7175 616c 6966 6965 7227 2920 6973 206e  qualifier') is n
-0003f650: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003f660: 2020 2020 2073 656c 662e 7175 616c 6966       self.qualif
-0003f670: 6965 7220 3d20 6d2e 6765 7428 2771 7561  ier = m.get('qua
-0003f680: 6c69 6669 6572 2729 0a20 2020 2020 2020  lifier').       
-0003f690: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0003f6a0: 6c61 7373 2050 7574 4173 796e 6349 6e76  lass PutAsyncInv
-0003f6b0: 6f6b 6543 6f6e 6669 6752 6573 706f 6e73  okeConfigRespons
-0003f6c0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+00038690: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+000386a0: 6f72 744f 7264 6572 4279 5469 6d65 275d  ortOrderByTime']
+000386b0: 203d 2073 656c 662e 736f 7274 5f6f 7264   = self.sort_ord
+000386c0: 6572 5f62 795f 7469 6d65 0a20 2020 2020  er_by_time.     
+000386d0: 2020 2069 6620 7365 6c66 2e73 7461 7274     if self.start
+000386e0: 6564 5f74 696d 655f 6265 6769 6e20 6973  ed_time_begin is
+000386f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038700: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00038710: 7461 7274 6564 5469 6d65 4265 6769 6e27  tartedTimeBegin'
+00038720: 5d20 3d20 7365 6c66 2e73 7461 7274 6564  ] = self.started
+00038730: 5f74 696d 655f 6265 6769 6e0a 2020 2020  _time_begin.    
+00038740: 2020 2020 6966 2073 656c 662e 7374 6172      if self.star
+00038750: 7465 645f 7469 6d65 5f65 6e64 2069 7320  ted_time_end is 
+00038760: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038770: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+00038780: 6172 7465 6454 696d 6545 6e64 275d 203d  artedTimeEnd'] =
+00038790: 2073 656c 662e 7374 6172 7465 645f 7469   self.started_ti
+000387a0: 6d65 5f65 6e64 0a20 2020 2020 2020 2069  me_end.        i
+000387b0: 6620 7365 6c66 2e73 7461 7475 7320 6973  f self.status is
+000387c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000387d0: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+000387e0: 7461 7475 7327 5d20 3d20 7365 6c66 2e73  tatus'] = self.s
+000387f0: 7461 7475 730a 2020 2020 2020 2020 7265  tatus.        re
+00038800: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00038810: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00038820: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00038830: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00038840: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00038850: 2020 2020 2069 6620 6d2e 6765 7428 2769       if m.get('i
+00038860: 6e63 6c75 6465 5061 796c 6f61 6427 2920  ncludePayload') 
+00038870: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00038880: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+00038890: 636c 7564 655f 7061 796c 6f61 6420 3d20  clude_payload = 
+000388a0: 6d2e 6765 7428 2769 6e63 6c75 6465 5061  m.get('includePa
+000388b0: 796c 6f61 6427 290a 2020 2020 2020 2020  yload').        
+000388c0: 6966 206d 2e67 6574 2827 6c69 6d69 7427  if m.get('limit'
+000388d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000388e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000388f0: 6c69 6d69 7420 3d20 6d2e 6765 7428 276c  limit = m.get('l
+00038900: 696d 6974 2729 0a20 2020 2020 2020 2069  imit').        i
+00038910: 6620 6d2e 6765 7428 276e 6578 7454 6f6b  f m.get('nextTok
+00038920: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
+00038930: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00038940: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
+00038950: 6d2e 6765 7428 276e 6578 7454 6f6b 656e  m.get('nextToken
+00038960: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00038970: 6765 7428 2770 7265 6669 7827 2920 6973  get('prefix') is
+00038980: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038990: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+000389a0: 6978 203d 206d 2e67 6574 2827 7072 6566  ix = m.get('pref
+000389b0: 6978 2729 0a20 2020 2020 2020 2069 6620  ix').        if 
+000389c0: 6d2e 6765 7428 2771 7561 6c69 6669 6572  m.get('qualifier
+000389d0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000389e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000389f0: 2e71 7561 6c69 6669 6572 203d 206d 2e67  .qualifier = m.g
+00038a00: 6574 2827 7175 616c 6966 6965 7227 290a  et('qualifier').
+00038a10: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00038a20: 2827 736f 7274 4f72 6465 7242 7954 696d  ('sortOrderByTim
+00038a30: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00038a40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00038a50: 662e 736f 7274 5f6f 7264 6572 5f62 795f  f.sort_order_by_
+00038a60: 7469 6d65 203d 206d 2e67 6574 2827 736f  time = m.get('so
+00038a70: 7274 4f72 6465 7242 7954 696d 6527 290a  rtOrderByTime').
+00038a80: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00038a90: 2827 7374 6172 7465 6454 696d 6542 6567  ('startedTimeBeg
+00038aa0: 696e 2729 2069 7320 6e6f 7420 4e6f 6e65  in') is not None
+00038ab0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00038ac0: 6c66 2e73 7461 7274 6564 5f74 696d 655f  lf.started_time_
+00038ad0: 6265 6769 6e20 3d20 6d2e 6765 7428 2773  begin = m.get('s
+00038ae0: 7461 7274 6564 5469 6d65 4265 6769 6e27  tartedTimeBegin'
+00038af0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00038b00: 6574 2827 7374 6172 7465 6454 696d 6545  et('startedTimeE
+00038b10: 6e64 2729 2069 7320 6e6f 7420 4e6f 6e65  nd') is not None
+00038b20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00038b30: 6c66 2e73 7461 7274 6564 5f74 696d 655f  lf.started_time_
+00038b40: 656e 6420 3d20 6d2e 6765 7428 2773 7461  end = m.get('sta
+00038b50: 7274 6564 5469 6d65 456e 6427 290a 2020  rtedTimeEnd').  
+00038b60: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00038b70: 7374 6174 7573 2729 2069 7320 6e6f 7420  status') is not 
+00038b80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00038b90: 2020 7365 6c66 2e73 7461 7475 7320 3d20    self.status = 
+00038ba0: 6d2e 6765 7428 2773 7461 7475 7327 290a  m.get('status').
+00038bb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00038bc0: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
+00038bd0: 4173 796e 6354 6173 6b73 5265 7370 6f6e  AsyncTasksRespon
+00038be0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00038bf0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00038c00: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00038c10: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+00038c20: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+00038c30: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+00038c40: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+00038c50: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+00038c60: 6f64 793a 204c 6973 7441 7379 6e63 5461  ody: ListAsyncTa
+00038c70: 736b 4f75 7470 7574 203d 204e 6f6e 652c  skOutput = None,
+00038c80: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00038c90: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+00038ca0: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
+00038cb0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00038cc0: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
+00038cd0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00038ce0: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
+00038cf0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00038d00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00038d10: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+00038d20: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+00038d30: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+00038d40: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00038d50: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00038d60: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+00038d70: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00038d80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038d90: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00038da0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00038db0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00038dc0: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+00038dd0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+00038de0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00038df0: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+00038e00: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+00038e10: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00038e20: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+00038e30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00038e40: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+00038e50: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+00038e60: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00038e70: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00038e80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00038e90: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00038ea0: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00038eb0: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00038ec0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00038ed0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00038ee0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00038ef0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00038f00: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00038f10: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00038f20: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+00038f30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00038f40: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+00038f50: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+00038f60: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+00038f70: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+00038f80: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+00038f90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00038fa0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00038fb0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+00038fc0: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+00038fd0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+00038fe0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00038ff0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00039000: 6f64 656c 203d 204c 6973 7441 7379 6e63  odel = ListAsync
+00039010: 5461 736b 4f75 7470 7574 2829 0a20 2020  TaskOutput().   
+00039020: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00039030: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+00039040: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+00039050: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+00039060: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00039070: 4c69 7374 436f 6e63 7572 7265 6e63 7943  ListConcurrencyC
+00039080: 6f6e 6669 6773 5265 7175 6573 7428 5465  onfigsRequest(Te
+00039090: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+000390a0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000390b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000390c0: 2066 756e 6374 696f 6e5f 6e61 6d65 3a20   function_name: 
+000390d0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000390e0: 2020 2020 6c69 6d69 743a 2069 6e74 203d      limit: int =
+000390f0: 204e 6f6e 652c 0a20 2020 2020 2020 206e   None,.        n
+00039100: 6578 745f 746f 6b65 6e3a 2073 7472 203d  ext_token: str =
+00039110: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00039120: 2020 2020 2020 2320 5468 6520 6675 6e63        # The func
+00039130: 7469 6f6e 206e 616d 652e 2049 6620 796f  tion name. If yo
+00039140: 7520 6c65 6176 6520 7468 6973 2070 6172  u leave this par
+00039150: 616d 6574 6572 2065 6d70 7479 2c20 7468  ameter empty, th
+00039160: 6520 636f 6e63 7572 7265 6e63 7920 636f  e concurrency co
+00039170: 6e66 6967 7572 6174 696f 6e73 206f 6620  nfigurations of 
+00039180: 616c 6c20 6675 6e63 7469 6f6e 7320 6172  all functions ar
+00039190: 6520 7265 7475 726e 6564 2e0a 2020 2020  e returned..    
+000391a0: 2020 2020 7365 6c66 2e66 756e 6374 696f      self.functio
+000391b0: 6e5f 6e61 6d65 203d 2066 756e 6374 696f  n_name = functio
+000391c0: 6e5f 6e61 6d65 0a20 2020 2020 2020 2023  n_name.        #
+000391d0: 2054 6865 206d 6178 696d 756d 206e 756d   The maximum num
+000391e0: 6265 7220 6f66 2065 6e74 7269 6573 2072  ber of entries r
+000391f0: 6574 7572 6e65 642e 0a20 2020 2020 2020  eturned..       
+00039200: 2073 656c 662e 6c69 6d69 7420 3d20 6c69   self.limit = li
+00039210: 6d69 740a 2020 2020 2020 2020 2320 5468  mit.        # Th
+00039220: 6520 7061 6769 6e61 7469 6f6e 2074 6f6b  e pagination tok
+00039230: 656e 2074 6861 7420 6973 2075 7365 6420  en that is used 
+00039240: 696e 2074 6865 206e 6578 7420 7265 7175  in the next requ
+00039250: 6573 7420 746f 2072 6574 7269 6576 6520  est to retrieve 
+00039260: 6120 6e65 7720 7061 6765 206f 6620 7265  a new page of re
+00039270: 7375 6c74 732e 0a20 2020 2020 2020 2073  sults..        s
+00039280: 656c 662e 6e65 7874 5f74 6f6b 656e 203d  elf.next_token =
+00039290: 206e 6578 745f 746f 6b65 6e0a 0a20 2020   next_token..   
+000392a0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000392b0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000392c0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+000392d0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000392e0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+000392f0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00039300: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00039310: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00039320: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00039330: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00039340: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00039350: 6620 7365 6c66 2e66 756e 6374 696f 6e5f  f self.function_
+00039360: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+00039370: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00039380: 7375 6c74 5b27 6675 6e63 7469 6f6e 4e61  sult['functionNa
+00039390: 6d65 275d 203d 2073 656c 662e 6675 6e63  me'] = self.func
+000393a0: 7469 6f6e 5f6e 616d 650a 2020 2020 2020  tion_name.      
+000393b0: 2020 6966 2073 656c 662e 6c69 6d69 7420    if self.limit 
+000393c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000393d0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000393e0: 276c 696d 6974 275d 203d 2073 656c 662e  'limit'] = self.
+000393f0: 6c69 6d69 740a 2020 2020 2020 2020 6966  limit.        if
+00039400: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+00039410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00039420: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00039430: 5b27 6e65 7874 546f 6b65 6e27 5d20 3d20  ['nextToken'] = 
+00039440: 7365 6c66 2e6e 6578 745f 746f 6b65 6e0a  self.next_token.
+00039450: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00039460: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00039470: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00039480: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00039490: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+000394a0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000394b0: 6620 6d2e 6765 7428 2766 756e 6374 696f  f m.get('functio
+000394c0: 6e4e 616d 6527 2920 6973 206e 6f74 204e  nName') is not N
+000394d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000394e0: 2073 656c 662e 6675 6e63 7469 6f6e 5f6e   self.function_n
+000394f0: 616d 6520 3d20 6d2e 6765 7428 2766 756e  ame = m.get('fun
+00039500: 6374 696f 6e4e 616d 6527 290a 2020 2020  ctionName').    
+00039510: 2020 2020 6966 206d 2e67 6574 2827 6c69      if m.get('li
+00039520: 6d69 7427 2920 6973 206e 6f74 204e 6f6e  mit') is not Non
+00039530: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00039540: 656c 662e 6c69 6d69 7420 3d20 6d2e 6765  elf.limit = m.ge
+00039550: 7428 276c 696d 6974 2729 0a20 2020 2020  t('limit').     
+00039560: 2020 2069 6620 6d2e 6765 7428 276e 6578     if m.get('nex
+00039570: 7454 6f6b 656e 2729 2069 7320 6e6f 7420  tToken') is not 
+00039580: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00039590: 2020 7365 6c66 2e6e 6578 745f 746f 6b65    self.next_toke
+000395a0: 6e20 3d20 6d2e 6765 7428 276e 6578 7454  n = m.get('nextT
+000395b0: 6f6b 656e 2729 0a20 2020 2020 2020 2072  oken').        r
+000395c0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000395d0: 7373 204c 6973 7443 6f6e 6375 7272 656e  ss ListConcurren
+000395e0: 6379 436f 6e66 6967 7352 6573 706f 6e73  cyConfigsRespons
+000395f0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+00039600: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00039610: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00039620: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+00039630: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+00039640: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+00039650: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+00039660: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+00039670: 6479 3a20 4c69 7374 436f 6e63 7572 7265  dy: ListConcurre
+00039680: 6e63 7943 6f6e 6669 6773 4f75 7470 7574  ncyConfigsOutput
+00039690: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+000396a0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000396b0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+000396c0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000396d0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+000396e0: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+000396f0: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+00039700: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00039710: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00039720: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00039730: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00039740: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00039750: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00039760: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00039770: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00039780: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00039790: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000397a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000397b0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000397c0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000397d0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000397e0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+000397f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00039800: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+00039810: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+00039820: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+00039830: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00039840: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00039850: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00039860: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+00039870: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+00039880: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+00039890: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+000398a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000398b0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+000398c0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+000398d0: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+000398e0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000398f0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00039900: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00039910: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00039920: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00039930: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00039940: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00039950: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00039960: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00039970: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00039980: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00039990: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+000399a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000399b0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000399c0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+000399d0: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000399e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000399f0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00039a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00039a10: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
+00039a20: 6973 7443 6f6e 6375 7272 656e 6379 436f  istConcurrencyCo
+00039a30: 6e66 6967 734f 7574 7075 7428 290a 2020  nfigsOutput().  
+00039a40: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00039a50: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+00039a60: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+00039a70: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+00039a80: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00039a90: 204c 6973 7443 7573 746f 6d44 6f6d 6169   ListCustomDomai
+00039aa0: 6e73 5265 7175 6573 7428 5465 614d 6f64  nsRequest(TeaMod
+00039ab0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00039ac0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00039ad0: 656c 662c 0a20 2020 2020 2020 206c 696d  elf,.        lim
+00039ae0: 6974 3a20 696e 7420 3d20 4e6f 6e65 2c0a  it: int = None,.
+00039af0: 2020 2020 2020 2020 6e65 7874 5f74 6f6b          next_tok
+00039b00: 656e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  en: str = None,.
+00039b10: 2020 2020 2020 2020 7072 6566 6978 3a20          prefix: 
+00039b20: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00039b30: 293a 0a20 2020 2020 2020 2023 2054 6865  ):.        # The
+00039b40: 206e 756d 6265 7220 6f66 2063 7573 746f   number of custo
+00039b50: 6d20 646f 6d61 696e 206e 616d 6573 2072  m domain names r
+00039b60: 6574 7572 6e65 642e 0a20 2020 2020 2020  eturned..       
+00039b70: 2073 656c 662e 6c69 6d69 7420 3d20 6c69   self.limit = li
+00039b80: 6d69 740a 2020 2020 2020 2020 2320 5468  mit.        # Th
+00039b90: 6520 7061 6769 6e61 7469 6f6e 2074 6f6b  e pagination tok
+00039ba0: 656e 2074 6861 7420 6973 2075 7365 6420  en that is used 
+00039bb0: 696e 2074 6865 206e 6578 7420 7265 7175  in the next requ
+00039bc0: 6573 7420 746f 2072 6574 7269 6576 6520  est to retrieve 
+00039bd0: 6120 6e65 7720 7061 6765 206f 6620 7265  a new page of re
+00039be0: 7375 6c74 732e 0a20 2020 2020 2020 2073  sults..        s
+00039bf0: 656c 662e 6e65 7874 5f74 6f6b 656e 203d  elf.next_token =
+00039c00: 206e 6578 745f 746f 6b65 6e0a 2020 2020   next_token.    
+00039c10: 2020 2020 2320 5468 6520 646f 6d61 696e      # The domain
+00039c20: 206e 616d 6520 7072 6566 6978 2e0a 2020   name prefix..  
+00039c30: 2020 2020 2020 7365 6c66 2e70 7265 6669        self.prefi
+00039c40: 7820 3d20 7072 6566 6978 0a0a 2020 2020  x = prefix..    
+00039c50: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00039c60: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00039c70: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00039c80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00039c90: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00039ca0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00039cb0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00039cc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00039cd0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00039ce0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00039cf0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00039d00: 2073 656c 662e 6c69 6d69 7420 6973 206e   self.limit is n
+00039d10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00039d20: 2020 2020 2072 6573 756c 745b 276c 696d       result['lim
+00039d30: 6974 275d 203d 2073 656c 662e 6c69 6d69  it'] = self.limi
+00039d40: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
+00039d50: 662e 6e65 7874 5f74 6f6b 656e 2069 7320  f.next_token is 
+00039d60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00039d70: 2020 2020 2020 7265 7375 6c74 5b27 6e65        result['ne
+00039d80: 7874 546f 6b65 6e27 5d20 3d20 7365 6c66  xtToken'] = self
+00039d90: 2e6e 6578 745f 746f 6b65 6e0a 2020 2020  .next_token.    
+00039da0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+00039db0: 6978 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ix is not None:.
+00039dc0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00039dd0: 6c74 5b27 7072 6566 6978 275d 203d 2073  lt['prefix'] = s
+00039de0: 656c 662e 7072 6566 6978 0a20 2020 2020  elf.prefix.     
+00039df0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00039e00: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00039e10: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+00039e20: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00039e30: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00039e40: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00039e50: 6574 2827 6c69 6d69 7427 2920 6973 206e  et('limit') is n
+00039e60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00039e70: 2020 2020 2073 656c 662e 6c69 6d69 7420       self.limit 
+00039e80: 3d20 6d2e 6765 7428 276c 696d 6974 2729  = m.get('limit')
+00039e90: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00039ea0: 7428 276e 6578 7454 6f6b 656e 2729 2069  t('nextToken') i
+00039eb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00039ec0: 2020 2020 2020 2020 7365 6c66 2e6e 6578          self.nex
+00039ed0: 745f 746f 6b65 6e20 3d20 6d2e 6765 7428  t_token = m.get(
+00039ee0: 276e 6578 7454 6f6b 656e 2729 0a20 2020  'nextToken').   
+00039ef0: 2020 2020 2069 6620 6d2e 6765 7428 2770       if m.get('p
+00039f00: 7265 6669 7827 2920 6973 206e 6f74 204e  refix') is not N
+00039f10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00039f20: 2073 656c 662e 7072 6566 6978 203d 206d   self.prefix = m
+00039f30: 2e67 6574 2827 7072 6566 6978 2729 0a20  .get('prefix'). 
+00039f40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00039f50: 6c66 0a0a 0a63 6c61 7373 204c 6973 7443  lf...class ListC
+00039f60: 7573 746f 6d44 6f6d 6169 6e73 5265 7370  ustomDomainsResp
+00039f70: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+00039f80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00039f90: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00039fa0: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+00039fb0: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
+00039fc0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00039fd0: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
+00039fe0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00039ff0: 2062 6f64 793a 204c 6973 7443 7573 746f   body: ListCusto
+0003a000: 6d44 6f6d 6169 6e4f 7574 7075 7420 3d20  mDomainOutput = 
+0003a010: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0003a020: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+0003a030: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+0003a040: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0003a050: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+0003a060: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
+0003a070: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+0003a080: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0003a090: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+0003a0a0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+0003a0b0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0003a0c0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+0003a0d0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0003a0e0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0003a0f0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+0003a100: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0003a110: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0003a120: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0003a130: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0003a140: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0003a150: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003a160: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+0003a170: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003a180: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+0003a190: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+0003a1a0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+0003a1b0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+0003a1c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003a1d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003a1e0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+0003a1f0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+0003a200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003a210: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+0003a220: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003a230: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+0003a240: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+0003a250: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0003a260: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+0003a270: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+0003a280: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+0003a290: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+0003a2a0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+0003a2b0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+0003a2c0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+0003a2d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003a2e0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+0003a2f0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+0003a300: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003a310: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+0003a320: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003a330: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0003a340: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+0003a350: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+0003a360: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+0003a370: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+0003a380: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0003a390: 656d 705f 6d6f 6465 6c20 3d20 4c69 7374  emp_model = List
+0003a3a0: 4375 7374 6f6d 446f 6d61 696e 4f75 7470  CustomDomainOutp
+0003a3b0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+0003a3c0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+0003a3d0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+0003a3e0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+0003a3f0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0003a400: 0a0a 636c 6173 7320 4c69 7374 4675 6e63  ..class ListFunc
+0003a410: 7469 6f6e 5665 7273 696f 6e73 5265 7175  tionVersionsRequ
+0003a420: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+0003a430: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0003a440: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0003a450: 2020 2020 2020 2064 6972 6563 7469 6f6e         direction
+0003a460: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0003a470: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
+0003a480: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0003a490: 206e 6578 745f 746f 6b65 6e3a 2073 7472   next_token: str
+0003a4a0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0003a4b0: 2020 2020 2020 2020 2320 5468 6520 736f          # The so
+0003a4c0: 7274 696e 6720 6d6f 6465 206f 6620 6675  rting mode of fu
+0003a4d0: 6e63 7469 6f6e 2076 6572 7369 6f6e 732e  nction versions.
+0003a4e0: 2056 616c 6964 2076 616c 7565 733a 2042   Valid values: B
+0003a4f0: 4143 4b57 4152 4420 616e 6420 464f 5257  ACKWARD and FORW
+0003a500: 4152 442e 0a20 2020 2020 2020 2073 656c  ARD..        sel
+0003a510: 662e 6469 7265 6374 696f 6e20 3d20 6469  f.direction = di
+0003a520: 7265 6374 696f 6e0a 2020 2020 2020 2020  rection.        
+0003a530: 2320 5468 6520 6e75 6d62 6572 206f 6620  # The number of 
+0003a540: 6675 6e63 7469 6f6e 2076 6572 7369 6f6e  function version
+0003a550: 7320 7468 6174 2061 7265 2072 6574 7572  s that are retur
+0003a560: 6e65 642e 0a20 2020 2020 2020 2073 656c  ned..        sel
+0003a570: 662e 6c69 6d69 7420 3d20 6c69 6d69 740a  f.limit = limit.
+0003a580: 2020 2020 2020 2020 2320 5468 6520 7061          # The pa
+0003a590: 6769 6e61 7469 6f6e 2074 6f6b 656e 2074  gination token t
+0003a5a0: 6861 7420 6973 2075 7365 6420 696e 2074  hat is used in t
+0003a5b0: 6865 206e 6578 7420 7265 7175 6573 7420  he next request 
+0003a5c0: 746f 2072 6574 7269 6576 6520 6120 6e65  to retrieve a ne
+0003a5d0: 7720 7061 6765 206f 6620 7265 7375 6c74  w page of result
+0003a5e0: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+0003a5f0: 6e65 7874 5f74 6f6b 656e 203d 206e 6578  next_token = nex
+0003a600: 745f 746f 6b65 6e0a 0a20 2020 2064 6566  t_token..    def
+0003a610: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0003a620: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+0003a630: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+0003a640: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+0003a650: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+0003a660: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0003a670: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0003a680: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003a690: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0003a6a0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0003a6b0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0003a6c0: 6c66 2e64 6972 6563 7469 6f6e 2069 7320  lf.direction is 
+0003a6d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003a6e0: 2020 2020 2020 7265 7375 6c74 5b27 6469        result['di
+0003a6f0: 7265 6374 696f 6e27 5d20 3d20 7365 6c66  rection'] = self
+0003a700: 2e64 6972 6563 7469 6f6e 0a20 2020 2020  .direction.     
+0003a710: 2020 2069 6620 7365 6c66 2e6c 696d 6974     if self.limit
+0003a720: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003a730: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003a740: 5b27 6c69 6d69 7427 5d20 3d20 7365 6c66  ['limit'] = self
+0003a750: 2e6c 696d 6974 0a20 2020 2020 2020 2069  .limit.        i
+0003a760: 6620 7365 6c66 2e6e 6578 745f 746f 6b65  f self.next_toke
+0003a770: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+0003a780: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003a790: 745b 276e 6578 7454 6f6b 656e 275d 203d  t['nextToken'] =
+0003a7a0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003a7b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003a7c0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0003a7d0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0003a7e0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+0003a7f0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0003a800: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0003a810: 6966 206d 2e67 6574 2827 6469 7265 6374  if m.get('direct
+0003a820: 696f 6e27 2920 6973 206e 6f74 204e 6f6e  ion') is not Non
+0003a830: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0003a840: 656c 662e 6469 7265 6374 696f 6e20 3d20  elf.direction = 
+0003a850: 6d2e 6765 7428 2764 6972 6563 7469 6f6e  m.get('direction
+0003a860: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003a870: 6765 7428 276c 696d 6974 2729 2069 7320  get('limit') is 
+0003a880: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003a890: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
+0003a8a0: 203d 206d 2e67 6574 2827 6c69 6d69 7427   = m.get('limit'
+0003a8b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003a8c0: 6574 2827 6e65 7874 546f 6b65 6e27 2920  et('nextToken') 
+0003a8d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003a8e0: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
+0003a8f0: 7874 5f74 6f6b 656e 203d 206d 2e67 6574  xt_token = m.get
+0003a900: 2827 6e65 7874 546f 6b65 6e27 290a 2020  ('nextToken').  
+0003a910: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0003a920: 660a 0a0a 636c 6173 7320 4c69 7374 4675  f...class ListFu
+0003a930: 6e63 7469 6f6e 5665 7273 696f 6e73 5265  nctionVersionsRe
+0003a940: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+0003a950: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0003a960: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0003a970: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0003a980: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+0003a990: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0003a9a0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+0003a9b0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+0003a9c0: 2020 2062 6f64 793a 204c 6973 7456 6572     body: ListVer
+0003a9d0: 7369 6f6e 734f 7574 7075 7420 3d20 4e6f  sionsOutput = No
+0003a9e0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0003a9f0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0003aa00: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
+0003aa10: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0003aa20: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+0003aa30: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+0003aa40: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
+0003aa50: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0003aa60: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+0003aa70: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+0003aa80: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+0003aa90: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+0003aaa0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0003aab0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0003aac0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0003aad0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0003aae0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003aaf0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0003ab00: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0003ab10: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0003ab20: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0003ab30: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0003ab40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003ab50: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0003ab60: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0003ab70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003ab80: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0003ab90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003aba0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0003abb0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0003abc0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0003abd0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0003abe0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0003abf0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003ac00: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0003ac10: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0003ac20: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003ac30: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003ac40: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0003ac50: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0003ac60: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003ac70: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003ac80: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+0003ac90: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003aca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003acb0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+0003acc0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+0003acd0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+0003ace0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+0003acf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003ad00: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0003ad10: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+0003ad20: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+0003ad30: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+0003ad40: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0003ad50: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0003ad60: 705f 6d6f 6465 6c20 3d20 4c69 7374 5665  p_model = ListVe
+0003ad70: 7273 696f 6e73 4f75 7470 7574 2829 0a20  rsionsOutput(). 
+0003ad80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003ad90: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+0003ada0: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+0003adb0: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+0003adc0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003add0: 7320 4c69 7374 4675 6e63 7469 6f6e 7352  s ListFunctionsR
+0003ade0: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+0003adf0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0003ae00: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0003ae10: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
+0003ae20: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+0003ae30: 2020 2020 206e 6578 745f 746f 6b65 6e3a       next_token:
+0003ae40: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0003ae50: 2020 2020 2070 7265 6669 783a 2073 7472       prefix: str
+0003ae60: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0003ae70: 2020 2020 2020 2020 2320 5468 6520 6e75          # The nu
+0003ae80: 6d62 6572 206f 6620 6675 6e63 7469 6f6e  mber of function
+0003ae90: 7320 746f 2072 6574 7572 6e2e 2054 6865  s to return. The
+0003aea0: 206d 696e 696d 756d 2076 616c 7565 2069   minimum value i
+0003aeb0: 7320 3120 616e 6420 7468 6520 6d61 7869  s 1 and the maxi
+0003aec0: 6d75 6d20 7661 6c75 6520 6973 2031 3030  mum value is 100
+0003aed0: 2e0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+0003aee0: 696d 6974 203d 206c 696d 6974 0a20 2020  imit = limit.   
+0003aef0: 2020 2020 2023 2054 6865 2070 6167 696e       # The pagin
+0003af00: 6174 696f 6e20 746f 6b65 6e2e 0a20 2020  ation token..   
+0003af10: 2020 2020 2073 656c 662e 6e65 7874 5f74       self.next_t
+0003af20: 6f6b 656e 203d 206e 6578 745f 746f 6b65  oken = next_toke
+0003af30: 6e0a 2020 2020 2020 2020 2320 5468 6520  n.        # The 
+0003af40: 7072 6566 6978 206f 6620 7468 6520 6675  prefix of the fu
+0003af50: 6e63 7469 6f6e 206e 616d 652e 0a20 2020  nction name..   
+0003af60: 2020 2020 2073 656c 662e 7072 6566 6978       self.prefix
+0003af70: 203d 2070 7265 6669 780a 0a20 2020 2064   = prefix..    d
+0003af80: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0003af90: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0003afa0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0003afb0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0003afc0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+0003afd0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0003afe0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0003aff0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003b000: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0003b010: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0003b020: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0003b030: 7365 6c66 2e6c 696d 6974 2069 7320 6e6f  self.limit is no
+0003b040: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003b050: 2020 2020 7265 7375 6c74 5b27 6c69 6d69      result['limi
+0003b060: 7427 5d20 3d20 7365 6c66 2e6c 696d 6974  t'] = self.limit
+0003b070: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003b080: 2e6e 6578 745f 746f 6b65 6e20 6973 206e  .next_token is n
+0003b090: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003b0a0: 2020 2020 2072 6573 756c 745b 276e 6578       result['nex
+0003b0b0: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
+0003b0c0: 6e65 7874 5f74 6f6b 656e 0a20 2020 2020  next_token.     
+0003b0d0: 2020 2069 6620 7365 6c66 2e70 7265 6669     if self.prefi
+0003b0e0: 7820 6973 206e 6f74 204e 6f6e 653a 0a20  x is not None:. 
+0003b0f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003b100: 745b 2770 7265 6669 7827 5d20 3d20 7365  t['prefix'] = se
+0003b110: 6c66 2e70 7265 6669 780a 2020 2020 2020  lf.prefix.      
+0003b120: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0003b130: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0003b140: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+0003b150: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0003b160: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0003b170: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003b180: 7428 276c 696d 6974 2729 2069 7320 6e6f  t('limit') is no
+0003b190: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003b1a0: 2020 2020 7365 6c66 2e6c 696d 6974 203d      self.limit =
+0003b1b0: 206d 2e67 6574 2827 6c69 6d69 7427 290a   m.get('limit').
+0003b1c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0003b1d0: 2827 6e65 7874 546f 6b65 6e27 2920 6973  ('nextToken') is
+0003b1e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003b1f0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
+0003b200: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
+0003b210: 6e65 7874 546f 6b65 6e27 290a 2020 2020  nextToken').    
+0003b220: 2020 2020 6966 206d 2e67 6574 2827 7072      if m.get('pr
+0003b230: 6566 6978 2729 2069 7320 6e6f 7420 4e6f  efix') is not No
+0003b240: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003b250: 7365 6c66 2e70 7265 6669 7820 3d20 6d2e  self.prefix = m.
+0003b260: 6765 7428 2770 7265 6669 7827 290a 2020  get('prefix').  
+0003b270: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0003b280: 660a 0a0a 636c 6173 7320 4c69 7374 4675  f...class ListFu
+0003b290: 6e63 7469 6f6e 7352 6573 706f 6e73 6528  nctionsResponse(
+0003b2a0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+0003b2b0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0003b2c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0003b2d0: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
+0003b2e0: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+0003b2f0: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
+0003b300: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
+0003b310: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+0003b320: 3a20 4c69 7374 4675 6e63 7469 6f6e 734f  : ListFunctionsO
+0003b330: 7574 7075 7420 3d20 4e6f 6e65 2c0a 2020  utput = None,.  
+0003b340: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+0003b350: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+0003b360: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+0003b370: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+0003b380: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+0003b390: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+0003b3a0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+0003b3b0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0003b3c0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+0003b3d0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+0003b3e0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+0003b3f0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+0003b400: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0003b410: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0003b420: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0003b430: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0003b440: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003b450: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0003b460: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0003b470: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0003b480: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+0003b490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003b4a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003b4b0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+0003b4c0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+0003b4d0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+0003b4e0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+0003b4f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003b500: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+0003b510: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+0003b520: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+0003b530: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+0003b540: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003b550: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+0003b560: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+0003b570: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0003b580: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0003b590: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0003b5a0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+0003b5b0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0003b5c0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0003b5d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003b5e0: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+0003b5f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003b600: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+0003b610: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+0003b620: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+0003b630: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+0003b640: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+0003b650: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003b660: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+0003b670: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+0003b680: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+0003b690: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+0003b6a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003b6b0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+0003b6c0: 6c20 3d20 4c69 7374 4675 6e63 7469 6f6e  l = ListFunction
+0003b6d0: 734f 7574 7075 7428 290a 2020 2020 2020  sOutput().      
+0003b6e0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0003b6f0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+0003b700: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+0003b710: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003b720: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+0003b730: 7449 6e73 7461 6e63 6573 5265 7175 6573  tInstancesReques
+0003b740: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+0003b750: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0003b760: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0003b770: 2020 2020 2071 7561 6c69 6669 6572 3a20       qualifier: 
+0003b780: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0003b790: 2020 2020 7769 7468 5f61 6c6c 5f61 6374      with_all_act
+0003b7a0: 6976 653a 2062 6f6f 6c20 3d20 4e6f 6e65  ive: bool = None
+0003b7b0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0003b7c0: 2023 2054 6865 2066 756e 6374 696f 6e20   # The function 
+0003b7d0: 7665 7273 696f 6e20 6f72 2061 6c69 6173  version or alias
+0003b7e0: 2e0a 2020 2020 2020 2020 7365 6c66 2e71  ..        self.q
+0003b7f0: 7561 6c69 6669 6572 203d 2071 7561 6c69  ualifier = quali
+0003b800: 6669 6572 0a20 2020 2020 2020 2023 2053  fier.        # S
+0003b810: 7065 6369 6669 6573 2077 6865 7468 6572  pecifies whether
+0003b820: 2074 6f20 6c69 7374 2061 6c6c 2069 6e73   to list all ins
+0003b830: 7461 6e63 6573 2e20 5661 6c69 6420 7661  tances. Valid va
+0003b840: 6c75 6573 3a20 7472 7565 2061 6e64 2066  lues: true and f
+0003b850: 616c 7365 2e0a 2020 2020 2020 2020 7365  alse..        se
+0003b860: 6c66 2e77 6974 685f 616c 6c5f 6163 7469  lf.with_all_acti
+0003b870: 7665 203d 2077 6974 685f 616c 6c5f 6163  ve = with_all_ac
+0003b880: 7469 7665 0a0a 2020 2020 6465 6620 7661  tive..    def va
+0003b890: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0003b8a0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0003b8b0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0003b8c0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0003b8d0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+0003b8e0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0003b8f0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0003b900: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0003b910: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0003b920: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0003b930: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003b940: 7175 616c 6966 6965 7220 6973 206e 6f74  qualifier is not
+0003b950: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003b960: 2020 2072 6573 756c 745b 2771 7561 6c69     result['quali
+0003b970: 6669 6572 275d 203d 2073 656c 662e 7175  fier'] = self.qu
+0003b980: 616c 6966 6965 720a 2020 2020 2020 2020  alifier.        
+0003b990: 6966 2073 656c 662e 7769 7468 5f61 6c6c  if self.with_all
+0003b9a0: 5f61 6374 6976 6520 6973 206e 6f74 204e  _active is not N
+0003b9b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003b9c0: 2072 6573 756c 745b 2777 6974 6841 6c6c   result['withAll
+0003b9d0: 4163 7469 7665 275d 203d 2073 656c 662e  Active'] = self.
+0003b9e0: 7769 7468 5f61 6c6c 5f61 6374 6976 650a  with_all_active.
+0003b9f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003ba00: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003ba10: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0003ba20: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0003ba30: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003ba40: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003ba50: 6620 6d2e 6765 7428 2771 7561 6c69 6669  f m.get('qualifi
+0003ba60: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
+0003ba70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003ba80: 6c66 2e71 7561 6c69 6669 6572 203d 206d  lf.qualifier = m
+0003ba90: 2e67 6574 2827 7175 616c 6966 6965 7227  .get('qualifier'
+0003baa0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003bab0: 6574 2827 7769 7468 416c 6c41 6374 6976  et('withAllActiv
+0003bac0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0003bad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003bae0: 662e 7769 7468 5f61 6c6c 5f61 6374 6976  f.with_all_activ
+0003baf0: 6520 3d20 6d2e 6765 7428 2777 6974 6841  e = m.get('withA
+0003bb00: 6c6c 4163 7469 7665 2729 0a20 2020 2020  llActive').     
+0003bb10: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0003bb20: 0a63 6c61 7373 204c 6973 7449 6e73 7461  .class ListInsta
+0003bb30: 6e63 6573 5265 7370 6f6e 7365 2854 6561  ncesResponse(Tea
+0003bb40: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0003bb50: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0003bb60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0003bb70: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+0003bb80: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+0003bb90: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+0003bba0: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+0003bbb0: 0a20 2020 2020 2020 2062 6f64 793a 204c  .        body: L
+0003bbc0: 6973 7449 6e73 7461 6e63 6573 4f75 7470  istInstancesOutp
+0003bbd0: 7574 203d 204e 6f6e 652c 0a20 2020 2029  ut = None,.    )
+0003bbe0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+0003bbf0: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+0003bc00: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0003bc10: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+0003bc20: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+0003bc30: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+0003bc40: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0003bc50: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0003bc60: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+0003bc70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003bc80: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+0003bc90: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0003bca0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0003bcb0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0003bcc0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0003bcd0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0003bce0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003bcf0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0003bd00: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0003bd10: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0003bd20: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+0003bd30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003bd40: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+0003bd50: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+0003bd60: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+0003bd70: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+0003bd80: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+0003bd90: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0003bda0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+0003bdb0: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+0003bdc0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
+0003bdd0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+0003bde0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003bdf0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
+0003be00: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
+0003be10: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
+0003be20: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+0003be30: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+0003be40: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+0003be50: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0003be60: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0003be70: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003be80: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+0003be90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003bea0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0003beb0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+0003bec0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003bed0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0003bee0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003bef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003bf00: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+0003bf10: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0003bf20: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003bf30: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+0003bf40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003bf50: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+0003bf60: 204c 6973 7449 6e73 7461 6e63 6573 4f75   ListInstancesOu
+0003bf70: 7470 7574 2829 0a20 2020 2020 2020 2020  tput().         
+0003bf80: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0003bf90: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0003bfa0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0003bfb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0003bfc0: 660a 0a0a 636c 6173 7320 4c69 7374 4c61  f...class ListLa
+0003bfd0: 7965 7256 6572 7369 6f6e 7352 6571 7565  yerVersionsReque
+0003bfe0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+0003bff0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0003c000: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0003c010: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
+0003c020: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0003c030: 2073 7461 7274 5f76 6572 7369 6f6e 3a20   start_version: 
+0003c040: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0003c050: 293a 0a20 2020 2020 2020 2023 2054 6865  ):.        # The
+0003c060: 206e 756d 6265 7220 6f66 2076 6572 7369   number of versi
+0003c070: 6f6e 7320 746f 2062 6520 7265 7475 726e  ons to be return
+0003c080: 6564 2e0a 2020 2020 2020 2020 7365 6c66  ed..        self
+0003c090: 2e6c 696d 6974 203d 206c 696d 6974 0a20  .limit = limit. 
+0003c0a0: 2020 2020 2020 2023 2054 6865 2069 6e69         # The ini
+0003c0b0: 7469 616c 2076 6572 7369 6f6e 206f 6620  tial version of 
+0003c0c0: 7468 6520 6c61 7965 722e 0a20 2020 2020  the layer..     
+0003c0d0: 2020 2073 656c 662e 7374 6172 745f 7665     self.start_ve
+0003c0e0: 7273 696f 6e20 3d20 7374 6172 745f 7665  rsion = start_ve
+0003c0f0: 7273 696f 6e0a 0a20 2020 2064 6566 2076  rsion..    def v
+0003c100: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0003c110: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0003c120: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0003c130: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0003c140: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+0003c150: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0003c160: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0003c170: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0003c180: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0003c190: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0003c1a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003c1b0: 2e6c 696d 6974 2069 7320 6e6f 7420 4e6f  .limit is not No
+0003c1c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003c1d0: 7265 7375 6c74 5b27 6c69 6d69 7427 5d20  result['limit'] 
+0003c1e0: 3d20 7365 6c66 2e6c 696d 6974 0a20 2020  = self.limit.   
+0003c1f0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+0003c200: 7274 5f76 6572 7369 6f6e 2069 7320 6e6f  rt_version is no
+0003c210: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003c220: 2020 2020 7265 7375 6c74 5b27 7374 6172      result['star
+0003c230: 7456 6572 7369 6f6e 275d 203d 2073 656c  tVersion'] = sel
+0003c240: 662e 7374 6172 745f 7665 7273 696f 6e0a  f.start_version.
+0003c250: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003c260: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003c270: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0003c280: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0003c290: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003c2a0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003c2b0: 6620 6d2e 6765 7428 276c 696d 6974 2729  f m.get('limit')
+0003c2c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003c2d0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0003c2e0: 696d 6974 203d 206d 2e67 6574 2827 6c69  imit = m.get('li
+0003c2f0: 6d69 7427 290a 2020 2020 2020 2020 6966  mit').        if
+0003c300: 206d 2e67 6574 2827 7374 6172 7456 6572   m.get('startVer
+0003c310: 7369 6f6e 2729 2069 7320 6e6f 7420 4e6f  sion') is not No
+0003c320: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003c330: 7365 6c66 2e73 7461 7274 5f76 6572 7369  self.start_versi
+0003c340: 6f6e 203d 206d 2e67 6574 2827 7374 6172  on = m.get('star
+0003c350: 7456 6572 7369 6f6e 2729 0a20 2020 2020  tVersion').     
+0003c360: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0003c370: 0a63 6c61 7373 204c 6973 744c 6179 6572  .class ListLayer
+0003c380: 5665 7273 696f 6e73 5265 7370 6f6e 7365  VersionsResponse
+0003c390: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0003c3a0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0003c3b0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0003c3c0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+0003c3d0: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+0003c3e0: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+0003c3f0: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+0003c400: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+0003c410: 793a 204c 6973 744c 6179 6572 5665 7273  y: ListLayerVers
+0003c420: 696f 6e4f 7574 7075 7420 3d20 4e6f 6e65  ionOutput = None
+0003c430: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0003c440: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+0003c450: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+0003c460: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0003c470: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
+0003c480: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0003c490: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
+0003c4a0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0003c4b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003c4c0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0003c4d0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0003c4e0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0003c4f0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0003c500: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0003c510: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0003c520: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0003c530: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003c540: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0003c550: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0003c560: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0003c570: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+0003c580: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+0003c590: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003c5a0: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+0003c5b0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+0003c5c0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0003c5d0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+0003c5e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003c5f0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+0003c600: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+0003c610: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0003c620: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0003c630: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003c640: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003c650: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+0003c660: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+0003c670: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0003c680: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0003c690: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+0003c6a0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+0003c6b0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0003c6c0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0003c6d0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0003c6e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003c6f0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0003c700: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+0003c710: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0003c720: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+0003c730: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+0003c740: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003c750: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0003c760: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+0003c770: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+0003c780: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+0003c790: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003c7a0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0003c7b0: 6d6f 6465 6c20 3d20 4c69 7374 4c61 7965  model = ListLaye
+0003c7c0: 7256 6572 7369 6f6e 4f75 7470 7574 2829  rVersionOutput()
+0003c7d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003c7e0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+0003c7f0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+0003c800: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+0003c810: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0003c820: 6173 7320 4c69 7374 4c61 7965 7273 5265  ass ListLayersRe
+0003c830: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+0003c840: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0003c850: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0003c860: 0a20 2020 2020 2020 206c 696d 6974 3a20  .        limit: 
+0003c870: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+0003c880: 2020 2020 6e65 7874 5f74 6f6b 656e 3a20      next_token: 
+0003c890: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0003c8a0: 2020 2020 6f66 6669 6369 616c 3a20 7374      official: st
+0003c8b0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0003c8c0: 2020 7072 6566 6978 3a20 7374 7220 3d20    prefix: str = 
+0003c8d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7075  None,.        pu
+0003c8e0: 626c 6963 3a20 7374 7220 3d20 4e6f 6e65  blic: str = None
+0003c8f0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0003c900: 2023 2054 6865 206e 756d 6265 7220 6f66   # The number of
+0003c910: 206c 6179 6572 7320 7468 6174 2061 7265   layers that are
+0003c920: 2072 6574 7572 6e65 640a 2020 2020 2020   returned.      
+0003c930: 2020 7365 6c66 2e6c 696d 6974 203d 206c    self.limit = l
+0003c940: 696d 6974 0a20 2020 2020 2020 2023 2054  imit.        # T
+0003c950: 6865 2070 6167 696e 6174 696f 6e20 746f  he pagination to
+0003c960: 6b65 6e20 7468 6174 2069 7320 7573 6564  ken that is used
+0003c970: 2069 6e20 7468 6520 6e65 7874 2072 6571   in the next req
+0003c980: 7565 7374 2074 6f20 7265 7472 6965 7665  uest to retrieve
+0003c990: 2061 206e 6577 2070 6167 6520 6f66 2072   a new page of r
+0003c9a0: 6573 756c 7473 2e0a 2020 2020 2020 2020  esults..        
+0003c9b0: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
+0003c9c0: 3d20 6e65 7874 5f74 6f6b 656e 0a20 2020  = next_token.   
+0003c9d0: 2020 2020 2023 2053 7065 6369 6669 6573       # Specifies
+0003c9e0: 2077 6865 7468 6572 2074 6865 206c 6179   whether the lay
+0003c9f0: 6572 2069 7320 6f66 6669 6369 616c 2e20  er is official. 
+0003ca00: 5661 6c69 6420 7661 6c75 6573 3a20 7472  Valid values: tr
+0003ca10: 7565 2061 6e64 2066 616c 7365 2e0a 2020  ue and false..  
+0003ca20: 2020 2020 2020 7365 6c66 2e6f 6666 6963        self.offic
+0003ca30: 6961 6c20 3d20 6f66 6669 6369 616c 0a20  ial = official. 
+0003ca40: 2020 2020 2020 2023 2054 6865 206e 616d         # The nam
+0003ca50: 6520 7072 6566 6978 206f 6620 7468 6520  e prefix of the 
+0003ca60: 6c61 7965 722e 0a20 2020 2020 2020 2073  layer..        s
+0003ca70: 656c 662e 7072 6566 6978 203d 2070 7265  elf.prefix = pre
+0003ca80: 6669 780a 2020 2020 2020 2020 2320 5370  fix.        # Sp
+0003ca90: 6563 6966 6965 7320 7768 6574 6865 7220  ecifies whether 
+0003caa0: 7468 6520 6c61 7965 7220 6973 2070 7562  the layer is pub
+0003cab0: 6c69 632e 2056 616c 6964 2076 616c 7565  lic. Valid value
+0003cac0: 733a 2074 7275 6520 616e 6420 6661 6c73  s: true and fals
+0003cad0: 652e 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+0003cae0: 7075 626c 6963 203d 2070 7562 6c69 630a  public = public.
+0003caf0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0003cb00: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0003cb10: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+0003cb20: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0003cb30: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0003cb40: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+0003cb50: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0003cb60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003cb70: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0003cb80: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0003cb90: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0003cba0: 2020 2069 6620 7365 6c66 2e6c 696d 6974     if self.limit
+0003cbb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003cbc0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003cbd0: 5b27 6c69 6d69 7427 5d20 3d20 7365 6c66  ['limit'] = self
+0003cbe0: 2e6c 696d 6974 0a20 2020 2020 2020 2069  .limit.        i
+0003cbf0: 6620 7365 6c66 2e6e 6578 745f 746f 6b65  f self.next_toke
+0003cc00: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+0003cc10: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003cc20: 745b 276e 6578 7454 6f6b 656e 275d 203d  t['nextToken'] =
+0003cc30: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003cc40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003cc50: 2e6f 6666 6963 6961 6c20 6973 206e 6f74  .official is not
+0003cc60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003cc70: 2020 2072 6573 756c 745b 276f 6666 6963     result['offic
+0003cc80: 6961 6c27 5d20 3d20 7365 6c66 2e6f 6666  ial'] = self.off
+0003cc90: 6963 6961 6c0a 2020 2020 2020 2020 6966  icial.        if
+0003cca0: 2073 656c 662e 7072 6566 6978 2069 7320   self.prefix is 
+0003ccb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003ccc0: 2020 2020 2020 7265 7375 6c74 5b27 7072        result['pr
+0003ccd0: 6566 6978 275d 203d 2073 656c 662e 7072  efix'] = self.pr
+0003cce0: 6566 6978 0a20 2020 2020 2020 2069 6620  efix.        if 
+0003ccf0: 7365 6c66 2e70 7562 6c69 6320 6973 206e  self.public is n
+0003cd00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003cd10: 2020 2020 2072 6573 756c 745b 2770 7562       result['pub
+0003cd20: 6c69 6327 5d20 3d20 7365 6c66 2e70 7562  lic'] = self.pub
+0003cd30: 6c69 630a 2020 2020 2020 2020 7265 7475  lic.        retu
+0003cd40: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0003cd50: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0003cd60: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0003cd70: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0003cd80: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0003cd90: 2020 2069 6620 6d2e 6765 7428 276c 696d     if m.get('lim
+0003cda0: 6974 2729 2069 7320 6e6f 7420 4e6f 6e65  it') is not None
+0003cdb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003cdc0: 6c66 2e6c 696d 6974 203d 206d 2e67 6574  lf.limit = m.get
+0003cdd0: 2827 6c69 6d69 7427 290a 2020 2020 2020  ('limit').      
+0003cde0: 2020 6966 206d 2e67 6574 2827 6e65 7874    if m.get('next
+0003cdf0: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
+0003ce00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003ce10: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003ce20: 203d 206d 2e67 6574 2827 6e65 7874 546f   = m.get('nextTo
+0003ce30: 6b65 6e27 290a 2020 2020 2020 2020 6966  ken').        if
+0003ce40: 206d 2e67 6574 2827 6f66 6669 6369 616c   m.get('official
+0003ce50: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003ce60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003ce70: 2e6f 6666 6963 6961 6c20 3d20 6d2e 6765  .official = m.ge
+0003ce80: 7428 276f 6666 6963 6961 6c27 290a 2020  t('official').  
+0003ce90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003cea0: 7072 6566 6978 2729 2069 7320 6e6f 7420  prefix') is not 
+0003ceb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003cec0: 2020 7365 6c66 2e70 7265 6669 7820 3d20    self.prefix = 
+0003ced0: 6d2e 6765 7428 2770 7265 6669 7827 290a  m.get('prefix').
+0003cee0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0003cef0: 2827 7075 626c 6963 2729 2069 7320 6e6f  ('public') is no
+0003cf00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003cf10: 2020 2020 7365 6c66 2e70 7562 6c69 6320      self.public 
+0003cf20: 3d20 6d2e 6765 7428 2770 7562 6c69 6327  = m.get('public'
+0003cf30: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0003cf40: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
+0003cf50: 7374 4c61 7965 7273 5265 7370 6f6e 7365  stLayersResponse
+0003cf60: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0003cf70: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0003cf80: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0003cf90: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+0003cfa0: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+0003cfb0: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+0003cfc0: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+0003cfd0: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+0003cfe0: 793a 204c 6973 744c 6179 6572 734f 7574  y: ListLayersOut
+0003cff0: 7075 7420 3d20 4e6f 6e65 2c0a 2020 2020  put = None,.    
+0003d000: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0003d010: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+0003d020: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+0003d030: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+0003d040: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+0003d050: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+0003d060: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+0003d070: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0003d080: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+0003d090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003d0a0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+0003d0b0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+0003d0c0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0003d0d0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+0003d0e0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003d0f0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0003d100: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003d110: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0003d120: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0003d130: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003d140: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+0003d150: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003d160: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003d170: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+0003d180: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+0003d190: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+0003d1a0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+0003d1b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003d1c0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+0003d1d0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+0003d1e0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+0003d1f0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+0003d200: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003d210: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+0003d220: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+0003d230: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0003d240: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0003d250: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0003d260: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+0003d270: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0003d280: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0003d290: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003d2a0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+0003d2b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003d2c0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0003d2d0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+0003d2e0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0003d2f0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0003d300: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003d310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003d320: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+0003d330: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0003d340: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003d350: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+0003d360: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003d370: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0003d380: 3d20 4c69 7374 4c61 7965 7273 4f75 7470  = ListLayersOutp
+0003d390: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+0003d3a0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+0003d3b0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+0003d3c0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+0003d3d0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0003d3e0: 0a0a 636c 6173 7320 4c69 7374 5072 6f76  ..class ListProv
+0003d3f0: 6973 696f 6e43 6f6e 6669 6773 5265 7175  isionConfigsRequ
+0003d400: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+0003d410: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0003d420: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0003d430: 2020 2020 2020 2066 756e 6374 696f 6e5f         function_
+0003d440: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
+0003d450: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
+0003d460: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+0003d470: 2020 2020 206e 6578 745f 746f 6b65 6e3a       next_token:
+0003d480: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0003d490: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
+0003d4a0: 6520 6e61 6d65 206f 6620 7468 6520 6675  e name of the fu
+0003d4b0: 6e63 7469 6f6e 2e20 4966 2074 6869 7320  nction. If this 
+0003d4c0: 7061 7261 6d65 7465 7220 6973 206e 6f74  parameter is not
+0003d4d0: 2073 7065 6369 6669 6564 2c20 7468 6520   specified, the 
+0003d4e0: 7072 6f76 6973 696f 6e65 6420 636f 6e66  provisioned conf
+0003d4f0: 6967 7572 6174 696f 6e73 206f 6620 616c  igurations of al
+0003d500: 6c20 6675 6e63 7469 6f6e 7320 6172 6520  l functions are 
+0003d510: 6c69 7374 6564 2e0a 2020 2020 2020 2020  listed..        
+0003d520: 7365 6c66 2e66 756e 6374 696f 6e5f 6e61  self.function_na
+0003d530: 6d65 203d 2066 756e 6374 696f 6e5f 6e61  me = function_na
+0003d540: 6d65 0a20 2020 2020 2020 2023 204e 756d  me.        # Num
+0003d550: 6265 7220 6f66 2070 726f 7669 7369 6f6e  ber of provision
+0003d560: 6564 2063 6f6e 6669 6775 7261 7469 6f6e  ed configuration
+0003d570: 7320 746f 2072 6574 7572 6e2e 0a20 2020  s to return..   
+0003d580: 2020 2020 2073 656c 662e 6c69 6d69 7420       self.limit 
+0003d590: 3d20 6c69 6d69 740a 2020 2020 2020 2020  = limit.        
+0003d5a0: 2320 4120 7061 6769 6e61 7469 6f6e 2074  # A pagination t
+0003d5b0: 6f6b 656e 2e0a 2020 2020 2020 2020 7365  oken..        se
+0003d5c0: 6c66 2e6e 6578 745f 746f 6b65 6e20 3d20  lf.next_token = 
+0003d5d0: 6e65 7874 5f74 6f6b 656e 0a0a 2020 2020  next_token..    
+0003d5e0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0003d5f0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0003d600: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0003d610: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0003d620: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0003d630: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0003d640: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0003d650: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003d660: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0003d670: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0003d680: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0003d690: 2073 656c 662e 6675 6e63 7469 6f6e 5f6e   self.function_n
+0003d6a0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+0003d6b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0003d6c0: 756c 745b 2766 756e 6374 696f 6e4e 616d  ult['functionNam
+0003d6d0: 6527 5d20 3d20 7365 6c66 2e66 756e 6374  e'] = self.funct
+0003d6e0: 696f 6e5f 6e61 6d65 0a20 2020 2020 2020  ion_name.       
+0003d6f0: 2069 6620 7365 6c66 2e6c 696d 6974 2069   if self.limit i
+0003d700: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003d710: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003d720: 6c69 6d69 7427 5d20 3d20 7365 6c66 2e6c  limit'] = self.l
+0003d730: 696d 6974 0a20 2020 2020 2020 2069 6620  imit.        if 
+0003d740: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
+0003d750: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003d760: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0003d770: 276e 6578 7454 6f6b 656e 275d 203d 2073  'nextToken'] = s
+0003d780: 656c 662e 6e65 7874 5f74 6f6b 656e 0a20  elf.next_token. 
+0003d790: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0003d7a0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0003d7b0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0003d7c0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0003d7d0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0003d7e0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0003d7f0: 206d 2e67 6574 2827 6675 6e63 7469 6f6e   m.get('function
+0003d800: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
+0003d810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003d820: 7365 6c66 2e66 756e 6374 696f 6e5f 6e61  self.function_na
+0003d830: 6d65 203d 206d 2e67 6574 2827 6675 6e63  me = m.get('func
+0003d840: 7469 6f6e 4e61 6d65 2729 0a20 2020 2020  tionName').     
+0003d850: 2020 2069 6620 6d2e 6765 7428 276c 696d     if m.get('lim
+0003d860: 6974 2729 2069 7320 6e6f 7420 4e6f 6e65  it') is not None
+0003d870: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0003d880: 6c66 2e6c 696d 6974 203d 206d 2e67 6574  lf.limit = m.get
+0003d890: 2827 6c69 6d69 7427 290a 2020 2020 2020  ('limit').      
+0003d8a0: 2020 6966 206d 2e67 6574 2827 6e65 7874    if m.get('next
+0003d8b0: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
+0003d8c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003d8d0: 2073 656c 662e 6e65 7874 5f74 6f6b 656e   self.next_token
+0003d8e0: 203d 206d 2e67 6574 2827 6e65 7874 546f   = m.get('nextTo
+0003d8f0: 6b65 6e27 290a 2020 2020 2020 2020 7265  ken').        re
+0003d900: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003d910: 7320 4c69 7374 5072 6f76 6973 696f 6e43  s ListProvisionC
+0003d920: 6f6e 6669 6773 5265 7370 6f6e 7365 2854  onfigsResponse(T
+0003d930: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0003d940: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0003d950: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0003d960: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+0003d970: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+0003d980: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+0003d990: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+0003d9a0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+0003d9b0: 204c 6973 7450 726f 7669 7369 6f6e 436f   ListProvisionCo
+0003d9c0: 6e66 6967 734f 7574 7075 7420 3d20 4e6f  nfigsOutput = No
+0003d9d0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0003d9e0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0003d9f0: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
+0003da00: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0003da10: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+0003da20: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+0003da30: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
+0003da40: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0003da50: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+0003da60: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+0003da70: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+0003da80: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+0003da90: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0003daa0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0003dab0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0003dac0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0003dad0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003dae0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0003daf0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0003db00: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0003db10: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0003db20: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0003db30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003db40: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0003db50: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0003db60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003db70: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0003db80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003db90: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0003dba0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0003dbb0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0003dbc0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0003dbd0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0003dbe0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003dbf0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0003dc00: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0003dc10: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003dc20: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003dc30: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0003dc40: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0003dc50: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003dc60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003dc70: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+0003dc80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003dc90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003dca0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+0003dcb0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+0003dcc0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+0003dcd0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+0003dce0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003dcf0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0003dd00: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+0003dd10: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+0003dd20: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+0003dd30: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0003dd40: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0003dd50: 705f 6d6f 6465 6c20 3d20 4c69 7374 5072  p_model = ListPr
+0003dd60: 6f76 6973 696f 6e43 6f6e 6669 6773 4f75  ovisionConfigsOu
+0003dd70: 7470 7574 2829 0a20 2020 2020 2020 2020  tput().         
+0003dd80: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0003dd90: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0003dda0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0003ddb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0003ddc0: 660a 0a0a 636c 6173 7320 4c69 7374 5461  f...class ListTa
+0003ddd0: 6752 6573 6f75 7263 6573 5265 7175 6573  gResourcesReques
+0003dde0: 7454 6167 2854 6561 4d6f 6465 6c29 3a0a  tTag(TeaModel):.
+0003ddf0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0003de00: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0003de10: 2020 2020 2020 2020 6b65 793a 2073 7472          key: str
+0003de20: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0003de30: 2076 616c 7565 3a20 7374 7220 3d20 4e6f   value: str = No
+0003de40: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0003de50: 2020 2023 2054 6865 2074 6167 206b 6579     # The tag key
+0003de60: 2e0a 2020 2020 2020 2020 2320 0a20 2020  ..        # .   
+0003de70: 2020 2020 2023 2054 6865 2074 6167 206b       # The tag k
+0003de80: 6579 2063 616e 2062 6520 7570 2074 6f20  ey can be up to 
+0003de90: 3634 2063 6861 7261 6374 6572 7320 696e  64 characters in
+0003dea0: 206c 656e 6774 682c 2061 6e64 2063 616e   length, and can
+0003deb0: 6e6f 7420 636f 6e74 6169 6e20 6068 7474  not contain `htt
+0003dec0: 703a 2f2f 6020 6f72 2060 6874 7470 733a  p://` or `https:
+0003ded0: 2f2f 602e 2054 6865 2074 6167 206b 6579  //`. The tag key
+0003dee0: 2063 616e 6e6f 7420 7374 6172 7420 7769   cannot start wi
+0003def0: 7468 2060 616c 6979 756e 6020 6f72 2060  th `aliyun` or `
+0003df00: 6163 733a 602e 0a20 2020 2020 2020 2073  acs:`..        s
+0003df10: 656c 662e 6b65 7920 3d20 6b65 790a 2020  elf.key = key.  
+0003df20: 2020 2020 2020 2320 5468 6520 7461 6720        # The tag 
+0003df30: 7661 6c75 652e 0a20 2020 2020 2020 2023  value..        #
+0003df40: 200a 2020 2020 2020 2020 2320 5468 6520   .        # The 
+0003df50: 7461 6720 7661 6c75 6520 6361 6e20 6265  tag value can be
+0003df60: 2075 7020 746f 2031 3238 2063 6861 7261   up to 128 chara
+0003df70: 6374 6572 7320 696e 206c 656e 6774 6820  cters in length 
+0003df80: 616e 6420 6361 6e20 6265 2061 6e20 656d  and can be an em
+0003df90: 7074 7920 7374 7269 6e67 2e0a 2020 2020  pty string..    
+0003dfa0: 2020 2020 7365 6c66 2e76 616c 7565 203d      self.value =
+0003dfb0: 2076 616c 7565 0a0a 2020 2020 6465 6620   value..    def 
+0003dfc0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0003dfd0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0003dfe0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0003dff0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0003e000: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+0003e010: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+0003e020: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+0003e030: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0003e040: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+0003e050: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+0003e060: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0003e070: 662e 6b65 7920 6973 206e 6f74 204e 6f6e  f.key is not Non
+0003e080: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003e090: 6573 756c 745b 274b 6579 275d 203d 2073  esult['Key'] = s
+0003e0a0: 656c 662e 6b65 790a 2020 2020 2020 2020  elf.key.        
+0003e0b0: 6966 2073 656c 662e 7661 6c75 6520 6973  if self.value is
+0003e0c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003e0d0: 2020 2020 2020 2072 6573 756c 745b 2756         result['V
+0003e0e0: 616c 7565 275d 203d 2073 656c 662e 7661  alue'] = self.va
+0003e0f0: 6c75 650a 2020 2020 2020 2020 7265 7475  lue.        retu
+0003e100: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0003e110: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0003e120: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0003e130: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0003e140: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0003e150: 2020 2069 6620 6d2e 6765 7428 274b 6579     if m.get('Key
+0003e160: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003e170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003e180: 2e6b 6579 203d 206d 2e67 6574 2827 4b65  .key = m.get('Ke
+0003e190: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
+0003e1a0: 2e67 6574 2827 5661 6c75 6527 2920 6973  .get('Value') is
+0003e1b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003e1c0: 2020 2020 2020 2073 656c 662e 7661 6c75         self.valu
+0003e1d0: 6520 3d20 6d2e 6765 7428 2756 616c 7565  e = m.get('Value
+0003e1e0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0003e1f0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
+0003e200: 6973 7454 6167 5265 736f 7572 6365 7352  istTagResourcesR
+0003e210: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+0003e220: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0003e230: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0003e240: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
+0003e250: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+0003e260: 2020 2020 206e 6578 745f 746f 6b65 6e3a       next_token:
+0003e270: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0003e280: 2020 2020 2072 6573 6f75 7263 655f 6964       resource_id
+0003e290: 3a20 4c69 7374 5b73 7472 5d20 3d20 4e6f  : List[str] = No
+0003e2a0: 6e65 2c0a 2020 2020 2020 2020 7265 736f  ne,.        reso
+0003e2b0: 7572 6365 5f74 7970 653a 2073 7472 203d  urce_type: str =
+0003e2c0: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+0003e2d0: 6167 3a20 4c69 7374 5b4c 6973 7454 6167  ag: List[ListTag
+0003e2e0: 5265 736f 7572 6365 7352 6571 7565 7374  ResourcesRequest
+0003e2f0: 5461 675d 203d 204e 6f6e 652c 0a20 2020  Tag] = None,.   
+0003e300: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
+0003e310: 6520 6e75 6d62 6572 206f 6620 7265 736f  e number of reso
+0003e320: 7572 6365 7320 746f 2072 6574 7572 6e2e  urces to return.
+0003e330: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+0003e340: 6d69 7420 3d20 6c69 6d69 740a 2020 2020  mit = limit.    
+0003e350: 2020 2020 2320 5468 6520 7061 6769 6e61      # The pagina
+0003e360: 7469 6f6e 2074 6f6b 656e 2074 6861 7420  tion token that 
+0003e370: 6973 2075 7365 6420 696e 2074 6865 206e  is used in the n
+0003e380: 6578 7420 7265 7175 6573 7420 746f 2072  ext request to r
+0003e390: 6574 7269 6576 6520 6120 6e65 7720 7061  etrieve a new pa
+0003e3a0: 6765 206f 6620 7265 7375 6c74 732e 0a20  ge of results.. 
+0003e3b0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
+0003e3c0: 5f74 6f6b 656e 203d 206e 6578 745f 746f  _token = next_to
+0003e3d0: 6b65 6e0a 2020 2020 2020 2020 2320 5468  ken.        # Th
+0003e3e0: 6520 7265 736f 7572 6365 2049 4473 2e0a  e resource IDs..
+0003e3f0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+0003e400: 6f75 7263 655f 6964 203d 2072 6573 6f75  ource_id = resou
+0003e410: 7263 655f 6964 0a20 2020 2020 2020 2023  rce_id.        #
+0003e420: 2054 6865 2072 6573 6f75 7263 6520 7479   The resource ty
+0003e430: 7065 2e0a 2020 2020 2020 2020 7365 6c66  pe..        self
+0003e440: 2e72 6573 6f75 7263 655f 7479 7065 203d  .resource_type =
+0003e450: 2072 6573 6f75 7263 655f 7479 7065 0a20   resource_type. 
+0003e460: 2020 2020 2020 2023 2054 6865 2074 6167         # The tag
+0003e470: 732e 0a20 2020 2020 2020 2023 200a 2020  s..        # .  
+0003e480: 2020 2020 2020 2320 596f 7520 6361 6e20        # You can 
+0003e490: 7175 6572 7920 7570 2074 6f20 3230 2074  query up to 20 t
+0003e4a0: 6167 7320 6174 2061 2074 696d 652e 0a20  ags at a time.. 
+0003e4b0: 2020 2020 2020 2073 656c 662e 7461 6720         self.tag 
+0003e4c0: 3d20 7461 670a 0a20 2020 2064 6566 2076  = tag..    def v
+0003e4d0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0003e4e0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+0003e4f0: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+0003e500: 666f 7220 6b20 696e 2073 656c 662e 7461  for k in self.ta
+0003e510: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+0003e520: 2020 2069 6620 6b3a 0a20 2020 2020 2020     if k:.       
+0003e530: 2020 2020 2020 2020 2020 2020 206b 2e76               k.v
+0003e540: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+0003e550: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0003e560: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0003e570: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0003e580: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0003e590: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003e5a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0003e5b0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0003e5c0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0003e5d0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+0003e5e0: 696d 6974 2069 7320 6e6f 7420 4e6f 6e65  imit is not None
+0003e5f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003e600: 7375 6c74 5b27 4c69 6d69 7427 5d20 3d20  sult['Limit'] = 
+0003e610: 7365 6c66 2e6c 696d 6974 0a20 2020 2020  self.limit.     
+0003e620: 2020 2069 6620 7365 6c66 2e6e 6578 745f     if self.next_
+0003e630: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+0003e640: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003e650: 6573 756c 745b 274e 6578 7454 6f6b 656e  esult['NextToken
+0003e660: 275d 203d 2073 656c 662e 6e65 7874 5f74  '] = self.next_t
+0003e670: 6f6b 656e 0a20 2020 2020 2020 2069 6620  oken.        if 
+0003e680: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
+0003e690: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003e6a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003e6b0: 5b27 5265 736f 7572 6365 4964 275d 203d  ['ResourceId'] =
+0003e6c0: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+0003e6d0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+0003e6e0: 662e 7265 736f 7572 6365 5f74 7970 6520  f.resource_type 
+0003e6f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003e700: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0003e710: 2752 6573 6f75 7263 6554 7970 6527 5d20  'ResourceType'] 
+0003e720: 3d20 7365 6c66 2e72 6573 6f75 7263 655f  = self.resource_
+0003e730: 7479 7065 0a20 2020 2020 2020 2072 6573  type.        res
+0003e740: 756c 745b 2754 6167 275d 203d 205b 5d0a  ult['Tag'] = [].
+0003e750: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003e760: 7461 6720 6973 206e 6f74 204e 6f6e 653a  tag is not None:
+0003e770: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0003e780: 206b 2069 6e20 7365 6c66 2e74 6167 3a0a   k in self.tag:.
+0003e790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e7a0: 7265 7375 6c74 5b27 5461 6727 5d2e 6170  result['Tag'].ap
+0003e7b0: 7065 6e64 286b 2e74 6f5f 6d61 7028 2920  pend(k.to_map() 
+0003e7c0: 6966 206b 2065 6c73 6520 4e6f 6e65 290a  if k else None).
+0003e7d0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003e7e0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003e7f0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0003e800: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0003e810: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003e820: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003e830: 6620 6d2e 6765 7428 274c 696d 6974 2729  f m.get('Limit')
+0003e840: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003e850: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0003e860: 696d 6974 203d 206d 2e67 6574 2827 4c69  imit = m.get('Li
+0003e870: 6d69 7427 290a 2020 2020 2020 2020 6966  mit').        if
+0003e880: 206d 2e67 6574 2827 4e65 7874 546f 6b65   m.get('NextToke
+0003e890: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+0003e8a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003e8b0: 662e 6e65 7874 5f74 6f6b 656e 203d 206d  f.next_token = m
+0003e8c0: 2e67 6574 2827 4e65 7874 546f 6b65 6e27  .get('NextToken'
+0003e8d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003e8e0: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
+0003e8f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003e900: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0003e910: 6573 6f75 7263 655f 6964 203d 206d 2e67  esource_id = m.g
+0003e920: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
+0003e930: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003e940: 7428 2752 6573 6f75 7263 6554 7970 6527  t('ResourceType'
+0003e950: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003e960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003e970: 7265 736f 7572 6365 5f74 7970 6520 3d20  resource_type = 
+0003e980: 6d2e 6765 7428 2752 6573 6f75 7263 6554  m.get('ResourceT
+0003e990: 7970 6527 290a 2020 2020 2020 2020 7365  ype').        se
+0003e9a0: 6c66 2e74 6167 203d 205b 5d0a 2020 2020  lf.tag = [].    
+0003e9b0: 2020 2020 6966 206d 2e67 6574 2827 5461      if m.get('Ta
+0003e9c0: 6727 2920 6973 206e 6f74 204e 6f6e 653a  g') is not None:
+0003e9d0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0003e9e0: 206b 2069 6e20 6d2e 6765 7428 2754 6167   k in m.get('Tag
+0003e9f0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0003ea00: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+0003ea10: 204c 6973 7454 6167 5265 736f 7572 6365   ListTagResource
+0003ea20: 7352 6571 7565 7374 5461 6728 290a 2020  sRequestTag().  
+0003ea30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0003ea40: 6c66 2e74 6167 2e61 7070 656e 6428 7465  lf.tag.append(te
+0003ea50: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+0003ea60: 7028 6b29 290a 2020 2020 2020 2020 7265  p(k)).        re
+0003ea70: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003ea80: 7320 4c69 7374 5461 6752 6573 6f75 7263  s ListTagResourc
+0003ea90: 6573 5368 7269 6e6b 5265 7175 6573 7428  esShrinkRequest(
+0003eaa0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+0003eab0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0003eac0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0003ead0: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
+0003eae0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6e65  None,.        ne
+0003eaf0: 7874 5f74 6f6b 656e 3a20 7374 7220 3d20  xt_token: str = 
+0003eb00: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
+0003eb10: 736f 7572 6365 5f69 645f 7368 7269 6e6b  source_id_shrink
+0003eb20: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0003eb30: 2020 2020 2020 7265 736f 7572 6365 5f74        resource_t
+0003eb40: 7970 653a 2073 7472 203d 204e 6f6e 652c  ype: str = None,
+0003eb50: 0a20 2020 2020 2020 2074 6167 5f73 6872  .        tag_shr
+0003eb60: 696e 6b3a 2073 7472 203d 204e 6f6e 652c  ink: str = None,
+0003eb70: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0003eb80: 2320 5468 6520 6e75 6d62 6572 206f 6620  # The number of 
+0003eb90: 7265 736f 7572 6365 7320 746f 2072 6574  resources to ret
+0003eba0: 7572 6e2e 0a20 2020 2020 2020 2073 656c  urn..        sel
+0003ebb0: 662e 6c69 6d69 7420 3d20 6c69 6d69 740a  f.limit = limit.
+0003ebc0: 2020 2020 2020 2020 2320 5468 6520 7061          # The pa
+0003ebd0: 6769 6e61 7469 6f6e 2074 6f6b 656e 2074  gination token t
+0003ebe0: 6861 7420 6973 2075 7365 6420 696e 2074  hat is used in t
+0003ebf0: 6865 206e 6578 7420 7265 7175 6573 7420  he next request 
+0003ec00: 746f 2072 6574 7269 6576 6520 6120 6e65  to retrieve a ne
+0003ec10: 7720 7061 6765 206f 6620 7265 7375 6c74  w page of result
+0003ec20: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+0003ec30: 6e65 7874 5f74 6f6b 656e 203d 206e 6578  next_token = nex
+0003ec40: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
+0003ec50: 2320 5468 6520 7265 736f 7572 6365 2049  # The resource I
+0003ec60: 4473 2e0a 2020 2020 2020 2020 7365 6c66  Ds..        self
+0003ec70: 2e72 6573 6f75 7263 655f 6964 5f73 6872  .resource_id_shr
+0003ec80: 696e 6b20 3d20 7265 736f 7572 6365 5f69  ink = resource_i
+0003ec90: 645f 7368 7269 6e6b 0a20 2020 2020 2020  d_shrink.       
+0003eca0: 2023 2054 6865 2072 6573 6f75 7263 6520   # The resource 
+0003ecb0: 7479 7065 2e0a 2020 2020 2020 2020 7365  type..        se
+0003ecc0: 6c66 2e72 6573 6f75 7263 655f 7479 7065  lf.resource_type
+0003ecd0: 203d 2072 6573 6f75 7263 655f 7479 7065   = resource_type
+0003ece0: 0a20 2020 2020 2020 2023 2054 6865 2074  .        # The t
+0003ecf0: 6167 732e 0a20 2020 2020 2020 2023 200a  ags..        # .
+0003ed00: 2020 2020 2020 2020 2320 596f 7520 6361          # You ca
+0003ed10: 6e20 7175 6572 7920 7570 2074 6f20 3230  n query up to 20
+0003ed20: 2074 6167 7320 6174 2061 2074 696d 652e   tags at a time.
+0003ed30: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0003ed40: 675f 7368 7269 6e6b 203d 2074 6167 5f73  g_shrink = tag_s
+0003ed50: 6872 696e 6b0a 0a20 2020 2064 6566 2076  hrink..    def v
+0003ed60: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0003ed70: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0003ed80: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0003ed90: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0003eda0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+0003edb0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0003edc0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0003edd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0003ede0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0003edf0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0003ee00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0003ee10: 2e6c 696d 6974 2069 7320 6e6f 7420 4e6f  .limit is not No
+0003ee20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003ee30: 7265 7375 6c74 5b27 4c69 6d69 7427 5d20  result['Limit'] 
+0003ee40: 3d20 7365 6c66 2e6c 696d 6974 0a20 2020  = self.limit.   
+0003ee50: 2020 2020 2069 6620 7365 6c66 2e6e 6578       if self.nex
+0003ee60: 745f 746f 6b65 6e20 6973 206e 6f74 204e  t_token is not N
+0003ee70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003ee80: 2072 6573 756c 745b 274e 6578 7454 6f6b   result['NextTok
+0003ee90: 656e 275d 203d 2073 656c 662e 6e65 7874  en'] = self.next
+0003eea0: 5f74 6f6b 656e 0a20 2020 2020 2020 2069  _token.        i
+0003eeb0: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
+0003eec0: 6964 5f73 6872 696e 6b20 6973 206e 6f74  id_shrink is not
+0003eed0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003eee0: 2020 2072 6573 756c 745b 2752 6573 6f75     result['Resou
+0003eef0: 7263 6549 6427 5d20 3d20 7365 6c66 2e72  rceId'] = self.r
+0003ef00: 6573 6f75 7263 655f 6964 5f73 6872 696e  esource_id_shrin
+0003ef10: 6b0a 2020 2020 2020 2020 6966 2073 656c  k.        if sel
+0003ef20: 662e 7265 736f 7572 6365 5f74 7970 6520  f.resource_type 
+0003ef30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003ef40: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0003ef50: 2752 6573 6f75 7263 6554 7970 6527 5d20  'ResourceType'] 
+0003ef60: 3d20 7365 6c66 2e72 6573 6f75 7263 655f  = self.resource_
+0003ef70: 7479 7065 0a20 2020 2020 2020 2069 6620  type.        if 
+0003ef80: 7365 6c66 2e74 6167 5f73 6872 696e 6b20  self.tag_shrink 
+0003ef90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003efa0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0003efb0: 2754 6167 275d 203d 2073 656c 662e 7461  'Tag'] = self.ta
+0003efc0: 675f 7368 7269 6e6b 0a20 2020 2020 2020  g_shrink.       
+0003efd0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0003efe0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0003eff0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+0003f000: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+0003f010: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+0003f020: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0003f030: 2827 4c69 6d69 7427 2920 6973 206e 6f74  ('Limit') is not
+0003f040: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003f050: 2020 2073 656c 662e 6c69 6d69 7420 3d20     self.limit = 
+0003f060: 6d2e 6765 7428 274c 696d 6974 2729 0a20  m.get('Limit'). 
+0003f070: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003f080: 274e 6578 7454 6f6b 656e 2729 2069 7320  'NextToken') is 
+0003f090: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003f0a0: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
+0003f0b0: 746f 6b65 6e20 3d20 6d2e 6765 7428 274e  token = m.get('N
+0003f0c0: 6578 7454 6f6b 656e 2729 0a20 2020 2020  extToken').     
+0003f0d0: 2020 2069 6620 6d2e 6765 7428 2752 6573     if m.get('Res
+0003f0e0: 6f75 7263 6549 6427 2920 6973 206e 6f74  ourceId') is not
+0003f0f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003f100: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+0003f110: 5f69 645f 7368 7269 6e6b 203d 206d 2e67  _id_shrink = m.g
+0003f120: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
+0003f130: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003f140: 7428 2752 6573 6f75 7263 6554 7970 6527  t('ResourceType'
+0003f150: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003f160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003f170: 7265 736f 7572 6365 5f74 7970 6520 3d20  resource_type = 
+0003f180: 6d2e 6765 7428 2752 6573 6f75 7263 6554  m.get('ResourceT
+0003f190: 7970 6527 290a 2020 2020 2020 2020 6966  ype').        if
+0003f1a0: 206d 2e67 6574 2827 5461 6727 2920 6973   m.get('Tag') is
+0003f1b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003f1c0: 2020 2020 2020 2073 656c 662e 7461 675f         self.tag_
+0003f1d0: 7368 7269 6e6b 203d 206d 2e67 6574 2827  shrink = m.get('
+0003f1e0: 5461 6727 290a 2020 2020 2020 2020 7265  Tag').        re
+0003f1f0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0003f200: 7320 4c69 7374 5461 6752 6573 6f75 7263  s ListTagResourc
+0003f210: 6573 5265 7370 6f6e 7365 2854 6561 4d6f  esResponse(TeaMo
+0003f220: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+0003f230: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0003f240: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+0003f250: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+0003f260: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+0003f270: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+0003f280: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+0003f290: 2020 2020 2020 2062 6f64 793a 204c 6973         body: Lis
+0003f2a0: 7454 6167 5265 736f 7572 6365 734f 7574  tTagResourcesOut
+0003f2b0: 7075 7420 3d20 4e6f 6e65 2c0a 2020 2020  put = None,.    
+0003f2c0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0003f2d0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+0003f2e0: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+0003f2f0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+0003f300: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+0003f310: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+0003f320: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+0003f330: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0003f340: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+0003f350: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003f360: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+0003f370: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+0003f380: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0003f390: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+0003f3a0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0003f3b0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0003f3c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003f3d0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0003f3e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0003f3f0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003f400: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+0003f410: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003f420: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003f430: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+0003f440: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+0003f450: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+0003f460: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+0003f470: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003f480: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+0003f490: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+0003f4a0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+0003f4b0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+0003f4c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003f4d0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+0003f4e0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+0003f4f0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0003f500: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0003f510: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0003f520: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+0003f530: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0003f540: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0003f550: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003f560: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+0003f570: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003f580: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0003f590: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+0003f5a0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0003f5b0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0003f5c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0003f5d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003f5e0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+0003f5f0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0003f600: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003f610: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+0003f620: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003f630: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0003f640: 3d20 4c69 7374 5461 6752 6573 6f75 7263  = ListTagResourc
+0003f650: 6573 4f75 7470 7574 2829 0a20 2020 2020  esOutput().     
+0003f660: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0003f670: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+0003f680: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+0003f690: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0003f6a0: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
+0003f6b0: 7374 5472 6967 6765 7273 5265 7175 6573  stTriggersReques
+0003f6c0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
 0003f6d0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
 0003f6e0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0003f6f0: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
-0003f700: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
-0003f710: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
-0003f720: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
-0003f730: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
-0003f740: 6479 3a20 4173 796e 6343 6f6e 6669 6720  dy: AsyncConfig 
-0003f750: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0003f760: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0003f770: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-0003f780: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0003f790: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0003f7a0: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-0003f7b0: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-0003f7c0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0003f7d0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0003f7e0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-0003f7f0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003f800: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-0003f810: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0003f820: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0003f830: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0003f840: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0003f850: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0003f860: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003f870: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0003f880: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0003f890: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0003f8a0: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-0003f8b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003f8c0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-0003f8d0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-0003f8e0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-0003f8f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003f900: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003f910: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003f920: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-0003f930: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0003f940: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0003f950: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-0003f960: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003f970: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-0003f980: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-0003f990: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0003f9a0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0003f9b0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0003f9c0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0003f9d0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0003f9e0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0003f9f0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-0003fa00: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-0003fa10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003fa20: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-0003fa30: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-0003fa40: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003fa50: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-0003fa60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003fa70: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0003fa80: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-0003fa90: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-0003faa0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003fab0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-0003fac0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003fad0: 2074 656d 705f 6d6f 6465 6c20 3d20 4173   temp_model = As
-0003fae0: 796e 6343 6f6e 6669 6728 290a 2020 2020  yncConfig().    
-0003faf0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0003fb00: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-0003fb10: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-0003fb20: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-0003fb30: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2050  n self...class P
-0003fb40: 7574 436f 6e63 7572 7265 6e63 7943 6f6e  utConcurrencyCon
-0003fb50: 6669 6752 6571 7565 7374 2854 6561 4d6f  figRequest(TeaMo
-0003fb60: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0003fb70: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0003fb80: 7365 6c66 2c0a 2020 2020 2020 2020 626f  self,.        bo
-0003fb90: 6479 3a20 5075 7443 6f6e 6375 7272 656e  dy: PutConcurren
-0003fba0: 6379 496e 7075 7420 3d20 4e6f 6e65 2c0a  cyInput = None,.
-0003fbb0: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
-0003fbc0: 2054 6865 2063 6f6e 6375 7272 656e 6379   The concurrency
-0003fbd0: 2063 6f6e 6669 6775 7261 7469 6f6e 732e   configurations.
-0003fbe0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-0003fbf0: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-0003fc00: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0003fc10: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-0003fc20: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
-0003fc30: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
-0003fc40: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-0003fc50: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0003fc60: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0003fc70: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-0003fc80: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0003fc90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003fca0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0003fcb0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0003fcc0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0003fcd0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0003fce0: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
-0003fcf0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003fd00: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
-0003fd10: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
-0003fd20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0003fd30: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-0003fd40: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-0003fd50: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-0003fd60: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0003fd70: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0003fd80: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-0003fd90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003fda0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-0003fdb0: 6f64 656c 203d 2050 7574 436f 6e63 7572  odel = PutConcur
-0003fdc0: 7265 6e63 7949 6e70 7574 2829 0a20 2020  rencyInput().   
-0003fdd0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0003fde0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-0003fdf0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-0003fe00: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-0003fe10: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0003fe20: 5075 7443 6f6e 6375 7272 656e 6379 436f  PutConcurrencyCo
-0003fe30: 6e66 6967 5265 7370 6f6e 7365 2854 6561  nfigResponse(Tea
-0003fe40: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0003fe50: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0003fe60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0003fe70: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
-0003fe80: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
-0003fe90: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
-0003fea0: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
-0003feb0: 0a20 2020 2020 2020 2062 6f64 793a 2043  .        body: C
-0003fec0: 6f6e 6375 7272 656e 6379 436f 6e66 6967  oncurrencyConfig
-0003fed0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-0003fee0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0003fef0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-0003ff00: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0003ff10: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-0003ff20: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-0003ff30: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-0003ff40: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0003ff50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0003ff60: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-0003ff70: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0003ff80: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-0003ff90: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0003ffa0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0003ffb0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-0003ffc0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-0003ffd0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-0003ffe0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003fff0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00040000: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00040010: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00040020: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-00040030: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00040040: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-00040050: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-00040060: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-00040070: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00040080: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00040090: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000400a0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-000400b0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-000400c0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-000400d0: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-000400e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000400f0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-00040100: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-00040110: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-00040120: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00040130: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00040140: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00040150: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00040160: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00040170: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-00040180: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-00040190: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000401a0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-000401b0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000401c0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000401d0: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-000401e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000401f0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00040200: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-00040210: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-00040220: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00040230: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-00040240: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00040250: 2020 7465 6d70 5f6d 6f64 656c 203d 2043    temp_model = C
-00040260: 6f6e 6375 7272 656e 6379 436f 6e66 6967  oncurrencyConfig
-00040270: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00040280: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00040290: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-000402a0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-000402b0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000402c0: 636c 6173 7320 5075 744c 6179 6572 4143  class PutLayerAC
-000402d0: 4c52 6571 7565 7374 2854 6561 4d6f 6465  LRequest(TeaMode
-000402e0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000402f0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00040300: 6c66 2c0a 2020 2020 2020 2020 7075 626c  lf,.        publ
-00040310: 6963 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ic: str = None,.
-00040320: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
-00040330: 2053 7065 6369 6669 6573 2077 6865 7468   Specifies wheth
-00040340: 6572 2074 6865 206c 6179 6572 2069 7320  er the layer is 
-00040350: 6120 7075 626c 6963 206c 6179 6572 2e20  a public layer. 
-00040360: 5661 6c69 6420 7661 6c75 6573 3a20 7472  Valid values: tr
-00040370: 7565 2061 6e64 2066 616c 7365 2e0a 2020  ue and false..  
-00040380: 2020 2020 2020 7365 6c66 2e70 7562 6c69        self.publi
-00040390: 6320 3d20 7075 626c 6963 0a0a 2020 2020  c = public..    
-000403a0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-000403b0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-000403c0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000403d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000403e0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000403f0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00040400: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00040410: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00040420: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00040430: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00040440: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00040450: 2073 656c 662e 7075 626c 6963 2069 7320   self.public is 
-00040460: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00040470: 2020 2020 2020 7265 7375 6c74 5b27 7075        result['pu
-00040480: 626c 6963 275d 203d 2073 656c 662e 7075  blic'] = self.pu
-00040490: 626c 6963 0a20 2020 2020 2020 2072 6574  blic.        ret
-000404a0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000404b0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000404c0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000404d0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000404e0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000404f0: 2020 2020 6966 206d 2e67 6574 2827 7075      if m.get('pu
-00040500: 626c 6963 2729 2069 7320 6e6f 7420 4e6f  blic') is not No
-00040510: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00040520: 7365 6c66 2e70 7562 6c69 6320 3d20 6d2e  self.public = m.
-00040530: 6765 7428 2770 7562 6c69 6327 290a 2020  get('public').  
-00040540: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00040550: 660a 0a0a 636c 6173 7320 5075 744c 6179  f...class PutLay
-00040560: 6572 4143 4c52 6573 706f 6e73 6528 5465  erACLResponse(Te
-00040570: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00040580: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00040590: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000405a0: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
-000405b0: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
-000405c0: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
-000405d0: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
-000405e0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-000405f0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-00040600: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-00040610: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00040620: 203d 2073 7461 7475 735f 636f 6465 0a0a   = status_code..
-00040630: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00040640: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00040650: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-00040660: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00040670: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00040680: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00040690: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-000406a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000406b0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-000406c0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000406d0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000406e0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-000406f0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00040700: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00040710: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-00040720: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-00040730: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00040740: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-00040750: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00040760: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-00040770: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-00040780: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00040790: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000407a0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000407b0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-000407c0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-000407d0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-000407e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000407f0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-00040800: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00040810: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00040820: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-00040830: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-00040840: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-00040850: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00040860: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00040870: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-00040880: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-00040890: 6527 290a 2020 2020 2020 2020 7265 7475  e').        retu
-000408a0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000408b0: 5075 7450 726f 7669 7369 6f6e 436f 6e66  PutProvisionConf
-000408c0: 6967 5265 7175 6573 7428 5465 614d 6f64  igRequest(TeaMod
-000408d0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000408e0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000408f0: 656c 662c 0a20 2020 2020 2020 2062 6f64  elf,.        bod
-00040900: 793a 2050 7574 5072 6f76 6973 696f 6e43  y: PutProvisionC
-00040910: 6f6e 6669 6749 6e70 7574 203d 204e 6f6e  onfigInput = Non
-00040920: 652c 0a20 2020 2020 2020 2071 7561 6c69  e,.        quali
-00040930: 6669 6572 3a20 7374 7220 3d20 4e6f 6e65  fier: str = None
-00040940: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00040950: 2023 2054 6865 2069 6e66 6f72 6d61 7469   # The informati
-00040960: 6f6e 2061 626f 7574 2074 6865 2070 726f  on about the pro
-00040970: 7669 7369 6f6e 6564 2063 6f6e 6669 6775  visioned configu
-00040980: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-00040990: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-000409a0: 0a20 2020 2020 2020 2023 2054 6865 2066  .        # The f
-000409b0: 756e 6374 696f 6e20 616c 6961 7320 6f72  unction alias or
-000409c0: 204c 4154 4553 542e 0a20 2020 2020 2020   LATEST..       
-000409d0: 2073 656c 662e 7175 616c 6966 6965 7220   self.qualifier 
-000409e0: 3d20 7175 616c 6966 6965 720a 0a20 2020  = qualifier..   
-000409f0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00040a00: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00040a10: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-00040a20: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00040a30: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-00040a40: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00040a50: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00040a60: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-00040a70: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00040a80: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00040a90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00040aa0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00040ab0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00040ac0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00040ad0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00040ae0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00040af0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00040b00: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00040b10: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00040b20: 6c66 2e71 7561 6c69 6669 6572 2069 7320  lf.qualifier is 
-00040b30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00040b40: 2020 2020 2020 7265 7375 6c74 5b27 7175        result['qu
-00040b50: 616c 6966 6965 7227 5d20 3d20 7365 6c66  alifier'] = self
-00040b60: 2e71 7561 6c69 6669 6572 0a20 2020 2020  .qualifier.     
-00040b70: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00040b80: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00040b90: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-00040ba0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-00040bb0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00040bc0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00040bd0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-00040be0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00040bf0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-00040c00: 2050 7574 5072 6f76 6973 696f 6e43 6f6e   PutProvisionCon
-00040c10: 6669 6749 6e70 7574 2829 0a20 2020 2020  figInput().     
-00040c20: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00040c30: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-00040c40: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-00040c50: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00040c60: 6574 2827 7175 616c 6966 6965 7227 2920  et('qualifier') 
-00040c70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00040c80: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
-00040c90: 616c 6966 6965 7220 3d20 6d2e 6765 7428  alifier = m.get(
-00040ca0: 2771 7561 6c69 6669 6572 2729 0a20 2020  'qualifier').   
-00040cb0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00040cc0: 0a0a 0a63 6c61 7373 2050 7574 5072 6f76  ...class PutProv
-00040cd0: 6973 696f 6e43 6f6e 6669 6752 6573 706f  isionConfigRespo
-00040ce0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-00040cf0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00040d00: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00040d10: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-00040d20: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-00040d30: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-00040d40: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
-00040d50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00040d60: 626f 6479 3a20 5072 6f76 6973 696f 6e43  body: ProvisionC
-00040d70: 6f6e 6669 6720 3d20 4e6f 6e65 2c0a 2020  onfig = None,.  
-00040d80: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00040d90: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-00040da0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-00040db0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-00040dc0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-00040dd0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-00040de0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-00040df0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00040e00: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00040e10: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00040e20: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-00040e30: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-00040e40: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00040e50: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00040e60: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00040e70: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00040e80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00040e90: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00040ea0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00040eb0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00040ec0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00040ed0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00040ee0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00040ef0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00040f00: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-00040f10: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00040f20: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00040f30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00040f40: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00040f50: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00040f60: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00040f70: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00040f80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00040f90: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00040fa0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00040fb0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00040fc0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00040fd0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00040fe0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00040ff0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00041000: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00041010: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00041020: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
-00041030: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00041040: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00041050: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
-00041060: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
-00041070: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-00041080: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
-00041090: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000410a0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-000410b0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-000410c0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
-000410d0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-000410e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000410f0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-00041100: 6c20 3d20 5072 6f76 6973 696f 6e43 6f6e  l = ProvisionCon
-00041110: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
-00041120: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-00041130: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-00041140: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-00041150: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00041160: 0a0a 0a63 6c61 7373 2054 6167 5265 736f  ...class TagReso
-00041170: 7572 6365 7352 6571 7565 7374 2854 6561  urcesRequest(Tea
-00041180: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00041190: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-000411a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000411b0: 626f 6479 3a20 5461 6752 6573 6f75 7263  body: TagResourc
-000411c0: 6573 496e 7075 7420 3d20 4e6f 6e65 2c0a  esInput = None,.
-000411d0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-000411e0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
-000411f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00041200: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00041210: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00041220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00041230: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-00041240: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00041250: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00041260: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-00041270: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00041280: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00041290: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000412a0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000412b0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000412c0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000412d0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-000412e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000412f0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-00041300: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-00041310: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-00041320: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00041330: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00041340: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00041350: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00041360: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00041370: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00041380: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-00041390: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000413a0: 7465 6d70 5f6d 6f64 656c 203d 2054 6167  temp_model = Tag
-000413b0: 5265 736f 7572 6365 7349 6e70 7574 2829  ResourcesInput()
-000413c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000413d0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-000413e0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-000413f0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-00041400: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00041410: 6173 7320 5461 6752 6573 6f75 7263 6573  ass TagResources
-00041420: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00041430: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00041440: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00041450: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-00041460: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-00041470: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00041480: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-00041490: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-000414a0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-000414b0: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-000414c0: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
-000414d0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-000414e0: 6174 7573 5f63 6f64 650a 0a20 2020 2064  atus_code..    d
-000414f0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00041500: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00041510: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00041520: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00041530: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-00041540: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00041550: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00041560: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00041570: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00041580: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00041590: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000415a0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-000415b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000415c0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-000415d0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-000415e0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-000415f0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-00041600: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-00041610: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00041620: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-00041630: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-00041640: 6f64 650a 2020 2020 2020 2020 7265 7475  ode.        retu
-00041650: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00041660: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00041670: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00041680: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00041690: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-000416a0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-000416b0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-000416c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000416d0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-000416e0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-000416f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00041700: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+0003f6f0: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
+0003f700: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0003f710: 6e65 7874 5f74 6f6b 656e 3a20 7374 7220  next_token: str 
+0003f720: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0003f730: 7072 6566 6978 3a20 7374 7220 3d20 4e6f  prefix: str = No
+0003f740: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0003f750: 2020 2023 2054 6865 206e 756d 6265 7220     # The number 
+0003f760: 6f66 2074 7269 6767 6572 7320 7265 7475  of triggers retu
+0003f770: 726e 6564 2e0a 2020 2020 2020 2020 7365  rned..        se
+0003f780: 6c66 2e6c 696d 6974 203d 206c 696d 6974  lf.limit = limit
+0003f790: 0a20 2020 2020 2020 2023 2054 6865 2074  .        # The t
+0003f7a0: 6f6b 656e 2066 6f72 2074 6865 206e 6578  oken for the nex
+0003f7b0: 7420 7061 6765 2e0a 2020 2020 2020 2020  t page..        
+0003f7c0: 7365 6c66 2e6e 6578 745f 746f 6b65 6e20  self.next_token 
+0003f7d0: 3d20 6e65 7874 5f74 6f6b 656e 0a20 2020  = next_token.   
+0003f7e0: 2020 2020 2023 2054 6865 2074 7269 6767       # The trigg
+0003f7f0: 6572 206e 616d 6520 7072 6566 6978 2e0a  er name prefix..
+0003f800: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+0003f810: 6669 7820 3d20 7072 6566 6978 0a0a 2020  fix = prefix..  
+0003f820: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0003f830: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0003f840: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+0003f850: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0003f860: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+0003f870: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0003f880: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0003f890: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003f8a0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0003f8b0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0003f8c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0003f8d0: 6966 2073 656c 662e 6c69 6d69 7420 6973  if self.limit is
+0003f8e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003f8f0: 2020 2020 2020 2072 6573 756c 745b 276c         result['l
+0003f900: 696d 6974 275d 203d 2073 656c 662e 6c69  imit'] = self.li
+0003f910: 6d69 740a 2020 2020 2020 2020 6966 2073  mit.        if s
+0003f920: 656c 662e 6e65 7874 5f74 6f6b 656e 2069  elf.next_token i
+0003f930: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003f940: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0003f950: 6e65 7874 546f 6b65 6e27 5d20 3d20 7365  nextToken'] = se
+0003f960: 6c66 2e6e 6578 745f 746f 6b65 6e0a 2020  lf.next_token.  
+0003f970: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0003f980: 6566 6978 2069 7320 6e6f 7420 4e6f 6e65  efix is not None
+0003f990: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003f9a0: 7375 6c74 5b27 7072 6566 6978 275d 203d  sult['prefix'] =
+0003f9b0: 2073 656c 662e 7072 6566 6978 0a20 2020   self.prefix.   
+0003f9c0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+0003f9d0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+0003f9e0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+0003f9f0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+0003fa00: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0003fa10: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0003fa20: 2e67 6574 2827 6c69 6d69 7427 2920 6973  .get('limit') is
+0003fa30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003fa40: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
+0003fa50: 7420 3d20 6d2e 6765 7428 276c 696d 6974  t = m.get('limit
+0003fa60: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003fa70: 6765 7428 276e 6578 7454 6f6b 656e 2729  get('nextToken')
+0003fa80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003fa90: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0003faa0: 6578 745f 746f 6b65 6e20 3d20 6d2e 6765  ext_token = m.ge
+0003fab0: 7428 276e 6578 7454 6f6b 656e 2729 0a20  t('nextToken'). 
+0003fac0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003fad0: 2770 7265 6669 7827 2920 6973 206e 6f74  'prefix') is not
+0003fae0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003faf0: 2020 2073 656c 662e 7072 6566 6978 203d     self.prefix =
+0003fb00: 206d 2e67 6574 2827 7072 6566 6978 2729   m.get('prefix')
+0003fb10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003fb20: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+0003fb30: 7454 7269 6767 6572 7352 6573 706f 6e73  tTriggersRespons
+0003fb40: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+0003fb50: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0003fb60: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0003fb70: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+0003fb80: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+0003fb90: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+0003fba0: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+0003fbb0: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+0003fbc0: 6479 3a20 4c69 7374 5472 6967 6765 7273  dy: ListTriggers
+0003fbd0: 4f75 7470 7574 203d 204e 6f6e 652c 0a20  Output = None,. 
+0003fbe0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0003fbf0: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+0003fc00: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
+0003fc10: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+0003fc20: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0003fc30: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+0003fc40: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
+0003fc50: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0003fc60: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0003fc70: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+0003fc80: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+0003fc90: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+0003fca0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0003fcb0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0003fcc0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+0003fcd0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0003fce0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003fcf0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0003fd00: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0003fd10: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0003fd20: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+0003fd30: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+0003fd40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003fd50: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+0003fd60: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+0003fd70: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+0003fd80: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+0003fd90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003fda0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+0003fdb0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+0003fdc0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+0003fdd0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+0003fde0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003fdf0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+0003fe00: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+0003fe10: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+0003fe20: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0003fe30: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0003fe40: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+0003fe50: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+0003fe60: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0003fe70: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003fe80: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+0003fe90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003fea0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0003feb0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+0003fec0: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+0003fed0: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+0003fee0: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+0003fef0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0003ff00: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0003ff10: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+0003ff20: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+0003ff30: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+0003ff40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003ff50: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+0003ff60: 656c 203d 204c 6973 7454 7269 6767 6572  el = ListTrigger
+0003ff70: 734f 7574 7075 7428 290a 2020 2020 2020  sOutput().      
+0003ff80: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0003ff90: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+0003ffa0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+0003ffb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0003ffc0: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+0003ffd0: 7456 7063 4269 6e64 696e 6773 5265 7370  tVpcBindingsResp
+0003ffe0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+0003fff0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00040000: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00040010: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+00040020: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
+00040030: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00040040: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
+00040050: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00040060: 2062 6f64 793a 204c 6973 7456 7063 4269   body: ListVpcBi
+00040070: 6e64 696e 6773 4f75 7470 7574 203d 204e  ndingsOutput = N
+00040080: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00040090: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000400a0: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+000400b0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000400c0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+000400d0: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
+000400e0: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
+000400f0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00040100: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00040110: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+00040120: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+00040130: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00040140: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00040150: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00040160: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00040170: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00040180: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00040190: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000401a0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000401b0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000401c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000401d0: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+000401e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000401f0: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+00040200: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+00040210: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00040220: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+00040230: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00040240: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00040250: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+00040260: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+00040270: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00040280: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+00040290: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000402a0: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+000402b0: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+000402c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000402d0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000402e0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000402f0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00040300: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00040310: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00040320: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00040330: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00040340: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00040350: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00040360: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00040370: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+00040380: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+00040390: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000403a0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000403b0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+000403c0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+000403d0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+000403e0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+000403f0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00040400: 6d70 5f6d 6f64 656c 203d 204c 6973 7456  mp_model = ListV
+00040410: 7063 4269 6e64 696e 6773 4f75 7470 7574  pcBindingsOutput
+00040420: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00040430: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+00040440: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+00040450: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+00040460: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00040470: 636c 6173 7320 5075 626c 6973 6846 756e  class PublishFun
+00040480: 6374 696f 6e56 6572 7369 6f6e 5265 7175  ctionVersionRequ
+00040490: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+000404a0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000404b0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000404c0: 2020 2020 2020 2062 6f64 793a 2050 7562         body: Pub
+000404d0: 6c69 7368 5665 7273 696f 6e49 6e70 7574  lishVersionInput
+000404e0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+000404f0: 2020 2020 2020 2020 2320 5468 6520 696e          # The in
+00040500: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00040510: 7468 6520 6675 6e63 7469 6f6e 2076 6572  the function ver
+00040520: 7369 6f6e 2e0a 2020 2020 2020 2020 7365  sion..        se
+00040530: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+00040540: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00040550: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00040560: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00040570: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00040580: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00040590: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000405a0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000405b0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000405c0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000405d0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000405e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000405f0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00040600: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00040610: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00040620: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+00040630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00040640: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+00040650: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+00040660: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+00040670: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00040680: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00040690: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000406a0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000406b0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000406c0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+000406d0: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+000406e0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+000406f0: 656d 705f 6d6f 6465 6c20 3d20 5075 626c  emp_model = Publ
+00040700: 6973 6856 6572 7369 6f6e 496e 7075 7428  ishVersionInput(
+00040710: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00040720: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
+00040730: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
+00040740: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
+00040750: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00040760: 6c61 7373 2050 7562 6c69 7368 4675 6e63  lass PublishFunc
+00040770: 7469 6f6e 5665 7273 696f 6e52 6573 706f  tionVersionRespo
+00040780: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+00040790: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000407a0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000407b0: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+000407c0: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+000407d0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000407e0: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
+000407f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00040800: 626f 6479 3a20 5665 7273 696f 6e20 3d20  body: Version = 
+00040810: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00040820: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00040830: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+00040840: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00040850: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00040860: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
+00040870: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+00040880: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00040890: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+000408a0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+000408b0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000408c0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+000408d0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000408e0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000408f0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00040900: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00040910: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00040920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00040930: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00040940: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00040950: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00040960: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+00040970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00040980: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+00040990: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+000409a0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+000409b0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+000409c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000409d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000409e0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+000409f0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+00040a00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00040a10: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+00040a20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00040a30: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00040a40: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00040a50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00040a60: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00040a70: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00040a80: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00040a90: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00040aa0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00040ab0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+00040ac0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+00040ad0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00040ae0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+00040af0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+00040b00: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00040b10: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+00040b20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00040b30: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00040b40: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00040b50: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00040b60: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00040b70: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+00040b80: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00040b90: 656d 705f 6d6f 6465 6c20 3d20 5665 7273  emp_model = Vers
+00040ba0: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
+00040bb0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
+00040bc0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+00040bd0: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
+00040be0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00040bf0: 0a0a 0a63 6c61 7373 2050 7574 4173 796e  ...class PutAsyn
+00040c00: 6349 6e76 6f6b 6543 6f6e 6669 6752 6571  cInvokeConfigReq
+00040c10: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+00040c20: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00040c30: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00040c40: 2020 2020 2020 2020 626f 6479 3a20 5075          body: Pu
+00040c50: 7441 7379 6e63 496e 766f 6b65 436f 6e66  tAsyncInvokeConf
+00040c60: 6967 496e 7075 7420 3d20 4e6f 6e65 2c0a  igInput = None,.
+00040c70: 2020 2020 2020 2020 7175 616c 6966 6965          qualifie
+00040c80: 723a 2073 7472 203d 204e 6f6e 652c 0a20  r: str = None,. 
+00040c90: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
+00040ca0: 5468 6520 636f 6e66 6967 7572 6174 696f  The configuratio
+00040cb0: 6e73 206f 6620 6173 796e 6368 726f 6e6f  ns of asynchrono
+00040cc0: 7573 2066 756e 6374 696f 6e20 696e 766f  us function invo
+00040cd0: 6361 7469 6f6e 2e0a 2020 2020 2020 2020  cation..        
+00040ce0: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00040cf0: 0a20 2020 2020 2020 2023 2054 6865 2076  .        # The v
+00040d00: 6572 7369 6f6e 206f 7220 616c 6961 7320  ersion or alias 
+00040d10: 6f66 2074 6865 2066 756e 6374 696f 6e2e  of the function.
+00040d20: 0a20 2020 2020 2020 2073 656c 662e 7175  .        self.qu
+00040d30: 616c 6966 6965 7220 3d20 7175 616c 6966  alifier = qualif
+00040d40: 6965 720a 0a20 2020 2064 6566 2076 616c  ier..    def val
+00040d50: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00040d60: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00040d70: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00040d80: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00040d90: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00040da0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00040db0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00040dc0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00040dd0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00040de0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00040df0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00040e00: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00040e10: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00040e20: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+00040e30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00040e40: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+00040e50: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00040e60: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00040e70: 2020 2069 6620 7365 6c66 2e71 7561 6c69     if self.quali
+00040e80: 6669 6572 2069 7320 6e6f 7420 4e6f 6e65  fier is not None
+00040e90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00040ea0: 7375 6c74 5b27 7175 616c 6966 6965 7227  sult['qualifier'
+00040eb0: 5d20 3d20 7365 6c66 2e71 7561 6c69 6669  ] = self.qualifi
+00040ec0: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
+00040ed0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00040ee0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00040ef0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00040f00: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00040f10: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00040f20: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+00040f30: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00040f40: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00040f50: 5f6d 6f64 656c 203d 2050 7574 4173 796e  _model = PutAsyn
+00040f60: 6349 6e76 6f6b 6543 6f6e 6669 6749 6e70  cInvokeConfigInp
+00040f70: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00040f80: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00040f90: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00040fa0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00040fb0: 2020 2020 6966 206d 2e67 6574 2827 7175      if m.get('qu
+00040fc0: 616c 6966 6965 7227 2920 6973 206e 6f74  alifier') is not
+00040fd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00040fe0: 2020 2073 656c 662e 7175 616c 6966 6965     self.qualifie
+00040ff0: 7220 3d20 6d2e 6765 7428 2771 7561 6c69  r = m.get('quali
+00041000: 6669 6572 2729 0a20 2020 2020 2020 2072  fier').        r
+00041010: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00041020: 7373 2050 7574 4173 796e 6349 6e76 6f6b  ss PutAsyncInvok
+00041030: 6543 6f6e 6669 6752 6573 706f 6e73 6528  eConfigResponse(
+00041040: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00041050: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00041060: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00041070: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
+00041080: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+00041090: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
+000410a0: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
+000410b0: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+000410c0: 3a20 4173 796e 6343 6f6e 6669 6720 3d20  : AsyncConfig = 
+000410d0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+000410e0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+000410f0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+00041100: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00041110: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00041120: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
+00041130: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+00041140: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00041150: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00041160: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+00041170: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00041180: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+00041190: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000411a0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000411b0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000411c0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000411d0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+000411e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000411f0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00041200: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00041210: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00041220: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+00041230: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00041240: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+00041250: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+00041260: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+00041270: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+00041280: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00041290: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000412a0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+000412b0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+000412c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000412d0: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+000412e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000412f0: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00041300: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00041310: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00041320: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00041330: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00041340: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00041350: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00041360: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00041370: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+00041380: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+00041390: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000413a0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+000413b0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+000413c0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000413d0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+000413e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000413f0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00041400: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00041410: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00041420: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00041430: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+00041440: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00041450: 656d 705f 6d6f 6465 6c20 3d20 4173 796e  emp_model = Asyn
+00041460: 6343 6f6e 6669 6728 290a 2020 2020 2020  cConfig().      
+00041470: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00041480: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00041490: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+000414a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000414b0: 7365 6c66 0a0a 0a63 6c61 7373 2050 7574  self...class Put
+000414c0: 436f 6e63 7572 7265 6e63 7943 6f6e 6669  ConcurrencyConfi
+000414d0: 6752 6571 7565 7374 2854 6561 4d6f 6465  gRequest(TeaMode
+000414e0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000414f0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00041500: 6c66 2c0a 2020 2020 2020 2020 626f 6479  lf,.        body
+00041510: 3a20 5075 7443 6f6e 6375 7272 656e 6379  : PutConcurrency
+00041520: 496e 7075 7420 3d20 4e6f 6e65 2c0a 2020  Input = None,.  
+00041530: 2020 293a 0a20 2020 2020 2020 2023 2054    ):.        # T
+00041540: 6865 2063 6f6e 6375 7272 656e 6379 2063  he concurrency c
+00041550: 6f6e 6669 6775 7261 7469 6f6e 732e 0a20  onfigurations.. 
+00041560: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00041570: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
+00041580: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00041590: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000415a0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+000415b0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+000415c0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+000415d0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000415e0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000415f0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00041600: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00041610: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00041620: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00041630: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00041640: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00041650: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00041660: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+00041670: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00041680: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+00041690: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+000416a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000416b0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000416c0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000416d0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000416e0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000416f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00041700: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
 00041710: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041720: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00041730: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-00041740: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-00041750: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00041760: 6c66 0a0a 0a63 6c61 7373 2055 6e74 6167  lf...class Untag
-00041770: 5265 736f 7572 6365 7352 6571 7565 7374  ResourcesRequest
-00041780: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00041790: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-000417a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000417b0: 2020 2020 616c 6c3a 2062 6f6f 6c20 3d20      all: bool = 
-000417c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
-000417d0: 736f 7572 6365 5f69 643a 204c 6973 745b  source_id: List[
-000417e0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-000417f0: 2020 2020 2072 6573 6f75 7263 655f 7479       resource_ty
-00041800: 7065 3a20 7374 7220 3d20 4e6f 6e65 2c0a  pe: str = None,.
-00041810: 2020 2020 2020 2020 7461 675f 6b65 793a          tag_key:
-00041820: 204c 6973 745b 7374 725d 203d 204e 6f6e   List[str] = Non
-00041830: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00041840: 2020 7365 6c66 2e61 6c6c 203d 2061 6c6c    self.all = all
-00041850: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00041860: 736f 7572 6365 5f69 6420 3d20 7265 736f  source_id = reso
-00041870: 7572 6365 5f69 640a 2020 2020 2020 2020  urce_id.        
-00041880: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
-00041890: 7065 203d 2072 6573 6f75 7263 655f 7479  pe = resource_ty
-000418a0: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-000418b0: 7461 675f 6b65 7920 3d20 7461 675f 6b65  tag_key = tag_ke
-000418c0: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-000418d0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000418e0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-000418f0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00041900: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00041910: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00041920: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00041930: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041940: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00041950: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00041960: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00041970: 2020 2020 2069 6620 7365 6c66 2e61 6c6c       if self.all
-00041980: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00041990: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000419a0: 5b27 416c 6c27 5d20 3d20 7365 6c66 2e61  ['All'] = self.a
-000419b0: 6c6c 0a20 2020 2020 2020 2069 6620 7365  ll.        if se
-000419c0: 6c66 2e72 6573 6f75 7263 655f 6964 2069  lf.resource_id i
-000419d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000419e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000419f0: 5265 736f 7572 6365 4964 275d 203d 2073  ResourceId'] = s
-00041a00: 656c 662e 7265 736f 7572 6365 5f69 640a  elf.resource_id.
-00041a10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00041a20: 7265 736f 7572 6365 5f74 7970 6520 6973  resource_type is
-00041a30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00041a40: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-00041a50: 6573 6f75 7263 6554 7970 6527 5d20 3d20  esourceType'] = 
-00041a60: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
-00041a70: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
-00041a80: 6c66 2e74 6167 5f6b 6579 2069 7320 6e6f  lf.tag_key is no
-00041a90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00041aa0: 2020 2020 7265 7375 6c74 5b27 5461 674b      result['TagK
-00041ab0: 6579 275d 203d 2073 656c 662e 7461 675f  ey'] = self.tag_
-00041ac0: 6b65 790a 2020 2020 2020 2020 7265 7475  key.        retu
-00041ad0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00041ae0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00041af0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00041b00: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00041b10: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00041b20: 2020 2069 6620 6d2e 6765 7428 2741 6c6c     if m.get('All
-00041b30: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00041b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00041b50: 2e61 6c6c 203d 206d 2e67 6574 2827 416c  .all = m.get('Al
-00041b60: 6c27 290a 2020 2020 2020 2020 6966 206d  l').        if m
-00041b70: 2e67 6574 2827 5265 736f 7572 6365 4964  .get('ResourceId
-00041b80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00041b90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00041ba0: 2e72 6573 6f75 7263 655f 6964 203d 206d  .resource_id = m
-00041bb0: 2e67 6574 2827 5265 736f 7572 6365 4964  .get('ResourceId
-00041bc0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00041bd0: 6765 7428 2752 6573 6f75 7263 6554 7970  get('ResourceTyp
-00041be0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00041720: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+00041730: 656c 203d 2050 7574 436f 6e63 7572 7265  el = PutConcurre
+00041740: 6e63 7949 6e70 7574 2829 0a20 2020 2020  ncyInput().     
+00041750: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00041760: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00041770: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00041780: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00041790: 2073 656c 660a 0a0a 636c 6173 7320 5075   self...class Pu
+000417a0: 7443 6f6e 6375 7272 656e 6379 436f 6e66  tConcurrencyConf
+000417b0: 6967 5265 7370 6f6e 7365 2854 6561 4d6f  igResponse(TeaMo
+000417c0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+000417d0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000417e0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+000417f0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00041800: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00041810: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00041820: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00041830: 2020 2020 2020 2062 6f64 793a 2043 6f6e         body: Con
+00041840: 6375 7272 656e 6379 436f 6e66 6967 203d  currencyConfig =
+00041850: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00041860: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00041870: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+00041880: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00041890: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+000418a0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+000418b0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
+000418c0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000418d0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+000418e0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+000418f0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00041900: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+00041910: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00041920: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00041930: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+00041940: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00041950: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00041960: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00041970: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00041980: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00041990: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000419a0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+000419b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000419c0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+000419d0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+000419e0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+000419f0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00041a00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00041a10: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00041a20: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+00041a30: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00041a40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00041a50: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+00041a60: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00041a70: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+00041a80: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+00041a90: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00041aa0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00041ab0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00041ac0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00041ad0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00041ae0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00041af0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+00041b00: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+00041b10: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00041b20: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+00041b30: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+00041b40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00041b50: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+00041b60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00041b70: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00041b80: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+00041b90: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+00041ba0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00041bb0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+00041bc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00041bd0: 7465 6d70 5f6d 6f64 656c 203d 2043 6f6e  temp_model = Con
+00041be0: 6375 7272 656e 6379 436f 6e66 6967 2829  currencyConfig()
 00041bf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00041c00: 662e 7265 736f 7572 6365 5f74 7970 6520  f.resource_type 
-00041c10: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
-00041c20: 6554 7970 6527 290a 2020 2020 2020 2020  eType').        
-00041c30: 6966 206d 2e67 6574 2827 5461 674b 6579  if m.get('TagKey
-00041c40: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00041c50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00041c60: 2e74 6167 5f6b 6579 203d 206d 2e67 6574  .tag_key = m.get
-00041c70: 2827 5461 674b 6579 2729 0a20 2020 2020  ('TagKey').     
-00041c80: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00041c90: 0a63 6c61 7373 2055 6e74 6167 5265 736f  .class UntagReso
-00041ca0: 7572 6365 7353 6872 696e 6b52 6571 7565  urcesShrinkReque
-00041cb0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-00041cc0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00041cd0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00041ce0: 2020 2020 2020 616c 6c3a 2062 6f6f 6c20        all: bool 
-00041cf0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00041d00: 7265 736f 7572 6365 5f69 645f 7368 7269  resource_id_shri
-00041d10: 6e6b 3a20 7374 7220 3d20 4e6f 6e65 2c0a  nk: str = None,.
-00041d20: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-00041d30: 5f74 7970 653a 2073 7472 203d 204e 6f6e  _type: str = Non
-00041d40: 652c 0a20 2020 2020 2020 2074 6167 5f6b  e,.        tag_k
-00041d50: 6579 5f73 6872 696e 6b3a 2073 7472 203d  ey_shrink: str =
-00041d60: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-00041d70: 2020 2020 2020 7365 6c66 2e61 6c6c 203d        self.all =
-00041d80: 2061 6c6c 0a20 2020 2020 2020 2073 656c   all.        sel
-00041d90: 662e 7265 736f 7572 6365 5f69 645f 7368  f.resource_id_sh
-00041da0: 7269 6e6b 203d 2072 6573 6f75 7263 655f  rink = resource_
-00041db0: 6964 5f73 6872 696e 6b0a 2020 2020 2020  id_shrink.      
-00041dc0: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
-00041dd0: 7479 7065 203d 2072 6573 6f75 7263 655f  type = resource_
-00041de0: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
-00041df0: 662e 7461 675f 6b65 795f 7368 7269 6e6b  f.tag_key_shrink
-00041e00: 203d 2074 6167 5f6b 6579 5f73 6872 696e   = tag_key_shrin
-00041e10: 6b0a 0a20 2020 2064 6566 2076 616c 6964  k..    def valid
-00041e20: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00041e30: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00041e40: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00041e50: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00041e60: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00041e70: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00041e80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041e90: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00041ea0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00041eb0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00041ec0: 2020 2020 2069 6620 7365 6c66 2e61 6c6c       if self.all
-00041ed0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00041ee0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00041ef0: 5b27 416c 6c27 5d20 3d20 7365 6c66 2e61  ['All'] = self.a
-00041f00: 6c6c 0a20 2020 2020 2020 2069 6620 7365  ll.        if se
-00041f10: 6c66 2e72 6573 6f75 7263 655f 6964 5f73  lf.resource_id_s
-00041f20: 6872 696e 6b20 6973 206e 6f74 204e 6f6e  hrink is not Non
-00041f30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00041f40: 6573 756c 745b 2752 6573 6f75 7263 6549  esult['ResourceI
-00041f50: 6427 5d20 3d20 7365 6c66 2e72 6573 6f75  d'] = self.resou
-00041f60: 7263 655f 6964 5f73 6872 696e 6b0a 2020  rce_id_shrink.  
-00041f70: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00041f80: 736f 7572 6365 5f74 7970 6520 6973 206e  source_type is n
-00041f90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00041fa0: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
-00041fb0: 6f75 7263 6554 7970 6527 5d20 3d20 7365  ourceType'] = se
-00041fc0: 6c66 2e72 6573 6f75 7263 655f 7479 7065  lf.resource_type
-00041fd0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00041fe0: 2e74 6167 5f6b 6579 5f73 6872 696e 6b20  .tag_key_shrink 
-00041ff0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00042000: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00042010: 2754 6167 4b65 7927 5d20 3d20 7365 6c66  'TagKey'] = self
-00042020: 2e74 6167 5f6b 6579 5f73 6872 696e 6b0a  .tag_key_shrink.
-00042030: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00042040: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00042050: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00042060: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00042070: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00042080: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00042090: 6620 6d2e 6765 7428 2741 6c6c 2729 2069  f m.get('All') i
-000420a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000420b0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000420c0: 203d 206d 2e67 6574 2827 416c 6c27 290a   = m.get('All').
-000420d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000420e0: 2827 5265 736f 7572 6365 4964 2729 2069  ('ResourceId') i
-000420f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00042100: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00042110: 6f75 7263 655f 6964 5f73 6872 696e 6b20  ource_id_shrink 
-00042120: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
-00042130: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
-00042140: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
-00042150: 5479 7065 2729 2069 7320 6e6f 7420 4e6f  Type') is not No
-00042160: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00042170: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
-00042180: 7065 203d 206d 2e67 6574 2827 5265 736f  pe = m.get('Reso
-00042190: 7572 6365 5479 7065 2729 0a20 2020 2020  urceType').     
-000421a0: 2020 2069 6620 6d2e 6765 7428 2754 6167     if m.get('Tag
-000421b0: 4b65 7927 2920 6973 206e 6f74 204e 6f6e  Key') is not Non
-000421c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000421d0: 656c 662e 7461 675f 6b65 795f 7368 7269  elf.tag_key_shri
-000421e0: 6e6b 203d 206d 2e67 6574 2827 5461 674b  nk = m.get('TagK
-000421f0: 6579 2729 0a20 2020 2020 2020 2072 6574  ey').        ret
-00042200: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00042210: 2055 6e74 6167 5265 736f 7572 6365 7352   UntagResourcesR
-00042220: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00042230: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00042240: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00042250: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-00042260: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-00042270: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00042280: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-00042290: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-000422a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000422b0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-000422c0: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-000422d0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-000422e0: 7475 735f 636f 6465 0a0a 2020 2020 6465  tus_code..    de
-000422f0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00042300: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00042310: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00042320: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00042330: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-00042340: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00042350: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00042360: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00042370: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00042380: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00042390: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000423a0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-000423b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000423c0: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-000423d0: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-000423e0: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-000423f0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00042400: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00042410: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00042420: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-00042430: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-00042440: 6465 0a20 2020 2020 2020 2072 6574 7572  de.        retur
-00042450: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00042460: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00042470: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-00042480: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00042490: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000424a0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-000424b0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-000424c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000424d0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-000424e0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-000424f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00042500: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-00042510: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00042520: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00042530: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-00042540: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-00042550: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00042560: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
-00042570: 416c 6961 7352 6571 7565 7374 2854 6561  AliasRequest(Tea
-00042580: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00042590: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-000425a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000425b0: 626f 6479 3a20 5570 6461 7465 416c 6961  body: UpdateAlia
-000425c0: 7349 6e70 7574 203d 204e 6f6e 652c 0a20  sInput = None,. 
-000425d0: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000425e0: 5468 6520 616c 6961 7320 696e 666f 726d  The alias inform
-000425f0: 6174 696f 6e20 746f 2062 6520 7570 6461  ation to be upda
-00042600: 7465 642e 0a20 2020 2020 2020 2073 656c  ted..        sel
-00042610: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-00042620: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00042630: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00042640: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-00042650: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00042660: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-00042670: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00042680: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00042690: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-000426a0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-000426b0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-000426c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000426d0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-000426e0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-000426f0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00042700: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-00042710: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042720: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-00042730: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-00042740: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-00042750: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00042760: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00042770: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00042780: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00042790: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000427a0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-000427b0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-000427c0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-000427d0: 6d70 5f6d 6f64 656c 203d 2055 7064 6174  mp_model = Updat
-000427e0: 6541 6c69 6173 496e 7075 7428 290a 2020  eAliasInput().  
-000427f0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00042800: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-00042810: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-00042820: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-00042830: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00042840: 2055 7064 6174 6541 6c69 6173 5265 7370   UpdateAliasResp
-00042850: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-00042860: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00042870: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00042880: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-00042890: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-000428a0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000428b0: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-000428c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000428d0: 2062 6f64 793a 2041 6c69 6173 203d 204e   body: Alias = N
-000428e0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000428f0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00042900: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
-00042910: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00042920: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-00042930: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
-00042940: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
-00042950: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00042960: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00042970: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
-00042980: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
-00042990: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
-000429a0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000429b0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000429c0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-000429d0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-000429e0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000429f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00042a00: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-00042a10: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-00042a20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00042a30: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
-00042a40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042a50: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
-00042a60: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
-00042a70: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-00042a80: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
-00042a90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00042aa0: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
-00042ab0: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
-00042ac0: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
-00042ad0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00042ae0: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
-00042af0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00042b00: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
-00042b10: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
-00042b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00042b30: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00042b40: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00042b50: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-00042b60: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00042b70: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00042b80: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-00042b90: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-00042ba0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00042bb0: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-00042bc0: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-00042bd0: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-00042be0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-00042bf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00042c00: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00042c10: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-00042c20: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-00042c30: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-00042c40: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-00042c50: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-00042c60: 6d70 5f6d 6f64 656c 203d 2041 6c69 6173  mp_model = Alias
-00042c70: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00042c80: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00042c90: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00042ca0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00042cb0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00042cc0: 636c 6173 7320 5570 6461 7465 4375 7374  class UpdateCust
-00042cd0: 6f6d 446f 6d61 696e 5265 7175 6573 7428  omDomainRequest(
-00042ce0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00042cf0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00042d00: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00042d10: 2020 2062 6f64 793a 2055 7064 6174 6543     body: UpdateC
-00042d20: 7573 746f 6d44 6f6d 6169 6e49 6e70 7574  ustomDomainInput
-00042d30: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-00042d40: 2020 2020 2020 2020 2320 5468 6520 696e          # The in
-00042d50: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-00042d60: 7468 6520 6375 7374 6f6d 2064 6f6d 6169  the custom domai
-00042d70: 6e20 6e61 6d65 2e0a 2020 2020 2020 2020  n name..        
-00042d80: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-00042d90: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00042da0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00042db0: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-00042dc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00042dd0: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-00042de0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00042df0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00042e00: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-00042e10: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00042e20: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00042e30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042e40: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00042e50: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00042e60: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00042e70: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-00042e80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00042e90: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-00042ea0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-00042eb0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00042ec0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00042ed0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00042ee0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00042ef0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00042f00: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00042f10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00042f20: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-00042f30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042f40: 2074 656d 705f 6d6f 6465 6c20 3d20 5570   temp_model = Up
-00042f50: 6461 7465 4375 7374 6f6d 446f 6d61 696e  dateCustomDomain
-00042f60: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
-00042f70: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00042f80: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00042f90: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-00042fa0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00042fb0: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
-00042fc0: 6543 7573 746f 6d44 6f6d 6169 6e52 6573  eCustomDomainRes
-00042fd0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-00042fe0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00042ff0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00043000: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-00043010: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-00043020: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00043030: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-00043040: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-00043050: 2020 626f 6479 3a20 4375 7374 6f6d 446f    body: CustomDo
-00043060: 6d61 696e 203d 204e 6f6e 652c 0a20 2020  main = None,.   
-00043070: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-00043080: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-00043090: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
-000430a0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-000430b0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-000430c0: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-000430d0: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-000430e0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-000430f0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-00043100: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00043110: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-00043120: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-00043130: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00043140: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-00043150: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00043160: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00043170: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00043180: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00043190: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000431a0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000431b0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-000431c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000431d0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000431e0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-000431f0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-00043200: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-00043210: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-00043220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00043230: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-00043240: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-00043250: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-00043260: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-00043270: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00043280: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-00043290: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-000432a0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000432b0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000432c0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000432d0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-000432e0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-000432f0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00043300: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00043310: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-00043320: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00043330: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00043340: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-00043350: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-00043360: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-00043370: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00043380: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00043390: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-000433a0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-000433b0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-000433c0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-000433d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000433e0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-000433f0: 203d 2043 7573 746f 6d44 6f6d 6169 6e28   = CustomDomain(
-00043400: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00043410: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-00043420: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-00043430: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-00043440: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00043450: 6c61 7373 2055 7064 6174 6546 756e 6374  lass UpdateFunct
-00043460: 696f 6e52 6571 7565 7374 2854 6561 4d6f  ionRequest(TeaMo
-00043470: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00043480: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00043490: 7365 6c66 2c0a 2020 2020 2020 2020 626f  self,.        bo
-000434a0: 6479 3a20 5570 6461 7465 4675 6e63 7469  dy: UpdateFuncti
-000434b0: 6f6e 496e 7075 7420 3d20 4e6f 6e65 2c0a  onInput = None,.
-000434c0: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
-000434d0: 2054 6865 2066 756e 6374 696f 6e20 696e   The function in
-000434e0: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
-000434f0: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-00043500: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-00043510: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00043520: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-00043530: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00043540: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-00043550: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-00043560: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00043570: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-00043580: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00043590: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-000435a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000435b0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-000435c0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000435d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000435e0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-000435f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00043600: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00043610: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00043620: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00043630: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00043640: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00043650: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00043660: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00043670: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00043680: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00043690: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-000436a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000436b0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-000436c0: 5570 6461 7465 4675 6e63 7469 6f6e 496e  UpdateFunctionIn
-000436d0: 7075 7428 290a 2020 2020 2020 2020 2020  put().          
-000436e0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-000436f0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-00043700: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-00043710: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00043720: 0a0a 0a63 6c61 7373 2055 7064 6174 6546  ...class UpdateF
-00043730: 756e 6374 696f 6e52 6573 706f 6e73 6528  unctionResponse(
-00043740: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00043750: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00043760: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00043770: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
-00043780: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-00043790: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
-000437a0: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
-000437b0: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
-000437c0: 3a20 4675 6e63 7469 6f6e 203d 204e 6f6e  : Function = Non
-000437d0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-000437e0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-000437f0: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-00043800: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00043810: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-00043820: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00043830: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-00043840: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00043850: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00043860: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00043870: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00043880: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00043890: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-000438a0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-000438b0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-000438c0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-000438d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000438e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000438f0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00043900: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00043910: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-00043920: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-00043930: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00043940: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-00043950: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-00043960: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00043970: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-00043980: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00043990: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-000439a0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-000439b0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-000439c0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-000439d0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-000439e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000439f0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-00043a00: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-00043a10: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00043a20: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00043a30: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00043a40: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00043a50: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00043a60: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00043a70: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00043a80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00043a90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00043aa0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00043ab0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00043ac0: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00043ad0: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00043ae0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00043af0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00043b00: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-00043b10: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-00043b20: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-00043b30: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00043b40: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00043b50: 5f6d 6f64 656c 203d 2046 756e 6374 696f  _model = Functio
-00043b60: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-00043b70: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-00043b80: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00043b90: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00043ba0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00043bb0: 0a63 6c61 7373 2055 7064 6174 6554 7269  .class UpdateTri
-00043bc0: 6767 6572 5265 7175 6573 7428 5465 614d  ggerRequest(TeaM
-00043bd0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00043be0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00043bf0: 2073 656c 662c 0a20 2020 2020 2020 2062   self,.        b
-00043c00: 6f64 793a 2055 7064 6174 6554 7269 6767  ody: UpdateTrigg
-00043c10: 6572 496e 7075 7420 3d20 4e6f 6e65 2c0a  erInput = None,.
-00043c20: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
-00043c30: 2054 6865 2074 7269 6767 6572 2063 6f6e   The trigger con
-00043c40: 6669 6775 7261 7469 6f6e 732e 0a20 2020  figurations..   
-00043c50: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00043c60: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-00043c70: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00043c80: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00043c90: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-00043ca0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-00043cb0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00043cc0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00043cd0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00043ce0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00043cf0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00043d00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00043d10: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00043d20: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00043d30: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00043d40: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-00043d50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00043d60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00043d70: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-00043d80: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-00043d90: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00043da0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-00043db0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-00043dc0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-00043dd0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00043de0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00043df0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-00043e00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00043e10: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-00043e20: 203d 2055 7064 6174 6554 7269 6767 6572   = UpdateTrigger
-00043e30: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
-00043e40: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-00043e50: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00043e60: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-00043e70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00043e80: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
-00043e90: 6554 7269 6767 6572 5265 7370 6f6e 7365  eTriggerResponse
-00043ea0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00043eb0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00043ec0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00043ed0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
-00043ee0: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
-00043ef0: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-00043f00: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
-00043f10: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
-00043f20: 793a 2054 7269 6767 6572 203d 204e 6f6e  y: Trigger = Non
-00043f30: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00043f40: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00043f50: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-00043f60: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00043f70: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-00043f80: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00043f90: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-00043fa0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00043fb0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00043fc0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00043fd0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00043fe0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00043ff0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00044000: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00044010: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-00044020: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00044030: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00044040: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00044050: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00044060: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00044070: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-00044080: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-00044090: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000440a0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-000440b0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-000440c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000440d0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-000440e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000440f0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-00044100: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-00044110: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-00044120: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00044130: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00044140: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00044150: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-00044160: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-00044170: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00044180: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00044190: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000441a0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000441b0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000441c0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000441d0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-000441e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000441f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00044200: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00044210: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00044220: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00044230: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00044240: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00044250: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00044260: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-00044270: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-00044280: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-00044290: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000442a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000442b0: 5f6d 6f64 656c 203d 2054 7269 6767 6572  _model = Trigger
-000442c0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000442d0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-000442e0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-000442f0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00044300: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00041c00: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+00041c10: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00041c20: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+00041c30: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00041c40: 6173 7320 5075 744c 6179 6572 4143 4c52  ass PutLayerACLR
+00041c50: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+00041c60: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00041c70: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00041c80: 2c0a 2020 2020 2020 2020 7075 626c 6963  ,.        public
+00041c90: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00041ca0: 2020 293a 0a20 2020 2020 2020 2023 2053    ):.        # S
+00041cb0: 7065 6369 6669 6573 2077 6865 7468 6572  pecifies whether
+00041cc0: 2074 6865 206c 6179 6572 2069 7320 6120   the layer is a 
+00041cd0: 7075 626c 6963 206c 6179 6572 2e20 5661  public layer. Va
+00041ce0: 6c69 6420 7661 6c75 6573 3a20 7472 7565  lid values: true
+00041cf0: 2061 6e64 2066 616c 7365 2e0a 2020 2020   and false..    
+00041d00: 2020 2020 7365 6c66 2e70 7562 6c69 6320      self.public 
+00041d10: 3d20 7075 626c 6963 0a0a 2020 2020 6465  = public..    de
+00041d20: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00041d30: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00041d40: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00041d50: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00041d60: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00041d70: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00041d80: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00041d90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00041da0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00041db0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00041dc0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00041dd0: 656c 662e 7075 626c 6963 2069 7320 6e6f  elf.public is no
+00041de0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00041df0: 2020 2020 7265 7375 6c74 5b27 7075 626c      result['publ
+00041e00: 6963 275d 203d 2073 656c 662e 7075 626c  ic'] = self.publ
+00041e10: 6963 0a20 2020 2020 2020 2072 6574 7572  ic.        retur
+00041e20: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00041e30: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00041e40: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00041e50: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00041e60: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00041e70: 2020 6966 206d 2e67 6574 2827 7075 626c    if m.get('publ
+00041e80: 6963 2729 2069 7320 6e6f 7420 4e6f 6e65  ic') is not None
+00041e90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00041ea0: 6c66 2e70 7562 6c69 6320 3d20 6d2e 6765  lf.public = m.ge
+00041eb0: 7428 2770 7562 6c69 6327 290a 2020 2020  t('public').    
+00041ec0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00041ed0: 0a0a 636c 6173 7320 5075 744c 6179 6572  ..class PutLayer
+00041ee0: 4143 4c52 6573 706f 6e73 6528 5465 614d  ACLResponse(TeaM
+00041ef0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00041f00: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00041f10: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
+00041f20: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
+00041f30: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
+00041f40: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
+00041f50: 6465 3a20 696e 7420 3d20 4e6f 6e65 2c0a  de: int = None,.
+00041f60: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00041f70: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+00041f80: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
+00041f90: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00041fa0: 2073 7461 7475 735f 636f 6465 0a0a 2020   status_code..  
+00041fb0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00041fc0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00041fd0: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+00041fe0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00041ff0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00042000: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00042010: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00042020: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00042030: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00042040: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00042050: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00042060: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00042070: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00042080: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00042090: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+000420a0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+000420b0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+000420c0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+000420d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000420e0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+000420f0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00042100: 735f 636f 6465 0a20 2020 2020 2020 2072  s_code.        r
+00042110: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00042120: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00042130: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00042140: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00042150: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00042160: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00042170: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+00042180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00042190: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+000421a0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+000421b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000421c0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+000421d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000421e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000421f0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+00042200: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+00042210: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00042220: 2073 656c 660a 0a0a 636c 6173 7320 5075   self...class Pu
+00042230: 7450 726f 7669 7369 6f6e 436f 6e66 6967  tProvisionConfig
+00042240: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00042250: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00042260: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00042270: 662c 0a20 2020 2020 2020 2062 6f64 793a  f,.        body:
+00042280: 2050 7574 5072 6f76 6973 696f 6e43 6f6e   PutProvisionCon
+00042290: 6669 6749 6e70 7574 203d 204e 6f6e 652c  figInput = None,
+000422a0: 0a20 2020 2020 2020 2071 7561 6c69 6669  .        qualifi
+000422b0: 6572 3a20 7374 7220 3d20 4e6f 6e65 2c0a  er: str = None,.
+000422c0: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
+000422d0: 2054 6865 2069 6e66 6f72 6d61 7469 6f6e   The information
+000422e0: 2061 626f 7574 2074 6865 2070 726f 7669   about the provi
+000422f0: 7369 6f6e 6564 2063 6f6e 6669 6775 7261  sioned configura
+00042300: 7469 6f6e 2e0a 2020 2020 2020 2020 7365  tion..        se
+00042310: 6c66 2e62 6f64 7920 3d20 626f 6479 0a20  lf.body = body. 
+00042320: 2020 2020 2020 2023 2054 6865 2066 756e         # The fun
+00042330: 6374 696f 6e20 616c 6961 7320 6f72 204c  ction alias or L
+00042340: 4154 4553 542e 0a20 2020 2020 2020 2073  ATEST..        s
+00042350: 656c 662e 7175 616c 6966 6965 7220 3d20  elf.qualifier = 
+00042360: 7175 616c 6966 6965 720a 0a20 2020 2064  qualifier..    d
+00042370: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00042380: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00042390: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+000423a0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+000423b0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+000423c0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+000423d0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000423e0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+000423f0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00042400: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00042410: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00042420: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00042430: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00042440: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00042450: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+00042460: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00042470: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+00042480: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+00042490: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000424a0: 2e71 7561 6c69 6669 6572 2069 7320 6e6f  .qualifier is no
+000424b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000424c0: 2020 2020 7265 7375 6c74 5b27 7175 616c      result['qual
+000424d0: 6966 6965 7227 5d20 3d20 7365 6c66 2e71  ifier'] = self.q
+000424e0: 7561 6c69 6669 6572 0a20 2020 2020 2020  ualifier.       
+000424f0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00042500: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00042510: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00042520: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00042530: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00042540: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00042550: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00042560: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00042570: 2020 7465 6d70 5f6d 6f64 656c 203d 2050    temp_model = P
+00042580: 7574 5072 6f76 6973 696f 6e43 6f6e 6669  utProvisionConfi
+00042590: 6749 6e70 7574 2829 0a20 2020 2020 2020  gInput().       
+000425a0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+000425b0: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+000425c0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+000425d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000425e0: 2827 7175 616c 6966 6965 7227 2920 6973  ('qualifier') is
+000425f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00042600: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
+00042610: 6966 6965 7220 3d20 6d2e 6765 7428 2771  ifier = m.get('q
+00042620: 7561 6c69 6669 6572 2729 0a20 2020 2020  ualifier').     
+00042630: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00042640: 0a63 6c61 7373 2050 7574 5072 6f76 6973  .class PutProvis
+00042650: 696f 6e43 6f6e 6669 6752 6573 706f 6e73  ionConfigRespons
+00042660: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+00042670: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00042680: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00042690: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+000426a0: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+000426b0: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+000426c0: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+000426d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+000426e0: 6479 3a20 5072 6f76 6973 696f 6e43 6f6e  dy: ProvisionCon
+000426f0: 6669 6720 3d20 4e6f 6e65 2c0a 2020 2020  fig = None,.    
+00042700: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00042710: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+00042720: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+00042730: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+00042740: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+00042750: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+00042760: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+00042770: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00042780: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+00042790: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000427a0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+000427b0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+000427c0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000427d0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+000427e0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000427f0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00042800: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00042810: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00042820: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00042830: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00042840: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+00042850: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00042860: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00042870: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+00042880: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+00042890: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+000428a0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+000428b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000428c0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+000428d0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+000428e0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+000428f0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+00042900: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00042910: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00042920: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00042930: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00042940: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00042950: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00042960: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00042970: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00042980: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00042990: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000429a0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+000429b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000429c0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000429d0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+000429e0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000429f0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00042a00: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00042a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00042a20: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00042a30: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00042a40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00042a50: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00042a60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00042a70: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+00042a80: 3d20 5072 6f76 6973 696f 6e43 6f6e 6669  = ProvisionConfi
+00042a90: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+00042aa0: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+00042ab0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+00042ac0: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+00042ad0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00042ae0: 0a63 6c61 7373 2053 746f 7041 7379 6e63  .class StopAsync
+00042af0: 5461 736b 5265 7175 6573 7428 5465 614d  TaskRequest(TeaM
+00042b00: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00042b10: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00042b20: 2073 656c 662c 0a20 2020 2020 2020 2071   self,.        q
+00042b30: 7561 6c69 6669 6572 3a20 7374 7220 3d20  ualifier: str = 
+00042b40: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00042b50: 2020 2020 2073 656c 662e 7175 616c 6966       self.qualif
+00042b60: 6965 7220 3d20 7175 616c 6966 6965 720a  ier = qualifier.
+00042b70: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00042b80: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00042b90: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00042ba0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00042bb0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00042bc0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00042bd0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00042be0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00042bf0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00042c00: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00042c10: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00042c20: 2020 2069 6620 7365 6c66 2e71 7561 6c69     if self.quali
+00042c30: 6669 6572 2069 7320 6e6f 7420 4e6f 6e65  fier is not None
+00042c40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00042c50: 7375 6c74 5b27 7175 616c 6966 6965 7227  sult['qualifier'
+00042c60: 5d20 3d20 7365 6c66 2e71 7561 6c69 6669  ] = self.qualifi
+00042c70: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
+00042c80: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00042c90: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00042ca0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00042cb0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00042cc0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00042cd0: 2020 6966 206d 2e67 6574 2827 7175 616c    if m.get('qual
+00042ce0: 6966 6965 7227 2920 6973 206e 6f74 204e  ifier') is not N
+00042cf0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00042d00: 2073 656c 662e 7175 616c 6966 6965 7220   self.qualifier 
+00042d10: 3d20 6d2e 6765 7428 2771 7561 6c69 6669  = m.get('qualifi
+00042d20: 6572 2729 0a20 2020 2020 2020 2072 6574  er').        ret
+00042d30: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00042d40: 2053 746f 7041 7379 6e63 5461 736b 5265   StopAsyncTaskRe
+00042d50: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00042d60: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00042d70: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00042d80: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+00042d90: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+00042da0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00042db0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+00042dc0: 6e74 203d 204e 6f6e 652c 0a20 2020 2029  nt = None,.    )
+00042dd0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+00042de0: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+00042df0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00042e00: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+00042e10: 7573 5f63 6f64 650a 0a20 2020 2064 6566  us_code..    def
+00042e20: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00042e30: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00042e40: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00042e50: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00042e60: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00042e70: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00042e80: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00042e90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00042ea0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00042eb0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00042ec0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00042ed0: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00042ee0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00042ef0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00042f00: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00042f10: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+00042f20: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00042f30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00042f40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00042f50: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+00042f60: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00042f70: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00042f80: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00042f90: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00042fa0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00042fb0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00042fc0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00042fd0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+00042fe0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+00042ff0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00043000: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+00043010: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+00043020: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00043030: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+00043040: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00043050: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00043060: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00043070: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00043080: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00043090: 0a0a 0a63 6c61 7373 2054 6167 5265 736f  ...class TagReso
+000430a0: 7572 6365 7352 6571 7565 7374 2854 6561  urcesRequest(Tea
+000430b0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000430c0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000430d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000430e0: 626f 6479 3a20 5461 6752 6573 6f75 7263  body: TagResourc
+000430f0: 6573 496e 7075 7420 3d20 4e6f 6e65 2c0a  esInput = None,.
+00043100: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
+00043110: 2054 6865 2063 6f6e 6669 6775 7261 7469   The configurati
+00043120: 6f6e 206f 6620 7468 6520 7265 736f 7572  on of the resour
+00043130: 6365 2074 6167 2e0a 2020 2020 2020 2020  ce tag..        
+00043140: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00043150: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00043160: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00043170: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+00043180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00043190: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+000431a0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000431b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000431c0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+000431d0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000431e0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000431f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043200: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00043210: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00043220: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00043230: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+00043240: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00043250: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00043260: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00043270: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00043280: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00043290: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+000432a0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+000432b0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+000432c0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000432d0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000432e0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+000432f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043300: 2074 656d 705f 6d6f 6465 6c20 3d20 5461   temp_model = Ta
+00043310: 6752 6573 6f75 7263 6573 496e 7075 7428  gResourcesInput(
+00043320: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00043330: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
+00043340: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
+00043350: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
+00043360: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00043370: 6c61 7373 2054 6167 5265 736f 7572 6365  lass TagResource
+00043380: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
+00043390: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000433a0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000433b0: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+000433c0: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+000433d0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000433e0: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+000433f0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00043400: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00043410: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00043420: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+00043430: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+00043440: 7461 7475 735f 636f 6465 0a0a 2020 2020  tatus_code..    
+00043450: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00043460: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00043470: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00043480: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00043490: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+000434a0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000434b0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000434c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000434d0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+000434e0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+000434f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00043500: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+00043510: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00043520: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+00043530: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+00043540: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00043550: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+00043560: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+00043570: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00043580: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+00043590: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+000435a0: 636f 6465 0a20 2020 2020 2020 2072 6574  code.        ret
+000435b0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000435c0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000435d0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000435e0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000435f0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00043600: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00043610: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00043620: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043630: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00043640: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00043650: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00043660: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00043670: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00043680: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00043690: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+000436a0: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000436b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000436c0: 656c 660a 0a0a 636c 6173 7320 556e 7461  elf...class Unta
+000436d0: 6752 6573 6f75 7263 6573 5265 7175 6573  gResourcesReques
+000436e0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+000436f0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00043700: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00043710: 2020 2020 2061 6c6c 3a20 626f 6f6c 203d       all: bool =
+00043720: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+00043730: 6573 6f75 7263 655f 6964 3a20 4c69 7374  esource_id: List
+00043740: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00043750: 2020 2020 2020 7265 736f 7572 6365 5f74        resource_t
+00043760: 7970 653a 2073 7472 203d 204e 6f6e 652c  ype: str = None,
+00043770: 0a20 2020 2020 2020 2074 6167 5f6b 6579  .        tag_key
+00043780: 3a20 4c69 7374 5b73 7472 5d20 3d20 4e6f  : List[str] = No
+00043790: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000437a0: 2020 2023 2053 7065 6369 6669 6573 2077     # Specifies w
+000437b0: 6865 7468 6572 2074 6f20 6465 6c65 7465  hether to delete
+000437c0: 2061 6c6c 2074 6167 732e 0a20 2020 2020   all tags..     
+000437d0: 2020 2073 656c 662e 616c 6c20 3d20 616c     self.all = al
+000437e0: 6c0a 2020 2020 2020 2020 2320 5468 6520  l.        # The 
+000437f0: 7265 736f 7572 6365 2069 6465 6e74 6966  resource identif
+00043800: 6965 7273 2e0a 2020 2020 2020 2020 7365  iers..        se
+00043810: 6c66 2e72 6573 6f75 7263 655f 6964 203d  lf.resource_id =
+00043820: 2072 6573 6f75 7263 655f 6964 0a20 2020   resource_id.   
+00043830: 2020 2020 2023 2054 6865 2072 6573 6f75       # The resou
+00043840: 7263 6520 7479 7065 2e0a 2020 2020 2020  rce type..      
+00043850: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+00043860: 7479 7065 203d 2072 6573 6f75 7263 655f  type = resource_
+00043870: 7479 7065 0a20 2020 2020 2020 2023 2054  type.        # T
+00043880: 6865 2074 6167 2074 6f20 7265 6d6f 7665  he tag to remove
+00043890: 2e20 596f 7520 6361 6e20 7370 6563 6966  . You can specif
+000438a0: 7920 6120 6d61 7869 6d75 6d20 6f66 2035  y a maximum of 5
+000438b0: 3020 7461 6773 2e0a 2020 2020 2020 2020  0 tags..        
+000438c0: 7365 6c66 2e74 6167 5f6b 6579 203d 2074  self.tag_key = t
+000438d0: 6167 5f6b 6579 0a0a 2020 2020 6465 6620  ag_key..    def 
+000438e0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000438f0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00043900: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00043910: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00043920: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+00043930: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00043940: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00043950: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00043960: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00043970: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00043980: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00043990: 662e 616c 6c20 6973 206e 6f74 204e 6f6e  f.all is not Non
+000439a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000439b0: 6573 756c 745b 2741 6c6c 275d 203d 2073  esult['All'] = s
+000439c0: 656c 662e 616c 6c0a 2020 2020 2020 2020  elf.all.        
+000439d0: 6966 2073 656c 662e 7265 736f 7572 6365  if self.resource
+000439e0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+000439f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00043a00: 756c 745b 2752 6573 6f75 7263 6549 6427  ult['ResourceId'
+00043a10: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
+00043a20: 655f 6964 0a20 2020 2020 2020 2069 6620  e_id.        if 
+00043a30: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
+00043a40: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
+00043a50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00043a60: 6c74 5b27 5265 736f 7572 6365 5479 7065  lt['ResourceType
+00043a70: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+00043a80: 6365 5f74 7970 650a 2020 2020 2020 2020  ce_type.        
+00043a90: 6966 2073 656c 662e 7461 675f 6b65 7920  if self.tag_key 
+00043aa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00043ab0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00043ac0: 2754 6167 4b65 7927 5d20 3d20 7365 6c66  'TagKey'] = self
+00043ad0: 2e74 6167 5f6b 6579 0a20 2020 2020 2020  .tag_key.       
+00043ae0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00043af0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00043b00: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00043b10: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00043b20: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00043b30: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00043b40: 2827 416c 6c27 2920 6973 206e 6f74 204e  ('All') is not N
+00043b50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043b60: 2073 656c 662e 616c 6c20 3d20 6d2e 6765   self.all = m.ge
+00043b70: 7428 2741 6c6c 2729 0a20 2020 2020 2020  t('All').       
+00043b80: 2069 6620 6d2e 6765 7428 2752 6573 6f75   if m.get('Resou
+00043b90: 7263 6549 6427 2920 6973 206e 6f74 204e  rceId') is not N
+00043ba0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043bb0: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+00043bc0: 6420 3d20 6d2e 6765 7428 2752 6573 6f75  d = m.get('Resou
+00043bd0: 7263 6549 6427 290a 2020 2020 2020 2020  rceId').        
+00043be0: 6966 206d 2e67 6574 2827 5265 736f 7572  if m.get('Resour
+00043bf0: 6365 5479 7065 2729 2069 7320 6e6f 7420  ceType') is not 
+00043c00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00043c10: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+00043c20: 7479 7065 203d 206d 2e67 6574 2827 5265  type = m.get('Re
+00043c30: 736f 7572 6365 5479 7065 2729 0a20 2020  sourceType').   
+00043c40: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
+00043c50: 6167 4b65 7927 2920 6973 206e 6f74 204e  agKey') is not N
+00043c60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043c70: 2073 656c 662e 7461 675f 6b65 7920 3d20   self.tag_key = 
+00043c80: 6d2e 6765 7428 2754 6167 4b65 7927 290a  m.get('TagKey').
+00043c90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00043ca0: 656c 660a 0a0a 636c 6173 7320 556e 7461  elf...class Unta
+00043cb0: 6752 6573 6f75 7263 6573 5368 7269 6e6b  gResourcesShrink
+00043cc0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00043cd0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00043ce0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00043cf0: 662c 0a20 2020 2020 2020 2061 6c6c 3a20  f,.        all: 
+00043d00: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
+00043d10: 2020 2020 2072 6573 6f75 7263 655f 6964       resource_id
+00043d20: 5f73 6872 696e 6b3a 2073 7472 203d 204e  _shrink: str = N
+00043d30: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
+00043d40: 6f75 7263 655f 7479 7065 3a20 7374 7220  ource_type: str 
+00043d50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00043d60: 7461 675f 6b65 795f 7368 7269 6e6b 3a20  tag_key_shrink: 
+00043d70: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00043d80: 293a 0a20 2020 2020 2020 2023 2053 7065  ):.        # Spe
+00043d90: 6369 6669 6573 2077 6865 7468 6572 2074  cifies whether t
+00043da0: 6f20 6465 6c65 7465 2061 6c6c 2074 6167  o delete all tag
+00043db0: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+00043dc0: 616c 6c20 3d20 616c 6c0a 2020 2020 2020  all = all.      
+00043dd0: 2020 2320 5468 6520 7265 736f 7572 6365    # The resource
+00043de0: 2069 6465 6e74 6966 6965 7273 2e0a 2020   identifiers..  
+00043df0: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+00043e00: 7263 655f 6964 5f73 6872 696e 6b20 3d20  rce_id_shrink = 
+00043e10: 7265 736f 7572 6365 5f69 645f 7368 7269  resource_id_shri
+00043e20: 6e6b 0a20 2020 2020 2020 2023 2054 6865  nk.        # The
+00043e30: 2072 6573 6f75 7263 6520 7479 7065 2e0a   resource type..
+00043e40: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+00043e50: 6f75 7263 655f 7479 7065 203d 2072 6573  ource_type = res
+00043e60: 6f75 7263 655f 7479 7065 0a20 2020 2020  ource_type.     
+00043e70: 2020 2023 2054 6865 2074 6167 2074 6f20     # The tag to 
+00043e80: 7265 6d6f 7665 2e20 596f 7520 6361 6e20  remove. You can 
+00043e90: 7370 6563 6966 7920 6120 6d61 7869 6d75  specify a maximu
+00043ea0: 6d20 6f66 2035 3020 7461 6773 2e0a 2020  m of 50 tags..  
+00043eb0: 2020 2020 2020 7365 6c66 2e74 6167 5f6b        self.tag_k
+00043ec0: 6579 5f73 6872 696e 6b20 3d20 7461 675f  ey_shrink = tag_
+00043ed0: 6b65 795f 7368 7269 6e6b 0a0a 2020 2020  key_shrink..    
+00043ee0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00043ef0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00043f00: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00043f10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00043f20: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00043f30: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00043f40: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00043f50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043f60: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00043f70: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00043f80: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00043f90: 2073 656c 662e 616c 6c20 6973 206e 6f74   self.all is not
+00043fa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00043fb0: 2020 2072 6573 756c 745b 2741 6c6c 275d     result['All']
+00043fc0: 203d 2073 656c 662e 616c 6c0a 2020 2020   = self.all.    
+00043fd0: 2020 2020 6966 2073 656c 662e 7265 736f      if self.reso
+00043fe0: 7572 6365 5f69 645f 7368 7269 6e6b 2069  urce_id_shrink i
+00043ff0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00044000: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00044010: 5265 736f 7572 6365 4964 275d 203d 2073  ResourceId'] = s
+00044020: 656c 662e 7265 736f 7572 6365 5f69 645f  elf.resource_id_
+00044030: 7368 7269 6e6b 0a20 2020 2020 2020 2069  shrink.        i
+00044040: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
+00044050: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+00044060: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00044070: 7375 6c74 5b27 5265 736f 7572 6365 5479  sult['ResourceTy
+00044080: 7065 275d 203d 2073 656c 662e 7265 736f  pe'] = self.reso
+00044090: 7572 6365 5f74 7970 650a 2020 2020 2020  urce_type.      
+000440a0: 2020 6966 2073 656c 662e 7461 675f 6b65    if self.tag_ke
+000440b0: 795f 7368 7269 6e6b 2069 7320 6e6f 7420  y_shrink is not 
+000440c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000440d0: 2020 7265 7375 6c74 5b27 5461 674b 6579    result['TagKey
+000440e0: 275d 203d 2073 656c 662e 7461 675f 6b65  '] = self.tag_ke
+000440f0: 795f 7368 7269 6e6b 0a20 2020 2020 2020  y_shrink.       
+00044100: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00044110: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00044120: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00044130: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00044140: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00044150: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00044160: 2827 416c 6c27 2920 6973 206e 6f74 204e  ('All') is not N
+00044170: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00044180: 2073 656c 662e 616c 6c20 3d20 6d2e 6765   self.all = m.ge
+00044190: 7428 2741 6c6c 2729 0a20 2020 2020 2020  t('All').       
+000441a0: 2069 6620 6d2e 6765 7428 2752 6573 6f75   if m.get('Resou
+000441b0: 7263 6549 6427 2920 6973 206e 6f74 204e  rceId') is not N
+000441c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000441d0: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+000441e0: 645f 7368 7269 6e6b 203d 206d 2e67 6574  d_shrink = m.get
+000441f0: 2827 5265 736f 7572 6365 4964 2729 0a20  ('ResourceId'). 
+00044200: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00044210: 2752 6573 6f75 7263 6554 7970 6527 2920  'ResourceType') 
+00044220: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00044230: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00044240: 736f 7572 6365 5f74 7970 6520 3d20 6d2e  source_type = m.
+00044250: 6765 7428 2752 6573 6f75 7263 6554 7970  get('ResourceTyp
+00044260: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00044270: 2e67 6574 2827 5461 674b 6579 2729 2069  .get('TagKey') i
+00044280: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00044290: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
+000442a0: 5f6b 6579 5f73 6872 696e 6b20 3d20 6d2e  _key_shrink = m.
+000442b0: 6765 7428 2754 6167 4b65 7927 290a 2020  get('TagKey').  
+000442c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000442d0: 660a 0a0a 636c 6173 7320 556e 7461 6752  f...class UntagR
+000442e0: 6573 6f75 7263 6573 5265 7370 6f6e 7365  esourcesResponse
+000442f0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00044300: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00044310: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00044320: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+00044330: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+00044340: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+00044350: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+00044360: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00044370: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00044380: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+00044390: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000443a0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+000443b0: 650a 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
+000443c0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000443d0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000443e0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000443f0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00044400: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00044410: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00044420: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00044430: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00044440: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00044450: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00044460: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00044470: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00044480: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00044490: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+000444a0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+000444b0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000444c0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+000444d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000444e0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+000444f0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+00044500: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00044510: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00044520: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00044530: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00044540: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00044550: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00044560: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00044570: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+00044580: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00044590: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000445a0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+000445b0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+000445c0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+000445d0: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+000445e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000445f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00044600: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+00044610: 436f 6465 2729 0a20 2020 2020 2020 2072  Code').        r
+00044620: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00044630: 7373 2055 7064 6174 6541 6c69 6173 5265  ss UpdateAliasRe
+00044640: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+00044650: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00044660: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00044670: 0a20 2020 2020 2020 2062 6f64 793a 2055  .        body: U
+00044680: 7064 6174 6541 6c69 6173 496e 7075 7420  pdateAliasInput 
+00044690: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+000446a0: 2020 2020 2020 2023 2054 6865 2061 6c69         # The ali
+000446b0: 6173 2069 6e66 6f72 6d61 7469 6f6e 2074  as information t
+000446c0: 6f20 6265 2075 7064 6174 6564 2e0a 2020  o be updated..  
+000446d0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+000446e0: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
+000446f0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00044700: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00044710: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+00044720: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+00044730: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+00044740: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00044750: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00044760: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+00044770: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00044780: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044790: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+000447a0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+000447b0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+000447c0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000447d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000447e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000447f0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00044800: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00044810: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00044820: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00044830: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00044840: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00044850: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00044860: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00044870: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+00044880: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044890: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000448a0: 6c20 3d20 5570 6461 7465 416c 6961 7349  l = UpdateAliasI
+000448b0: 6e70 7574 2829 0a20 2020 2020 2020 2020  nput().         
+000448c0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+000448d0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+000448e0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+000448f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00044900: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
+00044910: 416c 6961 7352 6573 706f 6e73 6528 5465  AliasResponse(Te
+00044920: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00044930: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00044940: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00044950: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
+00044960: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
+00044970: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
+00044980: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
+00044990: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
+000449a0: 416c 6961 7320 3d20 4e6f 6e65 2c0a 2020  Alias = None,.  
+000449b0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+000449c0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+000449d0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+000449e0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000449f0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00044a00: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+00044a10: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+00044a20: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00044a30: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00044a40: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00044a50: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00044a60: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00044a70: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00044a80: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00044a90: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00044aa0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00044ab0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00044ac0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00044ad0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00044ae0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00044af0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+00044b00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00044b10: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00044b20: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+00044b30: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+00044b40: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+00044b50: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+00044b60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00044b70: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+00044b80: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+00044b90: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00044ba0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+00044bb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00044bc0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+00044bd0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+00044be0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00044bf0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00044c00: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00044c10: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+00044c20: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+00044c30: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00044c40: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00044c50: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+00044c60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00044c70: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00044c80: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+00044c90: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+00044ca0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00044cb0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+00044cc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00044cd0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00044ce0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00044cf0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+00044d00: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+00044d10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044d20: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+00044d30: 6c20 3d20 416c 6961 7328 290a 2020 2020  l = Alias().    
+00044d40: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00044d50: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+00044d60: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+00044d70: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+00044d80: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
+00044d90: 7064 6174 6543 7573 746f 6d44 6f6d 6169  pdateCustomDomai
+00044da0: 6e52 6571 7565 7374 2854 6561 4d6f 6465  nRequest(TeaMode
+00044db0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00044dc0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00044dd0: 6c66 2c0a 2020 2020 2020 2020 626f 6479  lf,.        body
+00044de0: 3a20 5570 6461 7465 4375 7374 6f6d 446f  : UpdateCustomDo
+00044df0: 6d61 696e 496e 7075 7420 3d20 4e6f 6e65  mainInput = None
+00044e00: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00044e10: 2023 2054 6865 2069 6e66 6f72 6d61 7469   # The informati
+00044e20: 6f6e 2061 626f 7574 2074 6865 2063 7573  on about the cus
+00044e30: 746f 6d20 646f 6d61 696e 206e 616d 652e  tom domain name.
+00044e40: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+00044e50: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
+00044e60: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00044e70: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00044e80: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+00044e90: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+00044ea0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+00044eb0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00044ec0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00044ed0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00044ee0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00044ef0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00044f00: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00044f10: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00044f20: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00044f30: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00044f40: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+00044f50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00044f60: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+00044f70: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+00044f80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00044f90: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00044fa0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00044fb0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00044fc0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00044fd0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00044fe0: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+00044ff0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00045000: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00045010: 6f64 656c 203d 2055 7064 6174 6543 7573  odel = UpdateCus
+00045020: 746f 6d44 6f6d 6169 6e49 6e70 7574 2829  tomDomainInput()
+00045030: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00045040: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+00045050: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00045060: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+00045070: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00045080: 6173 7320 5570 6461 7465 4375 7374 6f6d  ass UpdateCustom
+00045090: 446f 6d61 696e 5265 7370 6f6e 7365 2854  DomainResponse(T
+000450a0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000450b0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000450c0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000450d0: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+000450e0: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+000450f0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+00045100: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+00045110: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+00045120: 2043 7573 746f 6d44 6f6d 6169 6e20 3d20   CustomDomain = 
+00045130: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00045140: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00045150: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+00045160: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00045170: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00045180: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
+00045190: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+000451a0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000451b0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+000451c0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+000451d0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000451e0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+000451f0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00045200: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00045210: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00045220: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00045230: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00045240: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00045250: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00045260: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00045270: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00045280: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+00045290: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000452a0: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+000452b0: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+000452c0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+000452d0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+000452e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000452f0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00045300: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+00045310: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+00045320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00045330: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+00045340: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00045350: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00045360: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00045370: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00045380: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00045390: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+000453a0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+000453b0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+000453c0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+000453d0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+000453e0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+000453f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00045400: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+00045410: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+00045420: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00045430: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+00045440: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00045450: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00045460: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00045470: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00045480: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00045490: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+000454a0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+000454b0: 656d 705f 6d6f 6465 6c20 3d20 4375 7374  emp_model = Cust
+000454c0: 6f6d 446f 6d61 696e 2829 0a20 2020 2020  omDomain().     
+000454d0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000454e0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+000454f0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00045500: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00045510: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+00045520: 6461 7465 4675 6e63 7469 6f6e 5265 7175  dateFunctionRequ
+00045530: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+00045540: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00045550: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00045560: 2020 2020 2020 2062 6f64 793a 2055 7064         body: Upd
+00045570: 6174 6546 756e 6374 696f 6e49 6e70 7574  ateFunctionInput
+00045580: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00045590: 2020 2020 2020 2020 2320 5468 6520 6675          # The fu
+000455a0: 6e63 7469 6f6e 2069 6e66 6f72 6d61 7469  nction informati
+000455b0: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
+000455c0: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+000455d0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000455e0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+000455f0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+00045600: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00045610: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+00045620: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00045630: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00045640: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00045650: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00045660: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00045670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00045680: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00045690: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+000456a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000456b0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+000456c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000456d0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+000456e0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+000456f0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00045700: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00045710: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00045720: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00045730: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00045740: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00045750: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+00045760: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00045770: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00045780: 5f6d 6f64 656c 203d 2055 7064 6174 6546  _model = UpdateF
+00045790: 756e 6374 696f 6e49 6e70 7574 2829 0a20  unctionInput(). 
+000457a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000457b0: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+000457c0: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+000457d0: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+000457e0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+000457f0: 7320 5570 6461 7465 4675 6e63 7469 6f6e  s UpdateFunction
+00045800: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+00045810: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00045820: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00045830: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
+00045840: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
+00045850: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00045860: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
+00045870: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+00045880: 2020 2020 2062 6f64 793a 2046 756e 6374       body: Funct
+00045890: 696f 6e20 3d20 4e6f 6e65 2c0a 2020 2020  ion = None,.    
+000458a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000458b0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+000458c0: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+000458d0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+000458e0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000458f0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+00045900: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+00045910: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00045920: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+00045930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00045940: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+00045950: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+00045960: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00045970: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00045980: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00045990: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+000459a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000459b0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+000459c0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000459d0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000459e0: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+000459f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00045a00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00045a10: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+00045a20: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+00045a30: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+00045a40: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+00045a50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00045a60: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+00045a70: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+00045a80: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+00045a90: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+00045aa0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00045ab0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00045ac0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00045ad0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00045ae0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00045af0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00045b00: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00045b10: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00045b20: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00045b30: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00045b40: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+00045b50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00045b60: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00045b70: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+00045b80: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+00045b90: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00045ba0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00045bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00045bc0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00045bd0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00045be0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00045bf0: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00045c00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00045c10: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+00045c20: 3d20 4675 6e63 7469 6f6e 2829 0a20 2020  = Function().   
+00045c30: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00045c40: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+00045c50: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+00045c60: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+00045c70: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00045c80: 5570 6461 7465 5472 6967 6765 7252 6571  UpdateTriggerReq
+00045c90: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+00045ca0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00045cb0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00045cc0: 2020 2020 2020 2020 626f 6479 3a20 5570          body: Up
+00045cd0: 6461 7465 5472 6967 6765 7249 6e70 7574  dateTriggerInput
+00045ce0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00045cf0: 2020 2020 2020 2020 2320 5468 6520 7472          # The tr
+00045d00: 6967 6765 7220 636f 6e66 6967 7572 6174  igger configurat
+00045d10: 696f 6e73 2e0a 2020 2020 2020 2020 7365  ions..        se
+00045d20: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+00045d30: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00045d40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00045d50: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00045d60: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00045d70: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00045d80: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00045d90: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00045da0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00045db0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00045dc0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00045dd0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00045de0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00045df0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00045e00: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00045e10: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+00045e20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00045e30: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+00045e40: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+00045e50: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+00045e60: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00045e70: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00045e80: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00045e90: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00045ea0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00045eb0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00045ec0: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+00045ed0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00045ee0: 656d 705f 6d6f 6465 6c20 3d20 5570 6461  emp_model = Upda
+00045ef0: 7465 5472 6967 6765 7249 6e70 7574 2829  teTriggerInput()
+00045f00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00045f10: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+00045f20: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00045f30: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+00045f40: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00045f50: 6173 7320 5570 6461 7465 5472 6967 6765  ass UpdateTrigge
+00045f60: 7252 6573 706f 6e73 6528 5465 614d 6f64  rResponse(TeaMod
+00045f70: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00045f80: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00045f90: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+00045fa0: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+00045fb0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00045fc0: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+00045fd0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00045fe0: 2020 2020 2020 626f 6479 3a20 5472 6967        body: Trig
+00045ff0: 6765 7220 3d20 4e6f 6e65 2c0a 2020 2020  ger = None,.    
+00046000: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00046010: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+00046020: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+00046030: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+00046040: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+00046050: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+00046060: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+00046070: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00046080: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+00046090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000460a0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+000460b0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+000460c0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000460d0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+000460e0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000460f0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00046100: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00046110: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00046120: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00046130: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00046140: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+00046150: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00046160: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00046170: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+00046180: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+00046190: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+000461a0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+000461b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000461c0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+000461d0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+000461e0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+000461f0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+00046200: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00046210: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00046220: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00046230: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00046240: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00046250: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00046260: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00046270: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00046280: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00046290: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000462a0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+000462b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000462c0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000462d0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+000462e0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000462f0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00046300: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00046310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00046320: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00046330: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00046340: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00046350: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00046360: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00046370: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+00046380: 3d20 5472 6967 6765 7228 290a 2020 2020  = Trigger().    
+00046390: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000463a0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+000463b0: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+000463c0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+000463d0: 6e20 7365 6c66 0a0a 0a                   n self...
```

### Comparing `alibabacloud_fc20230330-4.0.0/alibabacloud_fc20230330.egg-info/PKG-INFO` & `alibabacloud_fc20230330-4.1.0/alibabacloud_fc20230330.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-fc20230330
-Version: 4.0.0
+Version: 4.1.0
 Summary: Alibaba Cloud Function Compute (20230330) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc20230330-4.0.0/setup.py` & `alibabacloud_fc20230330-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_fc20230330.
 
-Created on 15/04/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_fc20230330"
 NAME = "alibabacloud_fc20230330" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Function Compute (20230330) SDK Library for Python"
```

