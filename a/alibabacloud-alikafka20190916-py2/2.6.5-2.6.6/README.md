# Comparing `tmp/alibabacloud_alikafka20190916_py2-2.6.5.tar.gz` & `tmp/alibabacloud_alikafka20190916_py2-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.6.5.tar", last modified: Thu Apr 11 17:09:45 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.6.6.tar", last modified: Tue Apr 23 17:11:06 2024, max compression
```

## Comparing `alibabacloud_alikafka20190916_py2-2.6.5.tar` & `alibabacloud_alikafka20190916_py2-2.6.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/
--rw-r--r--   0 root         (0) root         (0)     6217 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2506 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77934 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   397682 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2506 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/
+-rw-r--r--   0 root         (0) root         (0)     6524 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79117 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   403289 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-23 17:11:06.000000 alibabacloud_alikafka20190916_py2-2.6.6/setup.py
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/ChangeLog.md` & `alibabacloud_alikafka20190916_py2-2.6.6/ChangeLog.md`

 * *Files 2% similar despite different names*

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

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/LICENSE` & `alibabacloud_alikafka20190916_py2-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916_py2
-Version: 2.6.5
+Version: 2.6.6
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/README-CN.md` & `alibabacloud_alikafka20190916_py2-2.6.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/README.md` & `alibabacloud_alikafka20190916_py2-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -887,14 +887,16 @@
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
@@ -1255,14 +1257,24 @@
 
         @return: ReleaseInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.release_instance_with_options(request, runtime)
 
     def reopen_instance_with_options(self, request, runtime):
+        """
+        You can call this operation only if your instance is in the Stopped state.
+        
+
+        @param request: ReopenInstanceRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ReopenInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1281,14 +1293,22 @@
         )
         return TeaCore.from_map(
             alikafka_20190916_models.ReopenInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def reopen_instance(self, request):
+        """
+        You can call this operation only if your instance is in the Stopped state.
+        
+
+        @param request: ReopenInstanceRequest
+
+        @return: ReopenInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reopen_instance_with_options(request, runtime)
 
     def start_instance_with_options(self, request, runtime):
         """
         >  You can call this operation up to twice per second.
         
@@ -1371,14 +1391,24 @@
 
         @return: StartInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_instance_with_options(request, runtime)
 
     def stop_instance_with_options(self, request, runtime):
+        """
+        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        
+
+        @param request: StopInstanceRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: StopInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
@@ -1397,14 +1427,22 @@
         )
         return TeaCore.from_map(
             alikafka_20190916_models.StopInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def stop_instance(self, request):
+        """
+        You cannot stop a subscription ApsaraMQ for Kafka instance. If you want to stop a subscription ApsaraMQ for Kafka instance, submit a ticket.
+        
+
+        @param request: StopInstanceRequest
+
+        @return: StopInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_instance_with_options(request, runtime)
 
     def tag_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1670,14 +1670,22 @@
         return self
 
 
 class CreateSaslUserRequest(TeaModel):
     def __init__(self, instance_id=None, mechanism=None, password=None, region_id=None, type=None, username=None):
         # The instance ID.
         self.instance_id = instance_id  # type: str
+        # The encryption method. Valid values:
+        # 
+        # *   SCRAM-SHA-512 (default)
+        # *   SCRAM-SHA-256
+        # 
+        # > 
+        # 
+        # *   This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.mechanism = mechanism  # type: str
         # The password of the SASL user.
         self.password = password  # type: str
         # The region ID.
         self.region_id = region_id  # type: str
         # The SASL mechanism. Valid values:
         # 
@@ -2050,36 +2058,57 @@
         return self
 
 
 class DeleteAclRequest(TeaModel):
     def __init__(self, acl_operation_type=None, acl_operation_types=None, acl_permission_type=None,
                  acl_resource_name=None, acl_resource_pattern_type=None, acl_resource_type=None, host=None, instance_id=None,
                  region_id=None, username=None):
-        # The operation type. Valid values:
+        # The operation allowed by the access control list (ACL). Valid values:
         # 
-        # *   **Write**\
-        # *   **Read**\
+        # *   **Write**: data writes
+        # *   **Read**: data reads
+        # *   **Describe**: reads of transactional IDs
+        # *   **IdempotentWrite**: idempotent data writes to clusters
         self.acl_operation_type = acl_operation_type  # type: str
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
         self.acl_operation_types = acl_operation_types  # type: str
+        # The authorization method. Valid values:
+        # 
+        # *   Deny
+        # *   ALLOW
+        # 
+        # >  This parameter is available only for ApsaraMQ for Kafka V3 serverless instances.
         self.acl_permission_type = acl_permission_type  # type: str
         # The name of the resource.
         # 
         # *   The value can be the name of a topic or consumer group.
         # *   You can use an asterisk (\*) to indicate the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name  # type: str
         # The mode that is used to match resources. Valid values:
         # 
         # *   **LITERAL:** full match
         # *   **PREFIXED**: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type  # type: str
-        # The type of the resource.
+        # The resource type. Valid values:
         # 
-        # *   **Topic**\
-        # *   **Group**\
+        # *   **Topic**: topic
+        # *   **Group**: consumer group
+        # *   **Cluster**: cluster
+        # *   **TransactionalId**: transactional ID
         self.acl_resource_type = acl_resource_type  # type: str
+        # The IP address of the source.
         self.host = host  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The ID of the region.
         self.region_id = region_id  # type: str
         # The name of the user.
         self.username = username  # type: str
@@ -3778,17 +3807,19 @@
         return self
 
 
 class GetConsumerListRequest(TeaModel):
     def __init__(self, consumer_id=None, current_page=None, instance_id=None, page_size=None, region_id=None):
         # The name of the consumer group. If you do not configure this parameter, all consumer groups are queried.
         self.consumer_id = consumer_id  # type: str
+        # The page number.
         self.current_page = current_page  # type: int
         # The ID of the instance to which the consumer group belongs.
         self.instance_id = instance_id  # type: str
+        # The number of entries to be returned per page.
         self.page_size = page_size  # type: int
         # The region ID of the instance to which the consumer group belongs.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
@@ -3887,23 +3918,23 @@
                 self.tag_vo.append(temp_model.from_map(k))
         return self
 
 
 class GetConsumerListResponseBodyConsumerListConsumerVO(TeaModel):
     def __init__(self, automatically_created_group=None, consumer_id=None, instance_id=None, region_id=None,
                  remark=None, tags=None):
-        # The consumer group that is automatically created by the system.
+        # Indicates that the consumer group was automatically created by the system.
         self.automatically_created_group = automatically_created_group  # type: bool
-        # The ID of the consumer group.
+        # The consumer group ID.
         self.consumer_id = consumer_id  # type: str
         # The instance ID.
         self.instance_id = instance_id  # type: str
-        # The region ID.
+        # The ID of the region where the instance resides.
         self.region_id = region_id  # type: str
-        # The description of the consumer group.
+        # The instance description.
         self.remark = remark  # type: str
         # The tags.
         self.tags = tags  # type: GetConsumerListResponseBodyConsumerListConsumerVOTags
 
     def validate(self):
         if self.tags:
             self.tags.validate()
@@ -3981,22 +4012,25 @@
 class GetConsumerListResponseBody(TeaModel):
     def __init__(self, code=None, consumer_list=None, current_page=None, message=None, page_size=None,
                  request_id=None, success=None, total=None):
         # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
         self.code = code  # type: int
         # The consumer groups.
         self.consumer_list = consumer_list  # type: GetConsumerListResponseBodyConsumerList
+        # The number of the page to return. Pages start from page 1.
         self.current_page = current_page  # type: int
         # The returned message.
         self.message = message  # type: str
+        # The number of entries returned per page.
         self.page_size = page_size  # type: int
         # The ID of the request.
         self.request_id = request_id  # type: str
         # Indicates whether the request is successful.
         self.success = success  # type: bool
+        # The total number of entries returned.
         self.total = total  # type: long
 
     def validate(self):
         if self.consumer_list:
             self.consumer_list.validate()
 
     def to_map(self):
@@ -4117,19 +4151,25 @@
             self.region_id = m.get('RegionId')
         return self
 
 
 class GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList(TeaModel):
     def __init__(self, generation=None, group_id=None, last_rebalance_timestamp=None, reason=None,
                  rebalance_success=None, rebalance_time_consuming=None):
+        # The number of rebalances.
         self.generation = generation  # type: long
+        # The group ID of the subscriber.
         self.group_id = group_id  # type: str
+        # The time when the last rebalance occurred. Unit: milliseconds.
         self.last_rebalance_timestamp = last_rebalance_timestamp  # type: long
+        # The cause of the rebalance.
         self.reason = reason  # type: str
+        # Indicates whether new members are added to the consumer group in the rebalance.
         self.rebalance_success = rebalance_success  # type: bool
+        # The duration of the rebalance. Unit: milliseconds.
         self.rebalance_time_consuming = rebalance_time_consuming  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList, self).to_map()
@@ -4204,15 +4244,15 @@
     def __init__(self, broker_offset=None, consumer_offset=None, last_timestamp=None, partition=None):
         # The latest offset in the partition of the topic.
         self.broker_offset = broker_offset  # type: long
         # The consumer offset in the partition of the topic.
         self.consumer_offset = consumer_offset  # type: long
         # The time when the last consumed message in the partition was generated.
         self.last_timestamp = last_timestamp  # type: long
-        # The ID of the partition.
+        # The partition ID.
         self.partition = partition  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetConsumerProgressResponseBodyConsumerProgressTopicListTopicListOffsetListOffsetList, self).to_map()
@@ -4275,19 +4315,19 @@
         return self
 
 
 class GetConsumerProgressResponseBodyConsumerProgressTopicListTopicList(TeaModel):
     def __init__(self, last_timestamp=None, offset_list=None, topic=None, total_diff=None):
         # The time when the last consumed message in the topic was generated.
         self.last_timestamp = last_timestamp  # type: long
-        # The information about offsets in the topic.
+        # The consumer offsets.
         self.offset_list = offset_list  # type: GetConsumerProgressResponseBodyConsumerProgressTopicListTopicListOffsetList
-        # The name of the topic.
+        # The topic name.
         self.topic = topic  # type: str
-        # The number of messages that were not consumed in the topic. This is also known as the number of accumulated messages in the topic.
+        # The number of unconsumed messages in the topic to which the consumer group subscribes.
         self.total_diff = total_diff  # type: long
 
     def validate(self):
         if self.offset_list:
             self.offset_list.validate()
 
     def to_map(self):
@@ -4352,18 +4392,19 @@
         return self
 
 
 class GetConsumerProgressResponseBodyConsumerProgress(TeaModel):
     def __init__(self, last_timestamp=None, rebalance_info_list=None, topic_list=None, total_diff=None):
         # The time when the last message consumed by the consumer group was generated.
         self.last_timestamp = last_timestamp  # type: long
+        # The details of rebalances in the consumer group.
         self.rebalance_info_list = rebalance_info_list  # type: GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoList
-        # The consumption progress of each topic to which the consumer group is subscribed.
+        # The consumer progress of each topic to which the consumer group subscribes.
         self.topic_list = topic_list  # type: GetConsumerProgressResponseBodyConsumerProgressTopicList
-        # The number of messages that were not consumed in all topics. This is also known as the number of accumulated messages in all topics.
+        # The total number of unconsumed messages in all topics to which the consumer group subscribes.
         self.total_diff = total_diff  # type: long
 
     def validate(self):
         if self.rebalance_info_list:
             self.rebalance_info_list.validate()
         if self.topic_list:
             self.topic_list.validate()
@@ -4397,21 +4438,21 @@
         if m.get('TotalDiff') is not None:
             self.total_diff = m.get('TotalDiff')
         return self
 
 
 class GetConsumerProgressResponseBody(TeaModel):
     def __init__(self, code=None, consumer_progress=None, message=None, request_id=None, success=None):
-        # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
+        # The returned HTTP status code. If the request is successful, 200 is returned.
         self.code = code  # type: int
-        # The consumption status of the consumer group.
+        # The consumer progress of the consumer group.
         self.consumer_progress = consumer_progress  # type: GetConsumerProgressResponseBodyConsumerProgress
         # The returned message.
         self.message = message  # type: str
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
         # Indicates whether the request is successful.
         self.success = success  # type: bool
 
     def validate(self):
         if self.consumer_progress:
             self.consumer_progress.validate()
@@ -4520,23 +4561,25 @@
             self.key = m.get('Key')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class GetInstanceListRequest(TeaModel):
-    def __init__(self, instance_id=None, order_id=None, region_id=None, resource_group_id=None, tag=None):
+    def __init__(self, instance_id=None, order_id=None, region_id=None, resource_group_id=None, series=None,
+                 tag=None):
         # The IDs of instances.
         self.instance_id = instance_id  # type: list[str]
         # The ID of the order. You can obtain the order ID on the [Orders](https://usercenter2-intl.aliyun.com/order/list?pageIndex=1\&pageSize=20\&spm=5176.12818093.top-nav.ditem-ord.36f016d0OQFmJa) page in Alibaba Cloud User Center.
         self.order_id = order_id  # type: str
         # The ID of the region where the instance resides.
         self.region_id = region_id  # type: str
         # The ID of the resource group. You can obtain this ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id  # type: str
+        self.series = series  # type: str
         # The tags.
         self.tag = tag  # type: list[GetInstanceListRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -4552,14 +4595,16 @@
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
 
     def from_map(self, m=None):
@@ -4568,14 +4613,16 @@
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
 
@@ -4781,18 +4828,19 @@
 
 
 class GetInstanceListResponseBodyInstanceListInstanceVO(TeaModel):
     def __init__(self, all_config=None, confluent_config=None, create_time=None, deploy_type=None, disk_size=None,
                  disk_type=None, domain_endpoint=None, eip_max=None, end_point=None, expired_time=None, instance_id=None,
                  io_max=None, io_max_read=None, io_max_spec=None, io_max_write=None, kms_key_id=None, msg_retain=None,
                  name=None, paid_type=None, region_id=None, reserved_publish_capacity=None,
-                 reserved_subscribe_capacity=None, resource_group_id=None, sasl_domain_endpoint=None, security_group=None, service_status=None,
-                 spec_type=None, ssl_domain_endpoint=None, ssl_end_point=None, standard_zone_id=None, tags=None,
-                 topic_num_limit=None, upgrade_service_detail_info=None, used_group_count=None, used_partition_count=None,
-                 used_topic_count=None, v_switch_id=None, view_instance_status_code=None, vpc_id=None, zone_id=None):
+                 reserved_subscribe_capacity=None, resource_group_id=None, sasl_domain_endpoint=None, security_group=None, series=None,
+                 service_status=None, spec_type=None, ssl_domain_endpoint=None, ssl_end_point=None, standard_zone_id=None,
+                 tags=None, topic_num_limit=None, upgrade_service_detail_info=None, used_group_count=None,
+                 used_partition_count=None, used_topic_count=None, v_switch_id=None, view_instance_status_code=None, vpc_id=None,
+                 zone_id=None):
         # The configurations of the deployed ApsaraMQ for Kafka instance.
         self.all_config = all_config  # type: str
         self.confluent_config = confluent_config  # type: GetInstanceListResponseBodyInstanceListInstanceVOConfluentConfig
         # The time when the instance was created. Unit: milliseconds.
         self.create_time = create_time  # type: long
         # The type of the network in which the instance is deployed. Valid values:
         # 
@@ -4851,14 +4899,15 @@
         # *   Endpoints in IP address mode: An endpoint in this mode consists of the IP address of the broker and a port number. The format of an endpoint in this mode is `{Broker IP address}:{Port number}`.
         self.sasl_domain_endpoint = sasl_domain_endpoint  # type: str
         # The security group of the instance.
         # 
         # *   If the instance is deployed by using the ApsaraMQ for Kafka console or calling the [StartInstance](~~157786~~) operation without a security group configured, no value is returned.
         # *   If the instance is deployed by calling the [StartInstance](~~157786~~) operation with a security group configured, the returned value is the configured security group.
         self.security_group = security_group  # type: str
+        self.series = series  # type: str
         # The instance status. Valid values:
         # 
         # *   **0**: pending
         # *   **1**: preparing hardware resources
         # *   **2**: initializing
         # *   **3**: starting
         # *   **5**: running
@@ -4968,14 +5017,16 @@
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
@@ -5053,14 +5104,16 @@
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
@@ -7205,15 +7258,17 @@
             temp_model = ReleaseInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ReopenInstanceRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None):
+        # The instance ID.
         self.instance_id = instance_id  # type: str
+        # The ID of the region where the instance resides.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ReopenInstanceRequest, self).to_map()
@@ -7234,17 +7289,21 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class ReopenInstanceResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None, success=None):
+        # The returned HTTP status code. If the request is successful, 200 is returned.
         self.code = code  # type: int
+        # The returned message.
         self.message = message  # type: str
+        # The request ID.
         self.request_id = request_id  # type: str
+        # Indicates whether the request is successful.
         self.success = success  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ReopenInstanceResponseBody, self).to_map()
@@ -7594,15 +7653,17 @@
             temp_model = StartInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class StopInstanceRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None):
+        # The instance ID.
         self.instance_id = instance_id  # type: str
+        # The ID of the region where the instance resides.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StopInstanceRequest, self).to_map()
@@ -7623,17 +7684,21 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class StopInstanceResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None, success=None):
+        # The returned status code. If the request is successful, 200 is returned.
         self.code = code  # type: int
+        # The returned message.
         self.message = message  # type: str
+        # The request ID.
         self.request_id = request_id  # type: str
+        # Indicates whether the request is successful.
         self.success = success  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StopInstanceResponseBody, self).to_map()
@@ -8525,30 +8590,29 @@
         return self
 
 
 class UpdateTopicConfigRequest(TeaModel):
     def __init__(self, config=None, instance_id=None, region_id=None, topic=None, value=None):
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
         self.config = config  # type: str
         # The instance ID.
         self.instance_id = instance_id  # type: str
         # The ID of the region where the instance resides.
         self.region_id = region_id  # type: str
         # The topic name.
         self.topic = topic  # type: str
         # The value of the topic configuration.
         # 
-        # *   retention.hours specifies the message retention period. The value is a string. Valid values: 24 to 8760.
-        # *   max.message.bytes specifies the maximum size of a sent message. The value is a string. Valid values: 1048576 to 10485760.
-        # *   replications specifies the number of topic replicas. The value is a string. Valid values: 1 to 3.
+        # *   `retention.hours` specifies the message retention period. Value type: string. Valid values: 24 to 8760.
+        # *   `max.message.bytes` specifies the maximum size of a sent message. Value type: string. Valid values: 1048576 to 10485760.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateTopicConfigRequest, self).to_map()
@@ -8787,15 +8851,17 @@
             temp_model = UpgradeInstanceVersionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpgradePostPayOrderRequestServerlessConfig(TeaModel):
     def __init__(self, reserved_publish_capacity=None, reserved_subscribe_capacity=None):
+        # The traffic reserved for message publishing. Unit: MB/s. Valid values: 1 to 31457280. You can specify only integers for this parameter.
         self.reserved_publish_capacity = reserved_publish_capacity  # type: long
+        # The traffic reserved for message subscription. Unit: MB/s. Valid values: 1 to 31457280. You can specify only integers for this parameter.
         self.reserved_subscribe_capacity = reserved_subscribe_capacity  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpgradePostPayOrderRequestServerlessConfig, self).to_map()
@@ -8820,65 +8886,89 @@
 
 class UpgradePostPayOrderRequest(TeaModel):
     def __init__(self, disk_size=None, eip_max=None, eip_model=None, instance_id=None, io_max=None, io_max_spec=None,
                  partition_num=None, region_id=None, serverless_config=None, spec_type=None, topic_quota=None):
         # The disk size. Unit: GB.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.disk_size = disk_size  # type: int
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
         self.eip_max = eip_max  # type: int
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model  # type: bool
         # The instance ID.
         self.instance_id = instance_id  # type: str
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic that you specify must be greater than or equal to the current maximum traffic of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max = io_max  # type: int
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec  # type: str
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
         self.partition_num = partition_num  # type: int
         # The region ID of the instance.
         self.region_id = region_id  # type: str
+        # The parameters configured for the Serverless instance. When you create an ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
         self.serverless_config = serverless_config  # type: UpgradePostPayOrderRequestServerlessConfig
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
         self.spec_type = spec_type  # type: str
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
         self.topic_quota = topic_quota  # type: int
 
     def validate(self):
         if self.serverless_config:
             self.serverless_config.validate()
 
     def to_map(self):
@@ -8941,65 +9031,89 @@
 
 class UpgradePostPayOrderShrinkRequest(TeaModel):
     def __init__(self, disk_size=None, eip_max=None, eip_model=None, instance_id=None, io_max=None, io_max_spec=None,
                  partition_num=None, region_id=None, serverless_config_shrink=None, spec_type=None, topic_quota=None):
         # The disk size. Unit: GB.
         # 
         # *   The disk size that you specify must be greater than or equal to the current disk size of the instance.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.disk_size = disk_size  # type: int
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
         self.eip_max = eip_max  # type: int
         # Specifies whether to enable Internet access for the instance. Valid values:
         # 
         # *   true: enables Internet access.
         # *   false: disables Internet access.
         self.eip_model = eip_model  # type: bool
         # The instance ID.
         self.instance_id = instance_id  # type: str
         # The maximum traffic for the instance. We recommend that you do not configure this parameter.
         # 
         # *   The maximum traffic that you specify must be greater than or equal to the current maximum traffic of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max = io_max  # type: int
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   The traffic specification that you specify must be greater than or equal to the current traffic specification of the instance.
-        # *   You must configure at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
-        # *   For more information about the valid values, see [Billing](~~84737~~).
+        # *   You must configure at least one of IoMax and IoMaxSpec. If you configure both parameters, the value of IoMaxSpec takes effect. We recommend that you configure only IoMaxSpec.
+        # *   For information about the valid values of this parameter, see [Billing](~~84737~~).
+        # 
+        # >  When you create an ApsaraMQ for Kafka V3 serverless instance, you do not need to configure this parameter.
         self.io_max_spec = io_max_spec  # type: str
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
         self.partition_num = partition_num  # type: int
         # The region ID of the instance.
         self.region_id = region_id  # type: str
+        # The parameters configured for the Serverless instance. When you create an ApsaraMQ for Kafka V3 serverless instance, you must configure these parameters.
         self.serverless_config_shrink = serverless_config_shrink  # type: str
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
         self.spec_type = spec_type  # type: str
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
         self.topic_quota = topic_quota  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpgradePostPayOrderShrinkRequest, self).to_map()
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.6.6/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916-py2
-Version: 2.6.5
+Version: 2.6.6
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.5/setup.py` & `alibabacloud_alikafka20190916_py2-2.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916_py2.
 
-Created on 11/04/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2"
```

