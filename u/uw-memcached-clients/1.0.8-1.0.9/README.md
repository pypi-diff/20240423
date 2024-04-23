# Comparing `tmp/uw-memcached-clients-1.0.8.tar.gz` & `tmp/uw-memcached-clients-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uw-memcached-clients-1.0.8.tar", last modified: Mon Mar 22 19:01:17 2021, max compression
+gzip compressed data, was "uw-memcached-clients-1.0.9.tar", last modified: Mon May  3 23:34:17 2021, max compression
```

## Comparing `uw-memcached-clients-1.0.8.tar` & `uw-memcached-clients-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-22 19:01:17.185544 uw-memcached-clients-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)       72 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      621 2021-03-22 19:01:17.185544 uw-memcached-clients-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1205 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-22 19:01:17.181544 uw-memcached-clients-1.0.8/memcached_clients/
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-03-22 19:01:13.000000 uw-memcached-clients-1.0.8/memcached_clients/VERSION
--rw-r--r--   0 runner    (1001) docker     (116)      223 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1659 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/django_backend.py
--rw-r--r--   0 runner    (1001) docker     (116)     2858 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/restclient.py
--rw-r--r--   0 runner    (1001) docker     (116)      426 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-22 19:01:17.185544 uw-memcached-clients-1.0.8/memcached_clients/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      567 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/tests/django_settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1940 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1298 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/tests/test_django_backend.py
--rw-r--r--   0 runner    (1001) docker     (116)     5523 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/memcached_clients/tests/test_restclient.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-22 19:01:17.185544 uw-memcached-clients-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1156 2021-03-22 19:00:57.000000 uw-memcached-clients-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-22 19:01:17.185544 uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      621 2021-03-22 19:01:15.000000 uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      631 2021-03-22 19:01:17.000000 uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-22 19:01:15.000000 uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2021-03-22 19:01:15.000000 uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2021-03-22 19:01:15.000000 uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-03 23:34:17.946769 uw-memcached-clients-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)       72 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      621 2021-05-03 23:34:17.942769 uw-memcached-clients-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1205 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-03 23:34:17.938769 uw-memcached-clients-1.0.9/memcached_clients/
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2021-05-03 23:34:17.000000 uw-memcached-clients-1.0.9/memcached_clients/VERSION
+-rw-r--r--   0 runner    (1001) docker     (116)      223 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1659 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1135 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/django_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2858 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/restclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)      426 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-03 23:34:17.942769 uw-memcached-clients-1.0.9/memcached_clients/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      567 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/tests/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1940 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1298 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/tests/test_django_backend.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5523 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/memcached_clients/tests/test_restclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-05-03 23:34:17.946769 uw-memcached-clients-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1154 2021-05-03 23:34:10.000000 uw-memcached-clients-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-05-03 23:34:17.942769 uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      621 2021-05-03 23:34:17.000000 uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      631 2021-05-03 23:34:17.000000 uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-05-03 23:34:17.000000 uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       37 2021-05-03 23:34:17.000000 uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2021-05-03 23:34:17.000000 uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/top_level.txt
```

### Comparing `uw-memcached-clients-1.0.8/PKG-INFO` & `uw-memcached-clients-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uw-memcached-clients
-Version: 1.0.8
+Version: 1.0.9
 Summary: Memcached clients
 Home-page: https://github.com/uw-it-aca/uw-memcached-clients
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `uw-memcached-clients-1.0.8/README.md` & `uw-memcached-clients-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/memcached_clients/base.py` & `uw-memcached-clients-1.0.9/memcached_clients/base.py`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/memcached_clients/django_backend.py` & `uw-memcached-clients-1.0.9/memcached_clients/django_backend.py`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/memcached_clients/restclient.py` & `uw-memcached-clients-1.0.9/memcached_clients/restclient.py`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/memcached_clients/tests/django_settings.py` & `uw-memcached-clients-1.0.9/memcached_clients/tests/django_settings.py`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/memcached_clients/tests/test_base.py` & `uw-memcached-clients-1.0.9/memcached_clients/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/memcached_clients/tests/test_django_backend.py` & `uw-memcached-clients-1.0.9/memcached_clients/tests/test_django_backend.py`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/memcached_clients/tests/test_restclient.py` & `uw-memcached-clients-1.0.9/memcached_clients/tests/test_restclient.py`

 * *Files identical despite different names*

### Comparing `uw-memcached-clients-1.0.8/setup.py` & `uw-memcached-clients-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     name='uw-memcached-clients',
     version=VERSION,
     packages=['memcached_clients'],
     author="UW-IT AXDD",
     author_email="aca-it@uw.edu",
     include_package_data=True,
     install_requires=[
-        'pymemcache>=3.4.0',
-        'commonconf~=1.0',
+        'pymemcache~=3.4',
+        'commonconf~=1.1',
         'mock',
     ],
     license='Apache License, Version 2.0',
     description=('Memcached clients'),
     long_description=README,
     url=url,
     classifiers=[
```

### Comparing `uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/PKG-INFO` & `uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uw-memcached-clients
-Version: 1.0.8
+Version: 1.0.9
 Summary: Memcached clients
 Home-page: https://github.com/uw-it-aca/uw-memcached-clients
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `uw-memcached-clients-1.0.8/uw_memcached_clients.egg-info/SOURCES.txt` & `uw-memcached-clients-1.0.9/uw_memcached_clients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

