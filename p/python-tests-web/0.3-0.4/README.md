# Comparing `tmp/python_tests_web-0.3.tar.gz` & `tmp/python_tests_web-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tests_web-0.3.tar", last modified: Tue Apr 23 03:56:58 2024, max compression
+gzip compressed data, was "python_tests_web-0.4.tar", last modified: Tue Apr 23 13:39:04 2024, max compression
```

## Comparing `python_tests_web-0.3.tar` & `python_tests_web-0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 03:56:58.194714 python_tests_web-0.3/
--rw-rw-rw-   0        0        0      414 2024-04-23 03:56:58.193709 python_tests_web-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      929 2024-04-13 23:49:58.000000 python_tests_web-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 03:56:58.190412 python_tests_web-0.3/python_tests_web.egg-info/
--rw-rw-rw-   0        0        0      414 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      318 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 03:56:58.000000 python_tests_web-0.3/python_tests_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 03:56:58.194714 python_tests_web-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1001 2024-04-23 03:56:49.000000 python_tests_web-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:39:04.253443 python_tests_web-0.4/
+-rw-rw-rw-   0        0        0      414 2024-04-23 13:39:04.232029 python_tests_web-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 13:39:04.211094 python_tests_web-0.4/python_tests_web/
+-rw-rw-rw-   0        0        0      112 2024-04-23 12:33:01.000000 python_tests_web-0.4/python_tests_web/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:39:04.230504 python_tests_web-0.4/python_tests_web.egg-info/
+-rw-rw-rw-   0        0        0      414 2024-04-23 13:39:04.000000 python_tests_web-0.4/python_tests_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-04-23 13:39:04.000000 python_tests_web-0.4/python_tests_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:39:04.000000 python_tests_web-0.4/python_tests_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      335 2024-04-23 13:39:04.000000 python_tests_web-0.4/python_tests_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-23 13:39:04.000000 python_tests_web-0.4/python_tests_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:39:04.254023 python_tests_web-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2024-04-23 13:38:53.000000 python_tests_web-0.4/setup.py
```

### Comparing `python_tests_web-0.3/setup.py` & `python_tests_web-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages 
 
 setup(
     name='python_tests_web',
-    version='0.3',
+    version='0.4',
     description='A simple functional test library using Selenium and Chrome driver',
     author='Linda Lopez',
     packages=find_packages(),
     install_requires=[
         "allure-behave==2.13.4",
         "allure-python-commons==2.13.4",
         "behave==1.2.6",
@@ -19,14 +19,15 @@
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
         "selenium==4.1.3",
         "webdriver-manager==4.0.1",
         "webdrivermanager==0.10.0",
+        "keyboard==0.13.5"
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python'
     ],
```

