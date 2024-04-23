# Comparing `tmp/nxtomo-1.3.0.dev1.tar.gz` & `tmp/nxtomo-1.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxtomo-1.3.0.dev1.tar", last modified: Wed Mar 20 18:34:48 2024, max compression
+gzip compressed data, was "nxtomo-1.3.0.dev2.tar", last modified: Wed Mar 20 18:52:10 2024, max compression
```

## Comparing `nxtomo-1.3.0.dev1.tar` & `nxtomo-1.3.0.dev2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/
--rw-r--r--   0 payno     (1000) payno     (1000)     1266 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3402 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      351 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/README.md
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.602455 nxtomo-1.3.0.dev1/doc/
--rw-r--r--   0 payno     (1000) payno     (1000)     2526 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/doc/conf.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.602455 nxtomo-1.3.0.dev1/nxtomo/
--rw-r--r--   0 payno     (1000) payno     (1000)      227 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.602455 nxtomo-1.3.0.dev1/nxtomo/application/
--rw-r--r--   0 payno     (1000) payno     (1000)    32479 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/nxtomo/application/nxtomo.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.602455 nxtomo-1.3.0.dev1/nxtomo/application/test/
--rw-r--r--   0 payno     (1000) payno     (1000)    18265 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev1/nxtomo/application/test/test_nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5587 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/nxtomo/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/nxtomo/nxobject/
--rw-r--r--   0 payno     (1000) payno     (1000)      392 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    44483 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7895 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3834 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)    14413 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/nxobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10749 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7319 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11561 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/nxtransformations.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/
--rw-r--r--   0 payno     (1000) payno     (1000)    17345 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1333 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1077 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2706 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2076 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1127 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5487 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxtransformations.py
--rw-r--r--   0 payno     (1000) payno     (1000)      753 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/nxobject/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/nxtomo/paths/
--rw-r--r--   0 payno     (1000) payno     (1000)       62 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1332 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev1/nxtomo/paths/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      605 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)      437 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)      941 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)      459 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11988 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)      677 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/nxtransformations.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/nxtomo/paths/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     6676 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/paths/test/test_backward_compatibility.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/nxtomo/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)       73 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    20038 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/utils/detectorsplitter.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15649 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/nxtomo/utils/frameappender.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3830 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/nxtomo/utils/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/nxtomo/utils/test/
--rw-r--r--   0 payno     (1000) payno     (1000)    20111 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/utils/test/test_detectorsplitter.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7620 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/utils/test/test_transformation.py
--rw-r--r--   0 payno     (1000) payno     (1000)    21577 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/nxtomo/utils/transformation.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2365 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev1/nxtomo/utils/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-03-20 18:34:43.000000 nxtomo-1.3.0.dev1/nxtomo/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:34:48.602455 nxtomo-1.3.0.dev1/nxtomo.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3402 2024-03-20 18:34:48.000000 nxtomo-1.3.0.dev1/nxtomo.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     1374 2024-03-20 18:34:48.000000 nxtomo-1.3.0.dev1/nxtomo.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-03-20 18:34:48.000000 nxtomo-1.3.0.dev1/nxtomo.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      230 2024-03-20 18:34:48.000000 nxtomo-1.3.0.dev1/nxtomo.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       22 2024-03-20 18:34:48.000000 nxtomo-1.3.0.dev1/nxtomo.egg-info/top_level.txt
--rw-r--r--   0 payno     (1000) payno     (1000)     2298 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev1/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-03-20 18:34:48.606455 nxtomo-1.3.0.dev1/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev1/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1266 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3402 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      351 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/README.md
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/doc/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2526 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev2/doc/conf.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/
+-rw-r--r--   0 payno     (1000) payno     (1000)      227 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/application/
+-rw-r--r--   0 payno     (1000) payno     (1000)    32479 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev2/nxtomo/application/nxtomo.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/application/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)    18265 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev2/nxtomo/application/test/test_nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5573 2024-03-20 18:50:06.000000 nxtomo-1.3.0.dev2/nxtomo/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/nxobject/
+-rw-r--r--   0 payno     (1000) payno     (1000)      392 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    44483 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7893 2024-03-20 18:51:04.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3834 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14413 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10749 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7319 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11561 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/nxtransformations.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)    17345 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1333 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1077 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2706 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2076 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1127 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5487 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxtransformations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      753 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/nxobject/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/paths/
+-rw-r--r--   0 payno     (1000) payno     (1000)       62 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1332 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev2/nxtomo/paths/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      605 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      437 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      941 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      459 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11988 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      677 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/nxtransformations.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/paths/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     6676 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/paths/test/test_backward_compatibility.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)       73 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    20038 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/utils/detectorsplitter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15649 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev2/nxtomo/utils/frameappender.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3830 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev2/nxtomo/utils/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo/utils/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)    20111 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/utils/test/test_detectorsplitter.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7620 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/utils/test/test_transformation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    21577 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/nxtomo/utils/transformation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2365 2024-03-20 18:33:23.000000 nxtomo-1.3.0.dev2/nxtomo/utils/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-03-20 18:34:50.000000 nxtomo-1.3.0.dev2/nxtomo/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/nxtomo.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3402 2024-03-20 18:52:10.000000 nxtomo-1.3.0.dev2/nxtomo.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     1374 2024-03-20 18:52:10.000000 nxtomo-1.3.0.dev2/nxtomo.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-03-20 18:52:10.000000 nxtomo-1.3.0.dev2/nxtomo.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      230 2024-03-20 18:52:10.000000 nxtomo-1.3.0.dev2/nxtomo.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       22 2024-03-20 18:52:10.000000 nxtomo-1.3.0.dev2/nxtomo.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)     2298 2024-03-20 18:33:11.000000 nxtomo-1.3.0.dev2/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-03-20 18:52:10.192760 nxtomo-1.3.0.dev2/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-03-14 18:41:17.000000 nxtomo-1.3.0.dev2/setup.py
```

### Comparing `nxtomo-1.3.0.dev1/LICENSE` & `nxtomo-1.3.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/PKG-INFO` & `nxtomo-1.3.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomo
-Version: 1.3.0.dev1
+Version: 1.3.0.dev2
 Summary: module to create / edit NXtomo application
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The nxtomo library goal is to provide a powerful python interface to read / write nexus NXtomo application
         
         nxtomo is distributed under the MIT license.
