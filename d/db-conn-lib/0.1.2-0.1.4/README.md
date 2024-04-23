# Comparing `tmp/db_conn_lib-0.1.2.tar.gz` & `tmp/db_conn_lib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_conn_lib-0.1.2.tar", last modified: Tue Apr 23 11:25:09 2024, max compression
+gzip compressed data, was "db_conn_lib-0.1.4.tar", last modified: Tue Apr 23 11:34:23 2024, max compression
```

## Comparing `db_conn_lib-0.1.2.tar` & `db_conn_lib-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 11:25:09.951257 db_conn_lib-0.1.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 11:25:09.951257 db_conn_lib-0.1.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2024-04-23 10:42:17.000000 db_conn_lib-0.1.2/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 11:25:09.951257 db_conn_lib-0.1.2/db_conn_lib.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 11:25:09.000000 db_conn_lib-0.1.2/db_conn_lib.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      192 2024-04-23 11:25:09.000000 db_conn_lib-0.1.2/db_conn_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 11:25:09.000000 db_conn_lib-0.1.2/db_conn_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        7 2024-04-23 11:25:09.000000 db_conn_lib-0.1.2/db_conn_lib.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 11:25:09.000000 db_conn_lib-0.1.2/db_conn_lib.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2024-04-23 11:25:09.951257 db_conn_lib-0.1.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      648 2024-04-23 11:24:46.000000 db_conn_lib-0.1.2/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 11:34:23.382376 db_conn_lib-0.1.4/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 11:34:23.382376 db_conn_lib-0.1.4/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2024-04-23 10:42:17.000000 db_conn_lib-0.1.4/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-04-23 11:34:23.382376 db_conn_lib-0.1.4/db_conn_lib.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      375 2024-04-23 11:34:23.000000 db_conn_lib-0.1.4/db_conn_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      192 2024-04-23 11:34:23.000000 db_conn_lib-0.1.4/db_conn_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 11:34:23.000000 db_conn_lib-0.1.4/db_conn_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        7 2024-04-23 11:34:23.000000 db_conn_lib-0.1.4/db_conn_lib.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-04-23 11:34:23.000000 db_conn_lib-0.1.4/db_conn_lib.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2024-04-23 11:34:23.382376 db_conn_lib-0.1.4/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      647 2024-04-23 11:33:47.000000 db_conn_lib-0.1.4/setup.py
```

### Comparing `db_conn_lib-0.1.2/setup.py` & `db_conn_lib-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='db_conn_lib',
-    version='0.1.2',
+    version='0.1.4',
     author='Kogui',
     description='Uma biblioteca de conexão de teste',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/lucasaarrudaa/lib-repo-test',  
     packages=find_packages(),
     install_requires=[
         'pyodbc',
     ],
     python_requires='>=3.6',  
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-)
+)
```

