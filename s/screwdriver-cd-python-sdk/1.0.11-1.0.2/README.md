# Comparing `tmp/screwdriver-cd-python-sdk-1.0.11.tar.gz` & `tmp/screwdriver-cd-python-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screwdriver-cd-python-sdk-1.0.11.tar", last modified: Tue Apr 23 06:54:03 2024, max compression
+gzip compressed data, was "screwdriver-cd-python-sdk-1.0.2.tar", last modified: Mon Apr 22 05:04:15 2024, max compression
```

## Comparing `screwdriver-cd-python-sdk-1.0.11.tar` & `screwdriver-cd-python-sdk-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:54:03.428988 screwdriver-cd-python-sdk-1.0.11/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 06:54:03.428988 screwdriver-cd-python-sdk-1.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:54:03.428988 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/screwdriver_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:54:03.428988 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 06:54:03.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 06:54:03.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:54:03.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:54:03.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 06:54:03.000000 screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 06:54:03.428988 screwdriver-cd-python-sdk-1.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 06:53:57.000000 screwdriver-cd-python-sdk-1.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:04:15.231892 screwdriver-cd-python-sdk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 05:04:15.235892 screwdriver-cd-python-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:04:15.231892 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/screwdriver_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:04:15.231892 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 05:04:15.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-22 05:04:15.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:04:15.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:04:15.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 05:04:15.000000 screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 05:04:15.235892 screwdriver-cd-python-sdk-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-22 05:04:09.000000 screwdriver-cd-python-sdk-1.0.2/setup.py
```

### Comparing `screwdriver-cd-python-sdk-1.0.11/LICENSE` & `screwdriver-cd-python-sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-1.0.11/README.md` & `screwdriver-cd-python-sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/events.py` & `screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/events.py`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/pipeline.py` & `screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/pipeline.py`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-1.0.11/screwdriver_cd_python_sdk/secrets.py` & `screwdriver-cd-python-sdk-1.0.2/screwdriver_cd_python_sdk/secrets.py`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-1.0.11/setup.py` & `screwdriver-cd-python-sdk-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="screwdriver-cd-python-sdk",
-    version="1.0.11",
+    version="1.0.2",
     description="Screwdriver CD Python Software Development Kit (SDK) for managing resources in Screwdriver",
     url="https://github.com/QubitPi/screwdriver-cd-python-sdk",
     author="Jiaqi liu",
     author_email="jack20220723@gmail.com",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

