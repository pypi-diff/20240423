# Comparing `tmp/TitanDevice-0.1.1.tar.gz` & `tmp/TitanDevice-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.1.1.tar", last modified: Tue Apr 23 08:20:18 2024, max compression
+gzip compressed data, was "TitanDevice-0.1.2.tar", last modified: Tue Apr 23 08:57:20 2024, max compression
```

## Comparing `TitanDevice-0.1.1.tar` & `TitanDevice-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:20:18.005302 TitanDevice-0.1.1/
--rw-r--r--   0 mark      (1000) mark      (1000)      572 2024-04-23 08:20:18.005302 TitanDevice-0.1.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:20:18.005302 TitanDevice-0.1.1/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      572 2024-04-23 08:20:17.000000 TitanDevice-0.1.1/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      292 2024-04-23 08:20:17.000000 TitanDevice-0.1.1/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 08:20:17.000000 TitanDevice-0.1.1/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        9 2024-04-23 08:20:17.000000 TitanDevice-0.1.1/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 08:20:17.000000 TitanDevice-0.1.1/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 08:20:18.005302 TitanDevice-0.1.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      776 2024-04-23 08:20:14.000000 TitanDevice-0.1.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:20:18.005302 TitanDevice-0.1.1/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)      915 2024-04-23 08:15:59.000000 TitanDevice-0.1.1/tests/test__device_manager.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:20:18.005302 TitanDevice-0.1.1/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)      118 2024-04-23 08:20:14.000000 TitanDevice-0.1.1/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.1/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      454 2024-04-23 08:10:57.000000 TitanDevice-0.1.1/titan/_device_manager.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.2/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      316 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 08:29:39.000000 TitanDevice-0.1.2/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      915 2024-04-23 08:15:59.000000 TitanDevice-0.1.2/tests/test__device_manager.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      118 2024-04-23 08:20:14.000000 TitanDevice-0.1.2/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.2/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1066 2024-04-23 08:57:15.000000 TitanDevice-0.1.2/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      127 2024-04-23 08:57:14.000000 TitanDevice-0.1.2/titan/_device_models.py
```

### Comparing `TitanDevice-0.1.1/PKG-INFO` & `TitanDevice-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: adbutils
+Requires-Dist: pydantic
 
 # Titan
 
 A Python library used for managing devices, including:
 
 - Obtaining information of all devices
 - Checking the status of a device
```

### Comparing `TitanDevice-0.1.1/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.1.2/TitanDevice.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: adbutils
+Requires-Dist: pydantic
 
 # Titan
 
 A Python library used for managing devices, including:
 
 - Obtaining information of all devices
 - Checking the status of a device
```

### Comparing `TitanDevice-0.1.1/setup.py` & `TitanDevice-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.1.1",
+    version="0.1.2",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
-        'adbutils'
+        'adbutils',
+        'pydantic'
     ],
 )
```

### Comparing `TitanDevice-0.1.1/tests/test__device_manager.py` & `TitanDevice-0.1.2/tests/test__device_manager.py`

 * *Files identical despite different names*

