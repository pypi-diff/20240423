# Comparing `tmp/pyverless-0.0.8.tar.gz` & `tmp/pyverless-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyverless-0.0.8.tar", last modified: Tue Apr 28 18:37:03 2020, max compression
+gzip compressed data, was "dist/pyverless-0.0.9.tar", last modified: Mon May 11 12:00:40 2020, max compression
```

## Comparing `pyverless-0.0.8.tar` & `pyverless-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 foqum     (1000) foqum     (1000)        0 2020-04-28 18:37:03.000000 pyverless-0.0.8/
--rw-rw-r--   0 foqum     (1000) foqum     (1000)       38 2020-04-28 18:37:03.000000 pyverless-0.0.8/setup.cfg
-drwxrwxr-x   0 foqum     (1000) foqum     (1000)        0 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless/
--rw-r--r--   0 foqum     (1000) foqum     (1000)      616 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/exceptions.py
--rw-r--r--   0 foqum     (1000) foqum     (1000)      919 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/serializers.py
--rw-r--r--   0 foqum     (1000) foqum     (1000)      446 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/models.py
--rw-r--r--   0 foqum     (1000) foqum     (1000)        0 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/__init__.py
--rw-r--r--   0 foqum     (1000) foqum     (1000)      520 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/decorators.py
-drwxrwxr-x   0 foqum     (1000) foqum     (1000)        0 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless/config/
--rw-r--r--   0 foqum     (1000) foqum     (1000)      227 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/config/base_settings.py
--rw-r--r--   0 foqum     (1000) foqum     (1000)     2126 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/config/__init__.py
--rw-rw-r--   0 foqum     (1000) foqum     (1000)    14511 2020-04-28 18:31:37.000000 pyverless-0.0.8/pyverless/handlers.py
--rw-r--r--   0 foqum     (1000) foqum     (1000)      539 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/auth.py
--rw-r--r--   0 foqum     (1000) foqum     (1000)     3952 2020-04-23 18:07:33.000000 pyverless-0.0.8/pyverless/crypto.py
--rw-rw-r--   0 foqum     (1000) foqum     (1000)     6106 2020-04-23 18:17:10.000000 pyverless-0.0.8/README.md
--rw-rw-r--   0 foqum     (1000) foqum     (1000)     3919 2020-04-28 18:19:47.000000 pyverless-0.0.8/setup.py
--rw-rw-r--   0 foqum     (1000) foqum     (1000)     8205 2020-04-28 18:37:03.000000 pyverless-0.0.8/PKG-INFO
-drwxrwxr-x   0 foqum     (1000) foqum     (1000)        0 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless.egg-info/
--rw-rw-r--   0 foqum     (1000) foqum     (1000)       90 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless.egg-info/requires.txt
--rw-rw-r--   0 foqum     (1000) foqum     (1000)        1 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless.egg-info/dependency_links.txt
--rw-rw-r--   0 foqum     (1000) foqum     (1000)       10 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless.egg-info/top_level.txt
--rw-rw-r--   0 foqum     (1000) foqum     (1000)       40 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless.egg-info/entry_points.txt
--rw-rw-r--   0 foqum     (1000) foqum     (1000)      480 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless.egg-info/SOURCES.txt
--rw-rw-r--   0 foqum     (1000) foqum     (1000)     8205 2020-04-28 18:37:03.000000 pyverless-0.0.8/pyverless.egg-info/PKG-INFO
--rw-r--r--   0 foqum     (1000) foqum     (1000)     1599 2020-04-23 18:07:33.000000 pyverless-0.0.8/LICENSE.txt
--rw-r--r--   0 foqum     (1000) foqum     (1000)       71 2020-04-23 18:07:33.000000 pyverless-0.0.8/MANIFEST.in
+drwxr-xr-x   0 xiang     (1000) xiang     (1000)        0 2020-05-11 12:00:40.000000 pyverless-0.0.9/
+drwxr-xr-x   0 xiang     (1000) xiang     (1000)        0 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless/
+-rw-r--r--   0 xiang     (1000) xiang     (1000)      919 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/serializers.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)    14820 2020-05-11 11:49:55.000000 pyverless-0.0.9/pyverless/handlers.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)      616 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/exceptions.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)        0 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/__init__.py
+drwxr-xr-x   0 xiang     (1000) xiang     (1000)        0 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless/config/
+-rw-r--r--   0 xiang     (1000) xiang     (1000)     2126 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/config/__init__.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)      227 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/config/base_settings.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)      520 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/decorators.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)      446 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/models.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)      539 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/auth.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)     3952 2019-03-05 16:06:15.000000 pyverless-0.0.9/pyverless/crypto.py
+-rw-r--r--   0 xiang     (1000) xiang     (1000)     6106 2019-05-27 15:41:39.000000 pyverless-0.0.9/README.md
+-rw-r--r--   0 xiang     (1000) xiang     (1000)       71 2019-03-05 16:06:15.000000 pyverless-0.0.9/MANIFEST.in
+drwxr-xr-x   0 xiang     (1000) xiang     (1000)        0 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless.egg-info/
+-rw-r--r--   0 xiang     (1000) xiang     (1000)       90 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless.egg-info/requires.txt
+-rw-r--r--   0 xiang     (1000) xiang     (1000)      480 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless.egg-info/SOURCES.txt
+-rw-r--r--   0 xiang     (1000) xiang     (1000)        1 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless.egg-info/dependency_links.txt
+-rw-r--r--   0 xiang     (1000) xiang     (1000)       40 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless.egg-info/entry_points.txt
+-rw-r--r--   0 xiang     (1000) xiang     (1000)       10 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless.egg-info/top_level.txt
+-rw-r--r--   0 xiang     (1000) xiang     (1000)     8205 2020-05-11 12:00:40.000000 pyverless-0.0.9/pyverless.egg-info/PKG-INFO
+-rw-r--r--   0 xiang     (1000) xiang     (1000)     8205 2020-05-11 12:00:40.000000 pyverless-0.0.9/PKG-INFO
+-rw-r--r--   0 xiang     (1000) xiang     (1000)     1599 2019-03-05 16:06:15.000000 pyverless-0.0.9/LICENSE.txt
+-rw-r--r--   0 xiang     (1000) xiang     (1000)       38 2020-05-11 12:00:40.000000 pyverless-0.0.9/setup.cfg
+-rw-r--r--   0 xiang     (1000) xiang     (1000)     3919 2020-05-11 11:57:43.000000 pyverless-0.0.9/setup.py
```

### Comparing `pyverless-0.0.8/pyverless/exceptions.py` & `pyverless-0.0.9/pyverless/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyverless-0.0.8/pyverless/serializers.py` & `pyverless-0.0.9/pyverless/serializers.py`

 * *Files identical despite different names*

### Comparing `pyverless-0.0.8/pyverless/decorators.py` & `pyverless-0.0.9/pyverless/decorators.py`

 * *Files identical despite different names*

### Comparing `pyverless-0.0.8/pyverless/config/__init__.py` & `pyverless-0.0.9/pyverless/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyverless-0.0.8/pyverless/handlers.py` & `pyverless-0.0.9/pyverless/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import traceback
+from typing import Union
 
 import sentry_sdk
 from sentry_sdk import capture_exception, configure_scope
 
 from pyverless.config import settings
 from pyverless.decorators import warmup
 from pyverless.models import get_user_model
