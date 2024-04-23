# Comparing `tmp/dhuodata-lib-0.0.4.tar.gz` & `tmp/dhuodata-lib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.0.4.tar", last modified: Tue Apr 23 17:05:04 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.0.5.tar", last modified: Tue Apr 23 17:10:09 2024, max compression
```

## Comparing `dhuodata-lib-0.0.4.tar` & `dhuodata-lib-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:05:04.968802 dhuodata-lib-0.0.4/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:05:04.968802 dhuodata-lib-0.0.4/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.4/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-23 17:05:04.968802 dhuodata-lib-0.0.4/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-23 17:05:02.000000 dhuodata-lib-0.0.4/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:05:04.964801 dhuodata-lib-0.0.4/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:05:04.964801 dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:05:04.000000 dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      514 2024-04-23 17:05:04.000000 dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 17:05:04.000000 dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-04-23 17:05:04.000000 dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-23 17:05:04.000000 dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:05:04.968802 dhuodata-lib-0.0.4/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.4/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.0.4/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3518 2024-04-23 17:01:24.000000 dhuodata-lib-0.0.4/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-23 16:51:37.000000 dhuodata-lib-0.0.4/src/dhuolib/config.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:05:04.968802 dhuodata-lib-0.0.4/src/dhuolib/oci/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata-lib-0.0.4/src/dhuolib/oci/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-23 16:55:18.000000 dhuodata-lib-0.0.4/src/dhuolib/oci/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      762 2024-04-23 16:50:59.000000 dhuodata-lib-0.0.4/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-23 16:51:03.000000 dhuodata-lib-0.0.4/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-23 16:51:09.000000 dhuodata-lib-0.0.4/src/dhuolib/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.0.4/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:05:04.968802 dhuodata-lib-0.0.4/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-23 16:28:09.000000 dhuodata-lib-0.0.4/tests/test_dhuolib.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuodata-lib-0.0.4/tests/test_services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuodata-lib-0.0.4/tests/test_utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:10:09.850315 dhuodata-lib-0.0.5/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:10:09.850315 dhuodata-lib-0.0.5/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.5/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-23 17:10:09.850315 dhuodata-lib-0.0.5/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-23 17:09:57.000000 dhuodata-lib-0.0.5/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:10:09.846315 dhuodata-lib-0.0.5/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:10:09.846315 dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:10:09.000000 dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      514 2024-04-23 17:10:09.000000 dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 17:10:09.000000 dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-04-23 17:10:09.000000 dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-23 17:10:09.000000 dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:10:09.846315 dhuodata-lib-0.0.5/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.5/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.0.5/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3526 2024-04-23 17:09:42.000000 dhuodata-lib-0.0.5/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-23 16:51:37.000000 dhuodata-lib-0.0.5/src/dhuolib/config.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:10:09.850315 dhuodata-lib-0.0.5/src/dhuolib/oci/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata-lib-0.0.5/src/dhuolib/oci/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-23 16:55:18.000000 dhuodata-lib-0.0.5/src/dhuolib/oci/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      762 2024-04-23 16:50:59.000000 dhuodata-lib-0.0.5/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-23 16:51:03.000000 dhuodata-lib-0.0.5/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-23 16:51:09.000000 dhuodata-lib-0.0.5/src/dhuolib/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.0.5/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:10:09.850315 dhuodata-lib-0.0.5/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-23 16:28:09.000000 dhuodata-lib-0.0.5/tests/test_dhuolib.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuodata-lib-0.0.5/tests/test_services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuodata-lib-0.0.5/tests/test_utils.py
```

### Comparing `dhuodata-lib-0.0.4/PKG-INFO` & `dhuodata-lib-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.0.4/README.md` & `dhuodata-lib-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.4/setup.py` & `dhuodata-lib-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.0.4",
+    version="0.0.5",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.0.4/src/dhuodata_lib.egg-info/SOURCES.txt` & `dhuodata-lib-0.0.5/src/dhuodata_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.4/src/dhuolib/clients.py` & `dhuodata-lib-0.0.5/src/dhuolib/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dhuolib.config import logger
+from dhuolib.oci.utils import OCIUtils
 from dhuolib.services import ServiceAPIML
-from oci.utils import OCIUtils
 
 
 class DhuolibClient:
     def __init__(self, service_endpoint=None, config_file_path='~/.oci/config'):
         if not service_endpoint:
             raise ValueError("service_endpoint is required")
```

### Comparing `dhuodata-lib-0.0.4/src/dhuolib/oci/utils.py` & `dhuodata-lib-0.0.5/src/dhuolib/oci/utils.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.4/src/dhuolib/predict.py` & `dhuodata-lib-0.0.5/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.4/src/dhuolib/services.py` & `dhuodata-lib-0.0.5/src/dhuolib/services.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.4/tests/test_dhuolib.py` & `dhuodata-lib-0.0.5/tests/test_dhuolib.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.4/tests/test_services.py` & `dhuodata-lib-0.0.5/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.4/tests/test_utils.py` & `dhuodata-lib-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

