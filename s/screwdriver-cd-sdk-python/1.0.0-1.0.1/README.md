# Comparing `tmp/screwdriver-cd-sdk-python-1.0.0.tar.gz` & `tmp/screwdriver-cd-sdk-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screwdriver-cd-sdk-python-1.0.0.tar", last modified: Fri Apr 19 08:59:54 2024, max compression
+gzip compressed data, was "screwdriver-cd-sdk-python-1.0.1.tar", last modified: Tue Apr 23 12:47:26 2024, max compression
```

## Comparing `screwdriver-cd-sdk-python-1.0.0.tar` & `screwdriver-cd-sdk-python-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:59:54.783254 screwdriver-cd-sdk-python-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-19 08:59:54.783254 screwdriver-cd-sdk-python-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:59:54.783254 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/screwdriver_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:59:54.783254 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-19 08:59:54.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-19 08:59:54.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:59:54.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:59:54.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 08:59:54.000000 screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:59:54.783254 screwdriver-cd-sdk-python-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-19 08:59:53.000000 screwdriver-cd-sdk-python-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:47:26.458625 screwdriver-cd-sdk-python-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 12:47:26.458625 screwdriver-cd-sdk-python-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:47:26.458625 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/screwdriver_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:47:26.458625 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 12:47:26.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 12:47:26.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:47:26.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:47:26.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 12:47:26.000000 screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 12:47:26.458625 screwdriver-cd-sdk-python-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-23 12:47:15.000000 screwdriver-cd-sdk-python-1.0.1/setup.py
```

### Comparing `screwdriver-cd-sdk-python-1.0.0/LICENSE` & `screwdriver-cd-sdk-python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-sdk-python-1.0.0/README.md` & `screwdriver-cd-sdk-python-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,9 +27,10 @@
 [Apache License URL]: https://www.apache.org/licenses/LICENSE-2.0
 [Apache License, Version 2.0]: http://www.apache.org/licenses/LICENSE-2.0.html
 
 [GitHub Workflow Status badge]: https://img.shields.io/github/actions/workflow/status/paion-data/screwdriver-cd-sdk-python/ci-cd.yml?logo=github&style=for-the-badge
 [GitHub Workflow Status URL]: https://github.com/paion-data/screwdriver-cd-sdk-python/actions/workflows/ci-cd.yml
 
 [Python Version Badge]: https://img.shields.io/badge/Python-3.10-brightgreen?style=for-the-badge&logo=python&logoColor=white
+
 [PyPI project badge]: https://img.shields.io/pypi/v/screwdriver-cd-sdk-python?logo=pypi&logoColor=white&style=for-the-badge
 [PyPI project url]: https://pypi.org/project/screwdriver-cd-sdk-python/
```

### Comparing `screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/events.py` & `screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,44 +8,50 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import sys
+
 import requests
-import sys, os
+
 
 def start_build(pipeline_id: int, screwdriver_api_url: str, token: str) -> object:
     """
     Creates and starts a pipeline build.
 
     :param pipeline_id:  The ID of the pipeline to trigger the build
-    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or https://mysd.com
+    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or
+           https://mysd.com
     :param token:  The Screwdriver API token
 
     :return:  The exact same response body as the "POST /v4/events" Swagger API in JSON
     """
     return create_and_start_event(
         screwdriver_api_url,
         {
             'pipelineId': pipeline_id,
             'startFrom': '~commit',
             'causeMessage': 'Run on create',
         },
         token
     )
 
+
 def create_and_start_event(screwdriver_api_url: str, body: object, token: str) -> object:
     """
     Creates and starts a specific event.
 
     If an error occurs, this function returns nothing but throws the causing error.
 
-    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or https://mysd.com
+    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or
+           https://mysd.com
     :param body:  The exact same body as the one used in "POST /v4/events" Swagger API
     :param token:  The Screwdriver API token
 
     :return:  The exact same response body as the "POST /v4/events" Swagger API in JSON
     """
     headers = {
         'accept': 'application/json',
```

### Comparing `screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/pipeline.py` & `screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import os
+import sys
+
 import requests
-import sys, os
+
 
 def search_pipelines_by_name(name: str, screwdriver_api_url: str, token: str) -> list[object]:
     """
     Returns, at most 50 entries, all pipelines whose name contains a specified pipeline name
 
     :param name:  The pipeline name to search. e.g. "paion-data/my-project"
     :param screwdriver_api_url:  The URL of the Screwdriver API server
@@ -85,14 +88,15 @@
     response = requests.get('{}/v4/pipelines'.format(screwdriver_api_url), params=params, headers=headers)
 
     if response.status_code != 200:
         sys.exit(os.EX_CONFIG)
 
     return response.json()
 
+
 def create_pipeline(checkout_url: str, screwdriver_api_url: str, token: str, source_directory: object = None) -> object:
     """
     Creates a new Screwdriver pipeline for a particular repo and an optional source directory.
 
     If the source_directory is not specified, it defaults to the repo root.
 
     :param checkout_url:  The URL of the repository containing the screwdriver.yaml file of the pipeline created
```

### Comparing `screwdriver-cd-sdk-python-1.0.0/screwdriver_cd_sdk_python/secrets.py` & `screwdriver-cd-sdk-python-1.0.1/screwdriver_cd_sdk_python/secrets.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,37 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import os
+import sys
+
 import requests
-import sys, os
 
 logging.basicConfig(level=logging.DEBUG)
 
+
 def _headers(token: str) -> object:
     return {
         'accept': 'application/json',
         'Authorization': token,
         'Content-Type': 'application/json',
     }
 
 
-def create_or_update_secret(secret_name: str, secret_value: str, pipeline_id: int, screwdriver_api_url: str, token: str) -> None:
+def create_or_update_secret(
+        secret_name: str,
+        secret_value: str,
+        pipeline_id: int,
+        screwdriver_api_url: str,
+        token: str
+) -> None:
     """
     "allowInPR" is set to be false by default
 
     :param secret_name:
     :param secret_value:
     :param pipeline_id:
     :param token:
@@ -49,21 +58,27 @@
         for secrete in response.json():
             if secrete["name"] == secret_name:
                 json_data = {
                     'value': secret_value,
                     'allowInPR': False,
                 }
 
-                if requests.put('{}/v4/secrets/{}'.format(screwdriver_api_url, secrete["id"]), headers=_headers(token), json=json_data).status_code != 200:
+                if requests.put(
+                        '{}/v4/secrets/{}'.format(screwdriver_api_url, secrete["id"]),
+                        headers=_headers(token),
+                        json=json_data
+                ).status_code != 200:
                     sys.exit(os.EX_CONFIG)
     else:
         logging.debug("Creating secret '{}'".format(secret_name))
 
         json_data = {
             'pipelineId': pipeline_id,
             'name': secret_name,
             'value': secret_value,
             'allowInPR': False,
         }
 
-        if requests.post('{}/v4/secrets'.format(screwdriver_api_url), headers=_headers(token), json=json_data).status_code != 201:
+        if requests.post(
+                '{}/v4/secrets'.format(screwdriver_api_url), headers=_headers(token), json=json_data
+        ).status_code != 201:
             sys.exit(os.EX_CONFIG)
```

