# Comparing `tmp/SBMLDiagrams-1.4.1.tar.gz` & `tmp/SBMLDiagrams-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SBMLDiagrams-1.4.1.tar", last modified: Wed Feb 14 22:09:33 2024, max compression
+gzip compressed data, was "dist\SBMLDiagrams-1.4.2.tar", last modified: Tue Apr 23 20:34:13 2024, max compression
```

## Comparing `SBMLDiagrams-1.4.1.tar` & `SBMLDiagrams-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 22:09:33.250880 SBMLDiagrams-1.4.1/
--rw-rw-rw-   0        0        0     3004 2024-02-14 22:09:33.250880 SBMLDiagrams-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2068 2024-02-13 23:16:21.000000 SBMLDiagrams-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-14 22:09:33.242905 SBMLDiagrams-1.4.1/SBMLDiagrams/
--rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/__init__.py
--rw-rw-rw-   0        0        0       71 2024-02-13 23:08:25.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/_version.py
--rw-rw-rw-   0        0        0   122174 2023-11-02 18:49:59.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/drawNetwork.py
--rw-rw-rw-   0        0        0   128825 2023-10-12 18:39:51.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/editSBML.py
--rw-rw-rw-   0        0        0   104713 2023-07-20 22:23:28.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/exportSBML.py
--rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/point.py
--rw-rw-rw-   0        0        0   362039 2023-10-19 19:33:13.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/processSBML.py
--rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/styleSBML.py
--rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/visualizeInfo.py
--rw-rw-rw-   0        0        0   158713 2023-10-19 19:28:11.000000 SBMLDiagrams-1.4.1/SBMLDiagrams/visualizeSBML.py
-drwxrwxrwx   0        0        0        0 2024-02-14 22:09:33.249856 SBMLDiagrams-1.4.1/SBMLDiagrams.egg-info/
--rw-rw-rw-   0        0        0     3004 2024-02-14 22:09:33.000000 SBMLDiagrams-1.4.1/SBMLDiagrams.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2024-02-14 22:09:33.000000 SBMLDiagrams-1.4.1/SBMLDiagrams.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 22:09:33.000000 SBMLDiagrams-1.4.1/SBMLDiagrams.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2024-02-14 22:09:33.000000 SBMLDiagrams-1.4.1/SBMLDiagrams.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-14 22:09:33.000000 SBMLDiagrams-1.4.1/SBMLDiagrams.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-02-14 22:09:33.251850 SBMLDiagrams-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2084 2023-09-13 18:28:58.000000 SBMLDiagrams-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:34:13.594239 SBMLDiagrams-1.4.2/
+-rw-rw-rw-   0        0        0     3011 2024-04-23 20:34:13.594239 SBMLDiagrams-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2068 2024-02-13 23:16:21.000000 SBMLDiagrams-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 20:34:13.585232 SBMLDiagrams-1.4.2/SBMLDiagrams/
+-rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/__init__.py
+-rw-rw-rw-   0        0        0       71 2024-04-23 20:22:42.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/_version.py
+-rw-rw-rw-   0        0        0   122174 2023-11-02 18:49:59.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/drawNetwork.py
+-rw-rw-rw-   0        0        0   128825 2023-10-12 18:39:51.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/editSBML.py
+-rw-rw-rw-   0        0        0   104713 2023-07-20 22:23:28.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/exportSBML.py
+-rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/point.py
+-rw-rw-rw-   0        0        0   362039 2023-10-19 19:33:13.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/processSBML.py
+-rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/styleSBML.py
+-rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/visualizeInfo.py
+-rw-rw-rw-   0        0        0   158713 2023-10-19 19:28:11.000000 SBMLDiagrams-1.4.2/SBMLDiagrams/visualizeSBML.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:34:13.593238 SBMLDiagrams-1.4.2/SBMLDiagrams.egg-info/
+-rw-rw-rw-   0        0        0     3011 2024-04-23 20:34:13.000000 SBMLDiagrams-1.4.2/SBMLDiagrams.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2024-04-23 20:34:13.000000 SBMLDiagrams-1.4.2/SBMLDiagrams.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:34:13.000000 SBMLDiagrams-1.4.2/SBMLDiagrams.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2024-04-23 20:34:13.000000 SBMLDiagrams-1.4.2/SBMLDiagrams.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-23 20:34:13.000000 SBMLDiagrams-1.4.2/SBMLDiagrams.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-23 20:34:13.595205 SBMLDiagrams-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     2091 2024-04-23 20:10:32.000000 SBMLDiagrams-1.4.2/setup.py
```

### Comparing `SBMLDiagrams-1.4.1/PKG-INFO` & `SBMLDiagrams-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.4.1
+Version: 1.4.2
 Summary: Visualize, edit and write SBML files.
 Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
-Author-email: jxu2019@uw.edu
+Author-email: jin.xu.phys@gmail.com
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
         
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/SBMLDiagrams.svg)](https://badge.fury.io/py/SBMLDiagrams) [![PyPI download month](https://img.shields.io/pypi/dm/ansicolortags.svg)](https://pypi.python.org/pypi/SBMLDiagrams/) ![Funding](https://img.shields.io/badge/Funding-NIH%20(EB028887)-blue)
         
         ## Introduction
```

### Comparing `SBMLDiagrams-1.4.1/README.md` & `SBMLDiagrams-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/__init__.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/drawNetwork.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/drawNetwork.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/editSBML.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/editSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/exportSBML.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/exportSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/point.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/point.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/processSBML.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/processSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/styleSBML.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/styleSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/visualizeInfo.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/visualizeInfo.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams/visualizeSBML.py` & `SBMLDiagrams-1.4.2/SBMLDiagrams/visualizeSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.4.1/SBMLDiagrams.egg-info/PKG-INFO` & `SBMLDiagrams-1.4.2/SBMLDiagrams.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.4.1
+Version: 1.4.2
 Summary: Visualize, edit and write SBML files.
 Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
-Author-email: jxu2019@uw.edu
+Author-email: jin.xu.phys@gmail.com
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
         
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/SBMLDiagrams.svg)](https://badge.fury.io/py/SBMLDiagrams) [![PyPI download month](https://img.shields.io/pypi/dm/ansicolortags.svg)](https://pypi.python.org/pypi/SBMLDiagrams/) ![Funding](https://img.shields.io/badge/Funding-NIH%20(EB028887)-blue)
         
         ## Introduction
```

### Comparing `SBMLDiagrams-1.4.1/setup.py` & `SBMLDiagrams-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name='SBMLDiagrams',
     packages=['SBMLDiagrams'],
     version=get_version('SBMLDiagrams/_version.py'),
     description='Visualize, edit and write SBML files.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jin Xu, Jessie Jiang, Herbert M. Sauro',
-    author_email='jxu2019@uw.edu',
+    author_email='jin.xu.phys@gmail.com',
     url='https://github.com/sys-bio/SBMLDiagrams',
     license='MIT License',
     install_requires=[
         'coverage',
         'pip>20',
         'numpy',
         'pandas',
```

