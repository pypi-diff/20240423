# Comparing `tmp/wdl-lsp-0.0.88.tar.gz` & `tmp/wdl-lsp-0.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdl-lsp-0.0.88.tar", last modified: Mon Apr 22 22:45:00 2024, max compression
+gzip compressed data, was "wdl-lsp-0.0.89.tar", last modified: Tue Apr 23 15:56:58 2024, max compression
```

## Comparing `wdl-lsp-0.0.88.tar` & `wdl-lsp-0.0.89.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:45:00.388397 wdl-lsp-0.0.88/
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-22 22:45:00.388397 wdl-lsp-0.0.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:45:00.388397 wdl-lsp-0.0.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:45:00.384397 wdl-lsp-0.0.88/wdl_lsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/wdl_lsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/wdl_lsp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/wdl_lsp/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:45:00.388397 wdl-lsp-0.0.88/wdl_lsp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/wdl_lsp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:45:00.388397 wdl-lsp-0.0.88/wdl_lsp/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/wdl_lsp/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-22 22:44:54.000000 wdl-lsp-0.0.88/wdl_lsp/tests/unit/test_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:45:00.388397 wdl-lsp-0.0.88/wdl_lsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-22 22:45:00.000000 wdl-lsp-0.0.88/wdl_lsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-22 22:45:00.000000 wdl-lsp-0.0.88/wdl_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:45:00.000000 wdl-lsp-0.0.88/wdl_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 22:45:00.000000 wdl-lsp-0.0.88/wdl_lsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 22:45:00.000000 wdl-lsp-0.0.88/wdl_lsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 22:45:00.000000 wdl-lsp-0.0.88/wdl_lsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:56:58.203127 wdl-lsp-0.0.89/
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-23 15:56:58.203127 wdl-lsp-0.0.89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:56:58.203127 wdl-lsp-0.0.89/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:56:58.203127 wdl-lsp-0.0.89/wdl_lsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/wdl_lsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/wdl_lsp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/wdl_lsp/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:56:58.203127 wdl-lsp-0.0.89/wdl_lsp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/wdl_lsp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:56:58.203127 wdl-lsp-0.0.89/wdl_lsp/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/wdl_lsp/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 15:56:53.000000 wdl-lsp-0.0.89/wdl_lsp/tests/unit/test_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:56:58.203127 wdl-lsp-0.0.89/wdl_lsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-23 15:56:58.000000 wdl-lsp-0.0.89/wdl_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-23 15:56:58.000000 wdl-lsp-0.0.89/wdl_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:56:58.000000 wdl-lsp-0.0.89/wdl_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 15:56:58.000000 wdl-lsp-0.0.89/wdl_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 15:56:58.000000 wdl-lsp-0.0.89/wdl_lsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 15:56:58.000000 wdl-lsp-0.0.89/wdl_lsp.egg-info/top_level.txt
```

### Comparing `wdl-lsp-0.0.88/PKG-INFO` & `wdl-lsp-0.0.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdl-lsp
-Version: 0.0.88
+Version: 0.0.89
 Summary: Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)
 Home-page: https://github.com/broadinstitute/wdl-ide
 Author: Broad Institute
 License: BSD 3-clause "New" or "Revised" License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Interpreters
```

### Comparing `wdl-lsp-0.0.88/README.md` & `wdl-lsp-0.0.89/README.md`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/setup.py` & `wdl-lsp-0.0.89/setup.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/wdl_lsp/__init__.py` & `wdl-lsp-0.0.89/wdl_lsp/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/wdl_lsp/__main__.py` & `wdl-lsp-0.0.89/wdl_lsp/__main__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/wdl_lsp/server.py` & `wdl-lsp-0.0.89/wdl_lsp/server.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/wdl_lsp/tests/__init__.py` & `wdl-lsp-0.0.89/wdl_lsp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/wdl_lsp/tests/unit/__init__.py` & `wdl-lsp-0.0.89/wdl_lsp/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/wdl_lsp/tests/unit/test_features.py` & `wdl-lsp-0.0.89/wdl_lsp/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.88/wdl_lsp.egg-info/PKG-INFO` & `wdl-lsp-0.0.89/wdl_lsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdl-lsp
-Version: 0.0.88
+Version: 0.0.89
 Summary: Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)
 Home-page: https://github.com/broadinstitute/wdl-ide
 Author: Broad Institute
 License: BSD 3-clause "New" or "Revised" License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Interpreters
```

