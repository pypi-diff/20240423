# Comparing `tmp/hscloud-0.0.5.tar.gz` & `tmp/hscloud-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.5.tar", last modified: Tue Apr 23 06:52:54 2024, max compression
+gzip compressed data, was "hscloud-0.0.6.tar", last modified: Tue Apr 23 07:33:12 2024, max compression
```

## Comparing `hscloud-0.0.5.tar` & `hscloud-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 06:52:54.013961 hscloud-0.0.5/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      437 2024-04-23 06:52:54.011961 hscloud-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 06:52:54.000961 hscloud-0.0.5/hscloud/
--rw-rw-rw-   0        0        0        0 2024-04-23 06:50:43.000000 hscloud-0.0.5/hscloud/__init__.py
--rw-rw-rw-   0        0        0     2911 2024-04-23 06:44:47.000000 hscloud-0.0.5/hscloud/helpers.py
--rw-rw-rw-   0        0        0      967 2024-04-23 06:51:55.000000 hscloud-0.0.5/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-04-23 06:52:54.009962 hscloud-0.0.5/hscloud.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 06:52:53.000000 hscloud-0.0.5/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 06:52:54.013961 hscloud-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-04-23 06:52:16.000000 hscloud-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:33:12.360895 hscloud-0.0.6/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-04-23 07:33:12.358894 hscloud-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-22 09:32:34.000000 hscloud-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 07:33:12.347896 hscloud-0.0.6/hscloud/
+-rw-rw-rw-   0        0        0        0 2024-04-23 06:50:43.000000 hscloud-0.0.6/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     2911 2024-04-23 07:32:17.000000 hscloud-0.0.6/hscloud/helpers.py
+-rw-rw-rw-   0        0        0      967 2024-04-23 07:32:23.000000 hscloud-0.0.6/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:33:12.356895 hscloud-0.0.6/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 07:33:12.000000 hscloud-0.0.6/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 07:33:12.360895 hscloud-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-04-23 07:32:43.000000 hscloud-0.0.6/setup.py
```

### Comparing `hscloud-0.0.5/hscloud/helpers.py` & `hscloud-0.0.6/hscloud/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return data
 
     @staticmethod
     def timestamp():
         return int(datetime.now().timestamp() * 1000)
 
     @staticmethod
-    def requests(api: str, method: str, headers: Optional[dict] = None, params: Optional[dict] = None, json_body: Optional[dict] = None) -> tuple:
+    def call_api(api: str, method: str, headers: Optional[dict] = None, params: Optional[dict] = None, json_body: Optional[dict] = None) -> tuple:
         response = None
         response_code = False
         response_data = None
 
         try:
             if method.lower() == 'get':
                 response = requests.get(URL + api, headers=headers, params=params, timeout=TIMEOUT)
```

### Comparing `hscloud-0.0.5/hscloud/hscloud.py` & `hscloud-0.0.6/hscloud/hscloud.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
     def __init__(self, username=None, password=None):
         super().__init__()
         self.username = username
         self.password = password
 
     def login(self) -> tuple:
-        return Helpers.requests("/api/oauth/login", "post", Helpers.headers(), Helpers.params(), Helpers.login_body(self.username, self.password))
+        return Helpers.call_api("/api/oauth/login", "post", Helpers.headers(), Helpers.params(), Helpers.login_body(self.username, self.password))
 
     def devices(self, access_token) -> tuple:
-        return Helpers.requests("/api/device/list", "get", Helpers.headers(access_token), Helpers.params())
+        return Helpers.call_api("/api/device/list", "get", Helpers.headers(access_token), Helpers.params())
 
     def status(self, access_token, devicesn) -> tuple:
-        return Helpers.requests("/api/device/state", "get", Helpers.headers(access_token), Helpers.params(devicesn))
+        return Helpers.call_api("/api/device/state", "get", Helpers.headers(access_token), Helpers.params(devicesn))
 
     def update(self, access_token, devicesn, **kwargs) -> bool:
-        response = Helpers.requests("/api/device/control", "post", Helpers.headers(access_token), Helpers.params(), Helpers.update_body(devicesn, **kwargs))
+        response = Helpers.call_api("/api/device/control", "post", Helpers.headers(access_token), Helpers.params(), Helpers.update_body(devicesn, **kwargs))
         return response[0]
```

### Comparing `hscloud-0.0.5/setup.py` & `hscloud-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name="hscloud",
-    version="0.0.5",
+    version="0.0.6",
     author="kane",
     author_email="wang.xiangtao@qq.com",
     description="A small package to work with prime numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/clement-bonnet/medium-first-package",
     packages=find_packages(),
```

