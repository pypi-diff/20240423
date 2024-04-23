# Comparing `tmp/dhuolib-tools-0.0.4.tar.gz` & `tmp/dhuolib-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuolib-tools-0.0.4.tar", last modified: Mon Apr 22 14:03:29 2024, max compression
+gzip compressed data, was "dhuolib-tools-0.0.5.tar", last modified: Tue Apr 23 13:44:18 2024, max compression
```

## Comparing `dhuolib-tools-0.0.4.tar` & `dhuolib-tools-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-22 14:03:29.459707 dhuolib-tools-0.0.4/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2529 2024-04-22 14:03:29.459707 dhuolib-tools-0.0.4/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.4/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-22 14:03:29.459707 dhuolib-tools-0.0.4/dhuolib_tools.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2529 2024-04-22 14:03:29.000000 dhuolib-tools-0.0.4/dhuolib_tools.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      432 2024-04-22 14:03:29.000000 dhuolib-tools-0.0.4/dhuolib_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-22 14:03:29.000000 dhuolib-tools-0.0.4/dhuolib_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-04-22 14:03:29.000000 dhuolib-tools-0.0.4/dhuolib_tools.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        4 2024-04-22 14:03:29.000000 dhuolib-tools-0.0.4/dhuolib_tools.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-22 14:03:29.459707 dhuolib-tools-0.0.4/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      848 2024-04-22 14:03:11.000000 dhuolib-tools-0.0.4/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-22 14:03:29.459707 dhuolib-tools-0.0.4/src/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.4/src/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.4/src/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-19 11:44:28.000000 dhuolib-tools-0.0.4/src/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3508 2024-04-22 13:53:48.000000 dhuolib-tools-0.0.4/src/dhuolib.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-22 14:03:29.459707 dhuolib-tools-0.0.4/src/oci/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuolib-tools-0.0.4/src/oci/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-22 13:45:37.000000 dhuolib-tools-0.0.4/src/oci/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      762 2024-04-16 19:06:26.000000 dhuolib-tools-0.0.4/src/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-22 01:19:09.000000 dhuolib-tools-0.0.4/src/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      838 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.4/src/setup.py
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-15 20:24:53.000000 dhuolib-tools-0.0.4/src/utils.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.4/src/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-22 14:03:29.459707 dhuolib-tools-0.0.4/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-22 13:10:17.000000 dhuolib-tools-0.0.4/tests/test_dhuolib.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuolib-tools-0.0.4/tests/test_services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuolib-tools-0.0.4/tests/test_utils.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 13:44:18.437322 dhuolib-tools-0.0.5/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2529 2024-04-23 13:44:18.437322 dhuolib-tools-0.0.5/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.5/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 13:44:18.437322 dhuolib-tools-0.0.5/dhuolib_tools.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2529 2024-04-23 13:44:18.000000 dhuolib-tools-0.0.5/dhuolib_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      450 2024-04-23 13:44:18.000000 dhuolib-tools-0.0.5/dhuolib_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-23 13:44:18.000000 dhuolib-tools-0.0.5/dhuolib_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-04-23 13:44:18.000000 dhuolib-tools-0.0.5/dhuolib_tools.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       10 2024-04-23 13:44:18.000000 dhuolib-tools-0.0.5/dhuolib_tools.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-23 13:44:18.437322 dhuolib-tools-0.0.5/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      824 2024-04-23 13:44:05.000000 dhuolib-tools-0.0.5/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 13:44:18.437322 dhuolib-tools-0.0.5/src/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.5/src/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.5/src/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      358 2024-04-19 11:44:28.000000 dhuolib-tools-0.0.5/src/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3514 2024-04-23 13:44:14.000000 dhuolib-tools-0.0.5/src/dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 13:44:18.437322 dhuolib-tools-0.0.5/src/oci/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:52:32.000000 dhuolib-tools-0.0.5/src/oci/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      716 2024-04-22 13:45:37.000000 dhuolib-tools-0.0.5/src/oci/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      762 2024-04-16 19:06:26.000000 dhuolib-tools-0.0.5/src/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1087 2024-04-22 01:19:09.000000 dhuolib-tools-0.0.5/src/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      838 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.5/src/setup.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-15 20:24:53.000000 dhuolib-tools-0.0.5/src/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-16 18:35:41.000000 dhuolib-tools-0.0.5/src/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-23 13:44:18.437322 dhuolib-tools-0.0.5/tests/
+-rw-r--r--   0 diego     (1000) diego     (1000)        0 2024-04-15 20:51:07.000000 dhuolib-tools-0.0.5/tests/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2431 2024-04-22 13:10:17.000000 dhuolib-tools-0.0.5/tests/test_dhuolib.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1097 2024-04-17 13:15:56.000000 dhuolib-tools-0.0.5/tests/test_services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1331 2024-04-18 20:04:54.000000 dhuolib-tools-0.0.5/tests/test_utils.py
```

### Comparing `dhuolib-tools-0.0.4/PKG-INFO` & `dhuolib-tools-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuolib-tools
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuolib-tools-0.0.4/README.md` & `dhuolib-tools-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dhuolib-tools-0.0.4/dhuolib_tools.egg-info/PKG-INFO` & `dhuolib-tools-0.0.5/dhuolib_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuolib-tools
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

### Comparing `dhuolib-tools-0.0.4/setup.py` & `dhuolib-tools-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuolib-tools",
-    version="0.0.4",
+    version="0.0.5",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
-    packages=find_packages(include=["src", "src.*"]),
+    packages=find_packages(),
     platforms="any",
 )
```

### Comparing `dhuolib-tools-0.0.4/src/dhuolib.py` & `dhuolib-tools-0.0.5/src/dhuolib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from src.config import logger
 from src.oci.utils import OCIUtils
 from src.services import ServiceAPIML
 
 
-class Dhuolib:
+class DhuolibClient:
     def __init__(self, service_endpoint=None, config_file_path='~/.oci/config'):
         if not service_endpoint:
             raise ValueError("service_endpoint is required")
 
         self.service = ServiceAPIML(service_endpoint)
         self.oci = OCIUtils(config_file_path=config_file_path)
```

### Comparing `dhuolib-tools-0.0.4/src/oci/utils.py` & `dhuolib-tools-0.0.5/src/oci/utils.py`

 * *Files identical despite different names*

### Comparing `dhuolib-tools-0.0.4/src/predict.py` & `dhuolib-tools-0.0.5/src/predict.py`

 * *Files identical despite different names*

### Comparing `dhuolib-tools-0.0.4/src/services.py` & `dhuolib-tools-0.0.5/src/services.py`

 * *Files identical despite different names*

### Comparing `dhuolib-tools-0.0.4/src/setup.py` & `dhuolib-tools-0.0.5/src/setup.py`

 * *Files identical despite different names*

### Comparing `dhuolib-tools-0.0.4/tests/test_dhuolib.py` & `dhuolib-tools-0.0.5/tests/test_dhuolib.py`

 * *Files identical despite different names*

### Comparing `dhuolib-tools-0.0.4/tests/test_services.py` & `dhuolib-tools-0.0.5/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `dhuolib-tools-0.0.4/tests/test_utils.py` & `dhuolib-tools-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*
