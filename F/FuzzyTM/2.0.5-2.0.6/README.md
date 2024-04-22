# Comparing `tmp/FuzzyTM-2.0.5.tar.gz` & `tmp/FuzzyTM-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FuzzyTM-2.0.5.tar", last modified: Tue Nov  1 10:23:34 2022, max compression
+gzip compressed data, was "dist\FuzzyTM-2.0.6.tar", last modified: Mon Apr 22 22:32:27 2024, max compression
```

## Comparing `FuzzyTM-2.0.5.tar` & `FuzzyTM-2.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-11-01 10:23:34.649293 FuzzyTM-2.0.5/
-drwxrwxrwx   0        0        0        0 2022-11-01 10:23:34.625361 FuzzyTM-2.0.5/FuzzyTM/
--rw-rw-rw-   0        0        0    63128 2022-11-01 10:17:47.000000 FuzzyTM-2.0.5/FuzzyTM/FuzzyTM.py
--rw-rw-rw-   0        0        0      155 2022-10-19 17:02:01.000000 FuzzyTM-2.0.5/FuzzyTM/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-01 10:23:34.646301 FuzzyTM-2.0.5/FuzzyTM.egg-info/
--rw-rw-rw-   0        0        0     7860 2022-11-01 10:23:34.000000 FuzzyTM-2.0.5/FuzzyTM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2022-11-01 10:23:34.000000 FuzzyTM-2.0.5/FuzzyTM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-01 10:23:34.000000 FuzzyTM-2.0.5/FuzzyTM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-11-01 10:23:34.000000 FuzzyTM-2.0.5/FuzzyTM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-01 10:23:34.000000 FuzzyTM-2.0.5/FuzzyTM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2021-11-01 14:27:46.000000 FuzzyTM-2.0.5/LICENSE
--rw-rw-rw-   0        0        0     7860 2022-11-01 10:23:34.648329 FuzzyTM-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7542 2022-10-19 17:04:15.000000 FuzzyTM-2.0.5/README.md
--rw-rw-rw-   0        0        0       42 2022-11-01 10:23:34.649293 FuzzyTM-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      924 2022-11-01 10:19:46.000000 FuzzyTM-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:32:27.912982 FuzzyTM-2.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-22 22:32:27.881072 FuzzyTM-2.0.6/FuzzyTM/
+-rw-rw-rw-   0        0        0    63028 2022-11-23 10:50:28.000000 FuzzyTM-2.0.6/FuzzyTM/FuzzyTM.py
+-rw-rw-rw-   0        0        0      155 2022-10-19 17:02:01.000000 FuzzyTM-2.0.6/FuzzyTM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:32:27.910988 FuzzyTM-2.0.6/FuzzyTM.egg-info/
+-rw-rw-rw-   0        0        0     7835 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2021-11-01 14:27:46.000000 FuzzyTM-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0     7835 2024-04-22 22:32:27.912017 FuzzyTM-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7517 2024-04-22 21:30:36.000000 FuzzyTM-2.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 22:32:27.913979 FuzzyTM-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      924 2024-04-22 22:27:03.000000 FuzzyTM-2.0.6/setup.py
```

### Comparing `FuzzyTM-2.0.5/FuzzyTM/FuzzyTM.py` & `FuzzyTM-2.0.6/FuzzyTM/FuzzyTM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1211,18 +1211,14 @@
 
         Parameters
         ----------
              filepath : str
                 The directory in which the file should be stored,
                 either with or without
 
-        Returns
-        -------
-             float
-                 The interpretability score.
         """
         if not isinstance(filepath, str):
             raise ValueError('Make sure that "filepath" has type "str"')
         if filepath.endswith('.pickle'):
             pickle_out = open(filepath, 'wb')
         elif filepath.endswith('/'):
             pickle_out = open(filepath+'model.pickle', 'wb')
```

### Comparing `FuzzyTM-2.0.5/FuzzyTM.egg-info/PKG-INFO` & `FuzzyTM-2.0.6/FuzzyTM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuzzyTM
-Version: 2.0.5
+Version: 2.0.6
 Summary: A Python package for Fuzzy Topic Models
 Home-page: https://github.com/ERijck/FuzzyTM
 Author: Emil Rijcken
 Author-email: emil.rijcken@gmail.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -129,10 +129,9 @@
  5. Please check the [Vosviewer manual](https://www.vosviewer.com/documentation/Manual_VOSviewer_1.6.8.pdf) for more information. 
  
  ## Class Methods
  
  ## Dependencies
 numpy == 1.19.2 <br>
 pandas == 1.3.3 <br>
-sparsesvd == 0.2.2 <br>
 scipy == 1.5.2 <br>
 pyfume == 0.2.0 <br>
```

### Comparing `FuzzyTM-2.0.5/LICENSE` & `FuzzyTM-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FuzzyTM-2.0.5/PKG-INFO` & `FuzzyTM-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuzzyTM
-Version: 2.0.5
+Version: 2.0.6
 Summary: A Python package for Fuzzy Topic Models
 Home-page: https://github.com/ERijck/FuzzyTM
 Author: Emil Rijcken
 Author-email: emil.rijcken@gmail.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -129,10 +129,9 @@
  5. Please check the [Vosviewer manual](https://www.vosviewer.com/documentation/Manual_VOSviewer_1.6.8.pdf) for more information. 
  
  ## Class Methods
  
  ## Dependencies
 numpy == 1.19.2 <br>
 pandas == 1.3.3 <br>
-sparsesvd == 0.2.2 <br>
 scipy == 1.5.2 <br>
 pyfume == 0.2.0 <br>
```

### Comparing `FuzzyTM-2.0.5/README.md` & `FuzzyTM-2.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,10 +118,9 @@
  5. Please check the [Vosviewer manual](https://www.vosviewer.com/documentation/Manual_VOSviewer_1.6.8.pdf) for more information. 
  
  ## Class Methods
  
  ## Dependencies
 numpy == 1.19.2 <br>
 pandas == 1.3.3 <br>
-sparsesvd == 0.2.2 <br>
 scipy == 1.5.2 <br>
 pyfume == 0.2.0 <br>
```

### Comparing `FuzzyTM-2.0.5/setup.py` & `FuzzyTM-2.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.5'
+VERSION = '2.0.6'
 PACKAGE_NAME = 'FuzzyTM'
 AUTHOR = 'Emil Rijcken'
 AUTHOR_EMAIL = 'emil.rijcken@gmail.com'
 URL = 'https://github.com/ERijck/FuzzyTM'
 
 LICENSE = 'GNU General Public License v3.0'
 DESCRIPTION = 'A Python package for Fuzzy Topic Models'
```

