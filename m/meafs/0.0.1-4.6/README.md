# Comparing `tmp/meafs-0.0.1.tar.gz` & `tmp/meafs-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meafs-0.0.1.tar", last modified: Thu Apr 18 18:10:45 2024, max compression
+gzip compressed data, was "meafs-4.6.tar", last modified: Tue Apr 23 18:43:14 2024, max compression
```

## Comparing `meafs-0.0.1.tar` & `meafs-4.6.tar`

### file list

```diff
@@ -1,13 +1,40 @@
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-18 18:10:45.336705 meafs-0.0.1/
--rwxr-xr-x   0 castro    (1000) users      (984)     1074 2024-04-18 18:10:17.000000 meafs-0.0.1/LICENSE.txt
--rw-r--r--   0 castro    (1000) users      (984)     9638 2024-04-18 18:10:45.336705 meafs-0.0.1/PKG-INFO
--rwxr-xr-x   0 castro    (1000) users      (984)     8984 2024-04-18 16:36:21.000000 meafs-0.0.1/README.md
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-18 18:10:45.336705 meafs-0.0.1/meafs.egg-info/
--rw-r--r--   0 castro    (1000) users      (984)     9638 2024-04-18 18:10:45.000000 meafs-0.0.1/meafs.egg-info/PKG-INFO
--rw-r--r--   0 castro    (1000) users      (984)      212 2024-04-18 18:10:45.000000 meafs-0.0.1/meafs.egg-info/SOURCES.txt
--rw-r--r--   0 castro    (1000) users      (984)        1 2024-04-18 18:10:45.000000 meafs-0.0.1/meafs.egg-info/dependency_links.txt
--rw-r--r--   0 castro    (1000) users      (984)      156 2024-04-18 18:10:45.000000 meafs-0.0.1/meafs.egg-info/entry_points.txt
--rw-r--r--   0 castro    (1000) users      (984)       80 2024-04-18 18:10:45.000000 meafs-0.0.1/meafs.egg-info/requires.txt
--rw-r--r--   0 castro    (1000) users      (984)        1 2024-04-18 18:10:45.000000 meafs-0.0.1/meafs.egg-info/top_level.txt
--rwxr-xr-x   0 castro    (1000) users      (984)      761 2024-04-18 18:09:42.000000 meafs-0.0.1/pyproject.toml
--rw-r--r--   0 castro    (1000) users      (984)       38 2024-04-18 18:10:45.336705 meafs-0.0.1/setup.cfg
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:43:14.998347 meafs-4.6/
+-rwxr-xr-x   0 castro    (1000) users      (984)     1074 2024-04-23 18:38:27.000000 meafs-4.6/LICENSE.txt
+-rwxr-xr-x   0 castro    (1000) users      (984)       32 2024-04-23 18:38:27.000000 meafs-4.6/MANIFEST.in
+-rw-r--r--   0 castro    (1000) users      (984)     9641 2024-04-23 18:43:14.998347 meafs-4.6/PKG-INFO
+-rwxr-xr-x   0 castro    (1000) users      (984)     8984 2024-04-23 18:38:27.000000 meafs-4.6/README.md
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:43:14.998347 meafs-4.6/meafs.egg-info/
+-rw-r--r--   0 castro    (1000) users      (984)     9641 2024-04-23 18:43:14.000000 meafs-4.6/meafs.egg-info/PKG-INFO
+-rw-r--r--   0 castro    (1000) users      (984)      914 2024-04-23 18:43:14.000000 meafs-4.6/meafs.egg-info/SOURCES.txt
+-rw-r--r--   0 castro    (1000) users      (984)        1 2024-04-23 18:43:14.000000 meafs-4.6/meafs.egg-info/dependency_links.txt
+-rw-r--r--   0 castro    (1000) users      (984)      156 2024-04-23 18:43:14.000000 meafs-4.6/meafs.egg-info/entry_points.txt
+-rw-r--r--   0 castro    (1000) users      (984)       85 2024-04-23 18:43:14.000000 meafs-4.6/meafs.egg-info/requires.txt
+-rw-r--r--   0 castro    (1000) users      (984)       11 2024-04-23 18:43:14.000000 meafs-4.6/meafs.egg-info/top_level.txt
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:43:14.995014 meafs-4.6/meafs_code/
+-rwxr-xr-x   0 castro    (1000) users      (984)       26 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/__init__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)       37 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/__main__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)       78 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/convert.sh
+-rwxr-xr-x   0 castro    (1000) users      (984)     4259 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/desktop_entry.py
+-rw-r--r--   0 castro    (1000) users      (984)    11095 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/fitsettings.ui
+-rw-r--r--   0 castro    (1000) users      (984)    14517 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/fitsettings_qt.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    46615 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/gui.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    42133 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/gui_qt.py
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:43:14.995014 meafs-4.6/meafs_code/images/
+-rw-r--r--   0 castro    (1000) users      (984)   190114 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/images/Meafs_Gui.png
+-rwxr-xr-x   0 castro    (1000) users      (984)    42476 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/images/Meafs_Icon.ico
+-rwxr-xr-x   0 castro    (1000) users      (984)   220589 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/images/Meafs_Logo.png
+-rwxr-xr-x   0 castro    (1000) users      (984)    36066 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/meafs.ui
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:43:14.998347 meafs-4.6/meafs_code/scripts/
+-rwxr-xr-x   0 castro    (1000) users      (984)      142 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/__init__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    12110 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/abundance_analysis.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    28910 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/abundance_fit.py
+-rwxr-xr-x   0 castro    (1000) users      (984)     1936 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/bisec_interpol.c
+-rwxr-xr-x   0 castro    (1000) users      (984)    15472 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/bisec_interpol.so
+-rwxr-xr-x   0 castro    (1000) users      (984)      148 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/comp.sh
+-rw-r--r--   0 castro    (1000) users      (984)     5078 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/fit_functions.py
+-rw-r--r--   0 castro    (1000) users      (984)     4975 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/turbospec_functions.py
+-rwxr-xr-x   0 castro    (1000) users      (984)     3343 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/unify_plots.py
+-rw-r--r--   0 castro    (1000) users      (984)     2868 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/scripts/voigt_functions.py
+-rw-r--r--   0 castro    (1000) users      (984)       27 2024-04-23 18:38:27.000000 meafs-4.6/meafs_code/settings.csv
+-rwxr-xr-x   0 castro    (1000) users      (984)      764 2024-04-23 18:40:27.000000 meafs-4.6/pyproject.toml
+-rw-r--r--   0 castro    (1000) users      (984)       38 2024-04-23 18:43:14.998347 meafs-4.6/setup.cfg
```

### Comparing `meafs-0.0.1/LICENSE.txt` & `meafs-4.6/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Matheus J. Castro
+Copyright (c) 2022 Matheus J. Castro
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `meafs-0.0.1/PKG-INFO` & `meafs-4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meafs
-Version: 0.0.1
+Version: 4.6
 Summary: Multiple Element Abundance Fit Software
 Author: Matheus J. Castro
 Project-URL: Homepage, https://github.com/MatheusJCastro/meafs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,15 +12,15 @@
 License-File: LICENSE.txt
 Requires-Dist: astropy
 Requires-Dist: specutils
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: desktop_file
+Requires-Dist: desktop_file==1.3
 Requires-Dist: pathlib
 Requires-Dist: PyQt6
 Requires-Dist: dill
 
 ![Meafs Logo](meafs_code/images/Meafs_Logo.png)
 
 # Multiple Element Abundance Fit Software - MEAFS
```

