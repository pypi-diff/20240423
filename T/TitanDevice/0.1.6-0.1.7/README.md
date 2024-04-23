# Comparing `tmp/TitanDevice-0.1.6.tar.gz` & `tmp/TitanDevice-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.1.6.tar", last modified: Tue Apr 23 09:50:19 2024, max compression
+gzip compressed data, was "TitanDevice-0.1.7.tar", last modified: Tue Apr 23 10:13:28 2024, max compression
```

## Comparing `TitanDevice-0.1.6.tar` & `TitanDevice-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:50:19.798596 TitanDevice-0.1.6/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:50:19.798596 TitanDevice-0.1.6/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.6/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:50:19.798596 TitanDevice-0.1.6/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:50:19.000000 TitanDevice-0.1.6/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 09:50:19.000000 TitanDevice-0.1.6/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 09:50:19.000000 TitanDevice-0.1.6/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 09:50:19.000000 TitanDevice-0.1.6/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 09:50:19.000000 TitanDevice-0.1.6/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 09:50:19.798596 TitanDevice-0.1.6/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 09:50:14.000000 TitanDevice-0.1.6/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:50:19.798596 TitanDevice-0.1.6/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)      556 2024-04-23 09:50:14.000000 TitanDevice-0.1.6/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.6/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1783 2024-04-23 09:32:44.000000 TitanDevice-0.1.6/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      217 2024-04-23 09:14:41.000000 TitanDevice-0.1.6/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.7/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:13:28.610948 TitanDevice-0.1.7/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 10:13:28.000000 TitanDevice-0.1.7/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 10:13:25.000000 TitanDevice-0.1.7/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:13:28.614949 TitanDevice-0.1.7/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      704 2024-04-23 10:13:25.000000 TitanDevice-0.1.7/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.7/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1783 2024-04-23 09:32:44.000000 TitanDevice-0.1.7/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      217 2024-04-23 09:14:41.000000 TitanDevice-0.1.7/titan/_device_models.py
```

### Comparing `TitanDevice-0.1.6/PKG-INFO` & `TitanDevice-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.6/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.1.7/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.6/setup.py` & `TitanDevice-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.1.6",
+    version="0.1.7",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.1.6/titan/_device_manager.py` & `TitanDevice-0.1.7/titan/_device_manager.py`

 * *Files identical despite different names*

