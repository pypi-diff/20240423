# Comparing `tmp/alibabacloud_alikafka20190916-2.6.5.tar.gz` & `tmp/alibabacloud_alikafka20190916-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.6.5.tar", last modified: Thu Apr 11 17:10:00 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.6.6.tar", last modified: Tue Apr 23 17:13:02 2024, max compression
```

## Comparing `alibabacloud_alikafka20190916-2.6.5.tar` & `alibabacloud_alikafka20190916-2.6.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/
--rw-r--r--   0 root         (0) root         (0)     6474 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181950 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   395926 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/
+-rw-r--r--   0 root         (0) root         (0)     6781 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   184296 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   401503 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-04-23 17:13:02.000000 alibabacloud_alikafka20190916-2.6.6/setup.py
```

### Comparing `alibabacloud_alikafka20190916-2.6.5/ChangeLog.md` & `alibabacloud_alikafka20190916-2.6.6/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2024-04-11 Version: 2.6.5
+- Update API CreatePostPayOrder: add param PaidType.
+- Update API CreatePostPayOrder: add param ServerlessConfig.
+- Update API CreatePostPayOrder: update param DiskSize.
+- Update API CreatePostPayOrder: update param DiskType.
+- Update API GetInstanceList: update response param.
+
+
 2024-04-03 Version: 2.6.4
 - Update API CreateAcl: add param AclOperationTypes.
 - Update API CreateAcl: add param AclPermissionType.
 - Update API CreateAcl: add param Host.
 - Update API CreateAcl: update param AclOperationType.
 - Update API CreateSaslUser: add param Mechanism.
 - Update API DeleteAcl: add param AclOperationTypes.
```

### Comparing `alibabacloud_alikafka20190916-2.6.5/LICENSE` & `alibabacloud_alikafka20190916-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.5/PKG-INFO` & `alibabacloud_alikafka20190916-2.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916
-Version: 2.6.5
+Version: 2.6.6
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.5/README-CN.md` & `alibabacloud_alikafka20190916-2.6.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.5/README.md` & `alibabacloud_alikafka20190916-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2016,14 +2016,16 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.order_id):
             query['OrderId'] = request.order_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.series):
+            query['Series'] = request.series
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetInstanceList',
@@ -2052,14 +2054,16 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.order_id):
             query['OrderId'] = request.order_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.series):
