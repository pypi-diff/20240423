# Comparing `tmp/convertapi-1.7.0.tar.gz` & `tmp/convertapi-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convertapi-1.7.0.tar", last modified: Wed Jul 19 17:30:23 2023, max compression
+gzip compressed data, was "convertapi-1.8.0.tar", last modified: Tue Apr 23 20:13:15 2024, max compression
```

## Comparing `convertapi-1.7.0.tar` & `convertapi-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 laurynas  (1000) laurynas  (1000)        0 2023-07-19 17:30:23.448923 convertapi-1.7.0/
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)     1201 2018-08-17 18:13:30.000000 convertapi-1.7.0/LICENSE.txt
--rw-rw-r--   0 laurynas  (1000) laurynas  (1000)      699 2023-07-19 17:30:23.448923 convertapi-1.7.0/PKG-INFO
--rw-rw-r--   0 laurynas  (1000) laurynas  (1000)     3705 2023-07-19 17:10:29.000000 convertapi-1.7.0/README.md
-drwxrwxr-x   0 laurynas  (1000) laurynas  (1000)        0 2023-07-19 17:30:23.444923 convertapi-1.7.0/convertapi/
--rw-rw-r--   0 laurynas  (1000) laurynas  (1000)      443 2023-07-19 17:25:12.000000 convertapi-1.7.0/convertapi/__init__.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      287 2018-08-18 12:48:46.000000 convertapi-1.7.0/convertapi/api.py
--rw-rw-r--   0 laurynas  (1000) laurynas  (1000)     1745 2023-02-04 22:04:05.000000 convertapi-1.7.0/convertapi/client.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      434 2019-12-04 10:35:02.000000 convertapi-1.7.0/convertapi/exceptions.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      567 2018-09-30 06:26:25.000000 convertapi-1.7.0/convertapi/file_param.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      545 2018-09-30 08:20:27.000000 convertapi-1.7.0/convertapi/format_detector.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      461 2018-08-18 13:21:16.000000 convertapi-1.7.0/convertapi/result.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      645 2018-09-30 08:20:27.000000 convertapi-1.7.0/convertapi/result_file.py
--rw-rw-r--   0 laurynas  (1000) laurynas  (1000)     2148 2023-07-19 17:24:08.000000 convertapi-1.7.0/convertapi/task.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      767 2018-09-30 08:20:27.000000 convertapi-1.7.0/convertapi/upload_io.py
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      262 2020-07-04 19:16:08.000000 convertapi-1.7.0/convertapi/utils.py
-drwxrwxr-x   0 laurynas  (1000) laurynas  (1000)        0 2023-07-19 17:30:23.444923 convertapi-1.7.0/convertapi.egg-info/
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      699 2023-07-19 17:30:23.000000 convertapi-1.7.0/convertapi.egg-info/PKG-INFO
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      486 2023-07-19 17:30:23.000000 convertapi-1.7.0/convertapi.egg-info/SOURCES.txt
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)        1 2023-07-19 17:30:23.000000 convertapi-1.7.0/convertapi.egg-info/dependency_links.txt
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)       16 2023-07-19 17:30:23.000000 convertapi-1.7.0/convertapi.egg-info/requires.txt
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)       11 2023-07-19 17:30:23.000000 convertapi-1.7.0/convertapi.egg-info/top_level.txt
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)      124 2023-07-19 17:30:23.448923 convertapi-1.7.0/setup.cfg
--rw-r--r--   0 laurynas  (1000) laurynas  (1000)     1007 2018-08-17 18:13:30.000000 convertapi-1.7.0/setup.py
-drwxrwxr-x   0 laurynas  (1000) laurynas  (1000)        0 2023-07-19 17:30:23.444923 convertapi-1.7.0/tests/
--rw-rw-r--   0 laurynas  (1000) laurynas  (1000)     2854 2023-07-19 17:24:08.000000 convertapi-1.7.0/tests/test_convertapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:13:15.710756 convertapi-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-23 20:13:07.000000 convertapi-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 20:13:15.710756 convertapi-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-23 20:13:07.000000 convertapi-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:13:15.710756 convertapi-1.8.0/convertapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/file_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/format_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/result_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/upload_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 20:13:07.000000 convertapi-1.8.0/convertapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:13:15.710756 convertapi-1.8.0/convertapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 20:13:15.000000 convertapi-1.8.0/convertapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-23 20:13:15.000000 convertapi-1.8.0/convertapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:13:15.000000 convertapi-1.8.0/convertapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 20:13:15.000000 convertapi-1.8.0/convertapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 20:13:15.000000 convertapi-1.8.0/convertapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 20:13:15.710756 convertapi-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-23 20:13:07.000000 convertapi-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:13:15.710756 convertapi-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-23 20:13:07.000000 convertapi-1.8.0/tests/test_convertapi.py
```

### Comparing `convertapi-1.7.0/LICENSE.txt` & `convertapi-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `convertapi-1.7.0/PKG-INFO` & `convertapi-1.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: convertapi
-Version: 1.7.0
+Version: 1.8.0
 Summary: Convert API Python Client
 Home-page: https://github.com/ConvertAPI/convertapi-python
 Download-URL: https://github.com/ConvertAPI/convertapi-python
 Author: Tomas Rutkauskas
 Author-email: support@convertapi.com
 License: MIT
 Keywords: convert,api,client,conversion
 License-File: LICENSE.txt
+Requires-Dist: requests>=2.4.2
 
 Convert various files like MS Word, Excel, PowerPoint, Images to PDF and Images. Create PDF and Images from url and raw HTML. Extract and create PowerPoint presentation from PDF. Merge, Encrypt, Split, Repair and Decrypt PDF files. All supported files conversions and manipulations can be found at https://www.convertapi.com/doc/supported-formats
```

