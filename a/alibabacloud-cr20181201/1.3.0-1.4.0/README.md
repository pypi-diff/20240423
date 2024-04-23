# Comparing `tmp/alibabacloud_cr20181201-1.3.0.tar.gz` & `tmp/alibabacloud_cr20181201-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cr20181201-1.3.0.tar", last modified: Thu Apr 11 06:06:11 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cr20181201-1.4.0.tar", last modified: Tue Apr 23 17:11:48 2024, max compression
```

## Comparing `alibabacloud_cr20181201-1.3.0.tar` & `alibabacloud_cr20181201-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      794 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316752 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/client.py
--rw-r--r--   0 root         (0) root         (0)   597292 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2606 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334114 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201/client.py
+-rw-r--r--   0 root         (0) root         (0)   626357 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-23 17:11:48.000000 alibabacloud_cr20181201-1.4.0/setup.py
```

### Comparing `alibabacloud_cr20181201-1.3.0/LICENSE` & `alibabacloud_cr20181201-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201-1.3.0/PKG-INFO` & `alibabacloud_cr20181201-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cr20181201
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cr20181201-1.3.0/README-CN.md` & `alibabacloud_cr20181201-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201-1.3.0/README.md` & `alibabacloud_cr20181201-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/client.py` & `alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,14 +391,116 @@
         
         @param request: CreateArtifactBuildRuleRequest
         @return: CreateArtifactBuildRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_artifact_build_rule_with_options_async(request, runtime)
 
