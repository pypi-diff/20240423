# Comparing `tmp/TitanDevice-0.1.2.tar.gz` & `tmp/TitanDevice-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.1.2.tar", last modified: Tue Apr 23 08:57:20 2024, max compression
+gzip compressed data, was "TitanDevice-0.1.3.tar", last modified: Tue Apr 23 09:00:55 2024, max compression
```

## Comparing `TitanDevice-0.1.2.tar` & `TitanDevice-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.2/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      316 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 08:57:20.000000 TitanDevice-0.1.2/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 08:29:39.000000 TitanDevice-0.1.2/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)      915 2024-04-23 08:15:59.000000 TitanDevice-0.1.2/tests/test__device_manager.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 08:57:20.120336 TitanDevice-0.1.2/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)      118 2024-04-23 08:20:14.000000 TitanDevice-0.1.2/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.2/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1066 2024-04-23 08:57:15.000000 TitanDevice-0.1.2/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      127 2024-04-23 08:57:14.000000 TitanDevice-0.1.2/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:00:55.401035 TitanDevice-0.1.3/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:00:55.401035 TitanDevice-0.1.3/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.3/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:00:55.401035 TitanDevice-0.1.3/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 09:00:55.000000 TitanDevice-0.1.3/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      315 2024-04-23 09:00:55.000000 TitanDevice-0.1.3/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 09:00:55.000000 TitanDevice-0.1.3/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 09:00:55.000000 TitanDevice-0.1.3/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 09:00:55.000000 TitanDevice-0.1.3/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 09:00:55.401035 TitanDevice-0.1.3/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 09:00:50.000000 TitanDevice-0.1.3/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:00:55.401035 TitanDevice-0.1.3/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      915 2024-04-23 08:15:59.000000 TitanDevice-0.1.3/tests/test__device_manager.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 09:00:55.401035 TitanDevice-0.1.3/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      118 2024-04-23 08:20:14.000000 TitanDevice-0.1.3/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      154 2024-04-23 07:31:51.000000 TitanDevice-0.1.3/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1066 2024-04-23 08:57:15.000000 TitanDevice-0.1.3/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      127 2024-04-23 08:57:14.000000 TitanDevice-0.1.3/titan/device_models.py
```

### Comparing `TitanDevice-0.1.2/setup.py` & `TitanDevice-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.1.2",
+    version="0.1.3",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.1.2/tests/test__device_manager.py` & `TitanDevice-0.1.3/tests/test__device_manager.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.1.2/titan/_device_manager.py` & `TitanDevice-0.1.3/titan/_device_manager.py`

 * *Files identical despite different names*

