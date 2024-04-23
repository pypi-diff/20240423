# Comparing `tmp/python_optimization-0.0.7.tar.gz` & `tmp/python_optimization-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_optimization-0.0.7.tar", last modified: Mon Apr 22 11:59:19 2024, max compression
+gzip compressed data, was "python_optimization-0.0.8.tar", last modified: Tue Apr 23 11:24:23 2024, max compression
```

## Comparing `python_optimization-0.0.7.tar` & `python_optimization-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 11:59:19.987967 python_optimization-0.0.7/
--rw-rw-rw-   0        0        0      551 2024-04-22 11:59:19.986967 python_optimization-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 11:59:19.965961 python_optimization-0.0.7/python_optimization/
--rw-rw-rw-   0        0        0       53 2024-04-22 11:28:07.000000 python_optimization-0.0.7/python_optimization/__init__.py
--rw-rw-rw-   0        0        0    23973 2024-04-22 11:59:01.000000 python_optimization-0.0.7/python_optimization/python_optimization.py
-drwxrwxrwx   0        0        0        0 2024-04-22 11:59:19.984964 python_optimization-0.0.7/python_optimization.egg-info/
--rw-rw-rw-   0        0        0      551 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 11:59:19.987967 python_optimization-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      861 2024-04-22 11:47:43.000000 python_optimization-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:24:23.986207 python_optimization-0.0.8/
+-rw-rw-rw-   0        0        0      551 2024-04-23 11:24:23.986207 python_optimization-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 11:24:23.968168 python_optimization-0.0.8/python_optimization/
+-rw-rw-rw-   0        0        0       53 2024-04-22 11:28:07.000000 python_optimization-0.0.8/python_optimization/__init__.py
+-rw-rw-rw-   0        0        0    37262 2024-04-23 11:21:56.000000 python_optimization-0.0.8/python_optimization/python_optimization.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:24:23.985204 python_optimization-0.0.8/python_optimization.egg-info/
+-rw-rw-rw-   0        0        0      551 2024-04-23 11:24:23.000000 python_optimization-0.0.8/python_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-23 11:24:23.000000 python_optimization-0.0.8/python_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 11:24:23.000000 python_optimization-0.0.8/python_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-23 11:24:23.000000 python_optimization-0.0.8/python_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 11:24:23.987207 python_optimization-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-04-23 11:13:58.000000 python_optimization-0.0.8/setup.py
```

### Comparing `python_optimization-0.0.7/PKG-INFO` & `python_optimization-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_optimization
-Version: 0.0.7
+Version: 0.0.8
 Summary: python optimization
 Author: founder synergy
 Author-email: founders.synergy@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.7/python_optimization.egg-info/PKG-INFO` & `python_optimization-0.0.8/python_optimization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-optimization
-Version: 0.0.7
+Version: 0.0.8
 Summary: python optimization
 Author: founder synergy
 Author-email: founders.synergy@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_optimization-0.0.7/setup.py` & `python_optimization-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'python optimization'
 LONG_DESCRIPTION = 'A package that allows python optimization'
 
 # Setting up
 setup(
     name="python_optimization",
     version=VERSION,
```

