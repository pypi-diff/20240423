# Comparing `tmp/dmce_aids-0.0.5.tar.gz` & `tmp/dmce_aids-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmce_aids-0.0.5.tar", last modified: Tue Apr 23 19:03:02 2024, max compression
+gzip compressed data, was "dmce_aids-0.0.6.tar", last modified: Tue Apr 23 19:19:49 2024, max compression
```

## Comparing `dmce_aids-0.0.5.tar` & `dmce_aids-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 19:03:02.540134 dmce_aids-0.0.5/
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 19:03:02.539451 dmce_aids-0.0.5/DMCE_AIDS.egg-info/
--rw-r--r--   0 trish      (501) staff       (20)      608 2024-04-23 19:03:02.000000 dmce_aids-0.0.5/DMCE_AIDS.egg-info/PKG-INFO
--rw-r--r--   0 trish      (501) staff       (20)      358 2024-04-23 19:03:02.000000 dmce_aids-0.0.5/DMCE_AIDS.egg-info/SOURCES.txt
--rw-r--r--   0 trish      (501) staff       (20)        1 2024-04-23 19:03:02.000000 dmce_aids-0.0.5/DMCE_AIDS.egg-info/dependency_links.txt
--rw-r--r--   0 trish      (501) staff       (20)       42 2024-04-23 19:03:02.000000 dmce_aids-0.0.5/DMCE_AIDS.egg-info/entry_points.txt
--rw-r--r--   0 trish      (501) staff       (20)       42 2024-04-23 19:03:02.000000 dmce_aids-0.0.5/DMCE_AIDS.egg-info/requires.txt
--rw-r--r--   0 trish      (501) staff       (20)        5 2024-04-23 19:03:02.000000 dmce_aids-0.0.5/DMCE_AIDS.egg-info/top_level.txt
--rw-r--r--   0 trish      (501) staff       (20)      608 2024-04-23 19:03:02.539794 dmce_aids-0.0.5/PKG-INFO
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 19:03:02.538889 dmce_aids-0.0.5/sem6/
--rw-------   0 trish      (501) staff       (20)    13790 2024-04-23 17:25:44.000000 dmce_aids-0.0.5/sem6/DAV.py
--rw-r--r--   0 trish      (501) staff       (20)     2068 2024-04-23 16:09:23.000000 dmce_aids-0.0.5/sem6/ML-1.py
--rw-r--r--   0 trish      (501) staff       (20)      818 2024-04-23 16:17:51.000000 dmce_aids-0.0.5/sem6/ML-2.py
--rw-r--r--   0 trish      (501) staff       (20)     1355 2024-04-23 16:19:53.000000 dmce_aids-0.0.5/sem6/ML-3.py
--rw-r--r--   0 trish      (501) staff       (20)     1102 2024-04-23 16:20:40.000000 dmce_aids-0.0.5/sem6/ML-4.py
--rw-r--r--   0 trish      (501) staff       (20)      547 2024-04-23 16:21:36.000000 dmce_aids-0.0.5/sem6/ML-5.py
--rw-r--r--   0 trish      (501) staff       (20)      733 2024-04-23 16:23:24.000000 dmce_aids-0.0.5/sem6/ML-7.py
--rw-r--r--   0 trish      (501) staff       (20)     1590 2024-04-23 16:24:16.000000 dmce_aids-0.0.5/sem6/ML-8.py
--rw-r--r--   0 trish      (501) staff       (20)     1021 2024-04-23 16:24:39.000000 dmce_aids-0.0.5/sem6/ML-9.py
--rw-r--r--   0 trish      (501) staff       (20)       35 2024-04-23 16:37:22.000000 dmce_aids-0.0.5/sem6/__init__.py
--rw-r--r--   0 trish      (501) staff       (20)     1292 2024-04-23 18:54:04.000000 dmce_aids-0.0.5/sem6/programs.py
--rw-r--r--   0 trish      (501) staff       (20)       38 2024-04-23 19:03:02.540215 dmce_aids-0.0.5/setup.cfg
--rw-r--r--   0 trish      (501) staff       (20)      976 2024-04-23 19:02:39.000000 dmce_aids-0.0.5/setup.py
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 19:19:49.421024 dmce_aids-0.0.6/
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 19:19:49.420315 dmce_aids-0.0.6/DMCE_AIDS.egg-info/
+-rw-r--r--   0 trish      (501) staff       (20)      608 2024-04-23 19:19:49.000000 dmce_aids-0.0.6/DMCE_AIDS.egg-info/PKG-INFO
+-rw-r--r--   0 trish      (501) staff       (20)      372 2024-04-23 19:19:49.000000 dmce_aids-0.0.6/DMCE_AIDS.egg-info/SOURCES.txt
+-rw-r--r--   0 trish      (501) staff       (20)        1 2024-04-23 19:19:49.000000 dmce_aids-0.0.6/DMCE_AIDS.egg-info/dependency_links.txt
+-rw-r--r--   0 trish      (501) staff       (20)       42 2024-04-23 19:19:49.000000 dmce_aids-0.0.6/DMCE_AIDS.egg-info/entry_points.txt
+-rw-r--r--   0 trish      (501) staff       (20)       42 2024-04-23 19:19:49.000000 dmce_aids-0.0.6/DMCE_AIDS.egg-info/requires.txt
+-rw-r--r--   0 trish      (501) staff       (20)        5 2024-04-23 19:19:49.000000 dmce_aids-0.0.6/DMCE_AIDS.egg-info/top_level.txt
+-rw-r--r--   0 trish      (501) staff       (20)      608 2024-04-23 19:19:49.420700 dmce_aids-0.0.6/PKG-INFO
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 19:19:49.419943 dmce_aids-0.0.6/sem6/
+-rw-------   0 trish      (501) staff       (20)    13790 2024-04-23 17:25:44.000000 dmce_aids-0.0.6/sem6/DAV.py
+-rw-r--r--   0 trish      (501) staff       (20)     2068 2024-04-23 16:09:23.000000 dmce_aids-0.0.6/sem6/ML-1.py
+-rw-r--r--   0 trish      (501) staff       (20)    13790 2024-04-23 17:48:59.000000 dmce_aids-0.0.6/sem6/ML-10.py
+-rw-r--r--   0 trish      (501) staff       (20)      818 2024-04-23 16:17:51.000000 dmce_aids-0.0.6/sem6/ML-2.py
+-rw-r--r--   0 trish      (501) staff       (20)     1355 2024-04-23 16:19:53.000000 dmce_aids-0.0.6/sem6/ML-3.py
+-rw-r--r--   0 trish      (501) staff       (20)     1102 2024-04-23 16:20:40.000000 dmce_aids-0.0.6/sem6/ML-4.py
+-rw-r--r--   0 trish      (501) staff       (20)      547 2024-04-23 16:21:36.000000 dmce_aids-0.0.6/sem6/ML-5.py
+-rw-r--r--   0 trish      (501) staff       (20)      733 2024-04-23 16:23:24.000000 dmce_aids-0.0.6/sem6/ML-7.py
+-rw-r--r--   0 trish      (501) staff       (20)     1590 2024-04-23 16:24:16.000000 dmce_aids-0.0.6/sem6/ML-8.py
+-rw-r--r--   0 trish      (501) staff       (20)     1021 2024-04-23 16:24:39.000000 dmce_aids-0.0.6/sem6/ML-9.py
+-rw-r--r--   0 trish      (501) staff       (20)       35 2024-04-23 16:37:22.000000 dmce_aids-0.0.6/sem6/__init__.py
+-rw-r--r--   0 trish      (501) staff       (20)     1324 2024-04-23 19:18:27.000000 dmce_aids-0.0.6/sem6/programs.py
+-rw-r--r--   0 trish      (501) staff       (20)       38 2024-04-23 19:19:49.421117 dmce_aids-0.0.6/setup.cfg
+-rw-r--r--   0 trish      (501) staff       (20)      976 2024-04-23 19:19:45.000000 dmce_aids-0.0.6/setup.py
```

### Comparing `dmce_aids-0.0.5/DMCE_AIDS.egg-info/PKG-INFO` & `dmce_aids-0.0.6/DMCE_AIDS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMCE-AIDS
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Library for AIDS form DMCE s
 Author: sdad
 Author-email: aids@gmail.com
 Keywords: python,video,stream,aids,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `dmce_aids-0.0.5/PKG-INFO` & `dmce_aids-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMCE-AIDS
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Library for AIDS form DMCE s
 Author: sdad
 Author-email: aids@gmail.com
 Keywords: python,video,stream,aids,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `dmce_aids-0.0.5/sem6/DAV.py` & `dmce_aids-0.0.6/sem6/DAV.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-1.py` & `dmce_aids-0.0.6/sem6/ML-1.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-2.py` & `dmce_aids-0.0.6/sem6/ML-2.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-3.py` & `dmce_aids-0.0.6/sem6/ML-3.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-4.py` & `dmce_aids-0.0.6/sem6/ML-4.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-5.py` & `dmce_aids-0.0.6/sem6/ML-5.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-7.py` & `dmce_aids-0.0.6/sem6/ML-7.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-8.py` & `dmce_aids-0.0.6/sem6/ML-8.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/sem6/ML-9.py` & `dmce_aids-0.0.6/sem6/ML-9.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.5/setup.py` & `dmce_aids-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 DESCRIPTION = 'Python Library for AIDS form DMCE s'
 LONG_DESCRIPTION = 'Python Library for AIDS form DMCE'
 # Setting up
 setup(
     name="DMCE-AIDS",
     version=VERSION,
```

