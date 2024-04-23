# Comparing `tmp/akdpy-0.0.1.tar.gz` & `tmp/akdpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akdpy-0.0.1.tar", last modified: Tue Apr 23 13:53:37 2024, max compression
+gzip compressed data, was "akdpy-0.0.2.tar", last modified: Tue Apr 23 14:00:33 2024, max compression
```

## Comparing `akdpy-0.0.1.tar` & `akdpy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 13:53:37.757464 akdpy-0.0.1/
--rw-r--r--   0 erenarim  (1000) erenarim  (1000)      270 2024-04-23 13:53:37.757464 akdpy-0.0.1/PKG-INFO
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        8 2024-04-23 13:47:25.000000 akdpy-0.0.1/README.md
-drwxrwxr-x   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 13:53:37.757464 akdpy-0.0.1/akdpy.egg-info/
--rw-r--r--   0 erenarim  (1000) erenarim  (1000)      270 2024-04-23 13:53:37.000000 akdpy-0.0.1/akdpy.egg-info/PKG-INFO
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)      200 2024-04-23 13:53:37.000000 akdpy-0.0.1/akdpy.egg-info/SOURCES.txt
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        1 2024-04-23 13:53:37.000000 akdpy-0.0.1/akdpy.egg-info/dependency_links.txt
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        7 2024-04-23 13:53:37.000000 akdpy-0.0.1/akdpy.egg-info/requires.txt
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        8 2024-04-23 13:53:37.000000 akdpy-0.0.1/akdpy.egg-info/top_level.txt
-drwxrwxr-x   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 13:53:37.757464 akdpy-0.0.1/library/
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 13:48:38.000000 akdpy-0.0.1/library/__init__.py
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)     2049 2024-04-23 13:48:51.000000 akdpy-0.0.1/library/system.py
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)       38 2024-04-23 13:53:37.757464 akdpy-0.0.1/setup.cfg
--rw-rw-r--   0 erenarim  (1000) erenarim  (1000)      408 2024-04-23 13:53:33.000000 akdpy-0.0.1/setup.py
+drwxrwxr-x   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 14:00:33.223162 akdpy-0.0.2/
+-rw-r--r--   0 erenarim  (1000) erenarim  (1000)      270 2024-04-23 14:00:33.223162 akdpy-0.0.2/PKG-INFO
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        8 2024-04-23 13:47:25.000000 akdpy-0.0.2/README.md
+drwxrwxr-x   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 14:00:33.223162 akdpy-0.0.2/akdpy/
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 13:48:38.000000 akdpy-0.0.2/akdpy/__init__.py
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)     2049 2024-04-23 13:48:51.000000 akdpy-0.0.2/akdpy/system.py
+drwxrwxr-x   0 erenarim  (1000) erenarim  (1000)        0 2024-04-23 14:00:33.223162 akdpy-0.0.2/akdpy.egg-info/
+-rw-r--r--   0 erenarim  (1000) erenarim  (1000)      270 2024-04-23 14:00:33.000000 akdpy-0.0.2/akdpy.egg-info/PKG-INFO
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)      196 2024-04-23 14:00:33.000000 akdpy-0.0.2/akdpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        1 2024-04-23 14:00:33.000000 akdpy-0.0.2/akdpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        7 2024-04-23 14:00:33.000000 akdpy-0.0.2/akdpy.egg-info/requires.txt
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)        6 2024-04-23 14:00:33.000000 akdpy-0.0.2/akdpy.egg-info/top_level.txt
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)       38 2024-04-23 14:00:33.223162 akdpy-0.0.2/setup.cfg
+-rw-rw-r--   0 erenarim  (1000) erenarim  (1000)      408 2024-04-23 14:00:21.000000 akdpy-0.0.2/setup.py
```

### Comparing `akdpy-0.0.1/library/system.py` & `akdpy-0.0.2/akdpy/system.py`

 * *Files identical despite different names*

