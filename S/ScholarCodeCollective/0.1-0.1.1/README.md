# Comparing `tmp/ScholarCodeCollective-0.1.tar.gz` & `tmp/ScholarCodeCollective-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.tar", last modified: Mon Apr 22 17:09:33 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.1.tar", last modified: Mon Apr 22 17:18:56 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.tar` & `ScholarCodeCollective-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.259685 ScholarCodeCollective-0.1/
--rw-rw-rw-   0        0        0     3777 2024-04-22 17:09:33.257370 ScholarCodeCollective-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.218716 ScholarCodeCollective-0.1/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.243350 ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-21 08:57:01.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.245240 ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     5448 2024-04-22 16:57:34.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.251277 ScholarCodeCollective-0.1/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      156 2024-04-22 01:56:08.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.253013 ScholarCodeCollective-0.1/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.240703 ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     3777 2024-04-22 17:09:33.000000 ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2024-04-22 17:09:33.000000 ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 17:09:33.000000 ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-22 17:09:33.000000 ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-22 17:09:33.000000 ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 17:09:33.259685 ScholarCodeCollective-0.1/setup.cfg
--rw-rw-rw-   0        0        0      716 2024-04-22 17:09:20.000000 ScholarCodeCollective-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:09:33.256467 ScholarCodeCollective-0.1/tests/
--rw-rw-rw-   0        0        0      872 2024-04-22 16:47:46.000000 ScholarCodeCollective-0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.057505 ScholarCodeCollective-0.1.1/
+-rw-rw-rw-   0        0        0     3782 2024-04-22 17:18:56.056491 ScholarCodeCollective-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.022217 ScholarCodeCollective-0.1.1/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.041345 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.045621 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     5448 2024-04-22 16:57:34.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.049092 ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      156 2024-04-22 01:56:08.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.052046 ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.038045 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     3782 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-22 17:18:55.000000 ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 17:18:56.057673 ScholarCodeCollective-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-04-22 17:18:36.000000 ScholarCodeCollective-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 17:18:56.054371 ScholarCodeCollective-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.1/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1/PKG-INFO` & `ScholarCodeCollective-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1
+Version: 0.1.1
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >3.9,<3.12
-Description-Content-Type: text/plain
+Description-Content-Type: text/markdown
 
 # A template to structure your Python application
 A python project to use as a template when developing a Python application.
 
 ## In order to create a Python project with a similar structure you need to do the following: 
 ### The structure of the project should be as follows: 
 ```
```

### Comparing `ScholarCodeCollective-0.1/README.md` & `ScholarCodeCollective-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.1/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.1/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.1/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1
+Version: 0.1.1
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >3.9,<3.12
-Description-Content-Type: text/plain
+Description-Content-Type: text/markdown
 
 # A template to structure your Python application
 A python project to use as a template when developing a Python application.
 
 ## In order to create a Python project with a similar structure you need to do the following: 
 ### The structure of the project should be as follows: 
 ```
```

### Comparing `ScholarCodeCollective-0.1/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.1/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1/setup.py` & `ScholarCodeCollective-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from distutils.core import setup
 import pathlib
 import setuptools
 
 setuptools.setup(
     name='ScholarCodeCollective',
-    version='0.1',
+    version='0.1.1',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
-    long_description_content_type='text/plain',
+    long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name', 
     author_email='author_email@mail.com',
     license='The Unlicense',
     projects_urls={
         "Documentation": "x",
         "Source": "https://github.com"
```

