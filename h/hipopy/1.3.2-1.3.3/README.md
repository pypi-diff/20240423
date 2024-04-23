# Comparing `tmp/hipopy-1.3.2.tar.gz` & `tmp/hipopy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipopy-1.3.2.tar", max compression
+gzip compressed data, was "hipopy-1.3.3.tar", max compression
```

## Comparing `hipopy-1.3.2.tar` & `hipopy-1.3.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1098 2024-04-11 20:15:48.863986 hipopy-1.3.2/LICENSE
--rw-r--r--   0        0        0     1001 2024-04-18 20:43:32.190734 hipopy-1.3.2/README.md
--rw-r--r--   0        0        0      108 2024-04-19 18:06:30.197936 hipopy-1.3.2/hipopy/__init__.py
--rw-r--r--   0        0        0    34146 2024-04-19 18:01:31.986608 hipopy-1.3.2/hipopy/hipopy.py
--rw-r--r--   0        0        0    35778 2024-04-18 20:43:27.454609 hipopy-1.3.2/hipopy/hipopy__BACKUP.py
--rw-r--r--   0        0        0     5594 2024-04-18 21:19:07.532207 hipopy-1.3.2/hipopy/test1.py
--rw-r--r--   0        0        0     3317 2024-04-18 21:19:05.507302 hipopy-1.3.2/hipopy/test2.py
--rw-r--r--   0        0        0      513 2024-04-19 18:09:06.310662 hipopy-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 hipopy-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-11 20:15:48.863986 hipopy-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1001 2024-04-18 20:43:32.190734 hipopy-1.3.3/README.md
+-rw-r--r--   0        0        0      108 2024-04-23 19:37:49.543314 hipopy-1.3.3/hipopy/__init__.py
+-rw-r--r--   0        0        0    34250 2024-04-23 19:44:44.693757 hipopy-1.3.3/hipopy/hipopy.py
+-rw-r--r--   0        0        0    35778 2024-04-18 20:43:27.454609 hipopy-1.3.3/hipopy/hipopy__BACKUP.py
+-rw-r--r--   0        0        0     5594 2024-04-18 21:19:07.532207 hipopy-1.3.3/hipopy/test1.py
+-rw-r--r--   0        0        0     3317 2024-04-18 21:19:05.507302 hipopy-1.3.3/hipopy/test2.py
+-rw-r--r--   0        0        0      515 2024-04-23 19:43:13.065222 hipopy-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 hipopy-1.3.3/PKG-INFO
```

### Comparing `hipopy-1.3.2/LICENSE` & `hipopy-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopy-1.3.2/README.md` & `hipopy-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hipopy-1.3.2/hipopy/hipopy.py` & `hipopy-1.3.3/hipopy/hipopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     -----------
     Open a HIPO file to read.
     """
     f = hipofile(filename,mode=mode,tags=tags)
     f.open()
     return f
 
-def iterate(files,banks=None,step=100,tags=None,experimental=False):
+def iterate(files,banks=None,step=100,tags=None,experimental=True):
     """
     Parameters
     ----------
     files : list, required
         List of file names
     banks : list, optional
         List of bank names to read
@@ -50,15 +50,15 @@
         Default : 100
     tags : int or list of ints, optional
         Set bank tags for reader to use.  0 works for most banks.
         1 is needed for scaler banks.
         Default : None
     experimental : bool, optional
         Whether to use experimental hipopybind.HipoFileIterator to iterate files
-        Default : False
+        Default : True
 
     Description
     -----------
     Iterate through a list of hipofiles reading all banks unless specific banks are specified.
     Iteration is broken into batches of step events.
     """
     if tags is None and experimental: tags = []
@@ -856,21 +856,23 @@
     mode : string
         Currently fixed to always be in read mode ("r")
     verbose : boolean
         Currently fixed to always be False
     tags : int or list of ints
         Set bank tags for reader to use.  0 works for most banks.
         1 is needed for scaler banks.
+    experimental : bool
+        Do bank and event looping in C++ for added speed (see hipopybind package).
 
     Description
     -----------
     Chains files together so they may be read continuously.
     """
 
-    def __init__(self,names,banks=None,step=100,mode="r",tags=None,experimental=False):
+    def __init__(self,names,banks=None,step=100,mode="r",tags=None,experimental=True):
         self.names   = names
 
         # Parse regex NOTE: Must be full or relative path from $PWD.  ~/... does not work.
         if type(self.names)==str:
             self.names = glob.glob(names)
         else:
             newnames = []
```

### Comparing `hipopy-1.3.2/hipopy/hipopy__BACKUP.py` & `hipopy-1.3.3/hipopy/hipopy__BACKUP.py`

 * *Files identical despite different names*

### Comparing `hipopy-1.3.2/hipopy/test1.py` & `hipopy-1.3.3/hipopy/test1.py`

 * *Files identical despite different names*

### Comparing `hipopy-1.3.2/hipopy/test2.py` & `hipopy-1.3.3/hipopy/test2.py`

 * *Files identical despite different names*

### Comparing `hipopy-1.3.2/pyproject.toml` & `hipopy-1.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "hipopy"
-version = "1.3.2"
+version = "1.3.3"
 license = "MIT"
 description = "UpROOT-Like I/O Interface for CLAS12 HIPO Files"
 authors = ["Matthew McEneaney <matthew.mceneaney@duke.edu>"]
 repository = "https://github.com/mfmceneaney/hipopy.git"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.3"
-awkward = "^1.3.0"
-numpy = "^1.19.2"
+awkward = ">=1.3.0"
+numpy = ">=1.19.2"
 hipopybind = ">=1.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `hipopy-1.3.2/PKG-INFO` & `hipopy-1.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: hipopy
-Version: 1.3.2
+Version: 1.3.3
 Summary: UpROOT-Like I/O Interface for CLAS12 HIPO Files
 Home-page: https://github.com/mfmceneaney/hipopy.git
 License: MIT
 Author: Matthew McEneaney
 Author-email: matthew.mceneaney@duke.edu
 Requires-Python: >=3.7.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: awkward (>=1.3.0,<2.0.0)
+Requires-Dist: awkward (>=1.3.0)
 Requires-Dist: hipopybind (>=1.1.1)
-Requires-Dist: numpy (>=1.19.2,<2.0.0)
+Requires-Dist: numpy (>=1.19.2)
 Project-URL: Repository, https://github.com/mfmceneaney/hipopy.git
 Description-Content-Type: text/markdown
 
 # HIPOPy: UpROOT-like I/O Interface for CLAS12 HIPO Files
 
 ## Prerequisites
```

