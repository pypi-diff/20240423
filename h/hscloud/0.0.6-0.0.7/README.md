# Comparing `tmp/hscloud-0.0.6.tar.gz` & `tmp/hscloud-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.6.tar", last modified: Tue Apr 23 07:33:12 2024, max compression
+gzip compressed data, was "hscloud-0.0.7.tar", last modified: Tue Apr 23 09:17:37 2024, max compression
```

## Comparing `hscloud-0.0.6.tar` & `hscloud-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 07:33:12.360895 hscloud-0.0.6/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      437 2024-04-23 07:33:12.358894 hscloud-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 07:33:12.347896 hscloud-0.0.6/hscloud/
--rw-rw-rw-   0        0        0        0 2024-04-23 06:50:43.000000 hscloud-0.0.6/hscloud/__init__.py
--rw-rw-rw-   0        0        0     2911 2024-04-23 07:32:17.000000 hscloud-0.0.6/hscloud/helpers.py
--rw-rw-rw-   0        0        0      967 2024-04-23 07:32:23.000000 hscloud-0.0.6/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:33:12.356895 hscloud-0.0.6/hscloud.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 07:33:12.360895 hscloud-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-04-23 07:32:43.000000 hscloud-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:17:37.866399 hscloud-0.0.7/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-04-23 09:17:37.864400 hscloud-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 09:17:37.850399 hscloud-0.0.7/hscloud/
+-rw-rw-rw-   0        0        0        0 2024-04-23 06:50:43.000000 hscloud-0.0.7/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     2911 2024-04-23 07:32:17.000000 hscloud-0.0.7/hscloud/helpers.py
+-rw-rw-rw-   0        0        0     1090 2024-04-23 09:14:05.000000 hscloud-0.0.7/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:17:37.863400 hscloud-0.0.7/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-23 09:17:37.000000 hscloud-0.0.7/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-23 09:17:37.000000 hscloud-0.0.7/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 09:17:37.000000 hscloud-0.0.7/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 09:17:37.000000 hscloud-0.0.7/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 09:17:37.866399 hscloud-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-04-23 09:15:08.000000 hscloud-0.0.7/setup.py
```

### Comparing `hscloud-0.0.6/hscloud/helpers.py` & `hscloud-0.0.7/hscloud/helpers.py`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.6/hscloud/hscloud.py` & `hscloud-0.0.7/hscloud/hscloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 
 class HsCloud:
 
     def __init__(self, username=None, password=None):
         super().__init__()
         self.username = username
         self.password = password
+        self.access_token = None
 
     def login(self) -> tuple:
-        return Helpers.call_api("/api/oauth/login", "post", Helpers.headers(), Helpers.params(), Helpers.login_body(self.username, self.password))
+        response = Helpers.call_api("/api/oauth/login", "post", Helpers.headers(), Helpers.params(), Helpers.login_body(self.username, self.password))
+        self.access_token = response[1].get("access_token")
+        return response
 
-    def devices(self, access_token) -> tuple:
-        return Helpers.call_api("/api/device/list", "get", Helpers.headers(access_token), Helpers.params())
+    def get_devices(self) -> tuple:
+        return Helpers.call_api("/api/device/list", "get", Helpers.headers(self.access_token), Helpers.params())
 
-    def status(self, access_token, devicesn) -> tuple:
+    def get_status(self, access_token, devicesn) -> tuple:
         return Helpers.call_api("/api/device/state", "get", Helpers.headers(access_token), Helpers.params(devicesn))
 
     def update(self, access_token, devicesn, **kwargs) -> bool:
         response = Helpers.call_api("/api/device/control", "post", Helpers.headers(access_token), Helpers.params(), Helpers.update_body(devicesn, **kwargs))
         return response[0]
```

### Comparing `hscloud-0.0.6/setup.py` & `hscloud-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name="hscloud",
-    version="0.0.6",
+    version="0.0.7",
     author="kane",
     author_email="wang.xiangtao@qq.com",
     description="A small package to work with prime numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/clement-bonnet/medium-first-package",
     packages=find_packages(),
```