+            query['Series'] = request.series
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetInstanceList',
@@ -2906,14 +2910,21 @@
         return await self.release_instance_with_options_async(request, runtime)
 
     def reopen_instance_with_options(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
+        """
+        You can call this operation only if your instance is in the Stopped state.
+        
+        @param request: ReopenInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReopenInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -2936,14 +2947,21 @@
         )
 
     async def reopen_instance_with_options_async(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
+        """
+        You can call this operation only if your instance is in the Stopped state.
+        
+        @param request: ReopenInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReopenInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -2965,21 +2983,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reopen_instance(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
+        """
+        You can call this operation only if your instance is in the Stopped state.
+        
+        @param request: ReopenInstanceRequest
+        @return: ReopenInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reopen_instance_with_options(request, runtime)
 
     async def reopen_instance_async(
         self,
         request: alikafka_20190916_models.ReopenInstanceRequest,
     ) -> alikafka_20190916_models.ReopenInstanceResponse:
+        """
+        You can call this operation only if your instance is in the Stopped state.
+        
+        @param request: ReopenInstanceRequest
+        @return: ReopenInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.reopen_instance_with_options_async(request, runtime)
 
     def start_instance_with_options(
         self,
         request: alikafka_20190916_models.StartInstanceRequest,
         runtime: util_models.RuntimeOptions,
@@ -3156,14 +3186,21 @@
         return await self.start_instance_with_options_async(request, runtime)
 
     def stop_instance_with_options(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.StopInstanceResponse:
+        """
+        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        
+        @param request: StopInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -3186,14 +3223,21 @@
         )
 
     async def stop_instance_with_options_async(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.StopInstanceResponse:
+        """
+        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        
+        @param request: StopInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -3215,21 +3259,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_instance(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
     ) -> alikafka_20190916_models.StopInstanceResponse:
+        """
+        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        
+        @param request: StopInstanceRequest
+        @return: StopInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_instance_with_options(request, runtime)
 
     async def stop_instance_async(
         self,
         request: alikafka_20190916_models.StopInstanceRequest,
     ) -> alikafka_20190916_models.StopInstanceResponse:
+        """
+        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        
+        @param request: StopInstanceRequest
+        @return: StopInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_instance_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: alikafka_20190916_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1875,14 +1875,22 @@
         password: str = None,
         region_id: str = None,
         type: str = None,
         username: str = None,
     ):
         # The instance ID.
         self.instance_id = instance_id
+        # The encryption method. Valid values:
+        # 
+        # *   SCRAM-SHA-512 (default)
+        # *   SCRAM-SHA-256
+        # 
+        # > 
+        # 
+        # *   This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.mechanism = mechanism
         # The password of the SASL user.
         self.password = password
         # The region ID.
         self.region_id = region_id
         # The SASL mechanism. Valid values:
         # 
@@ -2302,36 +2310,57 @@
         acl_resource_pattern_type: str = None,
         acl_resource_type: str = None,
         host: str = None,
         instance_id: str = None,
         region_id: str = None,
         username: str = None,
     ):
-        # The operation type. Valid values:
+        # The operation allowed by the access control list (ACL). Valid values:
         # 
-        # *   **Write**\
-        # *   **Read**\
+        # *   **Write**: data writes
+        # *   **Read**: data reads
+        # *   **Describe**: reads of transactional IDs
+        # *   **IdempotentWrite**: idempotent data writes to clusters
         self.acl_operation_type = acl_operation_type
+        # The operations allowed by the ACL. Separate multiple operations with commas (,).
+        # 
+        # Valid values:
+        # 
+        # *   **Write**: data writes
+        # *   **Read**: data reads
+        # *   **Describe**: reads of **transactional IDs**\
+        # *   **IdempotentWrite**: idempotent data writes to **clusters**\
+        # 
+        # >  This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.acl_operation_types = acl_operation_types
+        # The authorization method. Valid values:
+        # 
+        # *   Deny
+        # *   ALLOW
+        # 
+        # >  This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.acl_permission_type = acl_permission_type
         # The name of the resource.
         # 
         # *   The value can be the name of a topic or consumer group.
         # *   You can use an asterisk (\*) to indicate the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name
         # The mode that is used to match resources. Valid values:
         # 
         # *   **LITERAL:** full match
         # *   **PREFIXED**: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type
-        # The type of the resource.
+        # The resource type. Valid values:
         # 
-        # *   **Topic**\
-        # *   **Group**\
+        # *   **Topic**: topic
+        # *   **Group**: consumer group
+        # *   **Cluster**: cluster
+        # *   **TransactionalId**: transactional ID
         self.acl_resource_type = acl_resource_type
+        # The IP address of the source.
         self.host = host
         # The ID of the instance.
         self.instance_id = instance_id
         # The ID of the region.
         self.region_id = region_id
         # The name of the user.
         self.username = username
@@ -4250,17 +4279,19 @@
         current_page: int = None,
         instance_id: str = None,
         page_size: int = None,
         region_id: str = None,
     ):
         # The name of the consumer group. If you do not configure this parameter, all consumer groups are queried.
         self.consumer_id = consumer_id
+        # The page number.
         self.current_page = current_page
         # The ID of the instance to which the consumer group belongs.
         self.instance_id = instance_id
+        # The number of entries to be returned per page.
         self.page_size = page_size
         # The region ID of the instance to which the consumer group belongs.
         self.region_id = region_id
 
     def validate(self):
         pass
 
@@ -4373,23 +4404,23 @@
         automatically_created_group: bool = None,
         consumer_id: str = None,
         instance_id: str = None,
         region_id: str = None,
         remark: str = None,
         tags: GetConsumerListResponseBodyConsumerListConsumerVOTags = None,
     ):
-        # The consumer group that is automatically created by the system.
+        # Indicates that the consumer group was automatically created by the system.
         self.automatically_created_group = automatically_created_group
-        # The ID of the consumer group.
+        # The consumer group ID.
         self.consumer_id = consumer_id
         # The instance ID.
         self.instance_id = instance_id
-        # The region ID.
+        # The ID of the region where the instance resides.
         self.region_id = region_id
-        # The description of the consumer group.
+        # The instance description.
         self.remark = remark
         # The tags.
         self.tags = tags
 
     def validate(self):
         if self.tags:
             self.tags.validate()
