# Comparing `tmp/testit_adapter_robotframework-3.0.2.tar.gz` & `tmp/testit_adapter_robotframework-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_adapter_robotframework-3.0.2.tar", last modified: Mon Apr 22 12:43:30 2024, max compression
+gzip compressed data, was "testit_adapter_robotframework-3.1.0.tar", last modified: Tue Apr 23 15:10:28 2024, max compression
```

## Comparing `testit_adapter_robotframework-3.0.2.tar` & `testit_adapter_robotframework-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:30.720339 testit_adapter_robotframework-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-22 12:43:30.720339 testit_adapter_robotframework-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-22 12:43:20.000000 testit_adapter_robotframework-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:43:30.720339 testit_adapter_robotframework-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-22 12:43:20.000000 testit_adapter_robotframework-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:30.720339 testit_adapter_robotframework-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:30.720339 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-22 12:43:20.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/TMSLibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:20.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-22 12:43:20.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-04-22 12:43:20.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-22 12:43:20.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:43:30.720339 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-22 12:43:30.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-22 12:43:30.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:43:30.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 12:43:30.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 12:43:30.000000 testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:28.152413 testit_adapter_robotframework-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-23 15:10:28.152413 testit_adapter_robotframework-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-23 15:10:23.000000 testit_adapter_robotframework-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:10:28.152413 testit_adapter_robotframework-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-23 15:10:23.000000 testit_adapter_robotframework-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:28.148413 testit_adapter_robotframework-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:28.152413 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-23 15:10:23.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:23.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-23 15:10:23.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-04-23 15:10:23.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-23 15:10:23.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:28.152413 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-23 15:10:28.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 15:10:28.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:10:28.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 15:10:28.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 15:10:28.000000 testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testit_adapter_robotframework-3.0.2/PKG-INFO` & `testit_adapter_robotframework-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 3.0.2
+Version: 3.1.0
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: robotframework
-Requires-Dist: testit-python-commons==3.0.2
+Requires-Dist: testit-python-commons==3.1.0
 
 # Test IT TMS adapter for Robot Framework
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
 [![Downloads](https://img.shields.io/pypi/dm/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
```

### Comparing `testit_adapter_robotframework-3.0.2/README.md` & `testit_adapter_robotframework-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `testit_adapter_robotframework-3.0.2/setup.py` & `testit_adapter_robotframework-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-robotframework',
-    version='3.0.2',
+    version='3.1.0',
     description='Robot Framework adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -19,9 +19,9 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testit-python-commons==3.0.2']
+    install_requires=['attrs', 'robotframework', 'testit-python-commons==3.1.0']
 )
```

### Comparing `testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/TMSLibrary.py` & `testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/TMSLibrary.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/listeners.py` & `testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/listeners.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/models.py` & `testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/models.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework/utils.py` & `testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework/utils.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/PKG-INFO` & `testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 3.0.2
+Version: 3.1.0
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: robotframework
-Requires-Dist: testit-python-commons==3.0.2
+Requires-Dist: testit-python-commons==3.1.0
 
 # Test IT TMS adapter for Robot Framework
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
 [![Downloads](https://img.shields.io/pypi/dm/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
```

### Comparing `testit_adapter_robotframework-3.0.2/src/testit_adapter_robotframework.egg-info/SOURCES.txt` & `testit_adapter_robotframework-3.1.0/src/testit_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*
