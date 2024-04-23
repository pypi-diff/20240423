# Comparing `tmp/oura-1.2.4.tar.gz` & `tmp/oura-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oura-1.2.4.tar", last modified: Tue Jul 19 04:55:05 2022, max compression
+gzip compressed data, was "oura-1.3.0.tar", last modified: Tue Apr 23 17:10:02 2024, max compression
```

## Comparing `oura-1.2.4.tar` & `oura-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 04:55:05.652221 oura-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-07-19 04:54:56.000000 oura-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2022-07-19 04:55:05.652221 oura-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-07-19 04:54:56.000000 oura-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 04:55:05.652221 oura-1.2.4/oura/
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-07-19 04:54:56.000000 oura-1.2.4/oura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-07-19 04:54:56.000000 oura-1.2.4/oura/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-07-19 04:54:56.000000 oura-1.2.4/oura/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7528 2022-07-19 04:54:56.000000 oura-1.2.4/oura/client_pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-07-19 04:54:56.000000 oura-1.2.4/oura/converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-07-19 04:54:56.000000 oura-1.2.4/oura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 04:55:05.652221 oura-1.2.4/oura/export/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 04:54:56.000000 oura-1.2.4/oura/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-07-19 04:54:56.000000 oura-1.2.4/oura/export/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 04:55:05.652221 oura-1.2.4/oura/v2/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-07-19 04:54:56.000000 oura-1.2.4/oura/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-07-19 04:54:56.000000 oura-1.2.4/oura/v2/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2022-07-19 04:54:56.000000 oura-1.2.4/oura/v2/client_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 04:55:05.652221 oura-1.2.4/oura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2022-07-19 04:55:05.000000 oura-1.2.4/oura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-07-19 04:55:05.000000 oura-1.2.4/oura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 04:55:05.000000 oura-1.2.4/oura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-19 04:55:05.000000 oura-1.2.4/oura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-19 04:55:05.000000 oura-1.2.4/oura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-07-19 04:55:05.652221 oura-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-19 04:54:56.000000 oura-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:02.723709 oura-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 17:09:53.000000 oura-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 17:10:02.723709 oura-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-23 17:09:53.000000 oura-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:02.719709 oura-1.3.0/oura/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-23 17:09:53.000000 oura-1.3.0/oura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-23 17:09:53.000000 oura-1.3.0/oura/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-23 17:09:53.000000 oura-1.3.0/oura/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-23 17:09:53.000000 oura-1.3.0/oura/client_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-23 17:09:53.000000 oura-1.3.0/oura/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-23 17:09:53.000000 oura-1.3.0/oura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:02.723709 oura-1.3.0/oura/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:09:53.000000 oura-1.3.0/oura/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 17:09:53.000000 oura-1.3.0/oura/export/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:02.723709 oura-1.3.0/oura/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 17:09:53.000000 oura-1.3.0/oura/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-23 17:09:53.000000 oura-1.3.0/oura/v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-23 17:09:53.000000 oura-1.3.0/oura/v2/client_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:02.723709 oura-1.3.0/oura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 17:10:02.000000 oura-1.3.0/oura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 17:10:02.000000 oura-1.3.0/oura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:10:02.000000 oura-1.3.0/oura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 17:10:02.000000 oura-1.3.0/oura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 17:10:02.000000 oura-1.3.0/oura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-23 17:10:02.723709 oura-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:09:53.000000 oura-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:10:02.723709 oura-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-23 17:09:53.000000 oura-1.3.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-23 17:09:53.000000 oura-1.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-23 17:09:53.000000 oura-1.3.0/tests/test_client_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-23 17:09:53.000000 oura-1.3.0/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-23 17:09:53.000000 oura-1.3.0/tests/test_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 17:09:53.000000 oura-1.3.0/tests/test_writers.py
```

### Comparing `oura-1.2.4/LICENSE` & `oura-1.3.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Jon Hagg
+Copyright (c) 2022
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `oura-1.2.4/PKG-INFO` & `oura-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: oura
-Version: 1.2.4
+Version: 1.3.0
 Summary: Oura API client
 Home-page: https://github.com/turing-complet/python-ouraring
 Author: turing-complet
 Author-email: turingcomplet@proton.me
 Project-URL: Bug Tracker, https://github.com/turing-complet/python-ouraring/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests-oauthlib
+Requires-Dist: pandas
 
 
 ## Installation
 
 Easiest way is to get it from [PyPI](https://pypi.org/project/oura/):
 
 `pip install oura`
```

### Comparing `oura-1.2.4/README.md` & `oura-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `oura-1.2.4/oura/auth.py` & `oura-1.3.0/oura/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     """
 
     AUTHORIZE_BASE_URL = "https://cloud.ouraring.com/oauth/authorize"
     TOKEN_BASE_URL = "https://api.ouraring.com/oauth/token"
     SCOPE = ["email", "personal", "daily", "heartrate", "workout", "tag", "session"]
 
     def __init__(self, client_id, client_secret):