@@ -4479,22 +4510,25 @@
         success: bool = None,
         total: int = None,
     ):
         # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
         self.code = code
         # The consumer groups.
         self.consumer_list = consumer_list
+        # The number of the page to return. Pages start from page 1.
         self.current_page = current_page
         # The returned message.
         self.message = message
+        # The number of entries returned per page.
         self.page_size = page_size
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request is successful.
         self.success = success
+        # The total number of entries returned.
         self.total = total
 
     def validate(self):
         if self.consumer_list:
             self.consumer_list.validate()
 
     def to_map(self):
@@ -4632,19 +4666,25 @@
         generation: int = None,
         group_id: str = None,
         last_rebalance_timestamp: int = None,
         reason: str = None,
         rebalance_success: bool = None,
         rebalance_time_consuming: int = None,
     ):
+        # The number of rebalances.
         self.generation = generation
+        # The group ID of the subscriber.
         self.group_id = group_id
+        # The time when the last rebalance occurred. Unit: milliseconds.
         self.last_rebalance_timestamp = last_rebalance_timestamp
+        # The cause of the rebalance.
         self.reason = reason
+        # Indicates whether new members are added to the consumer group in the rebalance.
         self.rebalance_success = rebalance_success
+        # The duration of the rebalance. Unit: milliseconds.
         self.rebalance_time_consuming = rebalance_time_consuming
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4728,15 +4768,15 @@
     ):
         # The latest offset in the partition of the topic.
         self.broker_offset = broker_offset
         # The consumer offset in the partition of the topic.
         self.consumer_offset = consumer_offset
         # The time when the last consumed message in the partition was generated.
         self.last_timestamp = last_timestamp
-        # The ID of the partition.
+        # The partition ID.
         self.partition = partition
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4808,19 +4848,19 @@
         last_timestamp: int = None,
         offset_list: GetConsumerProgressResponseBodyConsumerProgressTopicListTopicListOffsetList = None,
         topic: str = None,
         total_diff: int = None,
     ):
         # The time when the last consumed message in the topic was generated.
         self.last_timestamp = last_timestamp
-        # The information about offsets in the topic.
+        # The consumer offsets.
         self.offset_list = offset_list
-        # The name of the topic.
+        # The topic name.
         self.topic = topic
-        # The number of messages that were not consumed in the topic. This is also known as the number of accumulated messages in the topic.
+        # The number of unconsumed messages in the topic to which the consumer group subscribes.
         self.total_diff = total_diff
 
     def validate(self):
         if self.offset_list:
             self.offset_list.validate()
 
     def to_map(self):
@@ -4894,18 +4934,19 @@
         last_timestamp: int = None,
         rebalance_info_list: GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoList = None,
         topic_list: GetConsumerProgressResponseBodyConsumerProgressTopicList = None,
         total_diff: int = None,
     ):
         # The time when the last message consumed by the consumer group was generated.
         self.last_timestamp = last_timestamp
+        # The details of rebalances in the consumer group.
         self.rebalance_info_list = rebalance_info_list
-        # The consumption progress of each topic to which the consumer group is subscribed.
+        # The consumer progress of each topic to which the consumer group subscribes.
         self.topic_list = topic_list
-        # The number of messages that were not consumed in all topics. This is also known as the number of accumulated messages in all topics.
+        # The total number of unconsumed messages in all topics to which the consumer group subscribes.
         self.total_diff = total_diff
 
     def validate(self):
         if self.rebalance_info_list:
             self.rebalance_info_list.validate()
         if self.topic_list:
             self.topic_list.validate()
@@ -4946,21 +4987,21 @@
         self,
         code: int = None,
         consumer_progress: GetConsumerProgressResponseBodyConsumerProgress = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
+        # The returned HTTP status code. If the request is successful, 200 is returned.
         self.code = code
-        # The consumption status of the consumer group.
+        # The consumer progress of the consumer group.
         self.consumer_progress = consumer_progress
         # The returned message.
         self.message = message
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
         # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.consumer_progress:
             self.consumer_progress.validate()
