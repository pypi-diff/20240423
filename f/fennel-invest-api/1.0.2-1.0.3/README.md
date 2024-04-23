# Comparing `tmp/fennel_invest_api-1.0.2.tar.gz` & `tmp/fennel_invest_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fennel_invest_api-1.0.2.tar", last modified: Sun Apr 21 22:22:06 2024, max compression
+gzip compressed data, was "fennel_invest_api-1.0.3.tar", last modified: Mon Apr 22 17:02:48 2024, max compression
```

## Comparing `fennel_invest_api-1.0.2.tar` & `fennel_invest_api-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:22:06.846342 fennel_invest_api-1.0.2/fennel_invest_api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/fennel_invest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/fennel_invest_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/fennel_invest_api/fennel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 22:22:06.000000 fennel_invest_api-1.0.2/fennel_invest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:22:06.850342 fennel_invest_api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-21 22:21:59.000000 fennel_invest_api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:02:48.855506 fennel_invest_api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-22 17:02:48.851506 fennel_invest_api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-22 17:02:45.000000 fennel_invest_api-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:02:48.851506 fennel_invest_api-1.0.3/fennel_invest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 17:02:45.000000 fennel_invest_api-1.0.3/fennel_invest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-22 17:02:45.000000 fennel_invest_api-1.0.3/fennel_invest_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-22 17:02:45.000000 fennel_invest_api-1.0.3/fennel_invest_api/fennel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:02:48.851506 fennel_invest_api-1.0.3/fennel_invest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-22 17:02:48.000000 fennel_invest_api-1.0.3/fennel_invest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-22 17:02:48.000000 fennel_invest_api-1.0.3/fennel_invest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:02:48.000000 fennel_invest_api-1.0.3/fennel_invest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 17:02:48.000000 fennel_invest_api-1.0.3/fennel_invest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 17:02:48.000000 fennel_invest_api-1.0.3/fennel_invest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 17:02:48.855506 fennel_invest_api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-22 17:02:45.000000 fennel_invest_api-1.0.3/setup.py
```

### Comparing `fennel_invest_api-1.0.2/PKG-INFO` & `fennel_invest_api-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

### Comparing `fennel_invest_api-1.0.2/README.md` & `fennel_invest_api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fennel_invest_api-1.0.2/fennel_invest_api/endpoints.py` & `fennel_invest_api-1.0.3/fennel_invest_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `fennel_invest_api-1.0.2/fennel_invest_api/fennel.py` & `fennel_invest_api-1.0.3/fennel_invest_api/fennel.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 raise Exception("2FA required. Please provide the code.")
             print("2FA code sent to email")
             code = input("Enter 2FA code: ")
         url = self.endpoints.oauth_url()
         payload = {
             "grant_type": "http://auth0.com/oauth/grant-type/passwordless/otp",
             "client_id": self.client_id,
-            "otp": code,
+            "otp": str(code),
             "username": email,
             "scope": "openid profile offline_access email",
             "audience": "https://meta.api.fennel.com/graphql",
             "realm": "email",
         }
         response = self.session.post(url, json=payload)
         if response.status_code != 200:
```

### Comparing `fennel_invest_api-1.0.2/fennel_invest_api.egg-info/PKG-INFO` & `fennel_invest_api-1.0.3/fennel_invest_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

