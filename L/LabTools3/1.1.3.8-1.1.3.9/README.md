# Comparing `tmp/LabTools3-1.1.3.8.tar.gz` & `tmp/LabTools3-1.1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LabTools3-1.1.3.8.tar", last modified: Mon Aug 15 21:48:16 2022, max compression
+gzip compressed data, was "LabTools3-1.1.3.9.tar", last modified: Tue Aug 16 11:20:53 2022, max compression
```

## Comparing `LabTools3-1.1.3.8.tar` & `LabTools3-1.1.3.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-15 21:48:16.229023 LabTools3-1.1.3.8/
--rw-r--r--   0 boeglinw   (502) staff       (20)     1108 2020-07-21 14:25:10.000000 LabTools3-1.1.3.8/LICENSE
-drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-15 21:48:16.198304 LabTools3-1.1.3.8/LT/
--rw-r--r--   0 boeglinw   (502) staff       (20)     3680 2018-11-19 21:35:16.000000 LabTools3-1.1.3.8/LT/MCA.py
--rw-r--r--   0 boeglinw   (502) staff       (20)      171 2018-11-19 21:33:50.000000 LabTools3-1.1.3.8/LT/__init__.py
--rw-r--r--   0 boeglinw   (502) staff       (20)    75960 2022-08-12 12:00:53.000000 LabTools3-1.1.3.8/LT/box.py
--rw-r--r--   0 boeglinw   (502) staff       (20)    30254 2022-08-08 20:57:21.000000 LabTools3-1.1.3.8/LT/datafile.py
--rw-r--r--   0 boeglinw   (502) staff       (20)      308 2018-11-19 21:33:50.000000 LabTools3-1.1.3.8/LT/get_precision.py
--rw-r--r--   0 boeglinw   (502) staff       (20)     8690 2021-03-30 11:24:34.000000 LabTools3-1.1.3.8/LT/parameterfile.py
--rw-r--r--   0 boeglinw   (502) staff       (20)     3887 2022-08-08 21:00:31.000000 LabTools3-1.1.3.8/LT/pdatafile.py
--rw-r--r--   0 boeglinw   (502) staff       (20)    21128 2022-01-19 19:27:32.000000 LabTools3-1.1.3.8/LT/plotting.py
-drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-15 21:48:16.225922 LabTools3-1.1.3.8/LT_Fit/
--rw-r--r--   0 boeglinw   (502) staff       (20)      324 2018-11-19 21:33:50.000000 LabTools3-1.1.3.8/LT_Fit/__init__.py
--rw-r--r--   0 boeglinw   (502) staff       (20)    10307 2022-01-17 23:34:16.000000 LabTools3-1.1.3.8/LT_Fit/gen_fit.py
--rw-r--r--   0 boeglinw   (502) staff       (20)    16816 2022-01-17 22:03:54.000000 LabTools3-1.1.3.8/LT_Fit/linear_fit.py
--rw-r--r--   0 boeglinw   (502) staff       (20)     1991 2019-01-03 21:55:04.000000 LabTools3-1.1.3.8/LT_Fit/parameters.py
-drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-15 21:48:16.228418 LabTools3-1.1.3.8/LabTools3.egg-info/
--rw-r--r--   0 boeglinw   (502) staff       (20)     2116 2022-08-15 21:48:16.000000 LabTools3-1.1.3.8/LabTools3.egg-info/PKG-INFO
--rw-r--r--   0 boeglinw   (502) staff       (20)      358 2022-08-15 21:48:16.000000 LabTools3-1.1.3.8/LabTools3.egg-info/SOURCES.txt
--rw-r--r--   0 boeglinw   (502) staff       (20)        1 2022-08-15 21:48:16.000000 LabTools3-1.1.3.8/LabTools3.egg-info/dependency_links.txt
--rw-r--r--   0 boeglinw   (502) staff       (20)       10 2022-08-15 21:48:16.000000 LabTools3-1.1.3.8/LabTools3.egg-info/top_level.txt
--rw-r--r--   0 boeglinw   (502) staff       (20)     2116 2022-08-15 21:48:16.228773 LabTools3-1.1.3.8/PKG-INFO
--rw-r--r--   0 boeglinw   (502) staff       (20)     1704 2022-08-08 21:03:08.000000 LabTools3-1.1.3.8/README.md
--rw-r--r--   0 boeglinw   (502) staff       (20)       38 2022-08-15 21:48:16.229115 LabTools3-1.1.3.8/setup.cfg
--rw-r--r--   0 boeglinw   (502) staff       (20)      834 2022-08-08 21:03:19.000000 LabTools3-1.1.3.8/setup.py
+drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-16 11:20:53.631767 LabTools3-1.1.3.9/
+-rw-r--r--   0 boeglinw   (502) staff       (20)     1108 2020-07-21 14:25:10.000000 LabTools3-1.1.3.9/LICENSE
+drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-16 11:20:53.604962 LabTools3-1.1.3.9/LT/
+-rw-r--r--   0 boeglinw   (502) staff       (20)     3680 2018-11-19 21:35:16.000000 LabTools3-1.1.3.9/LT/MCA.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)      171 2018-11-19 21:33:50.000000 LabTools3-1.1.3.9/LT/__init__.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)    75960 2022-08-12 12:00:53.000000 LabTools3-1.1.3.9/LT/box.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)    30287 2022-08-16 11:07:54.000000 LabTools3-1.1.3.9/LT/datafile.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)      308 2018-11-19 21:33:50.000000 LabTools3-1.1.3.9/LT/get_precision.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)     8690 2021-03-30 11:24:34.000000 LabTools3-1.1.3.9/LT/parameterfile.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)     3887 2022-08-08 21:00:31.000000 LabTools3-1.1.3.9/LT/pdatafile.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)    21128 2022-01-19 19:27:32.000000 LabTools3-1.1.3.9/LT/plotting.py
+drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-16 11:20:53.627943 LabTools3-1.1.3.9/LT_Fit/
+-rw-r--r--   0 boeglinw   (502) staff       (20)      324 2018-11-19 21:33:50.000000 LabTools3-1.1.3.9/LT_Fit/__init__.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)    10307 2022-01-17 23:34:16.000000 LabTools3-1.1.3.9/LT_Fit/gen_fit.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)    16816 2022-01-17 22:03:54.000000 LabTools3-1.1.3.9/LT_Fit/linear_fit.py
+-rw-r--r--   0 boeglinw   (502) staff       (20)     1991 2019-01-03 21:55:04.000000 LabTools3-1.1.3.9/LT_Fit/parameters.py
+drwxr-xr-x   0 boeglinw   (502) staff       (20)        0 2022-08-16 11:20:53.630904 LabTools3-1.1.3.9/LabTools3.egg-info/
+-rw-r--r--   0 boeglinw   (502) staff       (20)     2268 2022-08-16 11:20:53.000000 LabTools3-1.1.3.9/LabTools3.egg-info/PKG-INFO
+-rw-r--r--   0 boeglinw   (502) staff       (20)      358 2022-08-16 11:20:53.000000 LabTools3-1.1.3.9/LabTools3.egg-info/SOURCES.txt
+-rw-r--r--   0 boeglinw   (502) staff       (20)        1 2022-08-16 11:20:53.000000 LabTools3-1.1.3.9/LabTools3.egg-info/dependency_links.txt
+-rw-r--r--   0 boeglinw   (502) staff       (20)       10 2022-08-16 11:20:53.000000 LabTools3-1.1.3.9/LabTools3.egg-info/top_level.txt
+-rw-r--r--   0 boeglinw   (502) staff       (20)     2268 2022-08-16 11:20:53.631441 LabTools3-1.1.3.9/PKG-INFO
+-rw-r--r--   0 boeglinw   (502) staff       (20)     1856 2022-08-16 11:19:43.000000 LabTools3-1.1.3.9/README.md
+-rw-r--r--   0 boeglinw   (502) staff       (20)       38 2022-08-16 11:20:53.631943 LabTools3-1.1.3.9/setup.cfg
+-rw-r--r--   0 boeglinw   (502) staff       (20)      834 2022-08-16 11:15:23.000000 LabTools3-1.1.3.9/setup.py
```

### Comparing `LabTools3-1.1.3.8/LICENSE` & `LabTools3-1.1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT/MCA.py` & `LabTools3-1.1.3.9/LT/MCA.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT/box.py` & `LabTools3-1.1.3.9/LT/box.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT/datafile.py` & `LabTools3-1.1.3.9/LT/datafile.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,16 +130,16 @@
                                  some limits for string entries. Best used for large purely
                                  numerical data.
                                  
         use_numpy = True (if numpy is installed) : set automatically but can be overridden
                                                    some attributes of datafile are not availables when
                                                    numpy is not present
                                                    
