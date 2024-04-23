# Comparing `tmp/qtapputils-0.5.1.tar.gz` & `tmp/qtapputils-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtapputils-0.5.1.tar", last modified: Fri Mar 22 17:33:34 2024, max compression
+gzip compressed data, was "qtapputils-0.5.2.tar", last modified: Tue Apr 23 13:24:55 2024, max compression
```

## Comparing `qtapputils-0.5.1.tar` & `qtapputils-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.139158 qtapputils-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-22 17:33:25.000000 qtapputils-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-22 17:33:34.139158 qtapputils-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-22 17:33:25.000000 qtapputils-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.135158 qtapputils-0.5.1/qtapputils/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/icons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.135158 qtapputils-0.5.1/qtapputils/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/managers/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7841 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/managers/taskmanagers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.135158 qtapputils-0.5.1/qtapputils/managers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/managers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/managers/tests/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/managers/tests/test_taskmanagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/qthelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.135158 qtapputils-0.5.1/qtapputils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/tests/test_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/tests/test_qthelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.135158 qtapputils-0.5.1/qtapputils/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/widgets/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/widgets/range.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.135158 qtapputils-0.5.1/qtapputils/widgets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/widgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/widgets/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/widgets/tests/test_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-03-22 17:33:25.000000 qtapputils-0.5.1/qtapputils/widgets/waitingspinner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:33:34.135158 qtapputils-0.5.1/qtapputils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-22 17:33:34.000000 qtapputils-0.5.1/qtapputils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-22 17:33:34.000000 qtapputils-0.5.1/qtapputils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:33:34.000000 qtapputils-0.5.1/qtapputils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 17:33:34.000000 qtapputils-0.5.1/qtapputils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 17:33:34.000000 qtapputils-0.5.1/qtapputils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 17:33:34.139158 qtapputils-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-22 17:33:25.000000 qtapputils-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.023975 qtapputils-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 13:24:48.000000 qtapputils-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-23 13:24:55.023975 qtapputils-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-23 13:24:48.000000 qtapputils-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.019975 qtapputils-0.5.2/qtapputils/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/icons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.019975 qtapputils-0.5.2/qtapputils/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/managers/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7841 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/managers/taskmanagers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.019975 qtapputils-0.5.2/qtapputils/managers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/managers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/managers/tests/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/managers/tests/test_taskmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/qthelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.019975 qtapputils-0.5.2/qtapputils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/tests/test_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/tests/test_qthelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.023975 qtapputils-0.5.2/qtapputils/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/splash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.023975 qtapputils-0.5.2/qtapputils/widgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/tests/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/tests/test_splash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-23 13:24:48.000000 qtapputils-0.5.2/qtapputils/widgets/waitingspinner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:24:55.023975 qtapputils-0.5.2/qtapputils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-23 13:24:55.000000 qtapputils-0.5.2/qtapputils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-23 13:24:55.000000 qtapputils-0.5.2/qtapputils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:24:55.000000 qtapputils-0.5.2/qtapputils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 13:24:55.000000 qtapputils-0.5.2/qtapputils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 13:24:55.000000 qtapputils-0.5.2/qtapputils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:24:55.023975 qtapputils-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-23 13:24:48.000000 qtapputils-0.5.2/setup.py
```

### Comparing `qtapputils-0.5.1/LICENSE` & `qtapputils-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/PKG-INFO` & `qtapputils-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtapputils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utilities for building Qt applications in Python.
 Home-page: https://github.com/jnsebgosselin/qtapputils
 Author: Jean-Sébastien Gosselin
 Author-email: jean-sebastien.gosselin@outlook.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtapputils-0.5.1/README.md` & `qtapputils-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/__init__.py` & `qtapputils-0.5.2/qtapputils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 # Copyright © QtAppUtils Project Contributors
 # https://github.com/jnsebgosselin/apputils
 #
 # This file is part of QtAppUtils.
 # Licensed under the terms of the MIT License.
 # -----------------------------------------------------------------------------
 
-version_info = (0, 5, 1)
+version_info = (0, 5, 2)
 __version__ = '.'.join(map(str, version_info))
-__date__ = '22/03/2024'
+__date__ = '23/04/2024'
 __project_url__ = "https://github.com/jnsebgosselin/qtapputils"
```

### Comparing `qtapputils-0.5.1/qtapputils/colors.py` & `qtapputils-0.5.2/qtapputils/colors.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/icons.py` & `qtapputils-0.5.2/qtapputils/icons.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/managers/fileio.py` & `qtapputils-0.5.2/qtapputils/managers/fileio.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/managers/taskmanagers.py` & `qtapputils-0.5.2/qtapputils/managers/taskmanagers.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/managers/tests/test_fileio.py` & `qtapputils-0.5.2/qtapputils/managers/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/managers/tests/test_taskmanagers.py` & `qtapputils-0.5.2/qtapputils/managers/tests/test_taskmanagers.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/qthelpers.py` & `qtapputils-0.5.2/qtapputils/qthelpers.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/tests/test_icons.py` & `qtapputils-0.5.2/qtapputils/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/tests/test_qthelpers.py` & `qtapputils-0.5.2/qtapputils/tests/test_qthelpers.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/widgets/path.py` & `qtapputils-0.5.2/qtapputils/widgets/path.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/widgets/range.py` & `qtapputils-0.5.2/qtapputils/widgets/range.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/widgets/tests/test_path.py` & `qtapputils-0.5.2/qtapputils/widgets/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/widgets/tests/test_range.py` & `qtapputils-0.5.2/qtapputils/widgets/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils/widgets/waitingspinner.py` & `qtapputils-0.5.2/qtapputils/widgets/waitingspinner.py`

 * *Files identical despite different names*

### Comparing `qtapputils-0.5.1/qtapputils.egg-info/PKG-INFO` & `qtapputils-0.5.2/qtapputils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtapputils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utilities for building Qt applications in Python.
 Home-page: https://github.com/jnsebgosselin/qtapputils
 Author: Jean-Sébastien Gosselin
 Author-email: jean-sebastien.gosselin@outlook.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtapputils-0.5.1/qtapputils.egg-info/SOURCES.txt` & `qtapputils-0.5.2/qtapputils.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,11 +18,13 @@
 qtapputils/managers/tests/test_taskmanagers.py
 qtapputils/tests/__init__.py
 qtapputils/tests/test_icons.py
 qtapputils/tests/test_qthelpers.py
 qtapputils/widgets/__init__.py
 qtapputils/widgets/path.py
 qtapputils/widgets/range.py
+qtapputils/widgets/splash.py
 qtapputils/widgets/waitingspinner.py
 qtapputils/widgets/tests/__init__.py
 qtapputils/widgets/tests/test_path.py
-qtapputils/widgets/tests/test_range.py
+qtapputils/widgets/tests/test_range.py
+qtapputils/widgets/tests/test_splash.py
```

### Comparing `qtapputils-0.5.1/setup.py` & `qtapputils-0.5.2/setup.py`

 * *Files identical despite different names*

