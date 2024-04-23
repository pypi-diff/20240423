# Comparing `tmp/nrstitcher_utils-0.1.0.dev0.tar.gz` & `tmp/nrstitcher_utils-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrstitcher_utils-0.1.0.dev0.tar", last modified: Mon Apr 22 14:45:53 2024, max compression
+gzip compressed data, was "nrstitcher_utils-0.1.0.dev1.tar", last modified: Tue Apr 23 06:38:05 2024, max compression
```

## Comparing `nrstitcher_utils-0.1.0.dev0.tar` & `nrstitcher_utils-0.1.0.dev1.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-22 14:45:53.659837 nrstitcher_utils-0.1.0.dev0/
--rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-22 13:12:35.000000 nrstitcher_utils-0.1.0.dev0/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3855 2024-04-22 14:45:53.659837 nrstitcher_utils-0.1.0.dev0/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      494 2024-04-22 14:12:35.000000 nrstitcher_utils-0.1.0.dev0/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     2113 2024-04-22 13:33:00.000000 nrstitcher_utils-0.1.0.dev0/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-22 14:45:53.659837 nrstitcher_utils-0.1.0.dev0/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       37 2024-04-22 13:02:47.000000 nrstitcher_utils-0.1.0.dev0/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-22 14:45:53.659837 nrstitcher_utils-0.1.0.dev0/src/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-22 14:45:53.659837 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-22 12:54:51.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-22 14:45:53.659837 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-22 13:26:01.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils/app/__init__.py
--rwxr-xr-x   0 payno     (1000) payno     (1000)    22370 2024-04-22 14:08:40.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils/app/nrs_config.py
--rw-r--r--   0 payno     (1000) payno     (1000)       44 2024-04-22 13:10:52.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-22 14:45:53.659837 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3855 2024-04-22 14:45:53.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      448 2024-04-22 14:45:53.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-22 14:45:53.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       68 2024-04-22 14:45:53.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-22 14:45:53.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-22 14:45:53.000000 nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-23 06:24:16.000000 nrstitcher_utils-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:19:33.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/app/__init__.py
+-rwxr-xr-x   0 payno     (1000) payno     (1000)     7807 2024-04-23 06:35:42.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.499125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-23 06:24:31.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3110 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/h5_settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8604 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/ht_vol.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3430 2024-04-23 06:34:32.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/core/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-23 06:37:53.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-23 06:38:05.503125 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      607 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-23 06:38:05.000000 nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/top_level.txt
```

### Comparing `nrstitcher_utils-0.1.0.dev0/LICENSE` & `nrstitcher_utils-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev0/PKG-INFO` & `nrstitcher_utils-0.1.0.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
         
@@ -71,17 +71,7 @@
 The goal of this project is to ease usage of ![NRSticher program](https://pi2-docs.readthedocs.io/en/latest/nr_stitcher.html) with esrf datasets
 
 ## how to access it from esrf infrascture
 
 ``` bash
 module load nrstitcher_utils
 ```
-
-## how to use
-
-Create a configuration file from the `nrs_config` application
-
-``` bash
-module load nrstitcher_utils
-```
-
-Then you can call `nr_stitcher.py` from ![NRSticher program](https://pi2-docs.readthedocs.io/en/latest/nr_stitcher.html)
```

### Comparing `nrstitcher_utils-0.1.0.dev0/pyproject.toml` & `nrstitcher_utils-0.1.0.dev1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     "nbconvert",
     "pandoc",
     "sphinx_autodoc_typehints",
     "pydata_sphinx_theme",
 ]
 
 [project.scripts]
-nrs-config = "nrstitcher_utils.app.nrs_config:main"
+nrs-config-id16a-ht = "nrstitcher_utils.app.nrs_config_id16a_ht:main"
 
 [build_sphinx]
 source_dir = "doc"
 build_dir = "build/sphinx"
 
 [tool.setuptools.dynamic]
 version = {attr = "nrstitcher_utils.version.version"}
```

### Comparing `nrstitcher_utils-0.1.0.dev0/src/nrstitcher_utils.egg-info/PKG-INFO` & `nrstitcher_utils-0.1.0.dev1/src/nrstitcher_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
         
@@ -71,17 +71,7 @@
 The goal of this project is to ease usage of ![NRSticher program](https://pi2-docs.readthedocs.io/en/latest/nr_stitcher.html) with esrf datasets
 
 ## how to access it from esrf infrascture
 
 ``` bash
 module load nrstitcher_utils
 ```
-
-## how to use
-
-Create a configuration file from the `nrs_config` application
-
-``` bash
-module load nrstitcher_utils
-```
-
-Then you can call `nr_stitcher.py` from ![NRSticher program](https://pi2-docs.readthedocs.io/en/latest/nr_stitcher.html)
```