```

### Comparing `nxtomo-1.3.0.dev1/doc/conf.py` & `nxtomo-1.3.0.dev2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/application/nxtomo.py` & `nxtomo-1.3.0.dev2/nxtomo/application/nxtomo.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/application/test/test_nxtomo.py` & `nxtomo-1.3.0.dev2/nxtomo/application/test/test_nxtomo.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/io.py` & `nxtomo-1.3.0.dev2/nxtomo/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import logging
 from typing import Optional
 import os
 from contextlib import contextmanager
 import h5py._hl.selections as selection
 from silx.io.url import DataUrl
-from silx.io.h5py_utils import File as HDF5File  # noqa F401
+from h5py import File as HDF5File  # noqa F401
 from silx.io.utils import open as hdf5_open
 
 import h5py
 
 _logger = logging.getLogger(__name__)
```

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/nxdetector.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/nxdetector.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/nxinstrument.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/nxinstrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import logging
 from functools import partial
 from operator import is_not
 from typing import Optional
 
 from silx.utils.proxy import docstring
-from nxtomo.io import HDF5File, get_swmr_mode
+from nxtomo.io import HDF5File
+from silx.io.utils import open as open_hdf5
 from pyunitsystem.voltagesystem import VoltageSystem
 
 from nxtomo.paths.nxtomo import get_paths as get_nexus_paths
 from nxtomo.nxobject.nxdetector import NXdetector, NXdetectorWithUnit
 from nxtomo.nxobject.nxsource import DefaultESRFSource, NXsource
 from nxtomo.nxobject.nxobject import NXobject
 from nxtomo.utils import get_data
@@ -149,15 +150,15 @@
     ) -> NXobject:
         """
         Create and load an NXsample from data on disk
         """
         nexus_paths = get_nexus_paths(nexus_version)
         nexus_instrument_paths = nexus_paths.nx_instrument_paths
 
-        with HDF5File(file_path, mode="r", swmr=get_swmr_mode()) as h5f:
+        with open_hdf5(file_path) as h5f:
             if data_path in h5f:
                 has_detector = "detector" in h5f[data_path]
                 has_diode = "diode" in h5f[data_path]
                 has_source = "source" in h5f[data_path]
             else:
                 has_detector = False
                 has_diode = False
```

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/nxmonitor.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/nxobject.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/nxobject.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/nxsample.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/nxsource.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/nxsource.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/nxtransformations.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxdetector.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxdetector.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxinstrument.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxinstrument.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxmonitor.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxmonitor.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxobject.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxobject.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxsample.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxsource.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxsource.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/test/test_nxtransformations.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/test/test_nxtransformations.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/nxobject/utils.py` & `nxtomo-1.3.0.dev2/nxtomo/nxobject/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/paths/nxdetector.py` & `nxtomo-1.3.0.dev2/nxtomo/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/paths/nxinstrument.py` & `nxtomo-1.3.0.dev2/nxtomo/paths/nxinstrument.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/paths/nxsample.py` & `nxtomo-1.3.0.dev2/nxtomo/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/paths/nxtomo.py` & `nxtomo-1.3.0.dev2/nxtomo/paths/nxtomo.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/paths/nxtransformations.py` & `nxtomo-1.3.0.dev2/nxtomo/paths/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/paths/test/test_backward_compatibility.py` & `nxtomo-1.3.0.dev2/nxtomo/paths/test/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/utils/detectorsplitter.py` & `nxtomo-1.3.0.dev2/nxtomo/utils/detectorsplitter.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/utils/frameappender.py` & `nxtomo-1.3.0.dev2/nxtomo/utils/frameappender.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/utils/io.py` & `nxtomo-1.3.0.dev2/nxtomo/utils/io.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/utils/test/test_detectorsplitter.py` & `nxtomo-1.3.0.dev2/nxtomo/utils/test/test_detectorsplitter.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/utils/test/test_transformation.py` & `nxtomo-1.3.0.dev2/nxtomo/utils/test/test_transformation.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/utils/transformation.py` & `nxtomo-1.3.0.dev2/nxtomo/utils/transformation.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo/utils/utils.py` & `nxtomo-1.3.0.dev2/nxtomo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/nxtomo.egg-info/PKG-INFO` & `nxtomo-1.3.0.dev2/nxtomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomo
-Version: 1.3.0.dev1
+Version: 1.3.0.dev2
 Summary: module to create / edit NXtomo application
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The nxtomo library goal is to provide a powerful python interface to read / write nexus NXtomo application
         
         nxtomo is distributed under the MIT license.
```

### Comparing `nxtomo-1.3.0.dev1/nxtomo.egg-info/SOURCES.txt` & `nxtomo-1.3.0.dev2/nxtomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxtomo-1.3.0.dev1/pyproject.toml` & `nxtomo-1.3.0.dev2/pyproject.toml`

 * *Files identical despite different names*

