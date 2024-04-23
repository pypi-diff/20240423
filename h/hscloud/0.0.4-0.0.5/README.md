# Comparing `tmp/hscloud-0.0.4.tar.gz` & `tmp/hscloud-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.4.tar", last modified: Mon Apr 22 11:35:12 2024, max compression
+gzip compressed data, was "hscloud-0.0.5.tar", last modified: Tue Apr 23 06:52:54 2024, max compression
```

## Comparing `hscloud-0.0.4.tar` & `hscloud-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 11:35:12.742620 hscloud-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      437 2024-04-22 11:35:12.741620 hscloud-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-22 11:35:12.731616 hscloud-0.0.4/hscloud/
--rw-rw-rw-   0        0        0     2054 2024-04-22 09:25:12.000000 hscloud-0.0.4/hscloud/__init__.py
--rw-rw-rw-   0        0        0     1987 2024-04-22 09:01:00.000000 hscloud-0.0.4/hscloud/helpers.py
--rw-rw-rw-   0        0        0     1374 2024-04-22 11:32:20.000000 hscloud-0.0.4/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-04-22 11:35:12.739616 hscloud-0.0.4/hscloud.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 11:35:12.000000 hscloud-0.0.4/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 11:35:12.742620 hscloud-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-04-22 11:34:42.000000 hscloud-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 06:52:54.013961 hscloud-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-04-23 06:52:54.011961 hscloud-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.5/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 06:52:54.000961 hscloud-0.0.5/hscloud/
+-rw-rw-rw-   0        0        0        0 2024-04-23 06:50:43.000000 hscloud-0.0.5/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     2911 2024-04-23 06:44:47.000000 hscloud-0.0.5/hscloud/helpers.py
+-rw-rw-rw-   0        0        0      967 2024-04-23 06:51:55.000000 hscloud-0.0.5/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-04-23 06:52:54.009962 hscloud-0.0.5/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 06:52:54.013961 hscloud-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-04-23 06:52:16.000000 hscloud-0.0.5/setup.py
```

### Comparing `hscloud-0.0.4/hscloud/helpers.py` & `hscloud-0.0.5/hscloud/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import requests
 from datetime import datetime
 import logging
 from typing import NamedTuple, Optional, Union
 
 logger = logging.getLogger(__name__)
 
-API_BASE_URL = 'http://10.10.20.109:2070'
-API_RATE_LIMIT = 30
-API_TIMEOUT = 8
+URL = 'http://10.10.20.109:2070'
+TIMEOUT = 8
 
 class Helpers:
 
     @staticmethod
     def headers(access_token=None):
         headers = None
         if access_token is not None:
@@ -25,35 +24,73 @@
             headers = {
                 'Content-Type': 'application/json',
                 'UA': 'dreo/'
             }
         return headers
 
     @staticmethod
+    def params(devicesn=None):
+        params = None
+        if devicesn is not None:
+            params = {
+                'deviceSn': devicesn,
+                'timestamp': Helpers.timestamp()
+            }
+        else:
+            params = {
+                'timestamp': Helpers.timestamp()
+            }
+        return params
+
+    @staticmethod
+    def login_body(username=None, password=None):
+        body = {
+                "client_id": "89ef537b2202481aaaf9077068bcb0c9",
+                "client_secret": "41b20a1f60e9499e89c8646c31f93ea1",
+                "grant_type": "openapi",
+                "scope": "all",
+                "email": username,
+                "password": password
+            }
+        return body
+
+    @staticmethod
+    def update_body(devicesn, **kwargs):
+        data = {
+            'devicesn': devicesn
+        }
+
+        desired = {}
+        for key, value in kwargs.items():
+            desired.update({key: value})
+
+        data.update({'desired': desired})
+        return data
+
+    @staticmethod
     def timestamp():
         return int(datetime.now().timestamp() * 1000)
 
     @staticmethod
-    def call_api(api: str, method: str, headers: Optional[dict] = None, params: Optional[dict] = None, json_body: Optional[dict] = None) -> tuple:
-        """Make API calls by passing endpoint, header and body."""
+    def requests(api: str, method: str, headers: Optional[dict] = None, params: Optional[dict] = None, json_body: Optional[dict] = None) -> tuple:
         response = None
-        result = None
-        status_code = None
+        response_code = False
+        response_data = None
 
         try:
             if method.lower() == 'get':
-                response = requests.get(API_BASE_URL + api, headers=headers, params=params, timeout=API_TIMEOUT)
+                response = requests.get(URL + api, headers=headers, params=params, timeout=TIMEOUT)
 
             elif method.lower() == 'post':
-                response = requests.post(API_BASE_URL + api, headers=headers, params=params, json=json_body, timeout=API_TIMEOUT)
+                response = requests.post(URL + api, headers=headers, params=params, json=json_body, timeout=TIMEOUT)
 
         except requests.exceptions.RequestException as e:
             logger.debug(e)
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:
             logger.debug(e)
         else:
             if response.status_code == 200:
                 response_body = response.json()
                 if response_body.get("code") == 0:
-                    status_code = response_body.get("code")
-                    result = response_body.get("data")
-        return status_code, result
+                    response_code = True
+                    response_data = response_body.get("data")
+        return response_code, response_data
```

### Comparing `hscloud-0.0.4/setup.py` & `hscloud-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name="hscloud",
-    version="0.0.4",
+    version="0.0.5",
     author="kane",
     author_email="wang.xiangtao@qq.com",
     description="A small package to work with prime numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/clement-bonnet/medium-first-package",
     packages=find_packages(),
```

