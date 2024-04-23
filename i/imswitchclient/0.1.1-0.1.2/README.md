# Comparing `tmp/imswitchclient-0.1.1.tar.gz` & `tmp/imswitchclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imswitchclient-0.1.1.tar", last modified: Sat Mar 23 18:02:36 2024, max compression
+gzip compressed data, was "imswitchclient-0.1.2.tar", last modified: Tue Apr 23 06:01:56 2024, max compression
```

## Comparing `imswitchclient-0.1.1.tar` & `imswitchclient-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:02:36.825472 imswitchclient-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-23 18:02:36.825472 imswitchclient-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:02:36.825472 imswitchclient-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4887 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:02:36.825472 imswitchclient-0.1.1/imswitchclient/
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/imswitchclient/ImSwitchClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-23 18:02:31.000000 imswitchclient-0.1.1/imswitchclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/imswitchclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/imswitchclient/positionersManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/imswitchclient/recordingManager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:02:36.825472 imswitchclient-0.1.1/imswitchclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-23 18:02:36.000000 imswitchclient-0.1.1/imswitchclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-23 18:02:36.000000 imswitchclient-0.1.1/imswitchclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 18:02:36.000000 imswitchclient-0.1.1/imswitchclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 18:02:36.000000 imswitchclient-0.1.1/imswitchclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-23 18:02:36.000000 imswitchclient-0.1.1/imswitchclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-23 18:02:36.829472 imswitchclient-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 18:02:36.825472 imswitchclient-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-23 18:02:30.000000 imswitchclient-0.1.1/tests/test_imswitchclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:56.137726 imswitchclient-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-23 06:01:56.137726 imswitchclient-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:56.133726 imswitchclient-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4887 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:56.133726 imswitchclient-0.1.2/imswitchclient/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/imswitchclient/ImSwitchClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 06:01:51.000000 imswitchclient-0.1.2/imswitchclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/imswitchclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/imswitchclient/lasersManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/imswitchclient/positionersManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/imswitchclient/recordingManager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:56.137726 imswitchclient-0.1.2/imswitchclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-23 06:01:56.000000 imswitchclient-0.1.2/imswitchclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 06:01:56.000000 imswitchclient-0.1.2/imswitchclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:01:56.000000 imswitchclient-0.1.2/imswitchclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:01:55.000000 imswitchclient-0.1.2/imswitchclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 06:01:56.000000 imswitchclient-0.1.2/imswitchclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-23 06:01:56.137726 imswitchclient-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:56.137726 imswitchclient-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-23 06:01:50.000000 imswitchclient-0.1.2/tests/test_imswitchclient.py
```

### Comparing `imswitchclient-0.1.1/CONTRIBUTING.rst` & `imswitchclient-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `imswitchclient-0.1.1/LICENSE` & `imswitchclient-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imswitchclient-0.1.1/docs/Makefile` & `imswitchclient-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `imswitchclient-0.1.1/docs/conf.py` & `imswitchclient-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imswitchclient-0.1.1/docs/installation.rst` & `imswitchclient-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `imswitchclient-0.1.1/docs/make.bat` & `imswitchclient-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `imswitchclient-0.1.1/imswitchclient/ImSwitchClient.py` & `imswitchclient-0.1.2/imswitchclient/ImSwitchClient.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 import PIL.Image
 import numpy as np
 import logging
 import os
 
 from .positionersManager import positionersManager
 from .recordingManager import recordingManager
+from .lasersManager import lasersManager
 
 
 class ImSwitchClient(object):
     def __init__(self, host="0.0.0.0", isHttps=True, port=8001):
         self.host = host
         self.port = port
         self.isHttps = isHttps
         self.get_json(self.base_uri+"/openapi.json")
         
         logging.info(f"Connecting to microscope {self.host}:{self.port}")
         
         # register managers
         self.positionersManager = positionersManager(self)
         self.recordingManager = recordingManager(self)
+        self.lasersManager = lasersManager(self)
         
     @property
     def base_uri(self):
         if self.isHttps:
             return f"https://{self.host}:{self.port}"
         else:
             return f"http://{self.host}:{self.port}"
```

### Comparing `imswitchclient-0.1.1/imswitchclient/client.py` & `imswitchclient-0.1.2/imswitchclient/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import io
 import PIL.Image
 import numpy as np
 import logging
 import zeroconf
 import os
 
+import urllib3
+urllib3.disable_warnings()
 
 class ImSwitchClient(object):
     def __init__(self, host="localhost", port=8000):
         self.host = host
         self.port = port
         self.get_json(self.base_uri)
         logging.info(f"Connecting to microscope {self.host}:{self.port}")
```

### Comparing `imswitchclient-0.1.1/imswitchclient/positionersManager.py` & `imswitchclient-0.1.2/imswitchclient/positionersManager.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,22 +7,42 @@
     def getAllDeviceNames(self):
         url = f"{self.parent.base_uri}/PositionerController/getPositionerNames"
         headers = {'accept': 'application/json'}
 
         response = self.parent.get_json(url, headers=headers)
         return response
     
-    def movePositioner(self, positioner_name, axis, dist, is_absolute=True, is_blocking=True):
+    def movePositionerForever(self, speed=(0, 0, 0, 0), is_stop=False):
+        url = f"{self.parent.base_uri}/PositionerController/movePositionerForever"
+        payload = {
+            'speed': speed,
+            'isStop': is_stop
+        }
+        response = self.parent.get_json(url, payload=payload)
+        return response       
+            
+    def setPositionerSpeed(self, positioner_name, axis, speed):
+        url = f"{self.parent.base_uri}/PositionerController/setPositionerSpeed"
+        payload = {
+            'positionerName': positioner_name,
+            'axis': axis,
+            'speed': speed
+        }
+        response = self.parent.get_json(url, payload=payload)
+        return response
+        
+    def movePositioner(self, positioner_name, axis, dist, is_absolute=True, is_blocking=True, speed=10000):
         url = f"{self.parent.base_uri}/PositionerController/movePositioner"
         payload = {
             'positionerName': positioner_name,
             'axis': axis,
             'dist': dist,
             'isAbsolute': is_absolute,
-            'isBlocking': is_blocking
+            'isBlocking': is_blocking, 
+            'speed': speed
         }
         #headers = {'accept': 'application/json'}
 
         response = self.parent.get_json(url, payload=payload)
         return response
 
     def getPositionerPositions(self):
```

### Comparing `imswitchclient-0.1.1/imswitchclient/recordingManager.py` & `imswitchclient-0.1.2/imswitchclient/recordingManager.py`

 * *Files identical despite different names*

### Comparing `imswitchclient-0.1.1/imswitchclient.egg-info/SOURCES.txt` & `imswitchclient-0.1.2/imswitchclient.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 imswitchclient/ImSwitchClient.py
 imswitchclient/__init__.py
 imswitchclient/client.py
+imswitchclient/lasersManager.py
 imswitchclient/positionersManager.py
 imswitchclient/recordingManager.py
 imswitchclient.egg-info/PKG-INFO
 imswitchclient.egg-info/SOURCES.txt
 imswitchclient.egg-info/dependency_links.txt
 imswitchclient.egg-info/not-zip-safe
 imswitchclient.egg-info/top_level.txt
```

### Comparing `imswitchclient-0.1.1/setup.py` & `imswitchclient-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     include_package_data=True,
     keywords='imswitchclient',
     name='imswitchclient',
     packages=find_packages(include=['imswitchclient', 'imswitchclient.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/beniroquai/imswitchclient',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