@@ -13,14 +14,17 @@
 
 class RequestBodyMixin(object):
     """
     Implement the get_body method that will be called to set self.body as the body
     of the request.
     """
 
+    event: dict
+    error: Union[list, tuple]
+
     required_body_keys = []
     optional_body_keys = []
 
     def get_required_body_keys(self):
         return self.required_body_keys
 
     def get_body(self):
@@ -69,14 +73,17 @@
 
     - attributes
     - text_message
     - queue_source
     - region
     """
 
+    event: dict
+    error: Union[list, tuple]
+
     def get_messages(self):
         messages = []
 
         try:
             temp_messages = self.event['Records'] if self.event['Records'] else []
         except json.decoder.JSONDecodeError:
             message = "Malformed message"
@@ -116,14 +123,16 @@
     - event_name
     - bucket
     - owner
     - file_name
     - size
     """
 
+    event: dict
+
     def get_file(self):
         try:
             temp_file_event = self.event['Records'] if self.event['Records'] else []
         except json.decoder.JSONDecodeError:
             message = "Malformed message"
             self.error = (message, 400)
             raise BadRequest(message=message)
@@ -155,14 +164,17 @@
 class AuthorizationMixin(object):
     """
     Implement the get_user method that will be called to set self.user
 
     USER_MODEL must be set on the pyverless settings
     """
 