+    def create_artifact_lifecycle_rule_with_options(
+        self,
+        request: cr_20181201_models.CreateArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.CreateArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auto):
+            query['Auto'] = request.auto
+        if not UtilClient.is_unset(request.enable_delete_tag):
+            query['EnableDeleteTag'] = request.enable_delete_tag
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.namespace_name):
+            query['NamespaceName'] = request.namespace_name
+        if not UtilClient.is_unset(request.repo_name):
+            query['RepoName'] = request.repo_name
+        if not UtilClient.is_unset(request.retention_tag_count):
+            query['RetentionTagCount'] = request.retention_tag_count
+        if not UtilClient.is_unset(request.schedule_time):
+            query['ScheduleTime'] = request.schedule_time
+        if not UtilClient.is_unset(request.scope):
+            query['Scope'] = request.scope
+        if not UtilClient.is_unset(request.tag_regexp):
+            query['TagRegexp'] = request.tag_regexp
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.CreateArtifactLifecycleRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_artifact_lifecycle_rule_with_options_async(
+        self,
+        request: cr_20181201_models.CreateArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.CreateArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auto):
+            query['Auto'] = request.auto
+        if not UtilClient.is_unset(request.enable_delete_tag):
+            query['EnableDeleteTag'] = request.enable_delete_tag
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.namespace_name):
+            query['NamespaceName'] = request.namespace_name
+        if not UtilClient.is_unset(request.repo_name):
+            query['RepoName'] = request.repo_name
+        if not UtilClient.is_unset(request.retention_tag_count):
+            query['RetentionTagCount'] = request.retention_tag_count
+        if not UtilClient.is_unset(request.schedule_time):
+            query['ScheduleTime'] = request.schedule_time
+        if not UtilClient.is_unset(request.scope):
+            query['Scope'] = request.scope
+        if not UtilClient.is_unset(request.tag_regexp):
+            query['TagRegexp'] = request.tag_regexp
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.CreateArtifactLifecycleRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_artifact_lifecycle_rule(
+        self,
+        request: cr_20181201_models.CreateArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.CreateArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_artifact_lifecycle_rule_with_options(request, runtime)
+
+    async def create_artifact_lifecycle_rule_async(
+        self,
+        request: cr_20181201_models.CreateArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.CreateArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_artifact_lifecycle_rule_with_options_async(request, runtime)
+
     def create_build_record_by_record_with_options(
         self,
         request: cr_20181201_models.CreateBuildRecordByRecordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.CreateBuildRecordByRecordResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1947,14 +2049,88 @@
     async def create_repository_async(
         self,
         request: cr_20181201_models.CreateRepositoryRequest,
     ) -> cr_20181201_models.CreateRepositoryResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_repository_with_options_async(request, runtime)
 
+    def delete_artifact_lifecycle_rule_with_options(
+        self,
+        request: cr_20181201_models.DeleteArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.DeleteArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.DeleteArtifactLifecycleRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_artifact_lifecycle_rule_with_options_async(
+        self,
+        request: cr_20181201_models.DeleteArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.DeleteArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.DeleteArtifactLifecycleRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_artifact_lifecycle_rule(
+        self,
+        request: cr_20181201_models.DeleteArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.DeleteArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_artifact_lifecycle_rule_with_options(request, runtime)
+
+    async def delete_artifact_lifecycle_rule_async(
+        self,
+        request: cr_20181201_models.DeleteArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.DeleteArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_artifact_lifecycle_rule_with_options_async(request, runtime)
+
     def delete_chain_with_options(
         self,
         request: cr_20181201_models.DeleteChainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.DeleteChainResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3171,14 +3347,80 @@
     async def get_artifact_build_task_async(
         self,
         request: cr_20181201_models.GetArtifactBuildTaskRequest,
     ) -> cr_20181201_models.GetArtifactBuildTaskResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_artifact_build_task_with_options_async(request, runtime)
 
+    def get_artifact_lifecycle_rule_with_options(
+        self,
+        request: cr_20181201_models.GetArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.GetArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.GetArtifactLifecycleRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_artifact_lifecycle_rule_with_options_async(
+        self,
+        request: cr_20181201_models.GetArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.GetArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.GetArtifactLifecycleRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_artifact_lifecycle_rule(
+        self,
+        request: cr_20181201_models.GetArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.GetArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_artifact_lifecycle_rule_with_options(request, runtime)
+
+    async def get_artifact_lifecycle_rule_async(
+        self,
+        request: cr_20181201_models.GetArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.GetArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_artifact_lifecycle_rule_with_options_async(request, runtime)
+
     def get_authorization_token_with_options(
         self,
         request: cr_20181201_models.GetAuthorizationTokenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.GetAuthorizationTokenResponse:
         """
         The ID of the Container Registry instance.
@@ -4789,14 +5031,80 @@
     async def list_artifact_build_task_log_async(
         self,
         request: cr_20181201_models.ListArtifactBuildTaskLogRequest,
     ) -> cr_20181201_models.ListArtifactBuildTaskLogResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_artifact_build_task_log_with_options_async(request, runtime)
 
+    def list_artifact_lifecycle_rule_with_options(
+        self,
+        request: cr_20181201_models.ListArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.ListArtifactLifecycleRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_artifact_lifecycle_rule_with_options_async(
+        self,
+        request: cr_20181201_models.ListArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.ListArtifactLifecycleRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_artifact_lifecycle_rule(
+        self,
+        request: cr_20181201_models.ListArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.ListArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_artifact_lifecycle_rule_with_options(request, runtime)
+
+    async def list_artifact_lifecycle_rule_async(
+        self,
+        request: cr_20181201_models.ListArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.ListArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_artifact_lifecycle_rule_with_options_async(request, runtime)
+
     def list_chain_with_options(
         self,
         request: cr_20181201_models.ListChainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.ListChainResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6929,14 +7237,120 @@
     async def untag_resources_async(
         self,
         request: cr_20181201_models.UntagResourcesRequest,
     ) -> cr_20181201_models.UntagResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
 
+    def update_artifact_lifecycle_rule_with_options(
+        self,
+        request: cr_20181201_models.UpdateArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.UpdateArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auto):
+            query['Auto'] = request.auto
+        if not UtilClient.is_unset(request.enable_delete_tag):
+            query['EnableDeleteTag'] = request.enable_delete_tag
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.namespace_name):
+            query['NamespaceName'] = request.namespace_name
+        if not UtilClient.is_unset(request.repo_name):
+            query['RepoName'] = request.repo_name
+        if not UtilClient.is_unset(request.retention_tag_count):
+            query['RetentionTagCount'] = request.retention_tag_count
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        if not UtilClient.is_unset(request.schedule_time):
+            query['ScheduleTime'] = request.schedule_time
+        if not UtilClient.is_unset(request.scope):
+            query['Scope'] = request.scope
+        if not UtilClient.is_unset(request.tag_regexp):
+            query['TagRegexp'] = request.tag_regexp
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.UpdateArtifactLifecycleRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_artifact_lifecycle_rule_with_options_async(
+        self,
+        request: cr_20181201_models.UpdateArtifactLifecycleRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.UpdateArtifactLifecycleRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auto):
+            query['Auto'] = request.auto
+        if not UtilClient.is_unset(request.enable_delete_tag):
+            query['EnableDeleteTag'] = request.enable_delete_tag
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.namespace_name):
+            query['NamespaceName'] = request.namespace_name
+        if not UtilClient.is_unset(request.repo_name):
+            query['RepoName'] = request.repo_name
+        if not UtilClient.is_unset(request.retention_tag_count):
+            query['RetentionTagCount'] = request.retention_tag_count
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        if not UtilClient.is_unset(request.schedule_time):
+            query['ScheduleTime'] = request.schedule_time
+        if not UtilClient.is_unset(request.scope):
+            query['Scope'] = request.scope
+        if not UtilClient.is_unset(request.tag_regexp):
+            query['TagRegexp'] = request.tag_regexp
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateArtifactLifecycleRule',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.UpdateArtifactLifecycleRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_artifact_lifecycle_rule(
+        self,
+        request: cr_20181201_models.UpdateArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.UpdateArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_artifact_lifecycle_rule_with_options(request, runtime)
+
+    async def update_artifact_lifecycle_rule_async(
+        self,
+        request: cr_20181201_models.UpdateArtifactLifecycleRuleRequest,
+    ) -> cr_20181201_models.UpdateArtifactLifecycleRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_artifact_lifecycle_rule_with_options_async(request, runtime)
+
     def update_chain_with_options(
         self,
         request: cr_20181201_models.UpdateChainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.UpdateChainResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/models.py` & `alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,14 +571,175 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateArtifactBuildRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(
+        self,
+        auto: bool = None,
+        enable_delete_tag: bool = None,
+        instance_id: str = None,
+        namespace_name: str = None,
+        repo_name: str = None,
+        retention_tag_count: int = None,
+        schedule_time: str = None,
+        scope: str = None,
+        tag_regexp: str = None,
+    ):
+        self.auto = auto
+        self.enable_delete_tag = enable_delete_tag
+        self.instance_id = instance_id
+        self.namespace_name = namespace_name
+        self.repo_name = repo_name
+        self.retention_tag_count = retention_tag_count
+        self.schedule_time = schedule_time
+        self.scope = scope
+        self.tag_regexp = tag_regexp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto is not None:
+            result['Auto'] = self.auto
+        if self.enable_delete_tag is not None:
+            result['EnableDeleteTag'] = self.enable_delete_tag
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.namespace_name is not None:
+            result['NamespaceName'] = self.namespace_name
+        if self.repo_name is not None:
+            result['RepoName'] = self.repo_name
+        if self.retention_tag_count is not None:
+            result['RetentionTagCount'] = self.retention_tag_count
+        if self.schedule_time is not None:
+            result['ScheduleTime'] = self.schedule_time
+        if self.scope is not None:
+            result['Scope'] = self.scope
+        if self.tag_regexp is not None:
+            result['TagRegexp'] = self.tag_regexp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Auto') is not None:
+            self.auto = m.get('Auto')
+        if m.get('EnableDeleteTag') is not None:
+            self.enable_delete_tag = m.get('EnableDeleteTag')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NamespaceName') is not None:
+            self.namespace_name = m.get('NamespaceName')
+        if m.get('RepoName') is not None:
+            self.repo_name = m.get('RepoName')
+        if m.get('RetentionTagCount') is not None:
+            self.retention_tag_count = m.get('RetentionTagCount')
+        if m.get('ScheduleTime') is not None:
+            self.schedule_time = m.get('ScheduleTime')
+        if m.get('Scope') is not None:
+            self.scope = m.get('Scope')
+        if m.get('TagRegexp') is not None:
+            self.tag_regexp = m.get('TagRegexp')
+        return self
+
+
+class CreateArtifactLifecycleRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        is_success: bool = None,
+        request_id: str = None,
+        rule_id: str = None,
+    ):
+        self.code = code
+        self.is_success = is_success
+        self.request_id = request_id
+        self.rule_id = rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.is_success is not None:
+            result['IsSuccess'] = self.is_success
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('IsSuccess') is not None:
+            self.is_success = m.get('IsSuccess')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class CreateArtifactLifecycleRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateArtifactLifecycleRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateArtifactLifecycleRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateBuildRecordByRecordRequest(TeaModel):
     def __init__(
         self,
         build_record_id: str = None,
         instance_id: str = None,
         repo_id: str = None,
     ):
@@ -3173,14 +3334,127 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateRepositoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        rule_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.rule_id = rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class DeleteArtifactLifecycleRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        is_success: bool = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.is_success = is_success
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.is_success is not None:
+            result['IsSuccess'] = self.is_success
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('IsSuccess') is not None:
+            self.is_success = m.get('IsSuccess')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteArtifactLifecycleRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteArtifactLifecycleRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteArtifactLifecycleRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteChainRequest(TeaModel):
     def __init__(
         self,
         chain_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the delivery pipeline.
@@ -5275,14 +5549,205 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetArtifactBuildTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        rule_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.rule_id = rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class GetArtifactLifecycleRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        auto: bool = None,
+        code: str = None,
+        create_time: int = None,
+        enable_delete_tag: bool = None,
+        instance_id: str = None,
+        is_success: bool = None,
+        modified_time: int = None,
+        namespace_name: str = None,
+        next_time: int = None,
+        repo_name: str = None,
+        request_id: str = None,
+        retention_tag_count: int = None,
+        rule_id: str = None,
+        schedule_time: str = None,
+        scope: str = None,
+        tag_regexp: str = None,
+    ):
+        self.auto = auto
+        self.code = code
+        self.create_time = create_time
+        self.enable_delete_tag = enable_delete_tag
+        self.instance_id = instance_id
+        self.is_success = is_success
+        self.modified_time = modified_time
+        self.namespace_name = namespace_name
+        self.next_time = next_time
+        self.repo_name = repo_name
+        self.request_id = request_id
+        self.retention_tag_count = retention_tag_count
+        self.rule_id = rule_id
+        self.schedule_time = schedule_time
+        self.scope = scope
+        self.tag_regexp = tag_regexp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto is not None:
+            result['Auto'] = self.auto
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.enable_delete_tag is not None:
+            result['EnableDeleteTag'] = self.enable_delete_tag
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.is_success is not None:
+            result['IsSuccess'] = self.is_success
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.namespace_name is not None:
+            result['NamespaceName'] = self.namespace_name
+        if self.next_time is not None:
+            result['NextTime'] = self.next_time
+        if self.repo_name is not None:
+            result['RepoName'] = self.repo_name
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.retention_tag_count is not None:
+            result['RetentionTagCount'] = self.retention_tag_count
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.schedule_time is not None:
+            result['ScheduleTime'] = self.schedule_time
+        if self.scope is not None:
+            result['Scope'] = self.scope
+        if self.tag_regexp is not None:
+            result['TagRegexp'] = self.tag_regexp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Auto') is not None:
+            self.auto = m.get('Auto')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('EnableDeleteTag') is not None:
+            self.enable_delete_tag = m.get('EnableDeleteTag')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('IsSuccess') is not None:
+            self.is_success = m.get('IsSuccess')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('NamespaceName') is not None:
+            self.namespace_name = m.get('NamespaceName')
+        if m.get('NextTime') is not None:
+            self.next_time = m.get('NextTime')
+        if m.get('RepoName') is not None:
+            self.repo_name = m.get('RepoName')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RetentionTagCount') is not None:
+            self.retention_tag_count = m.get('RetentionTagCount')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('ScheduleTime') is not None:
+            self.schedule_time = m.get('ScheduleTime')
+        if m.get('Scope') is not None:
+            self.scope = m.get('Scope')
+        if m.get('TagRegexp') is not None:
+            self.tag_regexp = m.get('TagRegexp')
+        return self
+
+
+class GetArtifactLifecycleRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetArtifactLifecycleRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetArtifactLifecycleRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetAuthorizationTokenRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The ID of the request.
         self.instance_id = instance_id
@@ -9873,14 +10338,270 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListArtifactBuildTaskLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(
+        self,
+        enable_delete_tag: bool = None,
+        instance_id: str = None,
+        page_no: int = None,
+        page_size: int = None,
+    ):
+        self.enable_delete_tag = enable_delete_tag
+        self.instance_id = instance_id
+        self.page_no = page_no
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_delete_tag is not None:
+            result['EnableDeleteTag'] = self.enable_delete_tag
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EnableDeleteTag') is not None:
+            self.enable_delete_tag = m.get('EnableDeleteTag')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        return self
+
+
+class ListArtifactLifecycleRuleResponseBodyRules(TeaModel):
+    def __init__(
+        self,
+        auto: bool = None,
+        create_time: int = None,
+        enable_delete_tag: bool = None,
+        instance_id: str = None,
+        modified_time: int = None,
+        namespace_name: str = None,
+        next_time: int = None,
+        repo_name: str = None,
+        retention_tag_count: int = None,
+        rule_id: str = None,
+        schedule_time: str = None,
+        scope: str = None,
+        tag_regexp: str = None,
+    ):
+        self.auto = auto
+        self.create_time = create_time
+        self.enable_delete_tag = enable_delete_tag
+        self.instance_id = instance_id
+        self.modified_time = modified_time
+        self.namespace_name = namespace_name
+        self.next_time = next_time
+        self.repo_name = repo_name
+        self.retention_tag_count = retention_tag_count
+        self.rule_id = rule_id
+        self.schedule_time = schedule_time
+        self.scope = scope
+        self.tag_regexp = tag_regexp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto is not None:
+            result['Auto'] = self.auto
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.enable_delete_tag is not None:
+            result['EnableDeleteTag'] = self.enable_delete_tag
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.namespace_name is not None:
+            result['NamespaceName'] = self.namespace_name
+        if self.next_time is not None:
+            result['NextTime'] = self.next_time
+        if self.repo_name is not None:
+            result['RepoName'] = self.repo_name
+        if self.retention_tag_count is not None:
+            result['RetentionTagCount'] = self.retention_tag_count
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.schedule_time is not None:
+            result['ScheduleTime'] = self.schedule_time
+        if self.scope is not None:
+            result['Scope'] = self.scope
+        if self.tag_regexp is not None:
+            result['TagRegexp'] = self.tag_regexp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Auto') is not None:
+            self.auto = m.get('Auto')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('EnableDeleteTag') is not None:
+            self.enable_delete_tag = m.get('EnableDeleteTag')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('NamespaceName') is not None:
+            self.namespace_name = m.get('NamespaceName')
+        if m.get('NextTime') is not None:
+            self.next_time = m.get('NextTime')
+        if m.get('RepoName') is not None:
+            self.repo_name = m.get('RepoName')
+        if m.get('RetentionTagCount') is not None:
+            self.retention_tag_count = m.get('RetentionTagCount')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('ScheduleTime') is not None:
+            self.schedule_time = m.get('ScheduleTime')
+        if m.get('Scope') is not None:
+            self.scope = m.get('Scope')
+        if m.get('TagRegexp') is not None:
+            self.tag_regexp = m.get('TagRegexp')
+        return self
+
+
+class ListArtifactLifecycleRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        is_success: bool = None,
+        page_no: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        rules: List[ListArtifactLifecycleRuleResponseBodyRules] = None,
+        total_count: int = None,
+    ):
+        self.code = code
+        self.is_success = is_success
+        self.page_no = page_no
+        self.page_size = page_size
+        self.request_id = request_id
+        self.rules = rules
+        self.total_count = total_count
+
+    def validate(self):
+        if self.rules:
+            for k in self.rules:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.is_success is not None:
+            result['IsSuccess'] = self.is_success
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Rules'] = []
+        if self.rules is not None:
+            for k in self.rules:
+                result['Rules'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('IsSuccess') is not None:
+            self.is_success = m.get('IsSuccess')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.rules = []
+        if m.get('Rules') is not None:
+            for k in m.get('Rules'):
+                temp_model = ListArtifactLifecycleRuleResponseBodyRules()
+                self.rules.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListArtifactLifecycleRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListArtifactLifecycleRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListArtifactLifecycleRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListChainRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         page_no: int = None,
         page_size: int = None,
         repo_name: str = None,
@@ -16437,14 +17158,175 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(
+        self,
+        auto: bool = None,
+        enable_delete_tag: bool = None,
+        instance_id: str = None,
+        namespace_name: str = None,
+        repo_name: str = None,
+        retention_tag_count: int = None,
+        rule_id: str = None,
+        schedule_time: str = None,
+        scope: str = None,
+        tag_regexp: str = None,
+    ):
+        self.auto = auto
+        self.enable_delete_tag = enable_delete_tag
+        self.instance_id = instance_id
+        self.namespace_name = namespace_name
+        self.repo_name = repo_name
+        self.retention_tag_count = retention_tag_count
+        self.rule_id = rule_id
+        self.schedule_time = schedule_time
+        self.scope = scope
+        self.tag_regexp = tag_regexp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto is not None:
+            result['Auto'] = self.auto
+        if self.enable_delete_tag is not None:
+            result['EnableDeleteTag'] = self.enable_delete_tag
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.namespace_name is not None:
+            result['NamespaceName'] = self.namespace_name
+        if self.repo_name is not None:
+            result['RepoName'] = self.repo_name
+        if self.retention_tag_count is not None:
+            result['RetentionTagCount'] = self.retention_tag_count
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.schedule_time is not None:
+            result['ScheduleTime'] = self.schedule_time
+        if self.scope is not None:
+            result['Scope'] = self.scope
+        if self.tag_regexp is not None:
+            result['TagRegexp'] = self.tag_regexp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Auto') is not None:
+            self.auto = m.get('Auto')
+        if m.get('EnableDeleteTag') is not None:
+            self.enable_delete_tag = m.get('EnableDeleteTag')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NamespaceName') is not None:
+            self.namespace_name = m.get('NamespaceName')
+        if m.get('RepoName') is not None:
+            self.repo_name = m.get('RepoName')
+        if m.get('RetentionTagCount') is not None:
+            self.retention_tag_count = m.get('RetentionTagCount')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('ScheduleTime') is not None:
+            self.schedule_time = m.get('ScheduleTime')
+        if m.get('Scope') is not None:
+            self.scope = m.get('Scope')
+        if m.get('TagRegexp') is not None:
+            self.tag_regexp = m.get('TagRegexp')
+        return self
+
+
+class UpdateArtifactLifecycleRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        is_success: bool = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.is_success = is_success
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.is_success is not None:
+            result['IsSuccess'] = self.is_success
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('IsSuccess') is not None:
+            self.is_success = m.get('IsSuccess')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateArtifactLifecycleRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateArtifactLifecycleRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateArtifactLifecycleRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateChainRequest(TeaModel):
     def __init__(
         self,
         chain_config: str = None,
         chain_id: str = None,
         description: str = None,
         instance_id: str = None,
```

### Comparing `alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/PKG-INFO` & `alibabacloud_cr20181201-1.4.0/alibabacloud_cr20181201.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cr20181201
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cr20181201-1.3.0/setup.py` & `alibabacloud_cr20181201-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cr20181201.
 
-Created on 11/04/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cr20181201"
 NAME = "alibabacloud_cr20181201" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cr (20181201) SDK Library for Python"
```

