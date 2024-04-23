# Comparing `tmp/alibabacloud_cr20181201_py2-1.3.0.tar.gz` & `tmp/alibabacloud_cr20181201_py2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cr20181201_py2-1.3.0.tar", last modified: Thu Apr 11 06:07:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cr20181201_py2-1.4.0.tar", last modified: Tue Apr 23 17:11:53 2024, max compression
```

## Comparing `alibabacloud_cr20181201_py2-1.3.0.tar` & `alibabacloud_cr20181201_py2-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2466 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131418 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/client.py
--rw-r--r--   0 root         (0) root         (0)   600366 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2466 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      908 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138459 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201/client.py
+-rw-r--r--   0 root         (0) root         (0)   629679 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-23 17:11:53.000000 alibabacloud_cr20181201_py2-1.4.0/setup.py
```

### Comparing `alibabacloud_cr20181201_py2-1.3.0/LICENSE` & `alibabacloud_cr20181201_py2-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201_py2-1.3.0/PKG-INFO` & `alibabacloud_cr20181201_py2-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cr20181201_py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cr20181201_py2-1.3.0/README-CN.md` & `alibabacloud_cr20181201_py2-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201_py2-1.3.0/README.md` & `alibabacloud_cr20181201_py2-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/client.py` & `alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,58 @@
         @param request: CreateArtifactBuildRuleRequest
 
         @return: CreateArtifactBuildRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_artifact_build_rule_with_options(request, runtime)
 
+    def create_artifact_lifecycle_rule_with_options(self, request, runtime):
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
+    def create_artifact_lifecycle_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_artifact_lifecycle_rule_with_options(request, runtime)
+
     def create_build_record_by_record_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.build_record_id):
             query['BuildRecordId'] = request.build_record_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -844,14 +888,44 @@
             self.call_api(params, req, runtime)
         )
 
     def create_repository(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_repository_with_options(request, runtime)
 
+    def delete_artifact_lifecycle_rule_with_options(self, request, runtime):
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
+    def delete_artifact_lifecycle_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_artifact_lifecycle_rule_with_options(request, runtime)
+
     def delete_chain_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.chain_id):
             query['ChainId'] = request.chain_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -1366,14 +1440,40 @@
             self.call_api(params, req, runtime)
         )
 
     def get_artifact_build_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_artifact_build_task_with_options(request, runtime)
 
