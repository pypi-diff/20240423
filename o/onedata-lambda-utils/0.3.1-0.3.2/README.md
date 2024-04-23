# Comparing `tmp/onedata_lambda_utils-0.3.1.tar.gz` & `tmp/onedata_lambda_utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onedata_lambda_utils-0.3.1.tar", last modified: Mon Mar 18 09:30:23 2024, max compression
+gzip compressed data, was "dist/onedata_lambda_utils-0.3.2.tar", last modified: Tue Apr 23 16:44:49 2024, max compression
```

## Comparing `onedata_lambda_utils-0.3.1.tar` & `onedata_lambda_utils-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 cyfrinet  (1000) cyfrinet  (1000)        0 2024-03-18 09:30:23.819894 onedata_lambda_utils-0.3.1/
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       24 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.1/MANIFEST.in
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1626 2024-03-18 09:30:23.815894 onedata_lambda_utils-0.3.1/PKG-INFO
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)      666 2024-03-11 14:19:20.000000 onedata_lambda_utils-0.3.1/README.md
-drwxrwxr-x   0 cyfrinet  (1000) cyfrinet  (1000)        0 2024-03-18 09:30:23.815894 onedata_lambda_utils-0.3.1/onedata_lambda_utils/
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)        0 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils/__init__.py
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     2328 2024-03-11 07:31:38.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils/logging.py
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)        0 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils/py.typed
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1618 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils/stats.py
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1228 2024-03-11 07:31:38.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils/streaming.py
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     7744 2024-03-18 09:15:34.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils/types.py
-drwxrwxr-x   0 cyfrinet  (1000) cyfrinet  (1000)        0 2024-03-18 09:30:23.815894 onedata_lambda_utils-0.3.1/onedata_lambda_utils.egg-info/
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1626 2024-03-18 09:30:23.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils.egg-info/PKG-INFO
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)      438 2024-03-18 09:30:23.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)        1 2024-03-18 09:30:23.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       25 2024-03-18 09:30:23.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils.egg-info/requires.txt
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       21 2024-03-18 09:30:23.000000 onedata_lambda_utils-0.3.1/onedata_lambda_utils.egg-info/top_level.txt
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       38 2024-03-18 09:30:23.819894 onedata_lambda_utils-0.3.1/setup.cfg
--rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1257 2024-03-18 09:10:59.000000 onedata_lambda_utils-0.3.1/setup.py
+drwxrwxr-x   0 cyfrinet  (1000) cyfrinet  (1000)        0 2024-04-23 16:44:49.188709 onedata_lambda_utils-0.3.2/
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       24 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.2/MANIFEST.in
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1626 2024-04-23 16:44:49.184709 onedata_lambda_utils-0.3.2/PKG-INFO
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)      666 2024-04-22 20:43:35.000000 onedata_lambda_utils-0.3.2/README.md
+drwxrwxr-x   0 cyfrinet  (1000) cyfrinet  (1000)        0 2024-04-23 16:44:49.184709 onedata_lambda_utils-0.3.2/onedata_lambda_utils/
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)        0 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils/__init__.py
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     2328 2024-03-11 07:31:38.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils/logging.py
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)        0 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils/py.typed
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1618 2023-02-21 14:17:58.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils/stats.py
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1228 2024-03-11 07:31:38.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils/streaming.py
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     8118 2024-04-22 21:00:57.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils/types.py
+drwxrwxr-x   0 cyfrinet  (1000) cyfrinet  (1000)        0 2024-04-23 16:44:49.184709 onedata_lambda_utils-0.3.2/onedata_lambda_utils.egg-info/
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1626 2024-04-23 16:44:49.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)      438 2024-04-23 16:44:49.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)        1 2024-04-23 16:44:49.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       25 2024-04-23 16:44:49.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils.egg-info/requires.txt
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       21 2024-04-23 16:44:49.000000 onedata_lambda_utils-0.3.2/onedata_lambda_utils.egg-info/top_level.txt
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)       38 2024-04-23 16:44:49.188709 onedata_lambda_utils-0.3.2/setup.cfg
+-rw-rw-r--   0 cyfrinet  (1000) cyfrinet  (1000)     1257 2024-04-23 09:42:43.000000 onedata_lambda_utils-0.3.2/setup.py
```

### Comparing `onedata_lambda_utils-0.3.1/PKG-INFO` & `onedata_lambda_utils-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedata_lambda_utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Library containing utility functions for use in OpenFaaS lambda implementations
 Home-page: UNKNOWN
 Author: Rafal Widziszewski
 License: MIT
 Description: onedata-lambda-utils
         ========================
         Python Library containing utility functions for use in OpenFaaS lambda implementations
