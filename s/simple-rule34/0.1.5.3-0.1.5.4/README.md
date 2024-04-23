# Comparing `tmp/simple_rule34-0.1.5.3.tar.gz` & `tmp/simple_rule34-0.1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\alexk\PycharmProjects\rule34-simple-api\SimpleRule34\dist\.tmp-wzkxyq0z\simple_rule34-0.1.5.3.tar", last modified: Mon Jan  1 18:43:26 2024, max compression
+gzip compressed data, was "C:\Users\alexk\PycharmProjects\rule34-simple-api\SimpleRule34\dist\.tmp-1dmg2l59\simple_rule34-0.1.5.4.tar", last modified: Tue Apr 23 10:47:19 2024, max compression
```

## Comparing `simple_rule34-0.1.5.3.tar` & `simple_rule34-0.1.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-01-01 18:43:26.024351 simple_rule34-0.1.5.3/
--rw-rw-rw-   0        0        0     1091 2023-07-16 23:21:11.000000 simple_rule34-0.1.5.3/LICENSE
--rw-rw-rw-   0        0        0     2050 2024-01-01 18:43:26.022355 simple_rule34-0.1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-07-16 23:04:58.000000 simple_rule34-0.1.5.3/README.md
--rw-rw-rw-   0        0        0     1738 2024-01-01 18:37:34.000000 simple_rule34-0.1.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-01 18:43:26.024351 simple_rule34-0.1.5.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-01 18:43:25.978998 simple_rule34-0.1.5.3/src/
-drwxrwxrwx   0        0        0        0 2024-01-01 18:43:25.990964 simple_rule34-0.1.5.3/src/SimpleRule34/
--rw-rw-rw-   0        0        0     7136 2023-08-09 15:50:58.000000 simple_rule34-0.1.5.3/src/SimpleRule34/Rule34.py
--rw-rw-rw-   0        0        0       31 2023-07-16 22:47:21.000000 simple_rule34-0.1.5.3/src/SimpleRule34/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-01 18:43:25.994953 simple_rule34-0.1.5.3/src/SimpleRule34/aio/
--rw-rw-rw-   0        0        0     6858 2023-10-06 08:28:11.000000 simple_rule34-0.1.5.3/src/SimpleRule34/aio/ARule34.py
--rw-rw-rw-   0        0        0     3679 2023-07-16 22:47:21.000000 simple_rule34-0.1.5.3/src/SimpleRule34/aio/types.py
--rw-rw-rw-   0        0        0      616 2023-08-09 15:24:47.000000 simple_rule34-0.1.5.3/src/SimpleRule34/aio/utils.py
--rw-rw-rw-   0        0        0      354 2023-07-16 22:41:52.000000 simple_rule34-0.1.5.3/src/SimpleRule34/exceptions.py
--rw-rw-rw-   0        0        0      735 2023-07-16 23:11:26.000000 simple_rule34-0.1.5.3/src/SimpleRule34/setup.py
--rw-rw-rw-   0        0        0     3278 2024-01-01 18:33:32.000000 simple_rule34-0.1.5.3/src/SimpleRule34/types.py
--rw-rw-rw-   0        0        0      854 2023-07-24 19:44:30.000000 simple_rule34-0.1.5.3/src/SimpleRule34/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-01 18:43:26.021358 simple_rule34-0.1.5.3/src/simple_rule34.egg-info/
--rw-rw-rw-   0        0        0     2050 2024-01-01 18:43:25.000000 simple_rule34-0.1.5.3/src/simple_rule34.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2024-01-01 18:43:25.000000 simple_rule34-0.1.5.3/src/simple_rule34.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-01 18:43:25.000000 simple_rule34-0.1.5.3/src/simple_rule34.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      747 2024-01-01 18:43:25.000000 simple_rule34-0.1.5.3/src/simple_rule34.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-01 18:43:25.000000 simple_rule34-0.1.5.3/src/simple_rule34.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-01 18:43:26.019364 simple_rule34-0.1.5.3/tests/
--rw-rw-rw-   0        0        0     1547 2024-01-01 18:32:54.000000 simple_rule34-0.1.5.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:47:19.673471 simple_rule34-0.1.5.4/
+-rw-rw-rw-   0        0        0     1091 2023-07-16 23:21:11.000000 simple_rule34-0.1.5.4/LICENSE
+-rw-rw-rw-   0        0        0     2050 2024-04-23 10:47:19.672474 simple_rule34-0.1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-07-16 23:04:58.000000 simple_rule34-0.1.5.4/README.md
+-rw-rw-rw-   0        0        0     1738 2024-04-23 10:44:16.000000 simple_rule34-0.1.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 10:47:19.673471 simple_rule34-0.1.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 10:47:19.635573 simple_rule34-0.1.5.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 10:47:19.646541 simple_rule34-0.1.5.4/src/SimpleRule34/
+-rw-rw-rw-   0        0        0     7136 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.4/src/SimpleRule34/Rule34.py
+-rw-rw-rw-   0        0        0       31 2023-07-16 22:47:21.000000 simple_rule34-0.1.5.4/src/SimpleRule34/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:47:19.651530 simple_rule34-0.1.5.4/src/SimpleRule34/aio/
+-rw-rw-rw-   0        0        0     6858 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.4/src/SimpleRule34/aio/ARule34.py
+-rw-rw-rw-   0        0        0     3713 2024-04-23 10:39:07.000000 simple_rule34-0.1.5.4/src/SimpleRule34/aio/types.py
+-rw-rw-rw-   0        0        0      616 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.4/src/SimpleRule34/aio/utils.py
+-rw-rw-rw-   0        0        0      354 2023-07-16 22:41:52.000000 simple_rule34-0.1.5.4/src/SimpleRule34/exceptions.py
+-rw-rw-rw-   0        0        0      735 2023-07-16 23:11:26.000000 simple_rule34-0.1.5.4/src/SimpleRule34/setup.py
+-rw-rw-rw-   0        0        0     3278 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.4/src/SimpleRule34/types.py
+-rw-rw-rw-   0        0        0      854 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.4/src/SimpleRule34/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:47:19.670481 simple_rule34-0.1.5.4/src/simple_rule34.egg-info/
+-rw-rw-rw-   0        0        0     2050 2024-04-23 10:47:19.000000 simple_rule34-0.1.5.4/src/simple_rule34.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2024-04-23 10:47:19.000000 simple_rule34-0.1.5.4/src/simple_rule34.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:47:19.000000 simple_rule34-0.1.5.4/src/simple_rule34.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      747 2024-04-23 10:47:19.000000 simple_rule34-0.1.5.4/src/simple_rule34.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-23 10:47:19.000000 simple_rule34-0.1.5.4/src/simple_rule34.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 10:47:19.668483 simple_rule34-0.1.5.4/tests/
+-rw-rw-rw-   0        0        0     1547 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.4/tests/test.py
```

### Comparing `simple_rule34-0.1.5.3/LICENSE` & `simple_rule34-0.1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/PKG-INFO` & `simple_rule34-0.1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_rule34
-Version: 0.1.5.3
+Version: 0.1.5.4
 Summary: Simple api wrapper of rule34.xxx for python with asynchronous support
 Author-email: StarMan12 <author@example.com>
 Project-URL: Homepage, https://github.com/SyperAlexKomp/simple-rule34-api
 Project-URL: Bug Tracker, https://github.com/SyperAlexKomp/simple-rule34-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_rule34-0.1.5.3/pyproject.toml` & `simple_rule34-0.1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_rule34"
