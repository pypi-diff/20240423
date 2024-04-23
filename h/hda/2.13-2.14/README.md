# Comparing `tmp/hda-2.13.tar.gz` & `tmp/hda-2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hda-2.13.tar", last modified: Fri Apr 12 17:32:43 2024, max compression
+gzip compressed data, was "hda-2.14.tar", last modified: Tue Apr 23 08:40:18 2024, max compression
```

## Comparing `hda-2.13.tar` & `hda-2.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:32:43.737866 hda-2.13/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-12 17:32:29.000000 hda-2.13/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-12 17:32:43.737866 hda-2.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-12 17:32:29.000000 hda-2.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:32:43.737866 hda-2.13/hda/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 17:32:29.000000 hda-2.13/hda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-04-12 17:32:29.000000 hda-2.13/hda/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-12 17:32:29.000000 hda-2.13/hda/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:32:43.737866 hda-2.13/hda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:32:43.737866 hda-2.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-12 17:32:29.000000 hda-2.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:40:18.429583 hda-2.14/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-23 08:40:07.000000 hda-2.14/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 08:40:18.429583 hda-2.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-23 08:40:07.000000 hda-2.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:40:18.429583 hda-2.14/hda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 08:40:07.000000 hda-2.14/hda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25544 2024-04-23 08:40:07.000000 hda-2.14/hda/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-23 08:40:07.000000 hda-2.14/hda/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:40:18.429583 hda-2.14/hda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 08:40:18.000000 hda-2.14/hda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-23 08:40:18.000000 hda-2.14/hda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:40:18.000000 hda-2.14/hda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 08:40:18.000000 hda-2.14/hda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 08:40:18.000000 hda-2.14/hda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:40:18.000000 hda-2.14/hda.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:40:18.429583 hda-2.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-23 08:40:07.000000 hda-2.14/setup.py
```

### Comparing `hda-2.13/LICENSE.txt` & `hda-2.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hda-2.13/PKG-INFO` & `hda-2.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hda
-Version: 2.13
+Version: 2.14
 Summary: API to harmonised data access for DIAS/WEkEO
 Home-page: https://github.com/ecmwf/hda
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `hda-2.13/README.md` & `hda-2.14/README.md`

 * *Files identical despite different names*

### Comparing `hda-2.13/hda/__init__.py` & `hda-2.14/hda/__init__.py`

 * *Files identical despite different names*

### Comparing `hda-2.13/hda/api.py` & `hda-2.14/hda/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,18 +316,15 @@
         self,
         url=os.environ.get("HDA_URL"),
         user=os.environ.get("HDA_USER"),
         password=os.environ.get("HDA_PASSWORD"),
         verify=True,
         path=None,
     ):
-        credentials = {
-            "user": None,
-            "password": None
-        }
+        credentials = {"user": None, "password": None}
 
         dotrc = path or os.environ.get("HDA_RC", os.path.expanduser("~/.hdarc"))
 
         if os.path.isfile(dotrc):
             config = read_config(dotrc)
 
             for key in credentials.keys():
```

### Comparing `hda-2.13/hda.egg-info/PKG-INFO` & `hda-2.14/hda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hda
-Version: 2.13
+Version: 2.14
 Summary: API to harmonised data access for DIAS/WEkEO
 Home-page: https://github.com/ecmwf/hda
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `hda-2.13/setup.py` & `hda-2.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return io.open(file_path, encoding="utf-8").read()
 
 
-version = "2.13"
+version = "2.14"
 
 setuptools.setup(
     name="hda",
     version=version,
     author="ECMWF",
     author_email="software.support@ecmwf.int",
     license="Apache 2.0",
```