@@ -5084,24 +5125,26 @@
 class GetInstanceListRequest(TeaModel):
     def __init__(
         self,
         instance_id: List[str] = None,
         order_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
+        series: str = None,
         tag: List[GetInstanceListRequestTag] = None,
     ):
         # The IDs of instances.
         self.instance_id = instance_id
         # The ID of the order. You can obtain the order ID on the [Orders](https://usercenter2-intl.aliyun.com/order/list?pageIndex=1\&pageSize=20\&spm=5176.12818093.top-nav.ditem-ord.36f016d0OQFmJa) page in Alibaba Cloud User Center.
         self.order_id = order_id
         # The ID of the region where the instance resides.
         self.region_id = region_id
         # The ID of the resource group. You can obtain this ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id
+        self.series = series
         # The tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -5117,14 +5160,16 @@
             result['InstanceId'] = self.instance_id
         if self.order_id is not None:
             result['OrderId'] = self.order_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        if self.series is not None:
+            result['Series'] = self.series
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
@@ -5133,14 +5178,16 @@
             self.instance_id = m.get('InstanceId')
         if m.get('OrderId') is not None:
             self.order_id = m.get('OrderId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('Series') is not None:
+            self.series = m.get('Series')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = GetInstanceListRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
@@ -5396,14 +5443,15 @@
         paid_type: int = None,
         region_id: str = None,
         reserved_publish_capacity: int = None,
         reserved_subscribe_capacity: int = None,
         resource_group_id: str = None,
         sasl_domain_endpoint: str = None,
         security_group: str = None,
+        series: str = None,
         service_status: int = None,
         spec_type: str = None,
         ssl_domain_endpoint: str = None,
         ssl_end_point: str = None,
         standard_zone_id: str = None,
         tags: GetInstanceListResponseBodyInstanceListInstanceVOTags = None,
         topic_num_limit: int = None,
@@ -5478,14 +5526,15 @@
         # *   Endpoints in IP address mode: An endpoint in this mode consists of the IP address of the broker and a port number. The format of an endpoint in this mode is `{Broker IP address}:{Port number}`.
         self.sasl_domain_endpoint = sasl_domain_endpoint
         # The security group of the instance.
         # 
         # *   If the instance is deployed by using the ApsaraMQ for Kafka console or calling the [StartInstance](~~157786~~) operation without a security group configured, no value is returned.
         # *   If the instance is deployed by calling the [StartInstance](~~157786~~) operation with a security group configured, the returned value is the configured security group.
         self.security_group = security_group
+        self.series = series
         # The instance status. Valid values:
         # 
         # *   **0**: pending
         # *   **1**: preparing hardware resources
         # *   **2**: initializing
         # *   **3**: starting
         # *   **5**: running
@@ -5595,14 +5644,16 @@
             result['ReservedSubscribeCapacity'] = self.reserved_subscribe_capacity
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.sasl_domain_endpoint is not None:
             result['SaslDomainEndpoint'] = self.sasl_domain_endpoint
         if self.security_group is not None:
             result['SecurityGroup'] = self.security_group
+        if self.series is not None:
+            result['Series'] = self.series
         if self.service_status is not None:
             result['ServiceStatus'] = self.service_status
         if self.spec_type is not None:
             result['SpecType'] = self.spec_type
         if self.ssl_domain_endpoint is not None:
             result['SslDomainEndpoint'] = self.ssl_domain_endpoint
         if self.ssl_end_point is not None:
@@ -5680,14 +5731,16 @@
             self.reserved_subscribe_capacity = m.get('ReservedSubscribeCapacity')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('SaslDomainEndpoint') is not None:
             self.sasl_domain_endpoint = m.get('SaslDomainEndpoint')
         if m.get('SecurityGroup') is not None:
             self.security_group = m.get('SecurityGroup')
+        if m.get('Series') is not None:
+            self.series = m.get('Series')
         if m.get('ServiceStatus') is not None:
             self.service_status = m.get('ServiceStatus')
         if m.get('SpecType') is not None:
             self.spec_type = m.get('SpecType')
         if m.get('SslDomainEndpoint') is not None:
             self.ssl_domain_endpoint = m.get('SslDomainEndpoint')
         if m.get('SslEndPoint') is not None:
@@ -8105,15 +8158,17 @@
 
 class ReopenInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
+        # The instance ID.
         self.instance_id = instance_id
+        # The ID of the region where the instance resides.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8140,17 +8195,21 @@
     def __init__(
         self,
         code: int = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The returned HTTP status code. If the request is successful, 200 is returned.
         self.code = code
+        # The returned message.
         self.message = message
+        # The request ID.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8540,15 +8599,17 @@
 
 class StopInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
+        # The instance ID.
         self.instance_id = instance_id
+        # The ID of the region where the instance resides.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8575,17 +8636,21 @@
     def __init__(
         self,
         code: int = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The returned status code. If the request is successful, 200 is returned.
         self.code = code
+        # The returned message.
         self.message = message
+        # The request ID.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9589,30 +9654,29 @@
         instance_id: str = None,
         region_id: str = None,
         topic: str = None,
         value: str = None,
     ):
         # The key of the topic configuration.
         # 
-        # *   Valid values: retention.hours, max.message.bytes, and replications.
-        # *   retention.hours specifies the message retention period.
-        # *   max.message.bytes specifies the maximum size of a sent message.
-        # *   replications specifies the number of topic replicas.
+        # *   ApsaraMQ for Kafka V2 instances allow you to modify configurations only for topics that use local storage.
+        # *   ApsaraMQ for Kafka V3 instances allow you to modify configurations for all topics.
+        # *   The following keys are supported by `local topic` of ApsaraMQ for Kafka V2 instances: retention.ms, retention.bytes, and replications.
+        # *   The following keys are supported by ApsaraMQ for Kafka V3 instances: retention.hours and max.message.bytes.
         self.config = config
         # The instance ID.
         self.instance_id = instance_id
         # The ID of the region where the instance resides.
         self.region_id = region_id
         # The topic name.
         self.topic = topic
         # The value of the topic configuration.
         # 
-        # *   retention.hours specifies the message retention period. The value is a string. Valid values: 24 to 8760.
-        # *   max.message.bytes specifies the maximum size of a sent message. The value is a string. Valid values: 1048576 to 10485760.
-        # *   replications specifies the number of topic replicas. The value is a string. Valid values: 1 to 3.
+        # *   `retention.hours` specifies the message retention period. Value type: string. Valid values: 24 to 8760.
+        # *   `max.message.bytes` specifies the maximum size of a sent message. Value type: string. Valid values: 1048576 to 10485760.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9883,15 +9947,17 @@
 
 class UpgradePostPayOrderRequestServerlessConfig(TeaModel):
     def __init__(
         self,
         reserved_publish_capacity: int = None,
         reserved_subscribe_capacity: int = None,
     ):
+        # The traffic reserved for message publishing. Unit: MB/s. Valid values: 1 to 31457280. You can specify only integers for this parameter.
         self.reserved_publish_capacity = reserved_publish_capacity
+        # The traffic reserved for message subscription. Unit: MB/s. Valid values: 1 to 31457280. You can specify only integers for this parameter.
         self.reserved_subscribe_capacity = reserved_subscribe_capacity
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9928,65 +9994,89 @@
         serverless_config: UpgradePostPayOrderRequestServerlessConfig = None,
         spec_type: str = None,
         topic_quota: int = None,
     ):
         # The disk size. Unit: GB.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.disk_size = disk_size
         # The Internet traffic for the instance.
         # 
-        # *   The Internet traffic volume that you specify must be greater than or equal to the current Internet traffic volume of the instance.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
-        # > - If the **EipModel** parameter is set to **true**, set the **EipMax** parameter to a value that is greater than 0.
-        # > - If the **EipModel** parameter is set to **false**, set the **EipMax** parameter to **0**.
+        # *   The Internet traffic that you specify must be greater than or equal to the current Internet traffic of the instance.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # > 
+        # 
+        # *   If you set **EipModel** to **true**, set **EipMax** to a value that is greater than 0.
+        # 
+        # *   If you set **EipModel** to **false**, set **EipMax** to **0**.
+        # 
+        # *   When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.eip_max = eip_max
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model
         # The instance ID.
         self.instance_id = instance_id
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic that you specify must be greater than or equal to the current maximum traffic of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec
         # The number of partitions. We recommend that you configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.partition_num = partition_num
         # The region ID of the instance.
         self.region_id = region_id
+        # The parameters configured for the Serverless instance. When you create an ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
         self.serverless_config = serverless_config
-        # The edition of the instance. Valid values:
+        # The instance edition.
         # 
-        # *   **normal**: Standard Edition (High Write)
-        # *   **professional**: Professional Edition (High Write)
-        # *   **professionalForHighRead**: Professional Edition (High Read)
+        # Valid values for this parameter if you set PaidType to 1:
+        # 
+        # *   normal: Standard Edition (High Write)
+        # *   professional: Professional Edition (High Write)
+        # *   professionalForHighRead: Professional Edition (High Read)
+        # 
+        # Valid values for this parameter if you set PaidType to 3:
         # 
-        # You cannot downgrade an instance from the Professional Edition to the Standard Edition. For more information about these instance editions, see [Billing](~~84737~~).
+        # *   normal: Serverless Standard Edition
+        # *   professional: Serverless Professional Edition
+        # 
+        # For more information, see [Billing](~~84737~~).
         self.spec_type = spec_type
         # The number of topics. We recommend that you do not configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   The default value of TopicQuota varies based on the value of IoMaxSpec. If the number of topics that you consume exceeds the default value, you are charged additional fees.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.topic_quota = topic_quota
 
     def validate(self):
         if self.serverless_config:
             self.serverless_config.validate()
 
     def to_map(self):
@@ -10061,65 +10151,89 @@
         serverless_config_shrink: str = None,
         spec_type: str = None,
         topic_quota: int = None,
     ):
         # The disk size. Unit: GB.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.disk_size = disk_size
         # The Internet traffic for the instance.
         # 
