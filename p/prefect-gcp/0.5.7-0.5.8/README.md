# Comparing `tmp/prefect-gcp-0.5.7.tar.gz` & `tmp/prefect_gcp-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-gcp-0.5.7.tar", last modified: Fri Mar 15 13:49:13 2024, max compression
+gzip compressed data, was "prefect_gcp-0.5.8.tar", last modified: Tue Apr 23 19:10:44 2024, max compression
```

## Comparing `prefect-gcp-0.5.7.tar` & `prefect_gcp-0.5.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:49:13.620145 prefect-gcp-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-03-15 13:49:13.620145 prefect-gcp-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:49:13.624145 prefect-gcp-0.5.7/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 13:49:13.624145 prefect-gcp-0.5.7/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)    32239 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    46400 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:49:13.616145 prefect-gcp-0.5.7/prefect_gcp/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/deployments/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:49:13.616145 prefect-gcp-0.5.7/prefect_gcp/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/models/cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:49:13.616145 prefect-gcp-0.5.7/prefect_gcp/workers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/workers/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/workers/cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/prefect_gcp/workers/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:49:13.620145 prefect-gcp-0.5.7/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-03-15 13:49:13.000000 prefect-gcp-0.5.7/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-15 13:49:13.000000 prefect-gcp-0.5.7/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 13:49:13.000000 prefect-gcp-0.5.7/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-15 13:49:13.000000 prefect-gcp-0.5.7/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-15 13:49:13.000000 prefect-gcp-0.5.7/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-15 13:49:13.000000 prefect-gcp-0.5.7/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-15 13:49:13.624145 prefect-gcp-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:49:13.620145 prefect-gcp-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_cloud_run_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_cloud_run_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_cloud_run_worker_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20315 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/tests/test_vertex_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-03-15 13:48:12.000000 prefect-gcp-0.5.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32239 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46400 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.158912 prefect_gcp-0.5.8/prefect_gcp/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/deployments/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.158912 prefect_gcp-0.5.8/prefect_gcp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/models/cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.158912 prefect_gcp-0.5.8/prefect_gcp/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28869 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/prefect_gcp/workers/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.162912 prefect_gcp-0.5.8/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:10:44.000000 prefect_gcp-0.5.8/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 19:10:44.166912 prefect_gcp-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:44.162912 prefect_gcp-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_run_worker_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20315 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/tests/test_vertex_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-04-23 19:09:30.000000 prefect_gcp-0.5.8/versioneer.py
```

### Comparing `prefect-gcp-0.5.7/LICENSE` & `prefect_gcp-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/PKG-INFO` & `prefect_gcp-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.5.7
+Version: 0.5.8
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.7 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.8 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.5.7/README.md` & `prefect_gcp-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/__init__.py` & `prefect_gcp-0.5.8/prefect_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/aiplatform.py` & `prefect_gcp-0.5.8/prefect_gcp/aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/bigquery.py` & `prefect_gcp-0.5.8/prefect_gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/cloud_run.py` & `prefect_gcp-0.5.8/prefect_gcp/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/cloud_storage.py` & `prefect_gcp-0.5.8/prefect_gcp/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/credentials.py` & `prefect_gcp-0.5.8/prefect_gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/deployments/steps.py` & `prefect_gcp-0.5.8/prefect_gcp/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/models/cloud_run_v2.py` & `prefect_gcp-0.5.8/prefect_gcp/models/cloud_run_v2.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/secret_manager.py` & `prefect_gcp-0.5.8/prefect_gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/utilities.py` & `prefect_gcp-0.5.8/prefect_gcp/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/workers/cloud_run.py` & `prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp/workers/cloud_run_v2.py` & `prefect_gcp-0.5.8/prefect_gcp/workers/cloud_run_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         "client": "prefect",
         "launchStage": "{{ launch_stage }}",
         "template": {
             "template": {
                 "serviceAccount": "{{ service_account_name }}",
                 "maxRetries": "{{ max_retries }}",
                 "timeout": "{{ timeout }}",
-                "vpcAccess": "{{ vpc_connector_name }}",
+                "vpcAccess": {"connector": "{{ vpc_connector_name }}"},
                 "containers": [
                     {
                         "env": [],
                         "image": "{{ image }}",
                         "command": "{{ command }}",
                         "args": "{{ args }}",
                         "resources": {
@@ -180,15 +180,15 @@
         )
 
         self._populate_env()
         self._populate_or_format_command()
         self._format_args_if_present()
         self._populate_image_if_not_present()
         self._populate_timeout()
-        self._populate_vpc_if_present()
+        self._remove_vpc_access_if_unset()
 
     def _populate_timeout(self):
         """
         Populates the job body with the timeout.
         """
         self.job_body["template"]["template"]["timeout"] = f"{self.timeout}s"
 
@@ -231,22 +231,32 @@
         args = self.job_body["template"]["template"]["containers"][0].get("args")
 
         if args is not None and isinstance(args, str):
             self.job_body["template"]["template"]["containers"][0][
                 "args"
             ] = shlex.split(args)
 
-    def _populate_vpc_if_present(self):
+    def _remove_vpc_access_if_unset(self):
         """
-        Populates the job body with the VPC connector if present.
+        Removes vpcAccess if unset.
         """
-        if self.job_body["template"]["template"].get("vpcAccess") is not None:
-            self.job_body["template"]["template"]["vpcAccess"] = {
-                "connector": self.job_body["template"]["template"]["vpcAccess"],
-            }
+
+        if "vpcAccess" not in self.job_body["template"]["template"]:
+            return
+
+        vpc_access = self.job_body["template"]["template"]["vpcAccess"]
+
+        # if vpcAccess is unset or connector is unset, remove the entire vpcAccess block
+        # otherwise leave the user provided value.
+        if not vpc_access or (
+            len(vpc_access) == 1
+            and "connector" in vpc_access
+            and vpc_access["connector"] is None
+        ):
+            self.job_body["template"]["template"].pop("vpcAccess")
 
     # noinspection PyMethodParameters
     @validator("job_body")
     def _ensure_job_includes_all_required_components(cls, value: Dict[str, Any]):
         """
         Ensures that the job body includes all required components.
```

### Comparing `prefect-gcp-0.5.7/prefect_gcp/workers/vertex.py` & `prefect_gcp-0.5.8/prefect_gcp/workers/vertex.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp.egg-info/PKG-INFO` & `prefect_gcp-0.5.8/prefect_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.5.7
+Version: 0.5.8
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.7 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.5.8 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.5.7/prefect_gcp.egg-info/SOURCES.txt` & `prefect_gcp-0.5.8/prefect_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/prefect_gcp.egg-info/requires.txt` & `prefect_gcp-0.5.8/prefect_gcp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/setup.cfg` & `prefect_gcp-0.5.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/setup.py` & `prefect_gcp-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_aiplatform.py` & `prefect_gcp-0.5.8/tests/test_aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_bigquery.py` & `prefect_gcp-0.5.8/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_block_standards.py` & `prefect_gcp-0.5.8/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_cloud_run.py` & `prefect_gcp-0.5.8/tests/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_cloud_run_v2.py` & `prefect_gcp-0.5.8/tests/test_cloud_run_v2.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_cloud_run_worker.py` & `prefect_gcp-0.5.8/tests/test_cloud_run_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_cloud_run_worker_v2.py` & `prefect_gcp-0.5.8/tests/test_cloud_run_worker_v2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     return {
         "client": "prefect",
         "launchStage": None,
         "template": {
             "template": {
                 "maxRetries": None,
                 "timeout": None,
-                "vpcAccess": "projects/my_project/locations/us-central1/connectors/my-connector",  # noqa: E501
+                "vpcAccess": {
+                    "connector": None,
+                },
                 "containers": [
                     {
                         "env": [],
                         "command": None,
                         "args": "-m prefect.engine",
                         "resources": {
                             "limits": {
@@ -118,16 +120,66 @@
     def test_format_args_if_present(self, cloud_run_worker_v2_job_config):
         cloud_run_worker_v2_job_config._format_args_if_present()
 
         assert cloud_run_worker_v2_job_config.job_body["template"]["template"][
             "containers"
         ][0]["args"] == ["-m", "prefect.engine"]
 
-    def test_populate_vpc_if_present(self, cloud_run_worker_v2_job_config):
-        cloud_run_worker_v2_job_config._populate_vpc_if_present()
+    @pytest.mark.parametrize("vpc_access", [{"connector": None}, {}, None])
+    def test_remove_vpc_access_if_connector_unset(
+        self, cloud_run_worker_v2_job_config, vpc_access
+    ):
+        cloud_run_worker_v2_job_config.job_body["template"]["template"][
+            "vpcAccess"
+        ] = vpc_access
+
+        cloud_run_worker_v2_job_config._remove_vpc_access_if_unset()
 
         assert (
-            cloud_run_worker_v2_job_config.job_body["template"]["template"][
-                "vpcAccess"
-            ]["connector"]
-            == "projects/my_project/locations/us-central1/connectors/my-connector"
+            "vpcAccess"
+            not in cloud_run_worker_v2_job_config.job_body["template"]["template"]
+        )
+
+    def test_remove_vpc_access_originally_not_present(
+        self, cloud_run_worker_v2_job_config
+    ):
+        cloud_run_worker_v2_job_config.job_body["template"]["template"].pop("vpcAccess")
+
+        cloud_run_worker_v2_job_config._remove_vpc_access_if_unset()
+
+        assert (
+            "vpcAccess"
+            not in cloud_run_worker_v2_job_config.job_body["template"]["template"]
         )
+
+    def test_vpc_access_left_alone_if_connector_set(
+        self, cloud_run_worker_v2_job_config
+    ):
+        cloud_run_worker_v2_job_config.job_body["template"]["template"]["vpcAccess"][
+            "connector"
+        ] = "projects/my_project/locations/us-central1/connectors/my-connector"
+
+        cloud_run_worker_v2_job_config._remove_vpc_access_if_unset()
+
+        assert cloud_run_worker_v2_job_config.job_body["template"]["template"][
+            "vpcAccess"
+        ] == {
+            "connector": "projects/my_project/locations/us-central1/connectors/my-connector"  # noqa E501
+        }
+
+    def test_vpc_access_left_alone_if_network_config_set(
+        self, cloud_run_worker_v2_job_config
+    ):
+        cloud_run_worker_v2_job_config.job_body["template"]["template"]["vpcAccess"][
+            "networkInterfaces"
+        ] = [{"network": "projects/my_project/global/networks/my-network"}]
+
+        cloud_run_worker_v2_job_config._remove_vpc_access_if_unset()
+
+        assert cloud_run_worker_v2_job_config.job_body["template"]["template"][
+            "vpcAccess"
+        ] == {
+            "connector": None,
+            "networkInterfaces": [
+                {"network": "projects/my_project/global/networks/my-network"}
+            ],
+        }
```

### Comparing `prefect-gcp-0.5.7/tests/test_cloud_storage.py` & `prefect_gcp-0.5.8/tests/test_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_credentials.py` & `prefect_gcp-0.5.8/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_deprecation.py` & `prefect_gcp-0.5.8/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_secret_manager.py` & `prefect_gcp-0.5.8/tests/test_secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/tests/test_vertex_worker.py` & `prefect_gcp-0.5.8/tests/test_vertex_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.5.7/versioneer.py` & `prefect_gcp-0.5.8/versioneer.py`

 * *Files identical despite different names*