-version = "0.1.5.3"
+version = "0.1.5.4"
 authors = [
   { name="StarMan12", email="author@example.com" },
 ]
 description = "Simple api wrapper of rule34.xxx for python with asynchronous support"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `simple_rule34-0.1.5.3/src/SimpleRule34/Rule34.py` & `simple_rule34-0.1.5.4/src/SimpleRule34/Rule34.py`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/src/SimpleRule34/aio/ARule34.py` & `simple_rule34-0.1.5.4/src/SimpleRule34/aio/ARule34.py`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/src/SimpleRule34/aio/types.py` & `simple_rule34-0.1.5.4/src/SimpleRule34/aio/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import typing
+
+import aiofiles
 import aiohttp
 import os
 import datetime
 
 from .utils import get_file_size, get_file_type
 
 
@@ -30,16 +32,16 @@
                     try:
                         os.mkdir(self.path)
                     except:
                         pass
 
                     file_name = os.path.basename(self.url)
                     save_path = os.path.join(path, file_name)
-                    with open(save_path, 'wb') as file:
-                        file.write(await response.read())
+                    with aiofiles.open(save_path, 'wb') as file:
+                        await file.write(await response.read())
 
                     return save_path
                 else:
                     pass
 
     async def get_bytes(self):
         async with aiohttp.ClientSession() as session:
```

### Comparing `simple_rule34-0.1.5.3/src/SimpleRule34/aio/utils.py` & `simple_rule34-0.1.5.4/src/SimpleRule34/aio/utils.py`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/src/SimpleRule34/setup.py` & `simple_rule34-0.1.5.4/src/SimpleRule34/setup.py`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/src/SimpleRule34/types.py` & `simple_rule34-0.1.5.4/src/SimpleRule34/types.py`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/src/SimpleRule34/utils.py` & `simple_rule34-0.1.5.4/src/SimpleRule34/utils.py`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/src/simple_rule34.egg-info/PKG-INFO` & `simple_rule34-0.1.5.4/src/simple_rule34.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_rule34
-Version: 0.1.5.3
+Version: 0.1.5.4
 Summary: Simple api wrapper of rule34.xxx for python with asynchronous support
 Author-email: StarMan12 <author@example.com>
 Project-URL: Homepage, https://github.com/SyperAlexKomp/simple-rule34-api
 Project-URL: Bug Tracker, https://github.com/SyperAlexKomp/simple-rule34-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_rule34-0.1.5.3/src/simple_rule34.egg-info/requires.txt` & `simple_rule34-0.1.5.4/src/simple_rule34.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.3/tests/test.py` & `simple_rule34-0.1.5.4/tests/test.py`

 * *Files identical despite different names*