+    event: dict
+    error: Union[list, tuple]
+
     def get_user(self):
         try:
             user_id = self.event['requestContext']['authorizer']['principalId']
         except KeyError:
             self.error = ('Unauthorized', 403)
             raise Unauthorized()
 
@@ -182,14 +194,17 @@
     the object 'id' must be present on the pathParameters.
 
     The user can also overwrite the get_queryset method to limit the visibility.
 
     The 'model' attribute must be set on the handler.
     """
 
+    event: dict
+    error: Union[list, tuple]
+
     model = None
     serializer = None
     id_in_path = 'id'
 
     def get_object(self):
         object_id = self.event['pathParameters'][self.id_in_path]
 
@@ -236,14 +251,19 @@
 
     def serialize(self, instance):
         return self.serializer(instance=instance).data
 
 
 class BaseHandler(object):
 
+    # type hints
+    event: dict
+    body: dict
+    error: Union[list, tuple]
+
     success_code = 200
 
     def perform_action(self):
         """
         This method is to be overriden. Here is where the particular handler
         action is performed. Its return value is a dictionary with the response body.
         """
```

### Comparing `pyverless-0.0.8/pyverless/auth.py` & `pyverless-0.0.9/pyverless/auth.py`

 * *Files identical despite different names*

### Comparing `pyverless-0.0.8/pyverless/crypto.py` & `pyverless-0.0.9/pyverless/crypto.py`

 * *Files identical despite different names*

### Comparing `pyverless-0.0.8/README.md` & `pyverless-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyverless-0.0.8/setup.py` & `pyverless-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='pyverless',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.8',
+    version='0.0.9',
 
     description='A mini-framework providing tools to help you make complex APIs with serverless',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/QuantumBA/pyverless',
```

### Comparing `pyverless-0.0.8/PKG-INFO` & `pyverless-0.0.9/pyverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverless
-Version: 0.0.8
+Version: 0.0.9
 Summary: A mini-framework providing tools to help you make complex APIs with serverless
 Home-page: https://github.com/QuantumBA/pyverless
 Author: Carlos de las Heras - Foqum
 Author-email: info@foqum.io
 License: BSD
 Description: [![Build Status](https://travis-ci.org/QuantumBA/pyverless.svg?branch=master)](https://travis-ci.org/QuantumBA/pyverless)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyverless.svg)](https://pypi.python.org/pypi/pyverless/)
@@ -188,9 +188,9 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
```

### Comparing `pyverless-0.0.8/pyverless.egg-info/PKG-INFO` & `pyverless-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyverless
-Version: 0.0.8
+Version: 0.0.9
 Summary: A mini-framework providing tools to help you make complex APIs with serverless
 Home-page: https://github.com/QuantumBA/pyverless
 Author: Carlos de las Heras - Foqum
 Author-email: info@foqum.io
 License: BSD
 Description: [![Build Status](https://travis-ci.org/QuantumBA/pyverless.svg?branch=master)](https://travis-ci.org/QuantumBA/pyverless)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyverless.svg)](https://pypi.python.org/pypi/pyverless/)
@@ -188,9 +188,9 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
```

### Comparing `pyverless-0.0.8/LICENSE.txt` & `pyverless-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

