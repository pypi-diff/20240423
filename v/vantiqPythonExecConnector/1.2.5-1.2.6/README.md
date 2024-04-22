# Comparing `tmp/vantiqpythonexecconnector-1.2.5.tar.gz` & `tmp/vantiqpythonexecconnector-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqpythonexecconnector-1.2.5.tar", last modified: Fri Apr 19 20:59:04 2024, max compression
+gzip compressed data, was "vantiqpythonexecconnector-1.2.6.tar", last modified: Mon Apr 22 23:14:42 2024, max compression
```

## Comparing `vantiqpythonexecconnector-1.2.5.tar` & `vantiqpythonexecconnector-1.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-19 20:59:04.446696 vantiqpythonexecconnector-1.2.5/
--rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-08-10 20:55:53.000000 vantiqpythonexecconnector-1.2.5/LICENSE.txt
--rw-r--r--   0 fcarter    (501) staff       (20)     5526 2024-04-19 20:59:04.445394 vantiqpythonexecconnector-1.2.5/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)     3732 2023-12-01 23:54:03.000000 vantiqpythonexecconnector-1.2.5/README.md
--rw-r--r--   0 fcarter    (501) staff       (20)      103 2022-08-10 20:55:53.000000 vantiqpythonexecconnector-1.2.5/pyproject.toml
--rw-r--r--   0 fcarter    (501) staff       (20)      860 2024-04-19 20:59:04.448415 vantiqpythonexecconnector-1.2.5/setup.cfg
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-19 20:59:04.436797 vantiqpythonexecconnector-1.2.5/src/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-19 20:59:04.437113 vantiqpythonexecconnector-1.2.5/src/main/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-19 20:59:04.439272 vantiqpythonexecconnector-1.2.5/src/main/python/
--rw-r--r--   0 fcarter    (501) staff       (20)    39013 2022-08-10 20:55:53.000000 vantiqpythonexecconnector-1.2.5/src/main/python/pyExecConnector.py
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-19 20:59:04.444694 vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/
--rw-r--r--   0 fcarter    (501) staff       (20)     5526 2024-04-19 20:59:04.000000 vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)      473 2024-04-19 20:59:04.000000 vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/SOURCES.txt
--rw-r--r--   0 fcarter    (501) staff       (20)        1 2024-04-19 20:59:04.000000 vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/dependency_links.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       67 2024-04-19 20:59:04.000000 vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/entry_points.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       91 2024-04-19 20:59:04.000000 vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/requires.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       16 2024-04-19 20:59:04.000000 vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/top_level.txt
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-22 23:14:42.136057 vantiqpythonexecconnector-1.2.6/
+-rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-08-10 20:55:53.000000 vantiqpythonexecconnector-1.2.6/LICENSE.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)     5526 2024-04-22 23:14:42.134705 vantiqpythonexecconnector-1.2.6/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)     3732 2023-12-01 23:54:03.000000 vantiqpythonexecconnector-1.2.6/README.md
+-rw-r--r--   0 fcarter    (501) staff       (20)      103 2022-08-10 20:55:53.000000 vantiqpythonexecconnector-1.2.6/pyproject.toml
+-rw-r--r--   0 fcarter    (501) staff       (20)      860 2024-04-22 23:14:42.137282 vantiqpythonexecconnector-1.2.6/setup.cfg
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-22 23:14:42.127569 vantiqpythonexecconnector-1.2.6/src/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-22 23:14:42.127706 vantiqpythonexecconnector-1.2.6/src/main/
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-22 23:14:42.129634 vantiqpythonexecconnector-1.2.6/src/main/python/
+-rw-r--r--   0 fcarter    (501) staff       (20)    39013 2022-08-10 20:55:53.000000 vantiqpythonexecconnector-1.2.6/src/main/python/pyExecConnector.py
+drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-04-22 23:14:42.134130 vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/
+-rw-r--r--   0 fcarter    (501) staff       (20)     5526 2024-04-22 23:14:42.000000 vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO
+-rw-r--r--   0 fcarter    (501) staff       (20)      473 2024-04-22 23:14:42.000000 vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)        1 2024-04-22 23:14:42.000000 vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       67 2024-04-22 23:14:42.000000 vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/entry_points.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       91 2024-04-22 23:14:42.000000 vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/requires.txt
+-rw-r--r--   0 fcarter    (501) staff       (20)       16 2024-04-22 23:14:42.000000 vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/top_level.txt
```

### Comparing `vantiqpythonexecconnector-1.2.5/LICENSE.txt` & `vantiqpythonexecconnector-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vantiqpythonexecconnector-1.2.5/PKG-INFO` & `vantiqpythonexecconnector-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqPythonExecConnector
-Version: 1.2.5
+Version: 1.2.6
 Summary: Vantiq Connector for Execution of Python Code
 Home-page: https://github.com/Vantiq/vantiq-extension-sources'
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp>=3.8
 Requires-Dist: websockets>=10.2
 Requires-Dist: codetiming>=1.3.0
-Requires-Dist: vantiqsdk>=1.2.4
+Requires-Dist: vantiqsdk>=1.2.5
 Requires-Dist: vantiqconnectorsdk>=1.2.6
 
 
 # Vantiq Python Execution Connector
 
 The [Vantiq](http://www.vantiq.com) Python Execution Connector is a Python package that provides the ability 
 to execute Python code as directed by a Vantiq server
```

### Comparing `vantiqpythonexecconnector-1.2.5/README.md` & `vantiqpythonexecconnector-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vantiqpythonexecconnector-1.2.5/setup.cfg` & `vantiqpythonexecconnector-1.2.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vantiqPythonExecConnector
-version = 1.2.5
+version = 1.2.6
 description = Vantiq Connector for Execution of Python Code
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/Vantiq/vantiq-extension-sources'
 author = Vantiq, Inc
 author_email = fcarter@vantiq.com
 license = MIT
@@ -18,15 +18,15 @@
 package_dir = =src/main/python
 py_modules = pyExecConnector
 python_requires = >=3.10
 install_requires = 
 	aiohttp>=3.8
 	websockets>=10.2
 	codetiming>=1.3.0
-	vantiqsdk>=1.2.4
+	vantiqsdk>=1.2.5
 	vantiqconnectorsdk>=1.2.6
 
 [options.entry_points]
 console_scripts = 
 	vantiqPythonExecConnector = pyExecConnector:main
 
 [egg_info]
```

### Comparing `vantiqpythonexecconnector-1.2.5/src/main/python/pyExecConnector.py` & `vantiqpythonexecconnector-1.2.6/src/main/python/pyExecConnector.py`

 * *Files identical despite different names*

### Comparing `vantiqpythonexecconnector-1.2.5/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO` & `vantiqpythonexecconnector-1.2.6/src/main/python/vantiqPythonExecConnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantiqPythonExecConnector
-Version: 1.2.5
+Version: 1.2.6
 Summary: Vantiq Connector for Execution of Python Code
 Home-page: https://github.com/Vantiq/vantiq-extension-sources'
 Author: Vantiq, Inc
 Author-email: fcarter@vantiq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp>=3.8
 Requires-Dist: websockets>=10.2
 Requires-Dist: codetiming>=1.3.0
-Requires-Dist: vantiqsdk>=1.2.4
+Requires-Dist: vantiqsdk>=1.2.5
 Requires-Dist: vantiqconnectorsdk>=1.2.6
 
 
 # Vantiq Python Execution Connector
 
 The [Vantiq](http://www.vantiq.com) Python Execution Connector is a Python package that provides the ability 
 to execute Python code as directed by a Vantiq server
```

