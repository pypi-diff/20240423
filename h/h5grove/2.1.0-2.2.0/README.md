# Comparing `tmp/h5grove-2.1.0.tar.gz` & `tmp/h5grove-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5grove-2.1.0.tar", last modified: Fri Mar 22 08:00:34 2024, max compression
+gzip compressed data, was "h5grove-2.2.0.tar", last modified: Tue Apr 23 12:51:41 2024, max compression
```

## Comparing `h5grove-2.1.0.tar` & `h5grove-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:00:34.469472 h5grove-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-22 07:59:57.000000 h5grove-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-22 07:59:57.000000 h5grove-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-03-22 08:00:34.469472 h5grove-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-22 07:59:57.000000 h5grove-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:00:34.465472 h5grove-2.1.0/example/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-22 07:59:57.000000 h5grove-2.1.0/example/fastapi_app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1641 2024-03-22 07:59:57.000000 h5grove-2.1.0/example/flask_app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1246 2024-03-22 07:59:57.000000 h5grove-2.1.0/example/tornado_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:00:34.465472 h5grove-2.1.0/h5grove/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/flask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/tornado_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-03-22 07:59:57.000000 h5grove-2.1.0/h5grove/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:00:34.465472 h5grove-2.1.0/h5grove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-03-22 08:00:34.000000 h5grove-2.1.0/h5grove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-22 08:00:34.000000 h5grove-2.1.0/h5grove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 08:00:34.000000 h5grove-2.1.0/h5grove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-22 08:00:34.000000 h5grove-2.1.0/h5grove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 08:00:34.000000 h5grove-2.1.0/h5grove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-22 07:59:57.000000 h5grove-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-22 08:00:34.469472 h5grove-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-22 07:59:57.000000 h5grove-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:51:41.626580 h5grove-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-23 12:51:10.000000 h5grove-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 12:51:10.000000 h5grove-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-23 12:51:41.626580 h5grove-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-23 12:51:10.000000 h5grove-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:51:41.622580 h5grove-2.2.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-23 12:51:10.000000 h5grove-2.2.0/example/fastapi_app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1641 2024-04-23 12:51:10.000000 h5grove-2.2.0/example/flask_app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1246 2024-04-23 12:51:10.000000 h5grove-2.2.0/example/tornado_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:51:41.622580 h5grove-2.2.0/h5grove/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/flask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/tornado_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-23 12:51:10.000000 h5grove-2.2.0/h5grove/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:51:41.622580 h5grove-2.2.0/h5grove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-23 12:51:41.000000 h5grove-2.2.0/h5grove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-23 12:51:41.000000 h5grove-2.2.0/h5grove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:51:41.000000 h5grove-2.2.0/h5grove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 12:51:41.000000 h5grove-2.2.0/h5grove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 12:51:41.000000 h5grove-2.2.0/h5grove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 12:51:10.000000 h5grove-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-23 12:51:41.626580 h5grove-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 12:51:10.000000 h5grove-2.2.0/setup.py
```

### Comparing `h5grove-2.1.0/LICENSE` & `h5grove-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/PKG-INFO` & `h5grove-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5grove
-Version: 2.1.0
+Version: 2.2.0
 Summary: Core utilities to serve HDF5 file contents
 Home-page: https://github.com/silx-kit/h5grove
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silx-kit/h5grove/-/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `h5grove-2.1.0/README.md` & `h5grove-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/example/fastapi_app.py` & `h5grove-2.2.0/example/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/example/flask_app.py` & `h5grove-2.2.0/example/flask_app.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/example/tornado_app.py` & `h5grove-2.2.0/example/tornado_app.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/h5grove/content.py` & `h5grove-2.2.0/h5grove/content.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/h5grove/encoders.py` & `h5grove-2.2.0/h5grove/encoders.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/h5grove/fastapi_utils.py` & `h5grove-2.2.0/h5grove/fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/h5grove/flask_utils.py` & `h5grove-2.2.0/h5grove/flask_utils.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/h5grove/models.py` & `h5grove-2.2.0/h5grove/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     {
         "class": int,  # HDF5 class code
         "dtype": StrDtype,  # Numpy-style dtype
         "size": int,  # all (but most relevant for int, float, string)
         "order": int,  # int, float, bitfield
         "sign": int,  # int
         "cset": int,  # string
+        "strpad": int,  # string
         "vlen": bool,  # string
         "tag": str,  # opaque
         "dims": Tuple[int, ...],  # array
         "members": Union[Dict[str, "TypeMetadata"], Dict[str, int]],  # compound, enum
         "base": "TypeMetadata",  # array, enum, vlen
     },
     total=False,
```

### Comparing `h5grove-2.1.0/h5grove/tornado_utils.py` & `h5grove-2.2.0/h5grove/tornado_utils.py`

 * *Files identical despite different names*

### Comparing `h5grove-2.1.0/h5grove/utils.py` & `h5grove-2.2.0/h5grove/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
             "order": type_id.get_order(),
         }
 
     if isinstance(type_id, h5py.h5t.TypeStringID):
         return {
             **base_metadata,
             "cset": type_id.get_cset(),
+            "strpad": type_id.get_strpad(),
             "vlen": type_id.is_variable_str(),
         }
 
     if isinstance(type_id, h5py.h5t.TypeBitfieldID):
         return {**base_metadata, "order": type_id.get_order()}
 
     if isinstance(type_id, h5py.h5t.TypeOpaqueID):
```

### Comparing `h5grove-2.1.0/h5grove.egg-info/PKG-INFO` & `h5grove-2.2.0/h5grove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5grove
-Version: 2.1.0
+Version: 2.2.0
 Summary: Core utilities to serve HDF5 file contents
 Home-page: https://github.com/silx-kit/h5grove
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silx-kit/h5grove/-/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `h5grove-2.1.0/setup.cfg` & `h5grove-2.2.0/setup.cfg`

 * *Files identical despite different names*

