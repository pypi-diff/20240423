# Comparing `tmp/nerveclient-0.1.1.tar.gz` & `tmp/nerveclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/src/nerve-engine-clients/python/nerveclient/dist/.tmp-l03wm_p_/nerveclient-0.1.1.tar", last modified: Fri Apr 19 07:30:59 2024, max compression
+gzip compressed data, was "/src/nerve-engine-clients/python/nerveclient/dist/.tmp-ggejctvw/nerveclient-0.1.2.tar", last modified: Tue Apr 23 21:23:02 2024, max compression
```

## Comparing `nerveclient-0.1.1.tar` & `nerveclient-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:30:59.000000 nerveclient-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-19 07:30:59.000000 nerveclient-0.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:30:59.000000 nerveclient-0.1.1/nerveclient/
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 22:32:48.000000 nerveclient-0.1.1/nerveclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-19 01:22:19.000000 nerveclient-0.1.1/nerveclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:30:59.000000 nerveclient-0.1.1/nerveclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-19 07:30:59.000000 nerveclient-0.1.1/nerveclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-19 07:30:59.000000 nerveclient-0.1.1/nerveclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 07:30:59.000000 nerveclient-0.1.1/nerveclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-19 07:30:59.000000 nerveclient-0.1.1/nerveclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-19 07:30:59.000000 nerveclient-0.1.1/nerveclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-19 07:30:50.000000 nerveclient-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 07:30:59.000000 nerveclient-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:23:02.000000 nerveclient-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-23 21:23:02.000000 nerveclient-0.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:23:02.000000 nerveclient-0.1.2/nerveclient/
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 22:32:48.000000 nerveclient-0.1.2/nerveclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 20:52:28.000000 nerveclient-0.1.2/nerveclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:23:02.000000 nerveclient-0.1.2/nerveclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-23 21:23:02.000000 nerveclient-0.1.2/nerveclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-23 21:23:02.000000 nerveclient-0.1.2/nerveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 21:23:02.000000 nerveclient-0.1.2/nerveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-23 21:23:02.000000 nerveclient-0.1.2/nerveclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-23 21:23:02.000000 nerveclient-0.1.2/nerveclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-23 21:22:51.000000 nerveclient-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 21:23:02.000000 nerveclient-0.1.2/setup.cfg
```

### Comparing `nerveclient-0.1.1/PKG-INFO` & `nerveclient-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerveclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple python client to send requests to the Nerve Engine.
 Author-email: Matthew Prast <mprast@get-nerve.com>
 Project-URL: Homepage, https://github.com/get-nerve/nerve-engine-clients
 Project-URL: Issues, https://github.com/get-nerve/nerve-engine-clients/issues
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nerveclient-0.1.1/nerveclient/client.py` & `nerveclient-0.1.2/nerveclient/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
     def __refreshJwt(self):
         r = self.s.post(self.connectionString + "/auth", json={
             "data": {
                 "apiKey": self.apiKey
             }
         })
+
+        if r.status_code != 200:
+          print("There was a problem authenticating to the Nerve Engine: " + r.content)
         r.raise_for_status()
         json = r.json()
         self.jwt = json["jwt"]
 
     def __init__(self, connectionString, apiKey):
         self.connectionString = connectionString
         self.apiKey = apiKey
@@ -48,10 +51,12 @@
             r = self.s.post(self.connectionString + "/query", json={"data": args});
 
             if not retry and r.status_code == 401:
                 self.__refreshJwt()
                 retry = True
                 continue
 
+            if r.status_code != 200:
+                print("There was a problem executing the query: " + r.content)
             r.raise_for_status()
 
             return r.json()
```

### Comparing `nerveclient-0.1.1/nerveclient.egg-info/PKG-INFO` & `nerveclient-0.1.2/nerveclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerveclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple python client to send requests to the Nerve Engine.
 Author-email: Matthew Prast <mprast@get-nerve.com>
 Project-URL: Homepage, https://github.com/get-nerve/nerve-engine-clients
 Project-URL: Issues, https://github.com/get-nerve/nerve-engine-clients/issues
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nerveclient-0.1.1/pyproject.toml` & `nerveclient-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nerveclient"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
   "requests"
 ]
 authors = [
   { name="Matthew Prast", email="mprast@get-nerve.com" },
 ]
 description = "A simple python client to send requests to the Nerve Engine."
```