-
         """
         Initialize the client for oauth flow.
 
         :param client_id: The client id from oura portal.
         :type client_id: str
         :param client_secret: The client secret from oura portal.
         :type client_secret: str
@@ -54,14 +53,15 @@
         return self.session.fetch_token(
             self.TOKEN_BASE_URL, code=code, client_secret=self.client_secret
         )
 
 
 class OAuthRequestHandler:
     TOKEN_BASE_URL = "https://api.ouraring.com/oauth/token"
+    TOKEN_REVOKE_URL = "https://api.ouraring.com/oauth/revoke"
 
     def __init__(
         self,
         client_id,
         client_secret=None,
         access_token=None,
         refresh_token=None,
@@ -80,40 +80,49 @@
         self._session = OAuth2Session(
             client_id,
             token=token,
             auto_refresh_url=self.TOKEN_BASE_URL,
             token_updater=refresh_callback,
         )
 
-    def make_request(self, url):
-        method = "GET"
+    def make_request(self, url, method="GET"):
         response = self._session.request(method, url)
         if response.status_code == 401:
             self._refresh_token()
             response = self._session.request(method, url)
         return response
 
-    def make_request_v2(self, url):
-        return self.make_request(url)
+    def make_request_v2(self, url, method="GET"):
+        return self.make_request(url, method)
 
     def _refresh_token(self):
         token = self._session.refresh_token(
             self.TOKEN_BASE_URL,
             client_id=self.client_id,
             client_secret=self.client_secret,
         )
         if self._session.token_updater:
             self._session.token_updater(token)
 
         return token
 
+    def revoke_token(self):
+        return self._session.request("POST", self.TOKEN_REVOKE_URL)
+
 
 class PersonalRequestHandler:
+    TOKEN_REVOKE_URL = "https://api.ouraring.com/oauth/revoke"
+
     def __init__(self, personal_access_token):
         self.personal_access_token = personal_access_token
 
-    def make_request(self, url):
-        return requests.get(url, params={"access_token": self.personal_access_token})
+    def make_request(self, url, method="GET"):
+        requests_method = requests.post if method == "POST" else requests.get
+        return requests_method(url, params={"access_token": self.personal_access_token})
 
-    def make_request_v2(self, url):
+    def make_request_v2(self, url, method="GET"):
+        requests_method = requests.post if method == "POST" else requests.get
         headers = {"Authorization": f"Bearer {self.personal_access_token}"}
-        return requests.get(url, headers=headers)
+        return requests_method(url, headers=headers)
+
+    def revoke_token(self):
+        return self.make_request_v2(self.TOKEN_REVOKE_URL, "POST")
```

### Comparing `oura-1.2.4/oura/client.py` & `oura-1.3.0/oura/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         client_id=None,
         client_secret=None,
         access_token=None,
         refresh_token=None,
         refresh_callback=None,
         personal_access_token=None,
     ):
-
         """
         :param client_id: The client id - identifies your application.
         :type client_id: str
 
         :param client_secret: The client secret. Required for auto refresh.
         :type client_secret: str
```

### Comparing `oura-1.2.4/oura/client_pandas.py` & `oura-1.3.0/oura/client_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     if isinstance(summary, dict):
         summary = [summary]
     df = pd.DataFrame(summary)
     if df.size == 0:
         return df
     if metrics is not None:
-        if type(metrics) == str:
+        if isinstance(metrics, str):
             metrics = [metrics]
         else:
             metrics = metrics.copy()
         # drop any invalid cols the user may have entered
         metrics = [m for m in metrics if m in df.columns]
 
         # always include summary_date (or date_key, as for bedtime)
```

### Comparing `oura-1.2.4/oura/converters.py` & `oura-1.3.0/oura/converters.py`

 * *Files identical despite different names*

### Comparing `oura-1.2.4/oura/exceptions.py` & `oura-1.3.0/oura/exceptions.py`

 * *Files identical despite different names*

### Comparing `oura-1.2.4/oura/export/writers.py` & `oura-1.3.0/oura/export/writers.py`

 * *Files identical despite different names*

### Comparing `oura-1.2.4/oura/v2/client_pandas.py` & `oura-1.3.0/oura/v2/client_pandas.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     if isinstance(summary, dict):
         summary = [summary]
     df = pd.DataFrame(summary)
     if df.size == 0:
         return df
     if metrics is not None:
-        if type(metrics) == str:
+        if isinstance(metrics, str):
             metrics = [metrics]
         else:
             metrics = metrics.copy()
         # drop any invalid cols the user may have entered
         metrics = [m for m in metrics if m in df.columns]
 
         # always include summary_date (or date_key, as for bedtime)
```

### Comparing `oura-1.2.4/oura.egg-info/PKG-INFO` & `oura-1.3.0/oura.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: oura
-Version: 1.2.4
+Version: 1.3.0
 Summary: Oura API client
 Home-page: https://github.com/turing-complet/python-ouraring
 Author: turing-complet
 Author-email: turingcomplet@proton.me
 Project-URL: Bug Tracker, https://github.com/turing-complet/python-ouraring/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests-oauthlib
+Requires-Dist: pandas
 
 
 ## Installation
 
 Easiest way is to get it from [PyPI](https://pypi.org/project/oura/):
 
 `pip install oura`
```

### Comparing `oura-1.2.4/setup.cfg` & `oura-1.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oura
-version = 1.2.4
+version = 1.3.0
 author = turing-complet
 author_email = turingcomplet@proton.me
 description = Oura API client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/turing-complet/python-ouraring
 project_urls =
```

