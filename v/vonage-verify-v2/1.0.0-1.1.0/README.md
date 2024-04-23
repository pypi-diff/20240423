# Comparing `tmp/vonage-verify-v2-1.0.0.tar.gz` & `tmp/vonage_verify_v2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-verify-v2-1.0.0.tar", last modified: Mon Apr  8 15:22:51 2024, max compression
+gzip compressed data, was "vonage_verify_v2-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
```

## Comparing `vonage-verify-v2-1.0.0.tar` & `vonage_verify_v2-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.556349 vonage-verify-v2-1.0.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     2645 2024-04-08 15:22:51.555764 vonage-verify-v2-1.0.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1864 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      838 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-08 15:22:51.556411 vonage-verify-v2-1.0.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.547708 vonage-verify-v2-1.0.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.551625 vonage-verify-v2-1.0.0/src/vonage_verify_v2/
--rw-r--r--   0 mkahan     (503) staff       (20)      580 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      455 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2/enums.py
--rw-r--r--   0 mkahan     (503) staff       (20)      141 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3222 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)      236 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2295 2024-04-08 15:22:50.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2/verify_v2.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.555038 vonage-verify-v2-1.0.0/src/vonage_verify_v2.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2645 2024-04-08 15:22:51.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      454 2024-04-08 15:22:51.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-08 15:22:51.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-08 15:22:51.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       17 2024-04-08 15:22:51.000000 vonage-verify-v2-1.0.0/src/vonage_verify_v2.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.254824 vonage_verify_v2-1.1.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2645 2024-04-23 14:16:53.254232 vonage_verify_v2-1.1.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1864 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      838 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.255038 vonage_verify_v2-1.1.0/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.245119 vonage_verify_v2-1.1.0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.250418 vonage_verify_v2-1.1.0/src/vonage_verify_v2/
+-rw-r--r--   0 mkahan     (503) staff       (20)      580 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      455 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2/enums.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      141 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3209 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      236 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2569 2024-04-23 14:16:51.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2/verify_v2.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.253254 vonage_verify_v2-1.1.0/src/vonage_verify_v2.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2645 2024-04-23 14:16:53.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      454 2024-04-23 14:16:53.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       17 2024-04-23 14:16:53.000000 vonage_verify_v2-1.1.0/src/vonage_verify_v2.egg-info/top_level.txt
```

### Comparing `vonage-verify-v2-1.0.0/PKG-INFO` & `vonage_verify_v2-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-verify-v2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Vonage verify v2 package
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
-Requires-Dist: vonage-http-client>=1.2.1
-Requires-Dist: vonage-utils>=1.0.1
+Requires-Dist: vonage-http-client>=1.3.0
+Requires-Dist: vonage-utils>=1.1.0
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage Verify V2 Package
 
 This package contains the code to use [Vonage's Verify v2 API](https://developer.vonage.com/en/verify/overview) in Python. This package includes methods for working with 2-factor authentication (2FA) messages sent via SMS, Voice, WhatsApp and Email. You can also make Silent Authentication requests with Verify v2 to give your end user a more seamless experience.
 
 ## Usage
```

### Comparing `vonage-verify-v2-1.0.0/README.md` & `vonage_verify_v2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vonage-verify-v2-1.0.0/backend_shim.py` & `vonage_verify_v2-1.1.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-v2-1.0.0/pyproject.toml` & `vonage_verify_v2-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = 'vonage-verify-v2'
-version = '1.0.0'
+version = '1.1.0'
 description = 'Vonage verify v2 package'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-http-client>=1.2.1",
-  "vonage-utils>=1.0.1",
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

### Comparing `vonage-verify-v2-1.0.0/src/vonage_verify_v2/__init__.py` & `vonage_verify_v2-1.1.0/src/vonage_verify_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-v2-1.0.0/src/vonage_verify_v2/requests.py` & `vonage_verify_v2-1.1.0/src/vonage_verify_v2/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from re import search
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Field, field_validator, model_validator
-from vonage_utils.types.phone_number import PhoneNumber
+from vonage_utils.types import PhoneNumber
 
 from .enums import ChannelType, Locale
 from .errors import VerifyError
 
 
 class Channel(BaseModel):
     to: PhoneNumber
```

### Comparing `vonage-verify-v2-1.0.0/src/vonage_verify_v2/verify_v2.py` & `vonage_verify_v2-1.1.0/src/vonage_verify_v2/verify_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 
 class VerifyV2:
     """Calls Vonage's Verify V2 API."""
 
     def __init__(self, http_client: HttpClient) -> None:
         self._http_client = http_client
 
+    @property
+    def http_client(self) -> HttpClient:
+        """The HTTP client used to make requests to the Verify V2 API.
+
+        Returns:
+            HttpClient: The HTTP client used to make requests to the Verify V2 API.
+        """
+        return self._http_client
+
     @validate_call
     def start_verification(
         self, verify_request: VerifyRequest
     ) -> StartVerificationResponse:
         """Start a verification process.
 
         Args:
```

### Comparing `vonage-verify-v2-1.0.0/src/vonage_verify_v2.egg-info/PKG-INFO` & `vonage_verify_v2-1.1.0/src/vonage_verify_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-verify-v2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Vonage verify v2 package
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
-Requires-Dist: vonage-http-client>=1.2.1
-Requires-Dist: vonage-utils>=1.0.1
+Requires-Dist: vonage-http-client>=1.3.0
+Requires-Dist: vonage-utils>=1.1.0
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage Verify V2 Package
 
 This package contains the code to use [Vonage's Verify v2 API](https://developer.vonage.com/en/verify/overview) in Python. This package includes methods for working with 2-factor authentication (2FA) messages sent via SMS, Voice, WhatsApp and Email. You can also make Silent Authentication requests with Verify v2 to give your end user a more seamless experience.
 
 ## Usage
```