### Comparing `convertapi-1.7.0/README.md` & `convertapi-1.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,25 @@
 
 ```python
 import convertapi
 
 convertapi.api_secret = 'your-api-secret'
 ```
 
+If you prefer to use [token and API key](https://www.convertapi.com/doc/auth#token), you can configure like this:
+
+```python
+import convertapi
+
+convertapi.api_token = 'your-api-token'
+convertapi.api_key = 000000 # your api key
+```
+
+If both API secret and token are configured, token will be used.
+
 #### Proxy configuration
 
 If you need to use a proxy, you can specify it using `HTTPS_PROXY` environment variable when running your script.
 
 Example:
 
 ```
```

### Comparing `convertapi-1.7.0/convertapi/client.py` & `convertapi-1.8.0/convertapi/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,20 @@
 				raise ApiError(r.json())
 			except ValueError:
 				raise e
 
 		return r.json()
 
 	def __url(self, path):
+		if convertapi.api_token != None and convertapi.api_key != None:
+			return "%s%s?Token=%s&ApiKey=%d" % (convertapi.base_uri, path, convertapi.api_token, convertapi.api_key)
+
+		if convertapi.api_token != None:
+			return "%s%s?Token=%s" % (convertapi.base_uri, path, convertapi.api_token)
+
 		return "%s%s?Secret=%s" % (convertapi.base_uri, path, convertapi.api_secret)
 
 	def __session(self):
 		s = requests.Session()
 		s.headers.update({ 'User-Agent': convertapi.user_agent })
 		s.verify = convertapi.verify_ssl
```

### Comparing `convertapi-1.7.0/convertapi/file_param.py` & `convertapi-1.8.0/convertapi/file_param.py`

 * *Files identical despite different names*

### Comparing `convertapi-1.7.0/convertapi/format_detector.py` & `convertapi-1.8.0/convertapi/format_detector.py`

 * *Files identical despite different names*

### Comparing `convertapi-1.7.0/convertapi/result_file.py` & `convertapi-1.8.0/convertapi/result_file.py`

 * *Files identical despite different names*

### Comparing `convertapi-1.7.0/convertapi/task.py` & `convertapi-1.8.0/convertapi/task.py`

 * *Files identical despite different names*

### Comparing `convertapi-1.7.0/convertapi/upload_io.py` & `convertapi-1.8.0/convertapi/upload_io.py`

 * *Files identical despite different names*

### Comparing `convertapi-1.7.0/convertapi.egg-info/PKG-INFO` & `convertapi-1.8.0/convertapi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: convertapi
-Version: 1.7.0
+Version: 1.8.0
 Summary: Convert API Python Client
 Home-page: https://github.com/ConvertAPI/convertapi-python
 Download-URL: https://github.com/ConvertAPI/convertapi-python
 Author: Tomas Rutkauskas
 Author-email: support@convertapi.com
 License: MIT
 Keywords: convert,api,client,conversion
 License-File: LICENSE.txt
+Requires-Dist: requests>=2.4.2
 
 Convert various files like MS Word, Excel, PowerPoint, Images to PDF and Images. Create PDF and Images from url and raw HTML. Extract and create PowerPoint presentation from PDF. Merge, Encrypt, Split, Repair and Decrypt PDF files. All supported files conversions and manipulations can be found at https://www.convertapi.com/doc/supported-formats
```

### Comparing `convertapi-1.7.0/setup.py` & `convertapi-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `convertapi-1.7.0/tests/test_convertapi.py` & `convertapi-1.8.0/tests/test_convertapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import convertapi
 import os
 import io
 import tempfile
 import requests
+import responses
 
 from . import utils
 from nose.tools import *
 
 class TestConvertapi(utils.TestCase):
 	def setUp(self):
 		convertapi.api_secret = os.environ['CONVERT_API_SECRET']
+		convertapi.api_key = None
+		convertapi.api_token = None
 		convertapi.max_parallel_uploads = 10
 
 	def test_defaults(self):
 		eq_('https://v2.convertapi.com/', convertapi.base_uri)
 
 	def test_configuration(self):
 		convertapi.api_secret = 'TEST'
@@ -75,7 +78,22 @@
 	def test_api_error(self):
 		convertapi.api_secret = 'TEST'
 		convertapi.convert('pdf', { 'Url': 'https://www.w3.org/TR/PNG/iso_8859-1.txt' })
 
 	def test_user_info(self):
 		user_info = convertapi.user()
 		assert user_info['Active']
+
+	@responses.activate
+	def test_with_token(self):
+		convertapi.api_token = 'TEST'
+		responses.add(responses.POST, 'https://v2.convertapi.com/convert/web/to/pdf?Token=TEST', json = { 'ConversionCost': 123 })
+		result = convertapi.convert('pdf', { 'Url': 'dummyurl' })
+		assert result.conversion_cost == 123
+
+	@responses.activate
+	def test_with_token_and_api_key(self):
+		convertapi.api_token = 'TEST'
+		convertapi.api_key = 1
+		responses.add(responses.POST, 'https://v2.convertapi.com/convert/web/to/pdf?Token=TEST&ApiKey=1', json = { 'ConversionCost': 123 })
+		result = convertapi.convert('pdf', { 'Url': 'dummyurl' })
+		assert result.conversion_cost == 123
```

