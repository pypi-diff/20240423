# Comparing `tmp/db-conn-lib-0.1.0.tar.gz` & `tmp/db_conn_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db-conn-lib-0.1.0.tar", last modified: Tue Apr 23 10:55:30 2024, max compression
+gzip compressed data, was "db_conn_lib-0.1.1.tar", last modified: Tue Apr 23 11:14:03 2024, max compression
```

## Comparing `db-conn-lib-0.1.0.tar` & `db_conn_lib-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 10:55:30.397009 db-conn-lib-0.1.0/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 10:55:30.397009 db-conn-lib-0.1.0/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2024-04-23 10:42:17.000000 db-conn-lib-0.1.0/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 10:55:30.393009 db-conn-lib-0.1.0/db_conn_lib.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 10:55:30.000000 db-conn-lib-0.1.0/db_conn_lib.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      192 2024-04-23 10:55:30.000000 db-conn-lib-0.1.0/db_conn_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 10:55:30.000000 db-conn-lib-0.1.0/db_conn_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        7 2024-04-23 10:55:30.000000 db-conn-lib-0.1.0/db_conn_lib.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 10:55:30.000000 db-conn-lib-0.1.0/db_conn_lib.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2024-04-23 10:55:30.397009 db-conn-lib-0.1.0/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      648 2024-04-23 10:50:27.000000 db-conn-lib-0.1.0/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 11:14:03.989508 db_conn_lib-0.1.1/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 11:14:03.989508 db_conn_lib-0.1.1/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2024-04-23 10:42:17.000000 db_conn_lib-0.1.1/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 11:14:03.989508 db_conn_lib-0.1.1/db_conn_lib.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 11:14:03.000000 db_conn_lib-0.1.1/db_conn_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      192 2024-04-23 11:14:03.000000 db_conn_lib-0.1.1/db_conn_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 11:14:03.000000 db_conn_lib-0.1.1/db_conn_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        7 2024-04-23 11:14:03.000000 db_conn_lib-0.1.1/db_conn_lib.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 11:14:03.000000 db_conn_lib-0.1.1/db_conn_lib.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2024-04-23 11:14:03.989508 db_conn_lib-0.1.1/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      648 2024-04-23 11:13:05.000000 db_conn_lib-0.1.1/setup.py
```

### Comparing `db-conn-lib-0.1.0/setup.py` & `db_conn_lib-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='db-conn-lib',
-    version='0.1.0',
+    name='db_conn_lib',
+    version='0.1.1',
     author='Kogui',
     description='Uma biblioteca de conexão de teste',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/lucasaarrudaa/lib-repo-test',  
     packages=find_packages(),
     install_requires=[
```