```

### Comparing `onedata_lambda_utils-0.3.1/README.md` & `onedata_lambda_utils-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `onedata_lambda_utils-0.3.1/onedata_lambda_utils/logging.py` & `onedata_lambda_utils-0.3.2/onedata_lambda_utils/logging.py`

 * *Files identical despite different names*

### Comparing `onedata_lambda_utils-0.3.1/onedata_lambda_utils/stats.py` & `onedata_lambda_utils-0.3.2/onedata_lambda_utils/stats.py`

 * *Files identical despite different names*

### Comparing `onedata_lambda_utils-0.3.1/onedata_lambda_utils/streaming.py` & `onedata_lambda_utils-0.3.2/onedata_lambda_utils/streaming.py`

 * *Files identical despite different names*

### Comparing `onedata_lambda_utils-0.3.1/onedata_lambda_utils/types.py` & `onedata_lambda_utils-0.3.2/onedata_lambda_utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,27 @@
     effDatasetProtectionFlags: List[ProtectionFlag]
     effDatasetInheritancePath: InheritancePath 
     effQosInheritancePath: InheritancePath 
     aggregateQosStatus: Literal["fulfilled", "pending", "impossible"]
     archiveRecallRootFileId: Optional[str]
 
 
+class AtmGroup(TypedDict):
+    """
+    JSON object describing group.
+
+    Refer to the API specification for more information:
+    https://onedata.org/#/home/api/latest/onezone?anchor=operation/get_group
+    """
+
+    groupId: str
+    name: str
+    type: Literal["organization", "unit", "team", "role_holders"]
+
+
 AtmObject: TypeAlias = Dict[str, Any]
 """
 Generic JSON object
 """
 
 
 class AtmRange(TypedDict):
@@ -174,14 +187,16 @@
 
 class AtmJobBatchRequestCtx(TypedDict, Generic[C]):
     """
     JSON object describing job batch request context.
 
     Fields
     --------
+    userId
+        Id of the scheduling user.
     spaceId
         Id of the space in context of which the workflow is executed.
     atmWorkflowExecutionId
         Workflow execution Id.
     oneproviderDomain
         Domain of job scheduling Oneprovider.
     oneproviderId
@@ -200,14 +215,15 @@
     logLevel
         Level controling the amount of information recorded in audit logs as only logs 
         with severity equal or higher to this level will be stored. 
     config
         User defined task configuration.
     """
 
+    userId: str
     spaceId: str
     atmWorkflowExecutionId: str
     oneproviderDomain: str
     oneproviderId: str
     onezoneDomain: str
     accessToken: str
     heartbeatUrl: str
```

### Comparing `onedata_lambda_utils-0.3.1/onedata_lambda_utils.egg-info/PKG-INFO` & `onedata_lambda_utils-0.3.2/onedata_lambda_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedata-lambda-utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Library containing utility functions for use in OpenFaaS lambda implementations
 Home-page: UNKNOWN
 Author: Rafal Widziszewski
 License: MIT
 Description: onedata-lambda-utils
         ========================
         Python Library containing utility functions for use in OpenFaaS lambda implementations
```

### Comparing `onedata_lambda_utils-0.3.1/setup.py` & `onedata_lambda_utils-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="onedata_lambda_utils",
-    version="0.3.1",
+    version="0.3.2",
     python_requires=">=3.8",
     description="Python Library containing utility functions for use in OpenFaaS lambda implementations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rafal Widziszewski",
     license="MIT",
     classifiers=[
```

