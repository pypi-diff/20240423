# Comparing `tmp/hddm_s-1.0.tar.gz` & `tmp/hddm_s-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_s-1.0.tar", last modified: Tue Apr 23 10:16:57 2024, max compression
+gzip compressed data, was "hddm_s-1.0.1.tar", last modified: Tue Apr 23 11:01:25 2024, max compression
```

## Comparing `hddm_s-1.0.tar` & `hddm_s-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:16:57.839967 hddm_s-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 10:16:51.000000 hddm_s-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 10:16:57.839967 hddm_s-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 10:16:51.000000 hddm_s-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:16:57.839967 hddm_s-1.0/hddm_s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 10:16:57.000000 hddm_s-1.0/hddm_s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 10:16:57.000000 hddm_s-1.0/hddm_s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:16:57.000000 hddm_s-1.0/hddm_s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 10:16:57.000000 hddm_s-1.0/hddm_s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 10:16:51.000000 hddm_s-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:16:57.839967 hddm_s-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-23 10:16:51.000000 hddm_s-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:01:25.957160 hddm_s-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 11:01:19.000000 hddm_s-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 11:01:25.957160 hddm_s-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 11:01:19.000000 hddm_s-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:01:25.957160 hddm_s-1.0.1/hddm_s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 11:01:25.000000 hddm_s-1.0.1/hddm_s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 11:01:25.000000 hddm_s-1.0.1/hddm_s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:01:25.000000 hddm_s-1.0.1/hddm_s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 11:01:25.000000 hddm_s-1.0.1/hddm_s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-23 11:01:19.000000 hddm_s-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:01:25.957160 hddm_s-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-23 11:01:19.000000 hddm_s-1.0.1/setup.py
```

### Comparing `hddm_s-1.0/LICENSE` & `hddm_s-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0/PKG-INFO` & `hddm_s-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0
+Version: 1.0.1
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0/README.md` & `hddm_s-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0/hddm_s.egg-info/PKG-INFO` & `hddm_s-1.0.1/hddm_s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0
+Version: 1.0.1
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0/pyproject.toml` & `hddm_s-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_s"
-version = "1.0"
+version = "1.0.1"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

### Comparing `hddm_s-1.0/setup.py` & `hddm_s-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 }
 
 sources = {
   "xerces-c.url": "https://github.com/apache/xerces-c.git",
   "xerces-c.tag": "tags/v3.2.5",
   "hdf5.url": "https://github.com/HDFGroup/hdf5.git",
   "hdf5.tag": "tags/hdf5-1_10_8",
-  "xrootd.url": "https://github.com/xrootd/xrootd.git",
-  "xrootd.tag": "tags/v5.6.9",
+#  "xrootd.url": "https://github.com/xrootd/xrootd.git",
+#  "xrootd.tag": "tags/v5.6.9",
   "HDDM.url": "https://github.com/rjones30/HDDM.git",
   "HDDM.tag": "tags/4.30.1",
 }
 
 class CMakeExtension(setuptools.Extension):
 
     def __init__(self, name):
@@ -85,19 +85,19 @@
     packages = setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires = '>=3.6',              # Minimum version requirement of the package
-    #packages = templates.keys(),            # Name of the python package
+    #packages = templates.keys(),           # Name of the python package
     install_requires = [],                  # Install other dependencies if any
     ext_modules = [
       CMakeExtension("xerces-c"),
       CMakeExtension("hdf5"),
-      CMakeExtension("xrootd"),
+      #CMakeExtension("xrootd"),
       CMakeExtension("HDDM"),
     ],
     cmdclass = {
       "build_ext": build_ext_with_cmake,
     }
 )
```