-        adata = None (default) : use the data provided in a list of string as data file content. This is to provdie
-                                 information directly in datafile format
+        adata = my_lines (default = None) : use the data provided in a list of strings (my_lines) as data file content. 
+                                            The content of my_lines must follow the datafile syntax.
         
     """
     def __init__(self, filename, debug = False, new=False, skip = True, use_numpy = numpy_ok, fast = False, adata = None):
         self.H=re.compile("^#\!") # pattern for header
         self.C=re.compile("^#")   # pattern for comment
         # pattern for splitting header
         # currently:
```

### Comparing `LabTools3-1.1.3.8/LT/parameterfile.py` & `LabTools3-1.1.3.9/LT/parameterfile.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT/pdatafile.py` & `LabTools3-1.1.3.9/LT/pdatafile.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT/plotting.py` & `LabTools3-1.1.3.9/LT/plotting.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT_Fit/gen_fit.py` & `LabTools3-1.1.3.9/LT_Fit/gen_fit.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT_Fit/linear_fit.py` & `LabTools3-1.1.3.9/LT_Fit/linear_fit.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LT_Fit/parameters.py` & `LabTools3-1.1.3.9/LT_Fit/parameters.py`

 * *Files identical despite different names*

### Comparing `LabTools3-1.1.3.8/LabTools3.egg-info/PKG-INFO` & `LabTools3-1.1.3.9/LabTools3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LabTools3
-Version: 1.1.3.8
+Version: 1.1.3.9
 Summary: Python 3 Package of modules for typical analysis tasks analyzing physics data
 Home-page: http://wanda.fiu.edu/LabTools3
 Author: Werner Boeglin
 Author-email: boeglinw@fiu.edu
 License: MIT
 Keywords: Data Analysis
 Classifier: Programming Language :: Python :: 3.6
@@ -27,14 +27,16 @@
 
 Version 1.1.3.2: minor bug fixes
 
 Version 1.1.3.3: histogram axis labels are preserved in rebinning and projection actions (for 2d histogram)
 
 Version 1.1.3.4: minor bug fixes
 
-Version 1.1.3.5: corrected problen with add_data
+Version 1.1.3.5: corrected problen with *add_data*
 
 Version 1.1.3.6: added features to fitting: *plot* attribute to plot the fit, the fit results is plotted by default (controlled with the *plot_fit* kwarg). The fit object are callable, returning the value of the fit function using the current values of the fit parameters. New attribute to datafile: *adata\_comment\_index*, a list of indices pointing to comment lines.
  
 Version 1.1.3.7: updated documentation
 
 Version 1.1.3.8: datafile can be initialized with a list of strings correponding to the regular syntax
+
+Version 1.1.3.9: Fixed a bug in *histo* where histogram window variable was not initialized when loading from file (required a *clear_window* call).
```

### Comparing `LabTools3-1.1.3.8/PKG-INFO` & `LabTools3-1.1.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LabTools3
-Version: 1.1.3.8
+Version: 1.1.3.9
 Summary: Python 3 Package of modules for typical analysis tasks analyzing physics data
 Home-page: http://wanda.fiu.edu/LabTools3
 Author: Werner Boeglin
 Author-email: boeglinw@fiu.edu
 License: MIT
 Keywords: Data Analysis
 Classifier: Programming Language :: Python :: 3.6
@@ -27,14 +27,16 @@
 
 Version 1.1.3.2: minor bug fixes
 
 Version 1.1.3.3: histogram axis labels are preserved in rebinning and projection actions (for 2d histogram)
 
 Version 1.1.3.4: minor bug fixes
 
-Version 1.1.3.5: corrected problen with add_data
+Version 1.1.3.5: corrected problen with *add_data*
 
 Version 1.1.3.6: added features to fitting: *plot* attribute to plot the fit, the fit results is plotted by default (controlled with the *plot_fit* kwarg). The fit object are callable, returning the value of the fit function using the current values of the fit parameters. New attribute to datafile: *adata\_comment\_index*, a list of indices pointing to comment lines.
  
 Version 1.1.3.7: updated documentation
 
 Version 1.1.3.8: datafile can be initialized with a list of strings correponding to the regular syntax
+
+Version 1.1.3.9: Fixed a bug in *histo* where histogram window variable was not initialized when loading from file (required a *clear_window* call).
```

### Comparing `LabTools3-1.1.3.8/README.md` & `LabTools3-1.1.3.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 Version 1.1.3.2: minor bug fixes
 
 Version 1.1.3.3: histogram axis labels are preserved in rebinning and projection actions (for 2d histogram)
 
 Version 1.1.3.4: minor bug fixes
 
-Version 1.1.3.5: corrected problen with add_data
+Version 1.1.3.5: corrected problen with *add_data*
 
 Version 1.1.3.6: added features to fitting: *plot* attribute to plot the fit, the fit results is plotted by default (controlled with the *plot_fit* kwarg). The fit object are callable, returning the value of the fit function using the current values of the fit parameters. New attribute to datafile: *adata\_comment\_index*, a list of indices pointing to comment lines.
  
 Version 1.1.3.7: updated documentation
 
-Version 1.1.3.8: datafile can be initialized with a list of strings correponding to the regular syntax
+Version 1.1.3.8: datafile can be initialized with a list of strings correponding to the regular syntax
+
+Version 1.1.3.9: Fixed a bug in *histo* where histogram window variable was not initialized when loading from file (required a *clear_window* call).
```

### Comparing `LabTools3-1.1.3.8/setup.py` & `LabTools3-1.1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "LabTools3",
-    version = "1.1.3.8",
+    version = "1.1.3.9",
     packages = find_packages(),
     # add additional files
     package_data = {'':['*.bat','*.command']},
     # meta data about package
     # metadata for upload to PyPI
     author = "Werner Boeglin",
     author_email = "boeglinw@fiu.edu",
```

