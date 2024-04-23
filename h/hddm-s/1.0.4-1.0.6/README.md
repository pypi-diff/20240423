# Comparing `tmp/hddm_s-1.0.4.tar.gz` & `tmp/hddm_s-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_s-1.0.4.tar", last modified: Tue Apr 23 14:43:46 2024, max compression
+gzip compressed data, was "hddm_s-1.0.6.tar", last modified: Tue Apr 23 15:07:53 2024, max compression
```

## Comparing `hddm_s-1.0.4.tar` & `hddm_s-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:43:46.937751 hddm_s-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 14:43:43.000000 hddm_s-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 14:43:46.937751 hddm_s-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 14:43:43.000000 hddm_s-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:43:46.937751 hddm_s-1.0.4/hddm_s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-23 14:43:43.000000 hddm_s-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:43:46.937751 hddm_s-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-23 14:43:43.000000 hddm_s-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:53.630736 hddm_s-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 15:07:49.000000 hddm_s-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 15:07:53.630736 hddm_s-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 15:07:49.000000 hddm_s-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:53.630736 hddm_s-1.0.6/hddm_s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 15:07:53.000000 hddm_s-1.0.6/hddm_s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 15:07:53.000000 hddm_s-1.0.6/hddm_s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:07:53.000000 hddm_s-1.0.6/hddm_s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 15:07:53.000000 hddm_s-1.0.6/hddm_s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-23 15:07:49.000000 hddm_s-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:07:53.630736 hddm_s-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-23 15:07:49.000000 hddm_s-1.0.6/setup.py
```

### Comparing `hddm_s-1.0.4/LICENSE` & `hddm_s-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0.4/PKG-INFO` & `hddm_s-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0.4
+Version: 1.0.6
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0.4/README.md` & `hddm_s-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0.4/hddm_s.egg-info/PKG-INFO` & `hddm_s-1.0.6/hddm_s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0.4
+Version: 1.0.6
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0.4/pyproject.toml` & `hddm_s-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_s"
-version = "1.0.4"
+version = "1.0.6"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

### Comparing `hddm_s-1.0.4/setup.py` & `hddm_s-1.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,17 +61,17 @@
             os.chdir(cwd)
             self.spawn(["rm", "-rf", ext.name, f"build.{ext.name}"])
         os.chdir(cwd)
         if ext.name == "HDDM": # finish construction of the hddm module
             os.environ['HDDM_DIR'] = f"{cwd}/build"
             os.environ['LD_LIBRARY_PATH'] += f":{cwd}/build/lib:{cwd}/build/lib64"
             for models in templates:
-                for mod in models:
-                    self.spawn(["build/bin/hddm-cpp", models[mod]])
-                    self.spawn(["build/bin/hddm-py", models[mod]])
+                for model in models:
+                    self.spawn(["build/bin/hddm-cpp", model])
+                    self.spawn(["build/bin/hddm-py", model])
                     self.spawn(["sed", "-i", "s/os\.path\.realpath(__file__)/'.'/", f"setup_{mod}.py"])
                     self.spawn(["python3", f"setup_{mod}.py"])
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
@@ -81,22 +81,23 @@
     url = "https://github.com/rjones30/hddm_s",
     author = "Richard T. Jones",
     description = "i/o module for GlueX simulated events",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     package_data = templates,
+    include_package_data = True,
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires = '>=3.6',              # Minimum version requirement of the package
     #packages = templates.keys(),           # Name of the python package
-    install_requires = [],                  # Install other dependencies if any
+    install_requires = ["setuptools-git"],  # Install other dependencies if any
     ext_modules = [
       CMakeExtension("xerces-c"),
       CMakeExtension("hdf5"),
       #CMakeExtension("xrootd"),
       CMakeExtension("HDDM"),
     ],
     cmdclass = {
```