+    def get_artifact_lifecycle_rule_with_options(self, request, runtime):
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
+    def get_artifact_lifecycle_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_artifact_lifecycle_rule_with_options(request, runtime)
+
     def get_authorization_token_with_options(self, request, runtime):
         """
         The ID of the Container Registry instance.
         
 
         @param request: GetAuthorizationTokenRequest
 
@@ -2042,14 +2142,40 @@
             self.call_api(params, req, runtime)
         )
 
     def list_artifact_build_task_log(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_artifact_build_task_log_with_options(request, runtime)
 
+    def list_artifact_lifecycle_rule_with_options(self, request, runtime):
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
+    def list_artifact_lifecycle_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_artifact_lifecycle_rule_with_options(request, runtime)
+
     def list_chain_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_no):
             query['PageNo'] = request.page_no
@@ -2930,14 +3056,60 @@
             self.call_api(params, req, runtime)
         )
 
     def untag_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
+    def update_artifact_lifecycle_rule_with_options(self, request, runtime):
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
+    def update_artifact_lifecycle_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.update_artifact_lifecycle_rule_with_options(request, runtime)
+
     def update_chain_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.chain_config):
             query['ChainConfig'] = request.chain_config
         if not UtilClient.is_unset(request.chain_id):
             query['ChainId'] = request.chain_id
```

### Comparing `alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/models.py` & `alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,14 +503,154 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateArtifactBuildRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(self, auto=None, enable_delete_tag=None, instance_id=None, namespace_name=None, repo_name=None,
+                 retention_tag_count=None, schedule_time=None, scope=None, tag_regexp=None):
+        self.auto = auto  # type: bool
+        self.enable_delete_tag = enable_delete_tag  # type: bool
+        self.instance_id = instance_id  # type: str
+        self.namespace_name = namespace_name  # type: str
+        self.repo_name = repo_name  # type: str
+        self.retention_tag_count = retention_tag_count  # type: long
+        self.schedule_time = schedule_time  # type: str
+        self.scope = scope  # type: str
+        self.tag_regexp = tag_regexp  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateArtifactLifecycleRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, is_success=None, request_id=None, rule_id=None):
+        self.code = code  # type: str
+        self.is_success = is_success  # type: bool
+        self.request_id = request_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateArtifactLifecycleRuleResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateArtifactLifecycleRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateArtifactLifecycleRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, build_record_id=None, instance_id=None, repo_id=None):
         self.build_record_id = build_record_id  # type: str
         self.instance_id = instance_id  # type: str
         self.repo_id = repo_id  # type: str
 
     def validate(self):
@@ -2798,14 +2938,113 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateRepositoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(self, instance_id=None, rule_id=None):
+        self.instance_id = instance_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteArtifactLifecycleRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class DeleteArtifactLifecycleRuleResponseBody(TeaModel):
+    def __init__(self, code=None, is_success=None, request_id=None):
+        self.code = code  # type: str
+        self.is_success = is_success  # type: bool
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteArtifactLifecycleRuleResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteArtifactLifecycleRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteArtifactLifecycleRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, chain_id=None, instance_id=None):
         # The ID of the delivery pipeline.
         self.chain_id = chain_id  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
 
@@ -4652,14 +4891,180 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetArtifactBuildTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(self, instance_id=None, rule_id=None):
+        self.instance_id = instance_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetArtifactLifecycleRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class GetArtifactLifecycleRuleResponseBody(TeaModel):
+    def __init__(self, auto=None, code=None, create_time=None, enable_delete_tag=None, instance_id=None,
+                 is_success=None, modified_time=None, namespace_name=None, next_time=None, repo_name=None, request_id=None,
+                 retention_tag_count=None, rule_id=None, schedule_time=None, scope=None, tag_regexp=None):
+        self.auto = auto  # type: bool
+        self.code = code  # type: str
+        self.create_time = create_time  # type: long
+        self.enable_delete_tag = enable_delete_tag  # type: bool
+        self.instance_id = instance_id  # type: str
+        self.is_success = is_success  # type: bool
+        self.modified_time = modified_time  # type: long
+        self.namespace_name = namespace_name  # type: str
+        self.next_time = next_time  # type: long
+        self.repo_name = repo_name  # type: str
+        self.request_id = request_id  # type: str
+        self.retention_tag_count = retention_tag_count  # type: long
+        self.rule_id = rule_id  # type: str
+        self.schedule_time = schedule_time  # type: str
+        self.scope = scope  # type: str
+        self.tag_regexp = tag_regexp  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetArtifactLifecycleRuleResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetArtifactLifecycleRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetArtifactLifecycleRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None):
         # The ID of the request.
         self.instance_id = instance_id  # type: str
 
     def validate(self):
         pass
@@ -8721,14 +9126,238 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListArtifactBuildTaskLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(self, enable_delete_tag=None, instance_id=None, page_no=None, page_size=None):
+        self.enable_delete_tag = enable_delete_tag  # type: bool
+        self.instance_id = instance_id  # type: str
+        self.page_no = page_no  # type: int
+        self.page_size = page_size  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListArtifactLifecycleRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, auto=None, create_time=None, enable_delete_tag=None, instance_id=None, modified_time=None,
+                 namespace_name=None, next_time=None, repo_name=None, retention_tag_count=None, rule_id=None, schedule_time=None,
+                 scope=None, tag_regexp=None):
+        self.auto = auto  # type: bool
+        self.create_time = create_time  # type: long
+        self.enable_delete_tag = enable_delete_tag  # type: bool
+        self.instance_id = instance_id  # type: str
+        self.modified_time = modified_time  # type: long
+        self.namespace_name = namespace_name  # type: str
+        self.next_time = next_time  # type: long
+        self.repo_name = repo_name  # type: str
+        self.retention_tag_count = retention_tag_count  # type: long
+        self.rule_id = rule_id  # type: str
+        self.schedule_time = schedule_time  # type: str
+        self.scope = scope  # type: str
+        self.tag_regexp = tag_regexp  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListArtifactLifecycleRuleResponseBodyRules, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, is_success=None, page_no=None, page_size=None, request_id=None, rules=None,
+                 total_count=None):
+        self.code = code  # type: str
+        self.is_success = is_success  # type: bool
+        self.page_no = page_no  # type: int
+        self.page_size = page_size  # type: int
+        self.request_id = request_id  # type: str
+        self.rules = rules  # type: list[ListArtifactLifecycleRuleResponseBodyRules]
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.rules:
+            for k in self.rules:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListArtifactLifecycleRuleResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListArtifactLifecycleRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListArtifactLifecycleRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, page_no=None, page_size=None, repo_name=None, repo_namespace_name=None):
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The number of the page to return.
         self.page_no = page_no  # type: int
         # The number of entries to return on each page.
@@ -14536,14 +15165,154 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateArtifactLifecycleRuleRequest(TeaModel):
+    def __init__(self, auto=None, enable_delete_tag=None, instance_id=None, namespace_name=None, repo_name=None,
+                 retention_tag_count=None, rule_id=None, schedule_time=None, scope=None, tag_regexp=None):
+        self.auto = auto  # type: bool
+        self.enable_delete_tag = enable_delete_tag  # type: bool
+        self.instance_id = instance_id  # type: str
+        self.namespace_name = namespace_name  # type: str
+        self.repo_name = repo_name  # type: str
+        self.retention_tag_count = retention_tag_count  # type: long
+        self.rule_id = rule_id  # type: str
+        self.schedule_time = schedule_time  # type: str
+        self.scope = scope  # type: str
+        self.tag_regexp = tag_regexp  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateArtifactLifecycleRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, is_success=None, request_id=None):
+        self.code = code  # type: str
+        self.is_success = is_success  # type: bool
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateArtifactLifecycleRuleResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateArtifactLifecycleRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateArtifactLifecycleRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, chain_config=None, chain_id=None, description=None, instance_id=None, name=None,
                  scope_exclude=None):
         # The configuration of the delivery chain in the JSON format.
         self.chain_config = chain_config  # type: str
         # The ID of the delivery chain.
         self.chain_id = chain_id  # type: str
```

### Comparing `alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO` & `alibabacloud_cr20181201_py2-1.4.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cr20181201-py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cr20181201_py2-1.3.0/setup.py` & `alibabacloud_cr20181201_py2-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cr20181201_py2.
 
-Created on 11/04/2024
+Created on 23/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cr20181201"
 NAME = "alibabacloud_cr20181201_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cr (20181201) SDK Library for Python2"
```

