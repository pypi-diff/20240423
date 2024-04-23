# Comparing `tmp/airflow-yeedu-operator-1.0.6.tar.gz` & `tmp/airflow-yeedu-operator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-yeedu-operator-1.0.6.tar", last modified: Mon Apr 22 12:57:18 2024, max compression
+gzip compressed data, was "airflow-yeedu-operator-1.0.7.tar", last modified: Tue Apr 23 13:16:30 2024, max compression
```

## Comparing `airflow-yeedu-operator-1.0.6.tar` & `airflow-yeedu-operator-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-22 12:57:18.713568 airflow-yeedu-operator-1.0.6/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    11357 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.6/LICENSE
--rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-22 12:57:18.713568 airflow-yeedu-operator-1.0.6/PKG-INFO
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     2647 2024-04-19 08:12:22.000000 airflow-yeedu-operator-1.0.6/README.md
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-22 12:57:18.709568 airflow-yeedu-operator-1.0.6/airflow_yeedu_operator.egg-info/
--rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-22 12:57:18.000000 airflow-yeedu-operator-1.0.6/airflow_yeedu_operator.egg-info/PKG-INFO
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      371 2024-04-22 12:57:18.000000 airflow-yeedu-operator-1.0.6/airflow_yeedu_operator.egg-info/SOURCES.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        1 2024-04-22 12:57:18.000000 airflow-yeedu-operator-1.0.6/airflow_yeedu_operator.egg-info/dependency_links.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       37 2024-04-22 12:57:18.000000 airflow-yeedu-operator-1.0.6/airflow_yeedu_operator.egg-info/requires.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        6 2024-04-22 12:57:18.000000 airflow-yeedu-operator-1.0.6/airflow_yeedu_operator.egg-info/top_level.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       38 2024-04-22 12:57:18.713568 airflow-yeedu-operator-1.0.6/setup.cfg
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      777 2024-04-22 12:54:54.000000 airflow-yeedu-operator-1.0.6/setup.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-22 12:57:18.709568 airflow-yeedu-operator-1.0.6/yeedu/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.6/yeedu/__init__.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-22 12:57:18.709568 airflow-yeedu-operator-1.0.6/yeedu/hooks/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.6/yeedu/hooks/__init__.py
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     9499 2024-04-17 12:36:38.000000 airflow-yeedu-operator-1.0.6/yeedu/hooks/yeedu.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-22 12:57:18.709568 airflow-yeedu-operator-1.0.6/yeedu/operators/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.6/yeedu/operators/__init__.py
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    29437 2024-04-22 12:56:30.000000 airflow-yeedu-operator-1.0.6/yeedu/operators/yeedu.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    11357 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/LICENSE
+-rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/PKG-INFO
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     2647 2024-04-19 08:12:22.000000 airflow-yeedu-operator-1.0.7/README.md
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/
+-rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/PKG-INFO
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      371 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/SOURCES.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        1 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/dependency_links.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       37 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/requires.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        6 2024-04-23 13:16:30.000000 airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/top_level.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       38 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/setup.cfg
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      777 2024-04-23 13:11:58.000000 airflow-yeedu-operator-1.0.7/setup.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/yeedu/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/yeedu/__init__.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/yeedu/hooks/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/yeedu/hooks/__init__.py
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     9653 2024-04-23 13:09:12.000000 airflow-yeedu-operator-1.0.7/yeedu/hooks/yeedu.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-23 13:16:30.449856 airflow-yeedu-operator-1.0.7/yeedu/operators/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.7/yeedu/operators/__init__.py
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    29437 2024-04-22 12:56:30.000000 airflow-yeedu-operator-1.0.7/yeedu/operators/yeedu.py
```

### Comparing `airflow-yeedu-operator-1.0.6/LICENSE` & `airflow-yeedu-operator-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.6/PKG-INFO` & `airflow-yeedu-operator-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-yeedu-operator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Submission and monitoring of jobs using the Yeedu API in Apache Airflow. 
 Author: Yeedu
 Author-email: yeedu@modak.com
 License: All Rights Reserved
 Project-URL: GitHub, https://github.com/yeedu-io/Apache-Airflow-Operator
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `airflow-yeedu-operator-1.0.6/README.md` & `airflow-yeedu-operator-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.6/airflow_yeedu_operator.egg-info/PKG-INFO` & `airflow-yeedu-operator-1.0.7/airflow_yeedu_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-yeedu-operator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Submission and monitoring of jobs using the Yeedu API in Apache Airflow. 
 Author: Yeedu
 Author-email: yeedu@modak.com
 License: All Rights Reserved
 Project-URL: GitHub, https://github.com/yeedu-io/Apache-Airflow-Operator
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `airflow-yeedu-operator-1.0.6/setup.py` & `airflow-yeedu-operator-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def read(*parts):
     return codecs.open(os.path.join(here, *parts), 'r').read()
 
 
 setup(
     name='airflow-yeedu-operator',
-    version='1.0.6',
+    version='1.0.7',
     description='Submission and monitoring of jobs using the Yeedu API in Apache Airflow. ',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='Yeedu',
     author_email='yeedu@modak.com',
     packages=find_packages(),
     install_requires=[
```

### Comparing `airflow-yeedu-operator-1.0.6/yeedu/__init__.py` & `airflow-yeedu-operator-1.0.7/yeedu/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.6/yeedu/hooks/__init__.py` & `airflow-yeedu-operator-1.0.7/yeedu/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.6/yeedu/hooks/yeedu.py` & `airflow-yeedu-operator-1.0.7/yeedu/hooks/yeedu.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 import logging
 from typing import Tuple
 from airflow.hooks.base import BaseHook
 from airflow.exceptions import AirflowException
 from typing import Optional, Dict
 import json
 import os
+from requests.exceptions import RequestException
+
 
 
 
 YEEDU_SCHEDULER_USER = os.getenv("YEEDU_SCHEDULER_USER")
 YEEDU_SCHEDULER_PASSWORD = os.getenv("YEEDU_SCHEDULER_PASSWORD")
 
 headers: dict = {
@@ -69,28 +71,25 @@
         self.tenant_id: str = tenant_id
         self.conf_id = conf_id
         self.workspace_id = workspace_id
         self.base_url: str = base_url
 
     def _api_request(self, method: str, url: str, data=None, params: Optional[Dict] = None) -> requests.Response:
         """
-        Makes an HTTP request to the Yeedu API.
+        Makes an HTTP request to the Yeedu API with retries.
 
         :param method: The HTTP method (GET, POST, etc.).
         :param url: The URL of the API endpoint.
         :param data: The JSON data for the request.
+        :param params: Optional dictionary of query parameters.
         :return: The API response.
         """
 
-        try:
-            response: requests.Response = requests.request(method, url, headers=headers, json=data, params=params)
-            return response
-                        
-        except Exception as e:
-            raise AirflowException(e)
+        response = requests.request(method, url, headers=headers, json=data, params=params)
+        return response  # Exit loop on successful response
             
 
     def yeedu_login(self):
         try:
             login_url = self.base_url+'login'
             data = {
                     "username": f"{YEEDU_SCHEDULER_USER}",
@@ -181,20 +180,16 @@
         """
         Retrieves the status of a Yeedu job.
 
         :param job_id: The ID of the job.
         :return: The API response containing job status.
         """
 
-        try:
-            job_status_url: str = self.base_url + f'workspace/{self.workspace_id}/spark/job/{job_id}'
-            return self._api_request('GET', job_status_url)
-                        
-        except Exception as e:
-            raise AirflowException(e)
+        job_status_url: str = self.base_url + f'workspace/{self.workspace_id}/spark/job/{job_id}'
+        return self._api_request('GET', job_status_url)
 
             
 
     def get_job_logs(self, job_id: int, log_type: str) -> str:
         """
         Retrieves logs for a Yeedu job.
 
@@ -224,28 +219,31 @@
         try:
             max_attempts: int = 5
             attempts_failure: int = 0
 
             while True:
                 time.sleep(5)
                 # Check job status
-                response: requests.Response = self.get_job_status(job_id)
-                api_status_code: int = response.status_code
-                self.log.info("Current API Status Code: %s",api_status_code)
-                if api_status_code == 200:
-                    # If API status is a success, reset the failure attempts counter
-                    attempts_failure = 0
-                    job_status: str = response.json().get('job_status')
-                    self.log.info("Current Job Status: %s ", job_status)
-                    if job_status in ['DONE', 'ERROR', 'TERMINATED', 'KILLED']:
-                        break
-                # If API status is an error, increment the failure attempts counter
-                else:
+                try:
+                    response: requests.Response = self.get_job_status(job_id)
+                    api_status_code: int = response.status_code
+                    self.log.info("Current API Status Code: %s",api_status_code)
+                    if api_status_code == 200:
+                        # If API status is a success, reset the failure attempts counter
+                        attempts_failure = 0
+                        job_status: str = response.json().get('job_status')
+                        self.log.info("Current Job Status: %s ", job_status)
+                        if job_status in ['DONE', 'ERROR', 'TERMINATED', 'KILLED']:
+                            break
+                except RequestException as e:
                     attempts_failure += 1
-                    self.log.info("failure attempts : %s", attempts_failure)
+                    delay = 20
+                    self.log.info(f"GET Job Status API request failed (attempt {attempts_failure}/{max_attempts}) due to {e}")
+                    self.log.info(f"Sleeping for {delay*attempts_failure} seconds before retrying...")
+                    time.sleep(delay*attempts_failure)
 
                 # If continuous failures reach the threshold, throw an error
                 if attempts_failure == max_attempts:
                     raise AirflowException("Continuous API failure reached the threshold")
 
             return job_status
```

### Comparing `airflow-yeedu-operator-1.0.6/yeedu/operators/__init__.py` & `airflow-yeedu-operator-1.0.7/yeedu/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.6/yeedu/operators/yeedu.py` & `airflow-yeedu-operator-1.0.7/yeedu/operators/yeedu.py`

 * *Files identical despite different names*

