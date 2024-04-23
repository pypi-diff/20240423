# Comparing `tmp/python_tests_web-0.2.tar.gz` & `tmp/python_tests_web-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tests_web-0.2.tar", last modified: Mon Apr 22 21:37:00 2024, max compression
+gzip compressed data, was "python_tests_web-0.3.tar", last modified: Tue Apr 23 03:56:58 2024, max compression
```

## Comparing `python_tests_web-0.2.tar` & `python_tests_web-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 21:37:00.710543 python_tests_web-0.2/
--rw-rw-rw-   0        0        0      344 2024-04-22 21:37:00.708964 python_tests_web-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      929 2024-04-13 23:49:58.000000 python_tests_web-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 21:37:00.698515 python_tests_web-0.2/python_tests_web.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-22 21:37:00.000000 python_tests_web-0.2/python_tests_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-04-22 21:37:00.000000 python_tests_web-0.2/python_tests_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 21:37:00.000000 python_tests_web-0.2/python_tests_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      318 2024-04-22 21:37:00.000000 python_tests_web-0.2/python_tests_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 21:37:00.000000 python_tests_web-0.2/python_tests_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 21:37:00.710782 python_tests_web-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1001 2024-04-22 21:36:47.000000 python_tests_web-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 03:56:58.194714 python_tests_web-0.3/
+-rw-rw-rw-   0        0        0      414 2024-04-23 03:56:58.193709 python_tests_web-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      929 2024-04-13 23:49:58.000000 python_tests_web-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 03:56:58.190412 python_tests_web-0.3/python_tests_web.egg-info/
+-rw-rw-rw-   0        0        0      414 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      318 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 03:56:58.194714 python_tests_web-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2024-04-23 03:56:49.000000 python_tests_web-0.3/setup.py
```

### Comparing `python_tests_web-0.2/README.md` & `python_tests_web-0.3/README.md`

 * *Files identical despite different names*

### Comparing `python_tests_web-0.2/setup.py` & `python_tests_web-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages 
 
 setup(
     name='python_tests_web',
-    version='0.2',
+    version='0.3',
     description='A simple functional test library using Selenium and Chrome driver',
     author='Linda Lopez',
     packages=find_packages(),
     install_requires=[
         "allure-behave==2.13.4",
         "allure-python-commons==2.13.4",
         "behave==1.2.6",
```