-        # *   The Internet traffic volume that you specify must be greater than or equal to the current Internet traffic volume of the instance.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
-        # > - If the **EipModel** parameter is set to **true**, set the **EipMax** parameter to a value that is greater than 0.
-        # > - If the **EipModel** parameter is set to **false**, set the **EipMax** parameter to **0**.
+        # *   The Internet traffic that you specify must be greater than or equal to the current Internet traffic of the instance.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # > 
+        # 
+        # *   If you set **EipModel** to **true**, set **EipMax** to a value that is greater than 0.
+        # 
+        # *   If you set **EipModel** to **false**, set **EipMax** to **0**.
+        # 
+        # *   When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.eip_max = eip_max
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model
         # The instance ID.
         self.instance_id = instance_id
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic that you specify must be greater than or equal to the current maximum traffic of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec
         # The number of partitions. We recommend that you configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.partition_num = partition_num
         # The region ID of the instance.
         self.region_id = region_id
+        # The parameters configured for the Serverless instance. When you create an ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
         self.serverless_config_shrink = serverless_config_shrink
-        # The edition of the instance. Valid values:
+        # The instance edition.
         # 
-        # *   **normal**: Standard Edition (High Write)
-        # *   **professional**: Professional Edition (High Write)
-        # *   **professionalForHighRead**: Professional Edition (High Read)
+        # Valid values for this parameter if you set PaidType to 1:
         # 
