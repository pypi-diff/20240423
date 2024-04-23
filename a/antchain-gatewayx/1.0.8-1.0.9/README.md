# Comparing `tmp/antchain_gatewayx-1.0.8.tar.gz` & `tmp/antchain_gatewayx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_gatewayx-1.0.8.tar", last modified: Tue Jul  6 02:40:14 2021, max compression
+gzip compressed data, was "dist/antchain_gatewayx-1.0.9.tar", last modified: Tue Apr 23 10:54:56 2024, max compression
```

## Comparing `antchain_gatewayx-1.0.8.tar` & `antchain_gatewayx-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      600 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2200 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      827 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1013 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_gatewayx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2200 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_gatewayx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_gatewayx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_gatewayx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_gatewayx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_gatewayx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_sdk_gatewayx/
--rw-r--r--   0 root         (0) root         (0)       21 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_sdk_gatewayx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19075 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_sdk_gatewayx/client.py
--rw-r--r--   0 root         (0) root         (0)    23973 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/antchain_sdk_gatewayx/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2513 2021-07-06 02:40:14.000000 antchain_gatewayx-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      819 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/antchain_gatewayx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/antchain_gatewayx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/antchain_gatewayx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/antchain_gatewayx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/antchain_gatewayx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/antchain_gatewayx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/antchain_sdk_gatewayx/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/antchain_sdk_gatewayx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19381 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/antchain_sdk_gatewayx/client.py
+-rw-r--r--   0 root         (0) root         (0)    25009 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/antchain_sdk_gatewayx/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 10:54:56.000000 antchain_gatewayx-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-23 10:54:55.000000 antchain_gatewayx-1.0.9/setup.py
```

### Comparing `antchain_gatewayx-1.0.8/LICENSE` & `antchain_gatewayx-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_gatewayx-1.0.8/PKG-INFO` & `antchain_gatewayx-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_gatewayx
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain GATEWAYX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_gatewayx
-        pip install antchain_sdk_gatewayx
+        # Install the antchain-gatewayx
+        pip install antchain-gatewayx
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_gatewayx-1.0.8/README-CN.md` & `antchain_gatewayx-1.0.9/README-CN.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain_sdk_gatewayx
-pip install antchain_sdk_gatewayx
+# 安装 antchain-gatewayx
+pip install antchain-gatewayx
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_gatewayx-1.0.8/README.md` & `antchain_gatewayx-1.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain_sdk_gatewayx
-pip install antchain_sdk_gatewayx
+# Install the antchain-gatewayx
+pip install antchain-gatewayx
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_gatewayx-1.0.8/antchain_gatewayx.egg-info/PKG-INFO` & `antchain_gatewayx-1.0.9/antchain_gatewayx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-gatewayx
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain GATEWAYX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_gatewayx
-        pip install antchain_sdk_gatewayx
+        # Install the antchain-gatewayx
+        pip install antchain-gatewayx
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_gatewayx-1.0.8/antchain_sdk_gatewayx/client.py` & `antchain_gatewayx-1.0.9/antchain_sdk_gatewayx/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8'
+                    'sdk_version': '1.0.9',
+                    '_prod_code': 'GATEWAYX',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -196,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -233,15 +235,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8'
+                    'sdk_version': '1.0.9',
+                    '_prod_code': 'GATEWAYX',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -302,30 +306,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> gatewayx_models.CreateBizeventMessageResponse:
         """
         Description: 接收业务事件消息，并将相关消息投递给对应的接手方
         Summary: 事件消息创建
         """
         UtilClient.validate_model(request)
