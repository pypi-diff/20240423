# Comparing `tmp/yoto_api-1.7.0.tar.gz` & `tmp/yoto_api-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.7.0.tar", last modified: Tue Apr 23 03:47:58 2024, max compression
+gzip compressed data, was "yoto_api-1.7.1.tar", last modified: Tue Apr 23 14:11:04 2024, max compression
```

## Comparing `yoto_api-1.7.0.tar` & `yoto_api-1.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:47:58.477805 yoto_api-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 03:47:37.000000 yoto_api-1.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 03:47:37.000000 yoto_api-1.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 03:47:37.000000 yoto_api-1.7.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 03:47:37.000000 yoto_api-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 03:47:37.000000 yoto_api-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 03:47:58.477805 yoto_api-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 03:47:37.000000 yoto_api-1.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 03:47:37.000000 yoto_api-1.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:47:58.477805 yoto_api-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 03:47:52.000000 yoto_api-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:47:58.473805 yoto_api-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:47:37.000000 yoto_api-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 03:47:37.000000 yoto_api-1.7.0/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:47:58.473805 yoto_api-1.7.0/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 03:47:37.000000 yoto_api-1.7.0/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 03:47:37.000000 yoto_api-1.7.0/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27096 2024-04-23 03:47:37.000000 yoto_api-1.7.0/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 03:47:37.000000 yoto_api-1.7.0/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-23 03:47:37.000000 yoto_api-1.7.0/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 03:47:37.000000 yoto_api-1.7.0/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 03:47:37.000000 yoto_api-1.7.0/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:47:58.477805 yoto_api-1.7.0/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 03:47:58.000000 yoto_api-1.7.0/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 03:47:58.000000 yoto_api-1.7.0/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:47:58.000000 yoto_api-1.7.0/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:47:58.000000 yoto_api-1.7.0/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 03:47:58.000000 yoto_api-1.7.0/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 03:47:58.000000 yoto_api-1.7.0/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.320131 yoto_api-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 14:10:38.000000 yoto_api-1.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 14:10:38.000000 yoto_api-1.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 14:10:38.000000 yoto_api-1.7.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 14:10:38.000000 yoto_api-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 14:10:38.000000 yoto_api-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 14:11:04.320131 yoto_api-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 14:10:38.000000 yoto_api-1.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 14:10:38.000000 yoto_api-1.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:11:04.320131 yoto_api-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 14:10:57.000000 yoto_api-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.316131 yoto_api-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:38.000000 yoto_api-1.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 14:10:38.000000 yoto_api-1.7.1/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.320131 yoto_api-1.7.1/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27096 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 14:10:38.000000 yoto_api-1.7.1/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:11:04.320131 yoto_api-1.7.1/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 14:11:04.000000 yoto_api-1.7.1/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.7.0/CONTRIBUTING.rst` & `yoto_api-1.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.0/LICENSE` & `yoto_api-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.0/PKG-INFO` & `yoto_api-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.7.0/README.rst` & `yoto_api-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.0/setup.py` & `yoto_api-1.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.7.0",
+    version="1.7.1",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.7.0/yoto_api/Card.py` & `yoto_api-1.7.1/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.0/yoto_api/YotoAPI.py` & `yoto_api-1.7.1/yoto_api/YotoAPI.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.0/yoto_api/YotoManager.py` & `yoto_api-1.7.1/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.0/yoto_api/YotoPlayer.py` & `yoto_api-1.7.1/yoto_api/YotoPlayer.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.0/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.7.1/yoto_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