-        # You cannot downgrade an instance from the Professional Edition to the Standard Edition. For more information about these instance editions, see [Billing](~~84737~~).
+        # *   normal: Standard Edition (High Write)
+        # *   professional: Professional Edition (High Write)
+        # *   professionalForHighRead: Professional Edition (High Read)
+        # 
+        # Valid values for this parameter if you set PaidType to 3:
+        # 
+        # *   normal: Serverless Standard Edition
+        # *   professional: Serverless Professional Edition
+        # 
+        # For more information, see [Billing](~~84737~~).
         self.spec_type = spec_type
         # The number of topics. We recommend that you do not configure this parameter.
         # 
-        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
-        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
-        # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure one of PartitionNum and TopicQuota. We recommend that you configure only ParittionNum.
+        # *   If you configure PartitionNum and TopicQuota at the same time, the system verifies whether the price of the partitions equals the price of the topics based on the previous topic-based selling mode. If the price of the partitions does not equal the price of the topics, an error is returned. If the price of the partitions equals the price of the topics, the instance is purchased based on the partition number.
+        # *   The default value of TopicQuota varies based on the value of IoMaxSpec. If the number of topics that you consume exceeds the default value, you are charged additional fees.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.topic_quota = topic_quota
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916-2.6.6/alibabacloud_alikafka20190916.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916
-Version: 2.6.5
+Version: 2.6.6
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.5/setup.py` & `alibabacloud_alikafka20190916-2.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916.
 
-Created on 11/04/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python"
```

