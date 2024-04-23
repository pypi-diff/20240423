# Comparing `tmp/mycttestsdk-0.1.0.tar.gz` & `tmp/mycttestsdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycttestsdk-0.1.0.tar", last modified: Tue Apr 23 03:19:13 2024, max compression
+gzip compressed data, was "mycttestsdk-0.1.1.tar", last modified: Tue Apr 23 07:05:09 2024, max compression
```

## Comparing `mycttestsdk-0.1.0.tar` & `mycttestsdk-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 03:19:13.146250 mycttestsdk-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-04-23 02:31:04.000000 mycttestsdk-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      790 2024-04-23 03:19:13.145250 mycttestsdk-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      597 2024-04-23 02:20:21.000000 mycttestsdk-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-23 03:19:13.124251 mycttestsdk-0.1.0/mycttestsdk/
--rw-rw-rw-   0        0        0        0 2024-04-23 02:20:21.000000 mycttestsdk-0.1.0/mycttestsdk/__init__.py
--rw-rw-rw-   0        0        0       48 2024-04-23 02:20:21.000000 mycttestsdk-0.1.0/mycttestsdk/run.py
-drwxrwxrwx   0        0        0        0 2024-04-23 03:19:13.143249 mycttestsdk-0.1.0/mycttestsdk.egg-info/
--rw-rw-rw-   0        0        0      790 2024-04-23 03:19:13.000000 mycttestsdk-0.1.0/mycttestsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-23 03:19:13.000000 mycttestsdk-0.1.0/mycttestsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 03:19:13.000000 mycttestsdk-0.1.0/mycttestsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-23 03:19:13.000000 mycttestsdk-0.1.0/mycttestsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 03:19:13.146250 mycttestsdk-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-04-23 03:19:11.000000 mycttestsdk-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:05:09.996862 mycttestsdk-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-23 02:31:04.000000 mycttestsdk-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      790 2024-04-23 07:05:09.994861 mycttestsdk-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2024-04-23 02:20:21.000000 mycttestsdk-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 07:05:09.985866 mycttestsdk-0.1.1/mycttestsdk/
+-rw-rw-rw-   0        0        0        0 2024-04-23 02:20:21.000000 mycttestsdk-0.1.1/mycttestsdk/__init__.py
+-rw-rw-rw-   0        0        0      740 2024-04-23 06:45:27.000000 mycttestsdk-0.1.1/mycttestsdk/run.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:05:09.994861 mycttestsdk-0.1.1/mycttestsdk.egg-info/
+-rw-rw-rw-   0        0        0      790 2024-04-23 07:05:09.000000 mycttestsdk-0.1.1/mycttestsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-23 07:05:09.000000 mycttestsdk-0.1.1/mycttestsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 07:05:09.000000 mycttestsdk-0.1.1/mycttestsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 07:05:09.000000 mycttestsdk-0.1.1/mycttestsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 07:05:09.996862 mycttestsdk-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-23 06:59:48.000000 mycttestsdk-0.1.1/setup.py
```

### Comparing `mycttestsdk-0.1.0/LICENSE` & `mycttestsdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mycttestsdk-0.1.0/PKG-INFO` & `mycttestsdk-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycttestsdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Used for integration with Application monitoring systems
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The purpose of this project is to show how to upload a python package to the PYPI server.
 
 Main commands:
```

### Comparing `mycttestsdk-0.1.0/README.rst` & `mycttestsdk-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `mycttestsdk-0.1.0/mycttestsdk.egg-info/PKG-INFO` & `mycttestsdk-0.1.1/mycttestsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycttestsdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Used for integration with Application monitoring systems
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The purpose of this project is to show how to upload a python package to the PYPI server.
 
 Main commands:
```

### Comparing `mycttestsdk-0.1.0/setup.py` & `mycttestsdk-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import pathlib
  
 setup(
     name='mycttestsdk',  # Replace with your actual package name
     # url = 'https://github.com/enomis-dev/test-package', # Replace with your github project link
-    version='0.1.0',
+    version='0.1.1',
     description="Used for integration with Application monitoring systems",
     long_description = pathlib.Path("README.rst").read_text(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         # Your project dependencies
     ],
```

