# Comparing `tmp/dmce_aids-0.0.0.tar.gz` & `tmp/dmce_aids-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmce_aids-0.0.0.tar", last modified: Tue Apr 23 16:48:52 2024, max compression
+gzip compressed data, was "dmce_aids-0.0.1.tar", last modified: Tue Apr 23 16:59:22 2024, max compression
```

## Comparing `dmce_aids-0.0.0.tar` & `dmce_aids-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 16:48:52.563747 dmce_aids-0.0.0/
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 16:48:52.563175 dmce_aids-0.0.0/DMCE_AIDS.egg-info/
--rw-r--r--   0 trish      (501) staff       (20)      624 2024-04-23 16:48:52.000000 dmce_aids-0.0.0/DMCE_AIDS.egg-info/PKG-INFO
--rw-r--r--   0 trish      (501) staff       (20)      192 2024-04-23 16:48:52.000000 dmce_aids-0.0.0/DMCE_AIDS.egg-info/SOURCES.txt
--rw-r--r--   0 trish      (501) staff       (20)        1 2024-04-23 16:48:52.000000 dmce_aids-0.0.0/DMCE_AIDS.egg-info/dependency_links.txt
--rw-r--r--   0 trish      (501) staff       (20)       46 2024-04-23 16:48:52.000000 dmce_aids-0.0.0/DMCE_AIDS.egg-info/requires.txt
--rw-r--r--   0 trish      (501) staff       (20)        8 2024-04-23 16:48:52.000000 dmce_aids-0.0.0/DMCE_AIDS.egg-info/top_level.txt
--rw-r--r--   0 trish      (501) staff       (20)      624 2024-04-23 16:48:52.563476 dmce_aids-0.0.0/PKG-INFO
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 16:48:52.562720 dmce_aids-0.0.0/libname/
--rw-r--r--   0 trish      (501) staff       (20)       35 2024-04-23 16:37:22.000000 dmce_aids-0.0.0/libname/__init__.py
--rw-r--r--   0 trish      (501) staff       (20)       38 2024-04-23 16:48:52.563814 dmce_aids-0.0.0/setup.cfg
--rw-r--r--   0 trish      (501) staff       (20)      888 2024-04-23 16:46:52.000000 dmce_aids-0.0.0/setup.py
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 16:59:22.779108 dmce_aids-0.0.1/
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 16:59:22.778517 dmce_aids-0.0.1/DMCE_AIDS.egg-info/
+-rw-r--r--   0 trish      (501) staff       (20)      595 2024-04-23 16:59:22.000000 dmce_aids-0.0.1/DMCE_AIDS.egg-info/PKG-INFO
+-rw-r--r--   0 trish      (501) staff       (20)      320 2024-04-23 16:59:22.000000 dmce_aids-0.0.1/DMCE_AIDS.egg-info/SOURCES.txt
+-rw-r--r--   0 trish      (501) staff       (20)        1 2024-04-23 16:59:22.000000 dmce_aids-0.0.1/DMCE_AIDS.egg-info/dependency_links.txt
+-rw-r--r--   0 trish      (501) staff       (20)       32 2024-04-23 16:59:22.000000 dmce_aids-0.0.1/DMCE_AIDS.egg-info/requires.txt
+-rw-r--r--   0 trish      (501) staff       (20)        8 2024-04-23 16:59:22.000000 dmce_aids-0.0.1/DMCE_AIDS.egg-info/top_level.txt
+-rw-r--r--   0 trish      (501) staff       (20)      595 2024-04-23 16:59:22.778809 dmce_aids-0.0.1/PKG-INFO
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 16:59:22.778056 dmce_aids-0.0.1/libname/
+-rw-r--r--   0 trish      (501) staff       (20)     2068 2024-04-23 16:09:23.000000 dmce_aids-0.0.1/libname/ML-1.py
+-rw-r--r--   0 trish      (501) staff       (20)      818 2024-04-23 16:17:51.000000 dmce_aids-0.0.1/libname/ML-2.py
+-rw-r--r--   0 trish      (501) staff       (20)     1355 2024-04-23 16:19:53.000000 dmce_aids-0.0.1/libname/ML-3.py
+-rw-r--r--   0 trish      (501) staff       (20)     1102 2024-04-23 16:20:40.000000 dmce_aids-0.0.1/libname/ML-4.py
+-rw-r--r--   0 trish      (501) staff       (20)      547 2024-04-23 16:21:36.000000 dmce_aids-0.0.1/libname/ML-5.py
+-rw-r--r--   0 trish      (501) staff       (20)      733 2024-04-23 16:23:24.000000 dmce_aids-0.0.1/libname/ML-7.py
+-rw-r--r--   0 trish      (501) staff       (20)     1590 2024-04-23 16:24:16.000000 dmce_aids-0.0.1/libname/ML-8.py
+-rw-r--r--   0 trish      (501) staff       (20)     1021 2024-04-23 16:24:39.000000 dmce_aids-0.0.1/libname/ML-9.py
+-rw-r--r--   0 trish      (501) staff       (20)       35 2024-04-23 16:37:22.000000 dmce_aids-0.0.1/libname/__init__.py
+-rw-r--r--   0 trish      (501) staff       (20)       38 2024-04-23 16:59:22.779171 dmce_aids-0.0.1/setup.cfg
+-rw-r--r--   0 trish      (501) staff       (20)      871 2024-04-23 16:58:50.000000 dmce_aids-0.0.1/setup.py
```

### Comparing `dmce_aids-0.0.0/DMCE_AIDS.egg-info/PKG-INFO` & `dmce_aids-0.0.1/DMCE_AIDS.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: DMCE_AIDS
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python Library for AIDS form DMCE s
 Author: Students of AIDS
 Author-email: aids@gmail.com
 Keywords: python,video,stream,aids,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: opencv-python
 Requires-Dist: scikit-learn
 Requires-Dist: tensorflow
 Requires-Dist: dataset
 
 Python Library for AIDS form DMCE
```

### Comparing `dmce_aids-0.0.0/PKG-INFO` & `dmce_aids-0.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: DMCE_AIDS
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python Library for AIDS form DMCE s
 Author: Students of AIDS
 Author-email: aids@gmail.com
 Keywords: python,video,stream,aids,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: opencv-python
 Requires-Dist: scikit-learn
 Requires-Dist: tensorflow
 Requires-Dist: dataset
 
 Python Library for AIDS form DMCE
```

### Comparing `dmce_aids-0.0.0/setup.py` & `dmce_aids-0.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.0'
+VERSION = '0.0.1'
 DESCRIPTION = 'Python Library for AIDS form DMCE s'
 LONG_DESCRIPTION = 'Python Library for AIDS form DMCE'
 # Setting up
 setup(
     name="DMCE_AIDS",
     version=VERSION,
     author="Students of AIDS",
     author_email="aids@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['opencv-python', 'scikit-learn', 'tensorflow', 'dataset'],
+    install_requires=['scikit-learn', 'tensorflow', 'dataset'],
     keywords=['python', 'video', 'stream', 'aids', 'camera stream', 'sockets'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

