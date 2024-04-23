# Comparing `tmp/ScholarCodeCollective-0.1.2.tar.gz` & `tmp/ScholarCodeCollective-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.2.tar", last modified: Tue Apr 23 11:59:43 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.3.tar", last modified: Tue Apr 23 12:07:27 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.2.tar` & `ScholarCodeCollective-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.333406 ScholarCodeCollective-0.1.2/
--rw-rw-rw-   0        0        0     3782 2024-04-23 11:59:43.332530 ScholarCodeCollective-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.296111 ScholarCodeCollective-0.1.2/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.315152 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.321231 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.322765 ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      156 2024-04-22 01:56:08.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.328699 ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.311939 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     3782 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-23 11:59:43.000000 ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 11:59:43.333406 ScholarCodeCollective-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      721 2024-04-23 11:59:34.000000 ScholarCodeCollective-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:59:43.330211 ScholarCodeCollective-0.1.2/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.221316 ScholarCodeCollective-0.1.3/
+-rw-rw-rw-   0        0        0     3782 2024-04-23 12:07:27.220315 ScholarCodeCollective-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.185988 ScholarCodeCollective-0.1.3/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.206380 ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.209035 ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.213634 ScholarCodeCollective-0.1.3/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      156 2024-04-22 01:56:08.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.217180 ScholarCodeCollective-0.1.3/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.202595 ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     3782 2024-04-23 12:07:27.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2024-04-23 12:07:27.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:07:27.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-23 12:07:27.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-23 12:07:27.000000 ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 12:07:27.221316 ScholarCodeCollective-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-04-23 12:07:24.000000 ScholarCodeCollective-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:07:27.218294 ScholarCodeCollective-0.1.3/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.3/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.2/PKG-INFO` & `ScholarCodeCollective-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >3.9,<3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.2/README.md` & `ScholarCodeCollective-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.2/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.3/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.2/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.3/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.2/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.3/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >3.9,<3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.2/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.3/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.2/setup.py` & `ScholarCodeCollective-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 import pathlib
 import setuptools
 
 setuptools.setup(
     name='ScholarCodeCollective',
-    version='0.1.2',
+    version='0.1.3',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name', 
     author_email='author_email@mail.com',
     license='The Unlicense',
```

### Comparing `ScholarCodeCollective-0.1.2/tests/__init__.py` & `ScholarCodeCollective-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

