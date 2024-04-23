# Comparing `tmp/brightspacepyclient-0.0.1.tar.gz` & `tmp/brightspacepyclient-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightspacepyclient-0.0.1.tar", last modified: Mon Apr 22 23:24:58 2024, max compression
+gzip compressed data, was "brightspacepyclient-0.0.2.tar", last modified: Tue Apr 23 21:12:07 2024, max compression
```

## Comparing `brightspacepyclient-0.0.1.tar` & `brightspacepyclient-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-22 23:24:58.479666 brightspacepyclient-0.0.1/
--rw-r--r--   0 jad        (501) staff       (20)      476 2024-04-22 23:24:58.479530 brightspacepyclient-0.0.1/PKG-INFO
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-22 23:24:58.477258 brightspacepyclient-0.0.1/brightspace-py-client/
--rw-r--r--   0 jad        (501) staff       (20)       47 2024-04-22 23:18:16.000000 brightspacepyclient-0.0.1/brightspace-py-client/__init__.py
--rw-r--r--   0 jad        (501) staff       (20)     1775 2024-04-22 23:10:55.000000 brightspacepyclient-0.0.1/brightspace-py-client/brightspaceclient.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-22 23:24:58.477409 brightspacepyclient-0.0.1/brightspace-py-client/src/
--rw-r--r--   0 jad        (501) staff       (20)        0 2024-04-22 22:10:28.000000 brightspacepyclient-0.0.1/brightspace-py-client/src/__init__.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-22 23:24:58.477799 brightspacepyclient-0.0.1/brightspace-py-client/src/decorators/
--rw-r--r--   0 jad        (501) staff       (20)       30 2024-04-22 22:08:44.000000 brightspacepyclient-0.0.1/brightspace-py-client/src/decorators/__init__.py
--rw-r--r--   0 jad        (501) staff       (20)      320 2024-04-22 23:12:57.000000 brightspacepyclient-0.0.1/brightspace-py-client/src/decorators/decorators.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-22 23:24:58.478242 brightspacepyclient-0.0.1/brightspace-py-client/src/models/
--rw-r--r--   0 jad        (501) staff       (20)      580 2024-04-22 22:58:03.000000 brightspacepyclient-0.0.1/brightspace-py-client/src/models/Response.py
--rw-r--r--   0 jad        (501) staff       (20)        0 2024-04-21 18:28:30.000000 brightspacepyclient-0.0.1/brightspace-py-client/src/models/__init__.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-22 23:24:58.478618 brightspacepyclient-0.0.1/brightspace-py-client/src/utils/
--rw-r--r--   0 jad        (501) staff       (20)       51 2024-04-22 22:11:31.000000 brightspacepyclient-0.0.1/brightspace-py-client/src/utils/__init__.py
--rw-r--r--   0 jad        (501) staff       (20)      412 2024-04-22 22:13:27.000000 brightspacepyclient-0.0.1/brightspace-py-client/src/utils/requestswrapper.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-22 23:24:58.479356 brightspacepyclient-0.0.1/brightspacepyclient.egg-info/
--rw-r--r--   0 jad        (501) staff       (20)      476 2024-04-22 23:24:58.000000 brightspacepyclient-0.0.1/brightspacepyclient.egg-info/PKG-INFO
--rw-r--r--   0 jad        (501) staff       (20)      622 2024-04-22 23:24:58.000000 brightspacepyclient-0.0.1/brightspacepyclient.egg-info/SOURCES.txt
--rw-r--r--   0 jad        (501) staff       (20)        1 2024-04-22 23:24:58.000000 brightspacepyclient-0.0.1/brightspacepyclient.egg-info/dependency_links.txt
--rw-r--r--   0 jad        (501) staff       (20)        9 2024-04-22 23:24:58.000000 brightspacepyclient-0.0.1/brightspacepyclient.egg-info/requires.txt
--rw-r--r--   0 jad        (501) staff       (20)       22 2024-04-22 23:24:58.000000 brightspacepyclient-0.0.1/brightspacepyclient.egg-info/top_level.txt
--rw-r--r--   0 jad        (501) staff       (20)       38 2024-04-22 23:24:58.479713 brightspacepyclient-0.0.1/setup.cfg
--rw-r--r--   0 jad        (501) staff       (20)      680 2024-04-22 23:22:38.000000 brightspacepyclient-0.0.1/setup.py
+drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:12:07.531421 brightspacepyclient-0.0.2/
+-rw-r--r--   0 jad        (501) staff       (20)      476 2024-04-23 21:12:07.531309 brightspacepyclient-0.0.2/PKG-INFO
+drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:12:07.529805 brightspacepyclient-0.0.2/brightspace-py-client/
+-rw-r--r--   0 jad        (501) staff       (20)       48 2024-04-23 21:01:36.000000 brightspacepyclient-0.0.2/brightspace-py-client/__init__.py
+-rw-r--r--   0 jad        (501) staff       (20)     1775 2024-04-23 21:05:40.000000 brightspacepyclient-0.0.2/brightspace-py-client/brightspaceclient.py
+drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:12:07.529920 brightspacepyclient-0.0.2/brightspace-py-client/src/
+-rw-r--r--   0 jad        (501) staff       (20)        0 2024-04-22 22:10:28.000000 brightspacepyclient-0.0.2/brightspace-py-client/src/__init__.py
+drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:12:07.530124 brightspacepyclient-0.0.2/brightspace-py-client/src/decorators/
+-rw-r--r--   0 jad        (501) staff       (20)       30 2024-04-22 22:08:44.000000 brightspacepyclient-0.0.2/brightspace-py-client/src/decorators/__init__.py
+-rw-r--r--   0 jad        (501) staff       (20)      320 2024-04-22 23:12:57.000000 brightspacepyclient-0.0.2/brightspace-py-client/src/decorators/decorators.py
+drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:12:07.530349 brightspacepyclient-0.0.2/brightspace-py-client/src/models/
+-rw-r--r--   0 jad        (501) staff       (20)      580 2024-04-22 22:58:03.000000 brightspacepyclient-0.0.2/brightspace-py-client/src/models/Response.py
+-rw-r--r--   0 jad        (501) staff       (20)        0 2024-04-21 18:28:30.000000 brightspacepyclient-0.0.2/brightspace-py-client/src/models/__init__.py
+drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:12:07.530584 brightspacepyclient-0.0.2/brightspace-py-client/src/utils/
+-rw-r--r--   0 jad        (501) staff       (20)       51 2024-04-22 22:11:31.000000 brightspacepyclient-0.0.2/brightspace-py-client/src/utils/__init__.py
+-rw-r--r--   0 jad        (501) staff       (20)      412 2024-04-22 22:13:27.000000 brightspacepyclient-0.0.2/brightspace-py-client/src/utils/requestswrapper.py
+drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:12:07.531157 brightspacepyclient-0.0.2/brightspacepyclient.egg-info/
+-rw-r--r--   0 jad        (501) staff       (20)      476 2024-04-23 21:12:07.000000 brightspacepyclient-0.0.2/brightspacepyclient.egg-info/PKG-INFO
+-rw-r--r--   0 jad        (501) staff       (20)      622 2024-04-23 21:12:07.000000 brightspacepyclient-0.0.2/brightspacepyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 jad        (501) staff       (20)        1 2024-04-23 21:12:07.000000 brightspacepyclient-0.0.2/brightspacepyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 jad        (501) staff       (20)        9 2024-04-23 21:12:07.000000 brightspacepyclient-0.0.2/brightspacepyclient.egg-info/requires.txt
+-rw-r--r--   0 jad        (501) staff       (20)       22 2024-04-23 21:12:07.000000 brightspacepyclient-0.0.2/brightspacepyclient.egg-info/top_level.txt
+-rw-r--r--   0 jad        (501) staff       (20)       38 2024-04-23 21:12:07.531462 brightspacepyclient-0.0.2/setup.cfg
+-rw-r--r--   0 jad        (501) staff       (20)      680 2024-04-23 21:04:32.000000 brightspacepyclient-0.0.2/setup.py
```

### Comparing `brightspacepyclient-0.0.1/brightspace-py-client/brightspaceclient.py` & `brightspacepyclient-0.0.2/brightspace-py-client/brightspaceclient.py`

 * *Files identical despite different names*

### Comparing `brightspacepyclient-0.0.1/brightspace-py-client/src/models/Response.py` & `brightspacepyclient-0.0.2/brightspace-py-client/src/models/Response.py`

 * *Files identical despite different names*

### Comparing `brightspacepyclient-0.0.1/brightspacepyclient.egg-info/SOURCES.txt` & `brightspacepyclient-0.0.2/brightspacepyclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightspacepyclient-0.0.1/setup.py` & `brightspacepyclient-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python API Client for BrightSpace'
 
 setup(
     name="brightspacepyclient",
     version=VERSION,
     author="CourseCompanion",
     author_email="admin@coursecompanion.ai",
```