### Comparing `meafs-0.0.1/README.md` & `meafs-4.6/README.md`

 * *Files identical despite different names*

### Comparing `meafs-0.0.1/meafs.egg-info/PKG-INFO` & `meafs-4.6/meafs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meafs
-Version: 0.0.1
+Version: 4.6
 Summary: Multiple Element Abundance Fit Software
 Author: Matheus J. Castro
 Project-URL: Homepage, https://github.com/MatheusJCastro/meafs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,15 +12,15 @@
 License-File: LICENSE.txt
 Requires-Dist: astropy
 Requires-Dist: specutils
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: desktop_file
+Requires-Dist: desktop_file==1.3
 Requires-Dist: pathlib
 Requires-Dist: PyQt6
 Requires-Dist: dill
 
 ![Meafs Logo](meafs_code/images/Meafs_Logo.png)
 
 # Multiple Element Abundance Fit Software - MEAFS
```

### Comparing `meafs-0.0.1/pyproject.toml` & `meafs-4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "meafs"
-version = "0.0.1"
+version = "4.6"
 authors = [
     { name="Matheus J. Castro" }
 ]
 description="Multiple Element Abundance Fit Software"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers=[
@@ -16,15 +16,15 @@
 dependencies = [
     "astropy",
     "specutils",
     "scipy",
     "matplotlib",
     "pandas",
     "numpy",
-    "desktop_file",
+    "desktop_file==1.3",
     "pathlib",
     "PyQt6",
     "dill"
 ]
 
 [project.scripts]
 meafs = "meafs_code.gui:main"
```

