# Comparing `tmp/vonage-verify-1.0.1.tar.gz` & `tmp/vonage_verify-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-verify-1.0.1.tar", last modified: Mon Apr  8 15:22:51 2024, max compression
+gzip compressed data, was "vonage_verify-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
```

## Comparing `vonage-verify-1.0.1.tar` & `vonage_verify-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.313634 vonage-verify-1.0.1/
--rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-08 15:22:51.312735 vonage-verify-1.0.1/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     2110 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      832 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-08 15:22:51.313958 vonage-verify-1.0.1/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.295217 vonage-verify-1.0.1/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.304479 vonage-verify-1.0.1/src/vonage_verify/
--rw-r--r--   0 mkahan     (503) staff       (20)      582 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      141 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1296 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/language_codes.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1957 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/requests.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1319 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/responses.py
--rw-r--r--   0 mkahan     (503) staff       (20)     7464 2024-04-08 15:22:50.000000 vonage-verify-1.0.1/src/vonage_verify/verify.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-08 15:22:51.312005 vonage-verify-1.0.1/src/vonage_verify.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      427 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       14 2024-04-08 15:22:51.000000 vonage-verify-1.0.1/src/vonage_verify.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.221319 vonage_verify-1.1.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-23 14:16:53.220464 vonage_verify-1.1.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2110 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      832 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.221372 vonage_verify-1.1.0/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.210137 vonage_verify-1.1.0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.215764 vonage_verify-1.1.0/src/vonage_verify/
+-rw-r--r--   0 mkahan     (503) staff       (20)      582 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/src/vonage_verify/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      141 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/src/vonage_verify/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1296 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/src/vonage_verify/language_codes.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1944 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/src/vonage_verify/requests.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1319 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/src/vonage_verify/responses.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     7732 2024-04-23 14:16:51.000000 vonage_verify-1.1.0/src/vonage_verify/verify.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.219547 vonage_verify-1.1.0/src/vonage_verify.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2884 2024-04-23 14:16:53.000000 vonage_verify-1.1.0/src/vonage_verify.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      427 2024-04-23 14:16:53.000000 vonage_verify-1.1.0/src/vonage_verify.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_verify-1.1.0/src/vonage_verify.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_verify-1.1.0/src/vonage_verify.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       14 2024-04-23 14:16:53.000000 vonage_verify-1.1.0/src/vonage_verify.egg-info/top_level.txt
```

### Comparing `vonage-verify-1.0.1/PKG-INFO` & `vonage_verify-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-verify
-Version: 1.0.1
+Version: 1.1.0
 Summary: Vonage verify package
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
 
 # Vonage Verify Package
 
 This package contains the code to use Vonage's Verify API in Python. This package includes methods for working with 2-factor authentication (2FA) messages sent via SMS or TTS.
 
 Note: There is a more current package available: [Vonage's Verify v2 API](https://developer.vonage.com/en/verify/overview) which is recommended for most use cases. The v2 API lets you send messages via multiple channels, including Email, SMS, MMS, WhatsApp, Messenger and others. You can also make Silent Authentication requests with Verify v2 to give an end user a more seamless experience.
```

### Comparing `vonage-verify-1.0.1/README.md` & `vonage_verify-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.1/backend_shim.py` & `vonage_verify-1.1.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.1/pyproject.toml` & `vonage_verify-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = 'vonage-verify'
-version = '1.0.1'
+version = '1.1.0'
 description = 'Vonage verify package'
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

### Comparing `vonage-verify-1.0.1/src/vonage_verify/__init__.py` & `vonage_verify-1.1.0/src/vonage_verify/__init__.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.1/src/vonage_verify/language_codes.py` & `vonage_verify-1.1.0/src/vonage_verify/language_codes.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.1/src/vonage_verify/requests.py` & `vonage_verify-1.1.0/src/vonage_verify/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from logging import getLogger
 from typing import Literal, Optional
 
 from pydantic import BaseModel, Field, model_validator
-from vonage_utils.types.phone_number import PhoneNumber
+from vonage_utils.types import PhoneNumber
 
 from .language_codes import LanguageCode, Psd2LanguageCode
 
 logger = getLogger('vonage_verify')
 
 
 class BaseVerifyRequest(BaseModel):
```

### Comparing `vonage-verify-1.0.1/src/vonage_verify/responses.py` & `vonage_verify-1.1.0/src/vonage_verify/responses.py`

 * *Files identical despite different names*

### Comparing `vonage-verify-1.0.1/src/vonage_verify/verify.py` & `vonage_verify-1.1.0/src/vonage_verify/verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,23 @@
     """
 
     def __init__(self, http_client: HttpClient) -> None:
         self._http_client = http_client
         self._sent_data_type = 'form'
         self._auth_type = 'body'
 
+    @property
+    def http_client(self) -> HttpClient:
+        """The HTTP client used to make requests to the Verify API.
+
+        Returns:
+            HttpClient: The HTTP client used to make requests to the Verify API.
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

### Comparing `vonage-verify-1.0.1/src/vonage_verify.egg-info/PKG-INFO` & `vonage_verify-1.1.0/src/vonage_verify.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-verify
-Version: 1.0.1
+Version: 1.1.0
 Summary: Vonage verify package
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
 
 # Vonage Verify Package
 
 This package contains the code to use Vonage's Verify API in Python. This package includes methods for working with 2-factor authentication (2FA) messages sent via SMS or TTS.
 
 Note: There is a more current package available: [Vonage's Verify v2 API](https://developer.vonage.com/en/verify/overview) which is recommended for most use cases. The v2 API lets you send messages via multiple channels, including Email, SMS, MMS, WhatsApp, Messenger and others. You can also make Silent Authentication requests with Verify v2 to give an end user a more seamless experience.
```

