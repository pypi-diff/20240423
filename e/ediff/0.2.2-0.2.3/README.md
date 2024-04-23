# Comparing `tmp/ediff-0.2.2.tar.gz` & `tmp/ediff-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediff-0.2.2.tar", last modified: Wed Apr 17 21:15:14 2024, max compression
+gzip compressed data, was "ediff-0.2.3.tar", last modified: Tue Apr 23 12:24:56 2024, max compression
```

## Comparing `ediff-0.2.2.tar` & `ediff-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.676257 ediff-0.2.2/
--rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:54.000000 ediff-0.2.2/LICENCE
--rw-rw-rw-   0        0        0     2742 2024-04-17 21:15:14.676257 ediff-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2204 2024-04-17 21:08:45.000000 ediff-0.2.2/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 21:15:14.676257 ediff-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1258 2021-12-09 19:48:00.000000 ediff-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.644303 ediff-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.667742 ediff-0.2.2/src/ediff/
--rw-rw-rw-   0        0        0     1623 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/background.py
--rw-rw-rw-   0        0        0    82026 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/center.py
--rw-rw-rw-   0        0        0     6813 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/io.py
--rw-rw-rw-   0        0        0    29312 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/pxrd.py
--rw-rw-rw-   0        0        0     4659 2024-04-17 21:08:45.000000 ediff-0.2.2/src/ediff/radial.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:15:14.676257 ediff-0.2.2/src/ediff.egg-info/
--rw-rw-rw-   0        0        0     2742 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 21:15:14.000000 ediff-0.2.2/src/ediff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 12:24:56.859091 ediff-0.2.3/
+-rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:54.000000 ediff-0.2.3/LICENCE
+-rw-rw-rw-   0        0        0     3049 2024-04-23 12:24:56.859091 ediff-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2024-04-23 12:18:40.000000 ediff-0.2.3/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 ediff-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 12:24:56.859091 ediff-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2021-12-09 19:48:00.000000 ediff-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:24:56.834233 ediff-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:24:56.856081 ediff-0.2.3/src/ediff/
+-rw-rw-rw-   0        0        0     1623 2024-04-23 12:05:12.000000 ediff-0.2.3/src/ediff/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-04-17 21:08:45.000000 ediff-0.2.3/src/ediff/background.py
+-rw-rw-rw-   0        0        0    82026 2024-04-17 21:08:45.000000 ediff-0.2.3/src/ediff/center.py
+-rw-rw-rw-   0        0        0     6813 2024-04-17 21:08:45.000000 ediff-0.2.3/src/ediff/io.py
+-rw-rw-rw-   0        0        0    29312 2024-04-17 21:08:45.000000 ediff-0.2.3/src/ediff/pxrd.py
+-rw-rw-rw-   0        0        0     4659 2024-04-17 21:08:45.000000 ediff-0.2.3/src/ediff/radial.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:24:56.859091 ediff-0.2.3/src/ediff.egg-info/
+-rw-rw-rw-   0        0        0     3049 2024-04-23 12:24:56.000000 ediff-0.2.3/src/ediff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-23 12:24:56.000000 ediff-0.2.3/src/ediff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:24:56.000000 ediff-0.2.3/src/ediff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-23 12:24:56.000000 ediff-0.2.3/src/ediff.egg-info/top_level.txt
```

### Comparing `ediff-0.2.2/LICENCE` & `ediff-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `ediff-0.2.2/PKG-INFO` & `ediff-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Processing of powder electron diffraction patterns
 Home-page: https://github.com/mirekslouf/ediff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/ediff/
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,18 @@
 -----------------------------------------------------------
 * EDIFF is under development, but key modules do work:
     - io = input/output data treatment
 	- background = background subtraction
 	- center = find center of 2D powder diffraction pattern
 	- radial = calculate radial distribution (2D-pattern &rArr; 1D-pattern) 
 	- pxrd = calculation of theoretical powder X-ray diffraction patterns
+* If you use EDIFF in your research, **please cite** the OpenAccess paper:
+	- Materials 14 (2011) 7550.
+	  [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
+	- The paper describes {stemdiff} package, {ediff} is a part of it.
 
 Installation
 ------------
 * Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
 * `pip install scikit-image` = 3rd party package for advanced image processing 
 * `pip install pymatgen` = 3rd party package employed in PXRD calculation
 * `pip install bground`= our package, interactive background subtraction
@@ -56,7 +60,9 @@
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
 * Version 0.1   = 1st semi-complete version with basic documentation
 * Version 0.1.1 = improved/simplified outputs
 * Version 0.1.2 = small improvements of code and documentation
 * Version 0.2   = important improvements of center.py
 * Version 0.2.2 = consolidation, update of docs and examples on www
+* Version 0.2.3 = small update of docs and citation
+
```

