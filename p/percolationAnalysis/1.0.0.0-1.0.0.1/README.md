# Comparing `tmp/percolationanalysis-1.0.0.0.tar.gz` & `tmp/percolationAnalysis-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percolationanalysis-1.0.0.0.tar", last modified: Mon Apr 22 12:20:42 2024, max compression
+gzip compressed data, was "percolationAnalysis-1.0.0.1.tar", last modified: Tue Apr 23 14:13:14 2024, max compression
```

## Comparing `percolationanalysis-1.0.0.0.tar` & `percolationAnalysis-1.0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-22 12:20:42.837722 percolationanalysis-1.0.0.0/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1078 2024-04-22 12:11:26.000000 percolationanalysis-1.0.0.0/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)      640 2024-04-22 12:20:42.837722 percolationanalysis-1.0.0.0/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      213 2024-04-22 12:12:25.000000 percolationanalysis-1.0.0.0/README.md
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-22 12:20:42.833722 percolationanalysis-1.0.0.0/percolationAnalysis/
--rwxrwxrwx   0 abhishek  (1000) abhishek  (1000)       57 2024-01-22 15:45:53.000000 percolationanalysis-1.0.0.0/percolationAnalysis/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2920 2024-04-22 10:01:35.000000 percolationanalysis-1.0.0.0/percolationAnalysis/percolationAnalysis.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)  4000000 2024-04-22 09:38:09.000000 percolationanalysis-1.0.0.0/percolationAnalysis/testData.bin
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-22 12:20:42.837722 percolationanalysis-1.0.0.0/percolationAnalysis.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)      640 2024-04-22 12:20:42.000000 percolationanalysis-1.0.0.0/percolationAnalysis.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2024-04-22 12:20:42.000000 percolationanalysis-1.0.0.0/percolationAnalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-04-22 12:20:42.000000 percolationanalysis-1.0.0.0/percolationAnalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       20 2024-04-22 12:20:42.000000 percolationanalysis-1.0.0.0/percolationAnalysis.egg-info/top_level.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       38 2024-04-22 12:20:42.837722 percolationanalysis-1.0.0.0/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      776 2024-04-22 12:20:35.000000 percolationanalysis-1.0.0.0/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-23 14:13:14.372089 percolationAnalysis-1.0.0.1/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1078 2024-04-22 12:11:26.000000 percolationAnalysis-1.0.0.1/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      660 2024-04-23 14:13:14.372089 percolationAnalysis-1.0.0.1/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      213 2024-04-22 12:12:25.000000 percolationAnalysis-1.0.0.1/README.md
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-23 14:13:14.356089 percolationAnalysis-1.0.0.1/percolationAnalysis/
+-rwxrwxrwx   0 abhishek  (1000) abhishek  (1000)        1 2024-04-23 14:12:26.000000 percolationAnalysis-1.0.0.1/percolationAnalysis/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2920 2024-04-22 10:01:35.000000 percolationAnalysis-1.0.0.1/percolationAnalysis/percolationAnalysis.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)  4000000 2024-04-22 09:38:09.000000 percolationAnalysis-1.0.0.1/percolationAnalysis/testData.bin
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-23 14:13:14.372089 percolationAnalysis-1.0.0.1/percolationAnalysis.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)      660 2024-04-23 14:13:14.000000 percolationAnalysis-1.0.0.1/percolationAnalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2024-04-23 14:13:14.000000 percolationAnalysis-1.0.0.1/percolationAnalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-04-23 14:13:14.000000 percolationAnalysis-1.0.0.1/percolationAnalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       20 2024-04-23 14:13:14.000000 percolationAnalysis-1.0.0.1/percolationAnalysis.egg-info/top_level.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       38 2024-04-23 14:13:14.372089 percolationAnalysis-1.0.0.1/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      776 2024-04-23 14:12:47.000000 percolationAnalysis-1.0.0.1/setup.py
```

### Comparing `percolationanalysis-1.0.0.0/LICENSE` & `percolationAnalysis-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `percolationanalysis-1.0.0.0/PKG-INFO` & `percolationAnalysis-1.0.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: percolationAnalysis
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: Identifying non-subjective thresholds for scalar indicators of coherent structures with percolation analysis
 Home-page: https://github.com/Phoenixfire1081/PercolationAnalysis
 Author: Abhishek Harikrishnan
 Author-email: abhishek.harikrishnan@fu-berlin.de
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Identifying non-subjective thresholds for scalar indicators of coherent structures with percolation analysis
 
 For a complete description of the code see https://github.com/Phoenixfire1081/PercolationAnalysis.
 
 
+
+
```

### Comparing `percolationanalysis-1.0.0.0/percolationAnalysis/percolationAnalysis.py` & `percolationAnalysis-1.0.0.1/percolationAnalysis/percolationAnalysis.py`

 * *Files identical despite different names*

### Comparing `percolationanalysis-1.0.0.0/percolationAnalysis/testData.bin` & `percolationAnalysis-1.0.0.1/percolationAnalysis/testData.bin`

 * *Files identical despite different names*

### Comparing `percolationanalysis-1.0.0.0/percolationAnalysis.egg-info/PKG-INFO` & `percolationAnalysis-1.0.0.1/percolationAnalysis.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: percolationAnalysis
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: Identifying non-subjective thresholds for scalar indicators of coherent structures with percolation analysis
 Home-page: https://github.com/Phoenixfire1081/PercolationAnalysis
 Author: Abhishek Harikrishnan
 Author-email: abhishek.harikrishnan@fu-berlin.de
 License: MIT
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Identifying non-subjective thresholds for scalar indicators of coherent structures with percolation analysis
 
 For a complete description of the code see https://github.com/Phoenixfire1081/PercolationAnalysis.
 
 
+
+
```

### Comparing `percolationanalysis-1.0.0.0/setup.py` & `percolationAnalysis-1.0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
   
 with open("README.md", "r") as fh: 
     description = fh.read() 
   
 setuptools.setup( 
     name="percolationAnalysis", 
-    version="1.0.0.0", 
+    version="1.0.0.1", 
     author="Abhishek Harikrishnan", 
     author_email="abhishek.harikrishnan@fu-berlin.de", 
     packages=["percolationAnalysis"], 
     package_dir={'percolationAnalysis': 'percolationAnalysis'},
     package_data={'percolationAnalysis': ['*.bin']},
     description="Identifying non-subjective thresholds for scalar indicators of coherent structures with percolation analysis", 
     long_description=description,
```

