# Comparing `tmp/vonage-sms-1.0.2.tar.gz` & `tmp/vonage_sms-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-sms-1.0.2.tar", last modified: Thu Mar 28 03:16:58 2024, max compression
+gzip compressed data, was "vonage_sms-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
```

## Comparing `vonage-sms-1.0.2.tar` & `vonage_sms-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.228682 vonage-sms-1.0.2/
--rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-03-28 03:16:58.227714 vonage-sms-1.0.2/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      714 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      826 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-03-28 03:16:58.228783 vonage-sms-1.0.2/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.212721 vonage-sms-1.0.2/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.222145 vonage-sms-1.0.2/src/vonage_sms/
--rw-r--r--   0 mkahan     (503) staff       (20)      285 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/src/vonage_sms/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      517 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/src/vonage_sms/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1912 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/src/vonage_sms/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)      656 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/src/vonage_sms/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3160 2024-03-28 03:16:57.000000 vonage-sms-1.0.2/src/vonage_sms/sms.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.226851 vonage-sms-1.0.2/src/vonage_sms.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-03-28 03:16:58.000000 vonage-sms-1.0.2/src/vonage_sms.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      358 2024-03-28 03:16:58.000000 vonage-sms-1.0.2/src/vonage_sms.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-03-28 03:16:58.000000 vonage-sms-1.0.2/src/vonage_sms.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-03-28 03:16:58.000000 vonage-sms-1.0.2/src/vonage_sms.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       11 2024-03-28 03:16:58.000000 vonage-sms-1.0.2/src/vonage_sms.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.642239 vonage_sms-1.1.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-04-23 14:16:53.641825 vonage_sms-1.1.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      714 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      826 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.642293 vonage_sms-1.1.0/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.636872 vonage_sms-1.1.0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.639166 vonage_sms-1.1.0/src/vonage_sms/
+-rw-r--r--   0 mkahan     (503) staff       (20)      285 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      517 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1912 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      656 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3422 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms/sms.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.641367 vonage_sms-1.1.0/src/vonage_sms.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1482 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      358 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       11 2024-04-23 14:16:53.000000 vonage_sms-1.1.0/src/vonage_sms.egg-info/top_level.txt
```

### Comparing `vonage-sms-1.0.2/PKG-INFO` & `vonage_sms-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-sms
-Version: 1.0.2
+Version: 1.1.0
 Summary: Vonage SMS package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.1.1
-Requires-Dist: vonage-utils>=1.0.0
+Requires-Dist: vonage-http-client>=1.3.0
+Requires-Dist: vonage-utils>=1.1.0
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage SMS Package
 
 This package contains the code to use Vonage's SMS API in Python.
 
 It includes a method for sending SMS messages and returns an `SmsResponse` class to handle the response.
```

### Comparing `vonage-sms-1.0.2/README.md` & `vonage_sms-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vonage-sms-1.0.2/backend_shim.py` & `vonage_sms-1.1.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-sms-1.0.2/pyproject.toml` & `vonage_sms-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = 'vonage-sms'
-version = '1.0.2'
+version = '1.1.0'
 description = 'Vonage SMS package'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-http-client>=1.1.1",
-  "vonage-utils>=1.0.0",
+  "vonage-http-client>=1.3.0",
+  "vonage-utils>=1.1.0",
   "pydantic>=2.6.1",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
```

### Comparing `vonage-sms-1.0.2/src/vonage_sms/errors.py` & `vonage_sms-1.1.0/src/vonage_sms/errors.py`

 * *Files identical despite different names*

### Comparing `vonage-sms-1.0.2/src/vonage_sms/requests.py` & `vonage_sms-1.1.0/src/vonage_sms/requests.py`

 * *Files identical despite different names*

### Comparing `vonage-sms-1.0.2/src/vonage_sms/responses.py` & `vonage_sms-1.1.0/src/vonage_sms/responses.py`

 * *Files identical despite different names*

### Comparing `vonage-sms-1.0.2/src/vonage_sms/sms.py` & `vonage_sms-1.1.0/src/vonage_sms/sms.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,23 @@
         self._http_client = http_client
         self._sent_data_type = 'form'
         if self._http_client._auth._signature_secret:
             self._auth_type = 'signature'
         else:
             self._auth_type = 'basic'
 
+    @property
+    def http_client(self) -> HttpClient:
+        """The HTTP client used to make requests to the SMS API.
+
+        Returns:
+            HttpClient: The HTTP client used to make requests to the SMS API.
+        """
+        return self._http_client
+
     @validate_call
     def send(self, message: SmsMessage) -> SmsResponse:
         """Send an SMS message."""
         response = self._http_client.post(
             self._http_client.rest_host,
             '/sms/json',
             message.model_dump(by_alias=True),
```

### Comparing `vonage-sms-1.0.2/src/vonage_sms.egg-info/PKG-INFO` & `vonage_sms-1.1.0/src/vonage_sms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-sms
-Version: 1.0.2
+Version: 1.1.0
 Summary: Vonage SMS package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.1.1
-Requires-Dist: vonage-utils>=1.0.0
+Requires-Dist: vonage-http-client>=1.3.0
+Requires-Dist: vonage-utils>=1.1.0
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage SMS Package
 
 This package contains the code to use Vonage's SMS API in Python.
 
 It includes a method for sending SMS messages and returns an `SmsResponse` class to handle the response.
```

