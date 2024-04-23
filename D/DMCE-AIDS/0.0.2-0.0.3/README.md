# Comparing `tmp/dmce_aids-0.0.2.tar.gz` & `tmp/dmce_aids-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmce_aids-0.0.2.tar", last modified: Tue Apr 23 17:38:23 2024, max compression
+gzip compressed data, was "dmce_aids-0.0.3.tar", last modified: Tue Apr 23 18:42:43 2024, max compression
```

## Comparing `dmce_aids-0.0.2.tar` & `dmce_aids-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 17:38:23.438876 dmce_aids-0.0.2/
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 17:38:23.438270 dmce_aids-0.0.2/DMCE_AIDS.egg-info/
--rw-r--r--   0 trish      (501) staff       (20)      595 2024-04-23 17:38:23.000000 dmce_aids-0.0.2/DMCE_AIDS.egg-info/PKG-INFO
--rw-r--r--   0 trish      (501) staff       (20)      305 2024-04-23 17:38:23.000000 dmce_aids-0.0.2/DMCE_AIDS.egg-info/SOURCES.txt
--rw-r--r--   0 trish      (501) staff       (20)        1 2024-04-23 17:38:23.000000 dmce_aids-0.0.2/DMCE_AIDS.egg-info/dependency_links.txt
--rw-r--r--   0 trish      (501) staff       (20)       32 2024-04-23 17:38:23.000000 dmce_aids-0.0.2/DMCE_AIDS.egg-info/requires.txt
--rw-r--r--   0 trish      (501) staff       (20)        5 2024-04-23 17:38:23.000000 dmce_aids-0.0.2/DMCE_AIDS.egg-info/top_level.txt
--rw-r--r--   0 trish      (501) staff       (20)      595 2024-04-23 17:38:23.438590 dmce_aids-0.0.2/PKG-INFO
-drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 17:38:23.437725 dmce_aids-0.0.2/sem6/
--rw-------   0 trish      (501) staff       (20)    13790 2024-04-23 17:25:44.000000 dmce_aids-0.0.2/sem6/DAV.py
--rw-r--r--   0 trish      (501) staff       (20)     2068 2024-04-23 16:09:23.000000 dmce_aids-0.0.2/sem6/ML-1.py
--rw-r--r--   0 trish      (501) staff       (20)      818 2024-04-23 16:17:51.000000 dmce_aids-0.0.2/sem6/ML-2.py
--rw-r--r--   0 trish      (501) staff       (20)     1355 2024-04-23 16:19:53.000000 dmce_aids-0.0.2/sem6/ML-3.py
--rw-r--r--   0 trish      (501) staff       (20)     1102 2024-04-23 16:20:40.000000 dmce_aids-0.0.2/sem6/ML-4.py
--rw-r--r--   0 trish      (501) staff       (20)      547 2024-04-23 16:21:36.000000 dmce_aids-0.0.2/sem6/ML-5.py
--rw-r--r--   0 trish      (501) staff       (20)      733 2024-04-23 16:23:24.000000 dmce_aids-0.0.2/sem6/ML-7.py
--rw-r--r--   0 trish      (501) staff       (20)     1590 2024-04-23 16:24:16.000000 dmce_aids-0.0.2/sem6/ML-8.py
--rw-r--r--   0 trish      (501) staff       (20)     1021 2024-04-23 16:24:39.000000 dmce_aids-0.0.2/sem6/ML-9.py
--rw-r--r--   0 trish      (501) staff       (20)       35 2024-04-23 16:37:22.000000 dmce_aids-0.0.2/sem6/__init__.py
--rw-r--r--   0 trish      (501) staff       (20)       38 2024-04-23 17:38:23.438940 dmce_aids-0.0.2/setup.cfg
--rw-r--r--   0 trish      (501) staff       (20)      872 2024-04-23 17:36:01.000000 dmce_aids-0.0.2/setup.py
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 18:42:43.234869 dmce_aids-0.0.3/
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 18:42:43.234269 dmce_aids-0.0.3/DMCE_AIDS.egg-info/
+-rw-r--r--   0 trish      (501) staff       (20)      620 2024-04-23 18:42:43.000000 dmce_aids-0.0.3/DMCE_AIDS.egg-info/PKG-INFO
+-rw-r--r--   0 trish      (501) staff       (20)      322 2024-04-23 18:42:43.000000 dmce_aids-0.0.3/DMCE_AIDS.egg-info/SOURCES.txt
+-rw-r--r--   0 trish      (501) staff       (20)        1 2024-04-23 18:42:43.000000 dmce_aids-0.0.3/DMCE_AIDS.egg-info/dependency_links.txt
+-rw-r--r--   0 trish      (501) staff       (20)       42 2024-04-23 18:42:43.000000 dmce_aids-0.0.3/DMCE_AIDS.egg-info/requires.txt
+-rw-r--r--   0 trish      (501) staff       (20)        5 2024-04-23 18:42:43.000000 dmce_aids-0.0.3/DMCE_AIDS.egg-info/top_level.txt
+-rw-r--r--   0 trish      (501) staff       (20)      620 2024-04-23 18:42:43.234580 dmce_aids-0.0.3/PKG-INFO
+drwxr-xr-x   0 trish      (501) staff       (20)        0 2024-04-23 18:42:43.233923 dmce_aids-0.0.3/sem6/
+-rw-------   0 trish      (501) staff       (20)    13790 2024-04-23 17:25:44.000000 dmce_aids-0.0.3/sem6/DAV.py
+-rw-r--r--   0 trish      (501) staff       (20)     2068 2024-04-23 16:09:23.000000 dmce_aids-0.0.3/sem6/ML-1.py
+-rw-r--r--   0 trish      (501) staff       (20)      818 2024-04-23 16:17:51.000000 dmce_aids-0.0.3/sem6/ML-2.py
+-rw-r--r--   0 trish      (501) staff       (20)     1355 2024-04-23 16:19:53.000000 dmce_aids-0.0.3/sem6/ML-3.py
+-rw-r--r--   0 trish      (501) staff       (20)     1102 2024-04-23 16:20:40.000000 dmce_aids-0.0.3/sem6/ML-4.py
+-rw-r--r--   0 trish      (501) staff       (20)      547 2024-04-23 16:21:36.000000 dmce_aids-0.0.3/sem6/ML-5.py
+-rw-r--r--   0 trish      (501) staff       (20)      733 2024-04-23 16:23:24.000000 dmce_aids-0.0.3/sem6/ML-7.py
+-rw-r--r--   0 trish      (501) staff       (20)     1590 2024-04-23 16:24:16.000000 dmce_aids-0.0.3/sem6/ML-8.py
+-rw-r--r--   0 trish      (501) staff       (20)     1021 2024-04-23 16:24:39.000000 dmce_aids-0.0.3/sem6/ML-9.py
+-rw-r--r--   0 trish      (501) staff       (20)       35 2024-04-23 16:37:22.000000 dmce_aids-0.0.3/sem6/__init__.py
+-rw-r--r--   0 trish      (501) staff       (20)     1291 2024-04-23 18:39:27.000000 dmce_aids-0.0.3/sem6/programs.py
+-rw-r--r--   0 trish      (501) staff       (20)       38 2024-04-23 18:42:43.234931 dmce_aids-0.0.3/setup.cfg
+-rw-r--r--   0 trish      (501) staff       (20)      885 2024-04-23 18:42:39.000000 dmce_aids-0.0.3/setup.py
```

### Comparing `dmce_aids-0.0.2/DMCE_AIDS.egg-info/PKG-INFO` & `dmce_aids-0.0.3/DMCE_AIDS.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: DMCE_AIDS
-Version: 0.0.2
+Version: 0.0.3
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
+Requires-Dist: pyperclip
 Requires-Dist: scikit-learn
 Requires-Dist: tensorflow
 Requires-Dist: dataset
 
 Python Library for AIDS form DMCE
