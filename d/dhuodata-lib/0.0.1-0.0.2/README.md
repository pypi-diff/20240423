# Comparing `tmp/dhuodata-lib-0.0.1.tar.gz` & `tmp/dhuodata-lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.0.1.tar", last modified: Tue Apr 23 16:34:42 2024, max compression
+gzip compressed data, was "dhuodata-lib-0.0.2.tar", last modified: Tue Apr 23 16:41:54 2024, max compression
```

## Comparing `dhuodata-lib-0.0.1.tar` & `dhuodata-lib-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:34:42.266603 dhuodata-lib-0.0.1/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 16:34:42.266603 dhuodata-lib-0.0.1/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.1/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:34:42.266603 dhuodata-lib-0.0.1/dhuodata_lib.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 16:34:42.000000 dhuodata-lib-0.0.1/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      262 2024-04-23 16:34:42.000000 dhuodata-lib-0.0.1/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 16:34:42.000000 dhuodata-lib-0.0.1/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-04-23 16:34:42.000000 dhuodata-lib-0.0.1/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 16:34:42.000000 dhuodata-lib-0.0.1/dhuodata_lib.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-23 16:34:42.266603 dhuodata-lib-0.0.1/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      873 2024-04-23 16:34:40.000000 dhuodata-lib-0.0.1/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:34:42.266603 dhuodata-lib-0.0.1/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-23 16:28:09.000000 dhuodata-lib-0.0.1/tests/test_dhuolib.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuodata-lib-0.0.1/tests/test_services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuodata-lib-0.0.1/tests/test_utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:41:54.392841 dhuodata-lib-0.0.2/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 16:41:54.392841 dhuodata-lib-0.0.2/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.0.2/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-23 16:41:54.392841 dhuodata-lib-0.0.2/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-23 16:41:23.000000 dhuodata-lib-0.0.2/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:41:54.392841 dhuodata-lib-0.0.2/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:41:54.392841 dhuodata-lib-0.0.2/src/dhuodata_lib.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-23 16:41:54.000000 dhuodata-lib-0.0.2/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      319 2024-04-23 16:41:54.000000 dhuodata-lib-0.0.2/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 16:41:54.000000 dhuodata-lib-0.0.2/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-04-23 16:41:54.000000 dhuodata-lib-0.0.2/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        4 2024-04-23 16:41:54.000000 dhuodata-lib-0.0.2/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:41:54.392841 dhuodata-lib-0.0.2/src/oci/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuodata-lib-0.0.2/src/oci/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-22 13:45:37.000000 dhuodata-lib-0.0.2/src/oci/utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 16:41:54.392841 dhuodata-lib-0.0.2/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-23 16:28:09.000000 dhuodata-lib-0.0.2/tests/test_dhuolib.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuodata-lib-0.0.2/tests/test_services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuodata-lib-0.0.2/tests/test_utils.py
```

### Comparing `dhuodata-lib-0.0.1/PKG-INFO` & `dhuodata-lib-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.0.1/README.md` & `dhuodata-lib-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.1/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.0.2/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuodata-lib-0.0.1/tests/test_dhuolib.py` & `dhuodata-lib-0.0.2/tests/test_dhuolib.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.1/tests/test_services.py` & `dhuodata-lib-0.0.2/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.0.1/tests/test_utils.py` & `dhuodata-lib-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

