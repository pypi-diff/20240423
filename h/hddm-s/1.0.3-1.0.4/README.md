# Comparing `tmp/hddm_s-1.0.3.tar.gz` & `tmp/hddm_s-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddm_s-1.0.3.tar", last modified: Tue Apr 23 14:32:09 2024, max compression
+gzip compressed data, was "hddm_s-1.0.4.tar", last modified: Tue Apr 23 14:43:46 2024, max compression
```

## Comparing `hddm_s-1.0.3.tar` & `hddm_s-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:09.452741 hddm_s-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 14:32:06.000000 hddm_s-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 14:32:09.452741 hddm_s-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 14:32:06.000000 hddm_s-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:09.452741 hddm_s-1.0.3/hddm_s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 14:32:09.000000 hddm_s-1.0.3/hddm_s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 14:32:09.000000 hddm_s-1.0.3/hddm_s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:32:09.000000 hddm_s-1.0.3/hddm_s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 14:32:09.000000 hddm_s-1.0.3/hddm_s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-23 14:32:06.000000 hddm_s-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:32:09.452741 hddm_s-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-23 14:32:06.000000 hddm_s-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:43:46.937751 hddm_s-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 14:43:43.000000 hddm_s-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 14:43:46.937751 hddm_s-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 14:43:43.000000 hddm_s-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:43:46.937751 hddm_s-1.0.4/hddm_s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 14:43:46.000000 hddm_s-1.0.4/hddm_s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-23 14:43:43.000000 hddm_s-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:43:46.937751 hddm_s-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-23 14:43:43.000000 hddm_s-1.0.4/setup.py
```

### Comparing `hddm_s-1.0.3/LICENSE` & `hddm_s-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0.3/PKG-INFO` & `hddm_s-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0.3
+Version: 1.0.4
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0.3/README.md` & `hddm_s-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hddm_s-1.0.3/hddm_s.egg-info/PKG-INFO` & `hddm_s-1.0.4/hddm_s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hddm_s
-Version: 1.0.3
+Version: 1.0.4
 Summary: methods for reading and writing GlueX simulated event data
 Home-page: https://github.com/rjones30/hddm_s
 Author: Richard T. Jones
 Author-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 Maintainer-email: "Richard T. Jones" <richard.t.jones@uconn.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/rjones30/hddm_s
```

### Comparing `hddm_s-1.0.3/pyproject.toml` & `hddm_s-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 38.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hddm_s"
-version = "1.0.3"
+version = "1.0.4"
 requires-python = ">= 3.6"
 authors = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
 maintainers = [
   {name = "Richard T. Jones", email = "richard.t.jones@uconn.edu"},
 ]
```

### Comparing `hddm_s-1.0.3/setup.py` & `hddm_s-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
             self.spawn(["rm", "-rf", ext.name, f"build.{ext.name}"])
         os.chdir(cwd)
         if ext.name == "HDDM": # finish construction of the hddm module
             os.environ['HDDM_DIR'] = f"{cwd}/build"
             os.environ['LD_LIBRARY_PATH'] += f":{cwd}/build/lib:{cwd}/build/lib64"
             for models in templates:
                 for mod in models:
-                    self.spawn(["ls", "-lR"])
                     self.spawn(["build/bin/hddm-cpp", models[mod]])
                     self.spawn(["build/bin/hddm-py", models[mod]])
                     self.spawn(["sed", "-i", "s/os\.path\.realpath(__file__)/'.'/", f"setup_{mod}.py"])
                     self.spawn(["python3", f"setup_{mod}.py"])
 
 
 with open("README.md", "r") as fh:
```