### Comparing `ediff-0.2.2/README.md` & `ediff-0.2.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 -----------------------------------------------------------
 * EDIFF is under development, but key modules do work:
     - io = input/output data treatment
 	- background = background subtraction
 	- center = find center of 2D powder diffraction pattern
 	- radial = calculate radial distribution (2D-pattern &rArr; 1D-pattern) 
 	- pxrd = calculation of theoretical powder X-ray diffraction patterns
+* If you use EDIFF in your research, **please cite** the OpenAccess paper:
+	- Materials 14 (2011) 7550.
+	  [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
+	- The paper describes {stemdiff} package, {ediff} is a part of it.
 
 Installation
 ------------
 * Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
 * `pip install scikit-image` = 3rd party package for advanced image processing 
 * `pip install pymatgen` = 3rd party package employed in PXRD calculation
 * `pip install bground`= our package, interactive background subtraction
@@ -40,7 +44,9 @@
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
 * Version 0.1   = 1st semi-complete version with basic documentation
 * Version 0.1.1 = improved/simplified outputs
 * Version 0.1.2 = small improvements of code and documentation
 * Version 0.2   = important improvements of center.py
 * Version 0.2.2 = consolidation, update of docs and examples on www
+* Version 0.2.3 = small update of docs and citation
+
```

### Comparing `ediff-0.2.2/setup.py` & `ediff-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `ediff-0.2.2/src/ediff/__init__.py` & `ediff-0.2.3/src/ediff/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Auxiliary package BGROUND:
 
 * the package enables simple, semi-automated, interactive background correction
 * it is imported during ediff initialization and accessible as ediff.background
 '''
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 # Import of modules so that we could use the package as follows:
 # >>> import ediff as ed
 # >>> ed.io.read_image ...
 import ediff.center
 import ediff.io
 import ediff.pxrd
```

### Comparing `ediff-0.2.2/src/ediff/background.py` & `ediff-0.2.3/src/ediff/background.py`

 * *Files identical despite different names*

### Comparing `ediff-0.2.2/src/ediff/center.py` & `ediff-0.2.3/src/ediff/center.py`

 * *Files identical despite different names*

### Comparing `ediff-0.2.2/src/ediff/io.py` & `ediff-0.2.3/src/ediff/io.py`

 * *Files identical despite different names*

### Comparing `ediff-0.2.2/src/ediff/pxrd.py` & `ediff-0.2.3/src/ediff/pxrd.py`

 * *Files identical despite different names*

### Comparing `ediff-0.2.2/src/ediff/radial.py` & `ediff-0.2.3/src/ediff/radial.py`

 * *Files identical despite different names*

### Comparing `ediff-0.2.2/src/ediff.egg-info/PKG-INFO` & `ediff-0.2.3/src/ediff.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Processing of powder electron diffraction patterns
 Home-page: https://github.com/mirekslouf/ediff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/ediff/
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,18 @@
 -----------------------------------------------------------
 * EDIFF is under development, but key modules do work:
     - io = input/output data treatment
 	- background = background subtraction
 	- center = find center of 2D powder diffraction pattern
 	- radial = calculate radial distribution (2D-pattern &rArr; 1D-pattern) 
 	- pxrd = calculation of theoretical powder X-ray diffraction patterns
+* If you use EDIFF in your research, **please cite** the OpenAccess paper:
+	- Materials 14 (2011) 7550.
+	  [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
+	- The paper describes {stemdiff} package, {ediff} is a part of it.
 
 Installation
 ------------
 * Requirement: Python with sci-modules: numpy, matplotlib, scipy, pandas
 * `pip install scikit-image` = 3rd party package for advanced image processing 
 * `pip install pymatgen` = 3rd party package employed in PXRD calculation
 * `pip install bground`= our package, interactive background subtraction
@@ -56,7 +60,9 @@
 * Version 0.0.3 = pxrd module works including profiles
 * Version 0.0.4 = bground module incorporated + slightly improved docstrings
 * Version 0.1   = 1st semi-complete version with basic documentation
 * Version 0.1.1 = improved/simplified outputs
 * Version 0.1.2 = small improvements of code and documentation
 * Version 0.2   = important improvements of center.py
 * Version 0.2.2 = consolidation, update of docs and examples on www
+* Version 0.2.3 = small update of docs and citation
+
```