```

### Comparing `dmce_aids-0.0.2/PKG-INFO` & `dmce_aids-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: DMCE_AIDS
-Version: 0.0.2
+Version: 0.0.3
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
+Requires-Dist: pyperclip
 Requires-Dist: scikit-learn
 Requires-Dist: tensorflow
 Requires-Dist: dataset
 
 Python Library for AIDS form DMCE
```

### Comparing `dmce_aids-0.0.2/sem6/DAV.py` & `dmce_aids-0.0.3/sem6/DAV.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-1.py` & `dmce_aids-0.0.3/sem6/ML-1.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-2.py` & `dmce_aids-0.0.3/sem6/ML-2.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-3.py` & `dmce_aids-0.0.3/sem6/ML-3.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-4.py` & `dmce_aids-0.0.3/sem6/ML-4.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-5.py` & `dmce_aids-0.0.3/sem6/ML-5.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-7.py` & `dmce_aids-0.0.3/sem6/ML-7.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-8.py` & `dmce_aids-0.0.3/sem6/ML-8.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/sem6/ML-9.py` & `dmce_aids-0.0.3/sem6/ML-9.py`

 * *Files identical despite different names*

### Comparing `dmce_aids-0.0.2/setup.py` & `dmce_aids-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
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
-    install_requires=['scikit-learn', 'tensorflow', 'dataset'],
+    install_requires=['pyperclip', 'scikit-learn', 'tensorflow', 'dataset'],
     keywords=['python', 'video', 'stream', 'aids', 'camera stream', 'sockets'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```
