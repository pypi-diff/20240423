# Comparing `tmp/keploy-2.0.0a8.tar.gz` & `tmp/keploy-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keploy-2.0.0a8.tar", last modified: Wed Feb 21 12:04:58 2024, max compression
+gzip compressed data, was "keploy-2.0.0a9.tar", last modified: Wed Feb 21 12:13:41 2024, max compression
```

## Comparing `keploy-2.0.0a8.tar` & `keploy-2.0.0a9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 pranshu    (501) pranshu   (1000)        0 2024-02-21 12:04:58.977656 keploy-2.0.0a8/
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)    11340 2024-02-15 09:06:51.000000 keploy-2.0.0a8/LICENSE
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)      688 2024-02-21 12:04:58.977656 keploy-2.0.0a8/PKG-INFO
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)      765 2024-02-15 09:06:51.000000 keploy-2.0.0a8/README.md
-drwxrwxr-x   0 pranshu    (501) pranshu   (1000)        0 2024-02-21 12:04:58.977656 keploy-2.0.0a8/keploy.egg-info/
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)      688 2024-02-21 12:04:58.000000 keploy-2.0.0a8/keploy.egg-info/PKG-INFO
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)      156 2024-02-21 12:04:58.000000 keploy-2.0.0a8/keploy.egg-info/SOURCES.txt
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)        1 2024-02-21 12:04:58.000000 keploy-2.0.0a8/keploy.egg-info/dependency_links.txt
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)        7 2024-02-21 12:04:58.000000 keploy-2.0.0a8/keploy.egg-info/top_level.txt
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)     6371 2024-02-21 11:32:03.000000 keploy-2.0.0a8/keploy.py
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)       38 2024-02-21 12:04:58.977656 keploy-2.0.0a8/setup.cfg
--rw-rw-r--   0 pranshu    (501) pranshu   (1000)     1037 2024-02-21 12:04:38.000000 keploy-2.0.0a8/setup.py
+drwxrwxr-x   0 pranshu    (501) pranshu   (1000)        0 2024-02-21 12:13:41.462995 keploy-2.0.0a9/
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)    11340 2024-02-15 09:06:51.000000 keploy-2.0.0a9/LICENSE
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)      688 2024-02-21 12:13:41.462995 keploy-2.0.0a9/PKG-INFO
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)      765 2024-02-15 09:06:51.000000 keploy-2.0.0a9/README.md
+drwxrwxr-x   0 pranshu    (501) pranshu   (1000)        0 2024-02-21 12:13:41.462995 keploy-2.0.0a9/keploy.egg-info/
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)      688 2024-02-21 12:13:41.000000 keploy-2.0.0a9/keploy.egg-info/PKG-INFO
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)      156 2024-02-21 12:13:41.000000 keploy-2.0.0a9/keploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)        1 2024-02-21 12:13:41.000000 keploy-2.0.0a9/keploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)        1 2024-02-21 12:13:41.000000 keploy-2.0.0a9/keploy.egg-info/top_level.txt
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)     6371 2024-02-21 11:32:03.000000 keploy-2.0.0a9/keploy.py
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)       38 2024-02-21 12:13:41.462995 keploy-2.0.0a9/setup.cfg
+-rw-rw-r--   0 pranshu    (501) pranshu   (1000)     1006 2024-02-21 12:13:33.000000 keploy-2.0.0a9/setup.py
```

### Comparing `keploy-2.0.0a8/LICENSE` & `keploy-2.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `keploy-2.0.0a8/PKG-INFO` & `keploy-2.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keploy
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: Run your unit tests with Keploy
 Home-page: UNKNOWN
 Author: Keploy Inc.
 Author-email: hello@keploy.io
 License: UNKNOWN
 Keywords: keploy,python,sdk
 Platform: UNKNOWN
```

### Comparing `keploy-2.0.0a8/README.md` & `keploy-2.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `keploy-2.0.0a8/keploy.egg-info/PKG-INFO` & `keploy-2.0.0a9/keploy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keploy
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: Run your unit tests with Keploy
 Home-page: UNKNOWN
 Author: Keploy Inc.
 Author-email: hello@keploy.io
 License: UNKNOWN
 Keywords: keploy,python,sdk
 Platform: UNKNOWN
```

### Comparing `keploy-2.0.0a8/keploy.py` & `keploy-2.0.0a9/keploy.py`

 * *Files identical despite different names*

### Comparing `keploy-2.0.0a8/setup.py` & `keploy-2.0.0a9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.0.0-alpha8'
+VERSION = '2.0.0-alpha9'
 DESCRIPTION = 'Keploy'
 LONG_DESCRIPTION = 'Keploy Python SDK'
 
 # Setting up
 setup(
         name="keploy",
         version=VERSION,
         author="Keploy Inc.",
         author_email="hello@keploy.io",
         description="Run your unit tests with Keploy",
         long_description="This module allows you to run your unit tests along with pytest and get coverage for the same using Keploy",
-        py_modules=['keploy'],
         install_requires=[], # add any additional packages that needs to be installed along with your package.
 
         keywords=['keploy', 'python', 'sdk'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
```

