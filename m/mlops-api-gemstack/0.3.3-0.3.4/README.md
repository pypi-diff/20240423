# Comparing `tmp/mlops_api_gemstack-0.3.3.tar.gz` & `tmp/mlops_api_gemstack-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.3.3.tar", last modified: Mon Apr 22 05:04:59 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.3.4.tar", last modified: Tue Apr 23 13:18:25 2024, max compression
```

## Comparing `mlops_api_gemstack-0.3.3.tar` & `mlops_api_gemstack-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-22 05:04:59.362135 mlops_api_gemstack-0.3.3/
--rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-22 05:04:59.361573 mlops_api_gemstack-0.3.3/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.3.3/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-22 05:04:59.355685 mlops_api_gemstack-0.3.3/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    11792 2024-04-22 03:59:28.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-22 05:04:59.360362 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-22 05:04:59.362357 mlops_api_gemstack-0.3.3/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      622 2024-04-22 05:04:50.000000 mlops_api_gemstack-0.3.3/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-23 13:18:25.800298 mlops_api_gemstack-0.3.4/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     1071 2024-04-22 05:08:20.000000 mlops_api_gemstack-0.3.4/LICENSE
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-23 13:18:25.768538 mlops_api_gemstack-0.3.4/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)     3807 2024-04-23 07:20:14.000000 mlops_api_gemstack-0.3.4/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-23 13:18:25.673971 mlops_api_gemstack-0.3.4/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    11792 2024-04-22 03:59:28.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-23 13:18:25.767519 mlops_api_gemstack-0.3.4/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)     4206 2024-04-23 13:18:25.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      337 2024-04-23 13:18:25.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-23 13:18:25.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-23 13:18:25.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-23 13:18:25.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-23 13:18:25.000000 mlops_api_gemstack-0.3.4/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-23 13:18:25.800993 mlops_api_gemstack-0.3.4/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      770 2024-04-23 13:17:56.000000 mlops_api_gemstack-0.3.4/setup.py
```

### Comparing `mlops_api_gemstack-0.3.3/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.3.4/mlops_api_gemstack/api.py`

 * *Files identical despite different names*

### Comparing `mlops_api_gemstack-0.3.3/setup.py` & `mlops_api_gemstack-0.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r') as f:
+    description = f.read()
+
 setup(
     name='mlops_api_gemstack',
-    version='0.3.3',
+    version='0.3.4',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
@@ -15,9 +18,11 @@
         'urllib3',
         'click'
     ],
     entry_points={
         'console_scripts': [
             'mlops=mlops_api_gemstack:cli'
         ]
-    }
+    },
+    long_description=description,
+    long_description_content_type='text/markdown',
 )
```

