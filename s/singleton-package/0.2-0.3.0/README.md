# Comparing `tmp/singleton_package-0.2.tar.gz` & `tmp/singleton_package-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singleton_package-0.2.tar", last modified: Tue Apr  9 14:18:42 2024, max compression
+gzip compressed data, was "singleton_package-0.3.0.tar", last modified: Tue Apr 23 15:31:19 2024, max compression
```

## Comparing `singleton_package-0.2.tar` & `singleton_package-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-09 14:18:42.157890 singleton_package-0.2/
--rw-r--r--   0 ali       (1001) ali       (1001)     1324 2024-04-09 14:18:42.157890 singleton_package-0.2/PKG-INFO
--rw-rw-r--   0 ali       (1001) ali       (1001)     1015 2024-04-09 13:55:12.000000 singleton_package-0.2/README.md
--rw-rw-r--   0 ali       (1001) ali       (1001)       38 2024-04-09 14:18:42.157890 singleton_package-0.2/setup.cfg
--rw-rw-r--   0 ali       (1001) ali       (1001)      926 2024-04-09 14:18:39.000000 singleton_package-0.2/setup.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-09 14:18:42.149889 singleton_package-0.2/singleton/
--rw-rw-r--   0 ali       (1001) ali       (1001)       47 2024-04-09 14:15:36.000000 singleton_package-0.2/singleton/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)      311 2024-04-09 13:48:51.000000 singleton_package-0.2/singleton/singleton.py
--rw-rw-r--   0 ali       (1001) ali       (1001)      568 2024-04-09 14:14:34.000000 singleton_package-0.2/singleton/test.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-09 14:18:42.157890 singleton_package-0.2/singleton_package.egg-info/
--rw-r--r--   0 ali       (1001) ali       (1001)     1324 2024-04-09 14:18:41.000000 singleton_package-0.2/singleton_package.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1001) ali       (1001)      285 2024-04-09 14:18:41.000000 singleton_package-0.2/singleton_package.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-09 14:18:41.000000 singleton_package-0.2/singleton_package.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-09 14:18:41.000000 singleton_package-0.2/singleton_package.egg-info/not-zip-safe
--rw-rw-r--   0 ali       (1001) ali       (1001)       10 2024-04-09 14:18:41.000000 singleton_package-0.2/singleton_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:31:19.199177 singleton_package-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 15:31:19.199177 singleton_package-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-23 15:31:15.000000 singleton_package-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:31:19.199177 singleton_package-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-23 15:31:15.000000 singleton_package-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:31:19.195177 singleton_package-0.3.0/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 15:31:15.000000 singleton_package-0.3.0/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 15:31:15.000000 singleton_package-0.3.0/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-23 15:31:15.000000 singleton_package-0.3.0/singleton/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:31:19.199177 singleton_package-0.3.0/singleton_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 15:31:19.000000 singleton_package-0.3.0/singleton_package.egg-info/top_level.txt
```

### Comparing `singleton_package-0.2/PKG-INFO` & `singleton_package-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton_package
-Version: 0.2
+Version: 0.3.0
 Summary: A simple Python package to create singleton objects
 Home-page: https://github.com/mahdikiani/singleton_package
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `singleton_package-0.2/README.md` & `singleton_package-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `singleton_package-0.2/setup.py` & `singleton_package-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `singleton_package-0.2/singleton/test.py` & `singleton_package-0.3.0/singleton/test.py`

 * *Files identical despite different names*

### Comparing `singleton_package-0.2/singleton_package.egg-info/PKG-INFO` & `singleton_package-0.3.0/singleton_package.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singleton_package
-Version: 0.2
+Version: 0.3.0
 Summary: A simple Python package to create singleton objects
 Home-page: https://github.com/mahdikiani/singleton_package
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

