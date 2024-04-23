# Comparing `tmp/dhuodata-lib-0.0.6.tar.gz` & `tmp/dhuodata-lib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.0.6.tar", last modified: Tue Apr 23 17:22:42 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.0.7.tar", last modified: Tue Apr 23 17:59:09 2024, max compression
```

## Comparing `dhuodata-lib-0.0.6.tar` & `dhuodata-lib-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.6/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-23 17:22:09.000000 dhuodata-lib-0.0.6/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:22:42.000000 dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      526 2024-04-23 17:22:42.000000 dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 17:22:42.000000 dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      128 2024-04-23 17:22:42.000000 dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-23 17:22:42.000000 dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.6/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.0.6/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3538 2024-04-23 17:21:58.000000 dhuodata-lib-0.0.6/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-23 16:51:37.000000 dhuodata-lib-0.0.6/src/dhuolib/config.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/src/dhuolib/oci_tools/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata-lib-0.0.6/src/dhuolib/oci_tools/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-23 16:55:18.000000 dhuodata-lib-0.0.6/src/dhuolib/oci_tools/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      762 2024-04-23 16:50:59.000000 dhuodata-lib-0.0.6/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-23 16:51:03.000000 dhuodata-lib-0.0.6/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-23 16:51:09.000000 dhuodata-lib-0.0.6/src/dhuolib/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.0.6/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:22:42.541257 dhuodata-lib-0.0.6/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-23 16:28:09.000000 dhuodata-lib-0.0.6/tests/test_dhuolib.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuodata-lib-0.0.6/tests/test_services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuodata-lib-0.0.6/tests/test_utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:59:09.815997 dhuodata-lib-0.0.7/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:59:09.815997 dhuodata-lib-0.0.7/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.7/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-23 17:59:09.815997 dhuodata-lib-0.0.7/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-23 17:59:08.000000 dhuodata-lib-0.0.7/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:59:09.811996 dhuodata-lib-0.0.7/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:59:09.811996 dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 17:59:09.000000 dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      526 2024-04-23 17:59:09.000000 dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 17:59:09.000000 dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      128 2024-04-23 17:59:09.000000 dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-23 17:59:09.000000 dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:59:09.811996 dhuodata-lib-0.0.7/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.7/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.0.7/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3538 2024-04-23 17:21:58.000000 dhuodata-lib-0.0.7/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-23 16:51:37.000000 dhuodata-lib-0.0.7/src/dhuolib/config.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:59:09.811996 dhuodata-lib-0.0.7/src/dhuolib/oci_tools/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata-lib-0.0.7/src/dhuolib/oci_tools/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-23 16:55:18.000000 dhuodata-lib-0.0.7/src/dhuolib/oci_tools/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      762 2024-04-23 16:50:59.000000 dhuodata-lib-0.0.7/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-23 16:51:03.000000 dhuodata-lib-0.0.7/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-23 16:51:09.000000 dhuodata-lib-0.0.7/src/dhuolib/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.0.7/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 17:59:09.815997 dhuodata-lib-0.0.7/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-23 16:28:09.000000 dhuodata-lib-0.0.7/tests/test_dhuolib.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuodata-lib-0.0.7/tests/test_services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuodata-lib-0.0.7/tests/test_utils.py
```

### Comparing `dhuodata-lib-0.0.6/PKG-INFO` & `dhuodata-lib-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.0.6/README.md` & `dhuodata-lib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/setup.py` & `dhuodata-lib-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.0.6",
+    version="0.0.7",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.0.6/src/dhuodata_lib.egg-info/SOURCES.txt` & `dhuodata-lib-0.0.7/src/dhuodata_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/src/dhuolib/clients.py` & `dhuodata-lib-0.0.7/src/dhuolib/clients.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/src/dhuolib/oci_tools/utils.py` & `dhuodata-lib-0.0.7/src/dhuolib/oci_tools/utils.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/src/dhuolib/predict.py` & `dhuodata-lib-0.0.7/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/src/dhuolib/services.py` & `dhuodata-lib-0.0.7/src/dhuolib/services.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/tests/test_dhuolib.py` & `dhuodata-lib-0.0.7/tests/test_dhuolib.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/tests/test_services.py` & `dhuodata-lib-0.0.7/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.6/tests/test_utils.py` & `dhuodata-lib-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*