-        return gatewayx_models.CreateBizeventMessageResponse().from_map(
+        return TeaCore.from_map(
+            gatewayx_models.CreateBizeventMessageResponse(),
             self.do_request('1.0', 'antcloud.gatewayx.bizevent.message.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_bizevent_message_ex_async(
         self,
         request: gatewayx_models.CreateBizeventMessageRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> gatewayx_models.CreateBizeventMessageResponse:
         """
         Description: 接收业务事件消息，并将相关消息投递给对应的接手方
         Summary: 事件消息创建
         """
         UtilClient.validate_model(request)
-        return gatewayx_models.CreateBizeventMessageResponse().from_map(
+        return TeaCore.from_map(
+            gatewayx_models.CreateBizeventMessageResponse(),
             await self.do_request_async('1.0', 'antcloud.gatewayx.bizevent.message.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_file_upload(
         self,
         request: gatewayx_models.CreateFileUploadRequest,
     ) -> gatewayx_models.CreateFileUploadResponse:
@@ -356,30 +362,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> gatewayx_models.CreateFileUploadResponse:
         """
         Description: 创建HTTP PUT提交的文件上传
         Summary: 文件上传创建
         """
         UtilClient.validate_model(request)
-        return gatewayx_models.CreateFileUploadResponse().from_map(
+        return TeaCore.from_map(
+            gatewayx_models.CreateFileUploadResponse(),
             self.do_request('1.0', 'antcloud.gatewayx.file.upload.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_file_upload_ex_async(
         self,
         request: gatewayx_models.CreateFileUploadRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> gatewayx_models.CreateFileUploadResponse:
         """
         Description: 创建HTTP PUT提交的文件上传
         Summary: 文件上传创建
         """
         UtilClient.validate_model(request)
-        return gatewayx_models.CreateFileUploadResponse().from_map(
+        return TeaCore.from_map(
+            gatewayx_models.CreateFileUploadResponse(),
             await self.do_request_async('1.0', 'antcloud.gatewayx.file.upload.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_file_download(
         self,
         request: gatewayx_models.GetFileDownloadRequest,
     ) -> gatewayx_models.GetFileDownloadResponse:
@@ -410,25 +418,27 @@
         runtime: util_models.RuntimeOptions,
     ) -> gatewayx_models.GetFileDownloadResponse:
         """
         Description: 创建HTTP GET获取的文件下载
         Summary: 下载地址获取
         """
         UtilClient.validate_model(request)
-        return gatewayx_models.GetFileDownloadResponse().from_map(
+        return TeaCore.from_map(
+            gatewayx_models.GetFileDownloadResponse(),
             self.do_request('1.0', 'antcloud.gatewayx.file.download.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_file_download_ex_async(
         self,
         request: gatewayx_models.GetFileDownloadRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> gatewayx_models.GetFileDownloadResponse:
         """
         Description: 创建HTTP GET获取的文件下载
         Summary: 下载地址获取
         """
         UtilClient.validate_model(request)
-        return gatewayx_models.GetFileDownloadResponse().from_map(
+        return TeaCore.from_map(
+            gatewayx_models.GetFileDownloadResponse(),
             await self.do_request_async('1.0', 'antcloud.gatewayx.file.download.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

### Comparing `antchain_gatewayx-1.0.8/antchain_sdk_gatewayx/models.py` & `antchain_gatewayx-1.0.9/antchain_sdk_gatewayx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         # 每个目标主机的最大连接数（分主机域名的长链接最大总数
         self.max_requests_per_host = max_requests_per_host
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.access_key_id is not None:
             result['accessKeyId'] = self.access_key_id
         if self.access_key_secret is not None:
             result['accessKeySecret'] = self.access_key_secret
         if self.security_token is not None:
             result['securityToken'] = self.security_token
@@ -162,14 +166,18 @@
         self.value = value
 
     def validate(self):
         self.validate_required(self.name, 'name')
         self.validate_required(self.value, 'value')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.name is not None:
             result['name'] = self.name
         if self.value is not None:
             result['value'] = self.value
         return result
 
@@ -202,14 +210,18 @@
     def validate(self):
         self.validate_required(self.invoke_channel, 'invoke_channel')
         self.validate_required(self.invoke_channel_uid, 'invoke_channel_uid')
         self.validate_required(self.invoke_tenant, 'invoke_tenant')
         self.validate_required(self.invoke_user_id, 'invoke_user_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.invoke_channel is not None:
             result['invoke_channel'] = self.invoke_channel
         if self.invoke_channel_uid is not None:
             result['invoke_channel_uid'] = self.invoke_channel_uid
         if self.invoke_tenant is not None:
             result['invoke_tenant'] = self.invoke_tenant
@@ -238,14 +250,15 @@
         utc_timestamp: int = None,
         msg_id: str = None,
         msg_key: str = None,
         consumer_id: str = None,
         consumer_type: str = None,
         tags: str = None,
         msg_type: str = None,
+        header: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 业务消息内容，json格式
         self.biz_content = biz_content
         # 日期对应的timestamp
         self.utc_timestamp = utc_timestamp
@@ -257,25 +270,31 @@
         self.consumer_id = consumer_id
         # 消费者类型，例如TENANT, APP
         self.consumer_type = consumer_type
         # 二级消息主题,订阅方可以过滤消息
         self.tags = tags
         # 消息类型，1：点对点，2: 广播消息
         self.msg_type = msg_type
+        # 上下文透传的自定义header
+        self.header = header
 
     def validate(self):
         self.validate_required(self.biz_content, 'biz_content')
         self.validate_required(self.utc_timestamp, 'utc_timestamp')
         self.validate_required(self.msg_id, 'msg_id')
         self.validate_required(self.msg_key, 'msg_key')
         self.validate_required(self.consumer_id, 'consumer_id')
         self.validate_required(self.consumer_type, 'consumer_type')
         self.validate_required(self.msg_type, 'msg_type')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.biz_content is not None:
             result['biz_content'] = self.biz_content
         if self.utc_timestamp is not None:
             result['utc_timestamp'] = self.utc_timestamp
@@ -287,14 +306,16 @@
             result['consumer_id'] = self.consumer_id
         if self.consumer_type is not None:
             result['consumer_type'] = self.consumer_type
         if self.tags is not None:
             result['tags'] = self.tags
         if self.msg_type is not None:
             result['msg_type'] = self.msg_type
+        if self.header is not None:
+            result['header'] = self.header
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('biz_content') is not None:
@@ -309,14 +330,16 @@
             self.consumer_id = m.get('consumer_id')
         if m.get('consumer_type') is not None:
             self.consumer_type = m.get('consumer_type')
         if m.get('tags') is not None:
             self.tags = m.get('tags')
         if m.get('msg_type') is not None:
             self.msg_type = m.get('msg_type')
+        if m.get('header') is not None:
+            self.header = m.get('header')
         return self
 
 
 class CreateBizeventMessageResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -330,14 +353,18 @@
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -386,14 +413,18 @@
             self.validate_max_length(self.file_label, 'file_label', 100)
         if self.file_metadata is not None:
             self.validate_max_length(self.file_metadata, 'file_metadata', 1000)
         if self.file_name is not None:
             self.validate_max_length(self.file_name, 'file_name', 100)
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.api_code is not None:
             result['api_code'] = self.api_code
         if self.file_label is not None:
             result['file_label'] = self.file_label
@@ -457,14 +488,18 @@
             self.validate_pattern(self.expired_time, 'expired_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         if self.upload_headers:
             for k in self.upload_headers:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -513,14 +548,18 @@
         # 文件唯一id
         self.file_id = file_id
 
     def validate(self):
         self.validate_required(self.file_id, 'file_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.file_id is not None:
             result['file_id'] = self.file_id
         return result
 
@@ -577,14 +616,18 @@
     def validate(self):
         if self.expired_time is not None:
             self.validate_pattern(self.expired_time, 'expired_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         if self.upload_invoker:
             self.upload_invoker.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
```

### Comparing `antchain_gatewayx-1.0.8/setup.py` & `antchain_gatewayx-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_gatewayx.
 
-Created on 06/07/2021
+Created on 23/04/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_gatewayx"
 NAME = "antchain_gatewayx" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain GATEWAYX SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "antchain_alipay_util>=1.0.0, <2.0.0",
-    "alibabacloud_tea_util>=0.3.3, <1.0.0",
-    "alibabacloud_rpc_util>=0.0.3, <1.0.0"
+    "antchain_alipay_util>=1.0.1, <2.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

