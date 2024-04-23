# Comparing `tmp/daac-0.1.1.tar.gz` & `tmp/daac-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daac-0.1.1.tar", last modified: Tue Apr 23 17:50:03 2024, max compression
+gzip compressed data, was "daac-1.0.tar", last modified: Tue Apr 23 18:02:36 2024, max compression
```

## Comparing `daac-0.1.1.tar` & `daac-1.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:50:03.673357 daac-0.1.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      192 2024-04-23 17:50:03.673357 daac-0.1.1/PKG-INFO
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:50:03.673357 daac-0.1.1/daac/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:31:37.000000 daac-0.1.1/daac/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13790 2024-04-23 17:48:59.000000 daac-0.1.1/daac/program.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      347 2024-04-23 17:32:05.000000 daac-0.1.1/daac/programs.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:50:03.673357 daac-0.1.1/daac.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      192 2024-04-23 17:50:03.000000 daac-0.1.1/daac.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      228 2024-04-23 17:50:03.000000 daac-0.1.1/daac.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-23 17:50:03.000000 daac-0.1.1/daac.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       44 2024-04-23 17:50:03.000000 daac-0.1.1/daac.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-04-23 17:50:03.000000 daac-0.1.1/daac.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        5 2024-04-23 17:50:03.000000 daac-0.1.1/daac.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-23 17:50:03.673357 daac-0.1.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      417 2024-04-23 17:49:40.000000 daac-0.1.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:02:36.228650 daac-1.0/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      190 2024-04-23 18:02:36.224650 daac-1.0/PKG-INFO
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:02:36.224650 daac-1.0/daac/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:31:37.000000 daac-1.0/daac/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      642 2024-04-23 18:00:43.000000 daac-1.0/daac/p1.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1489 2024-04-23 18:00:57.000000 daac-1.0/daac/p2.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1483 2024-04-23 18:01:12.000000 daac-1.0/daac/p3.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1705 2024-04-23 18:01:28.000000 daac-1.0/daac/p4.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1730 2024-04-23 18:01:39.000000 daac-1.0/daac/p5.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4111 2024-04-23 18:01:51.000000 daac-1.0/daac/p6.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2383 2024-04-23 18:02:06.000000 daac-1.0/daac/p7.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13790 2024-04-23 17:48:59.000000 daac-1.0/daac/program.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1332 2024-04-23 18:00:20.000000 daac-1.0/daac/programs.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:02:36.224650 daac-1.0/daac.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      190 2024-04-23 18:02:36.000000 daac-1.0/daac.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      305 2024-04-23 18:02:36.000000 daac-1.0/daac.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-23 18:02:36.000000 daac-1.0/daac.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       44 2024-04-23 18:02:36.000000 daac-1.0/daac.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-04-23 18:02:36.000000 daac-1.0/daac.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        5 2024-04-23 18:02:36.000000 daac-1.0/daac.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-23 18:02:36.228650 daac-1.0/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      415 2024-04-23 18:02:21.000000 daac-1.0/setup.py
```

### Comparing `daac-0.1.1/daac/program.py` & `daac-1.0/daac/program.py`

 * *Files identical despite different names*

