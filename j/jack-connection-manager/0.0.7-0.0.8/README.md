# Comparing `tmp/jack_connection_manager-0.0.7.tar.gz` & `tmp/jack_connection_manager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jack_connection_manager-0.0.7.tar", last modified: Tue Apr  2 16:45:22 2024, max compression
+gzip compressed data, was "jack_connection_manager-0.0.8.tar", last modified: Tue Apr 23 13:03:41 2024, max compression
```

## Comparing `jack_connection_manager-0.0.7.tar` & `jack_connection_manager-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leto      (1000) leto      (1000)        0 2024-04-02 16:45:22.852186 jack_connection_manager-0.0.7/
--rw-r--r--   0 leto      (1000) leto      (1000)    35149 2024-03-22 11:50:15.000000 jack_connection_manager-0.0.7/LICENSE
--rw-r--r--   0 leto      (1000) leto      (1000)    42450 2024-04-02 16:45:22.852186 jack_connection_manager-0.0.7/PKG-INFO
--rw-r--r--   0 leto      (1000) leto      (1000)     1384 2024-03-28 19:03:22.000000 jack_connection_manager-0.0.7/README.md
--rw-r--r--   0 leto      (1000) leto      (1000)     1113 2024-04-02 16:42:21.000000 jack_connection_manager-0.0.7/pyproject.toml
--rw-r--r--   0 leto      (1000) leto      (1000)       38 2024-04-02 16:45:22.852186 jack_connection_manager-0.0.7/setup.cfg
--rw-r--r--   0 leto      (1000) leto      (1000)      124 2024-03-25 19:52:51.000000 jack_connection_manager-0.0.7/setup.py
-drwxr-xr-x   0 leto      (1000) leto      (1000)        0 2024-04-02 16:45:22.848852 jack_connection_manager-0.0.7/src/
-drwxr-xr-x   0 leto      (1000) leto      (1000)        0 2024-04-02 16:45:22.852186 jack_connection_manager-0.0.7/src/jack_connection_manager/
--rw-r--r--   0 leto      (1000) leto      (1000)     5365 2024-04-02 14:48:57.000000 jack_connection_manager-0.0.7/src/jack_connection_manager/ConnectionManager.py
--rw-r--r--   0 leto      (1000) leto      (1000)       73 2024-03-25 19:52:51.000000 jack_connection_manager-0.0.7/src/jack_connection_manager/__init__.py
--rw-r--r--   0 leto      (1000) leto      (1000)      497 2024-04-02 16:45:22.852186 jack_connection_manager-0.0.7/src/jack_connection_manager/_version.py
--rw-r--r--   0 leto      (1000) leto      (1000)     3826 2024-04-02 14:48:25.000000 jack_connection_manager-0.0.7/src/jack_connection_manager/jack_connection_manager.py
-drwxr-xr-x   0 leto      (1000) leto      (1000)        0 2024-04-02 16:45:22.852186 jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/
--rw-r--r--   0 leto      (1000) leto      (1000)    42450 2024-04-02 16:45:22.000000 jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/PKG-INFO
--rw-r--r--   0 leto      (1000) leto      (1000)      533 2024-04-02 16:45:22.000000 jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/SOURCES.txt
--rw-r--r--   0 leto      (1000) leto      (1000)        1 2024-04-02 16:45:22.000000 jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/dependency_links.txt
--rw-r--r--   0 leto      (1000) leto      (1000)       97 2024-04-02 16:45:22.000000 jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/entry_points.txt
--rw-r--r--   0 leto      (1000) leto      (1000)       25 2024-04-02 16:45:22.000000 jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/requires.txt
--rw-r--r--   0 leto      (1000) leto      (1000)       24 2024-04-02 16:45:22.000000 jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:41.279175 jack_connection_manager-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 13:03:36.000000 jack_connection_manager-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42450 2024-04-23 13:03:41.279175 jack_connection_manager-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-23 13:03:36.000000 jack_connection_manager-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-23 13:03:36.000000 jack_connection_manager-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:03:41.279175 jack_connection_manager-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 13:03:36.000000 jack_connection_manager-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:41.275175 jack_connection_manager-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:41.275175 jack_connection_manager-0.0.8/src/jack_connection_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-23 13:03:36.000000 jack_connection_manager-0.0.8/src/jack_connection_manager/ConnectionManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 13:03:36.000000 jack_connection_manager-0.0.8/src/jack_connection_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 13:03:41.279175 jack_connection_manager-0.0.8/src/jack_connection_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-23 13:03:36.000000 jack_connection_manager-0.0.8/src/jack_connection_manager/jack_connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:03:41.279175 jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42450 2024-04-23 13:03:41.000000 jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 13:03:41.000000 jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:03:41.000000 jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 13:03:41.000000 jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 13:03:41.000000 jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 13:03:41.000000 jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/top_level.txt
```

### Comparing `jack_connection_manager-0.0.7/LICENSE` & `jack_connection_manager-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jack_connection_manager-0.0.7/PKG-INFO` & `jack_connection_manager-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jack_connection_manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for automatically connecting jack clients with lots of ports
 Author-email: Max Weidauer <weidauer@campus.tu-berlin.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jack_connection_manager-0.0.7/README.md` & `jack_connection_manager-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jack_connection_manager-0.0.7/pyproject.toml` & `jack_connection_manager-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jack_connection_manager-0.0.7/src/jack_connection_manager/ConnectionManager.py` & `jack_connection_manager-0.0.8/src/jack_connection_manager/ConnectionManager.py`

 * *Files identical despite different names*

### Comparing `jack_connection_manager-0.0.7/src/jack_connection_manager/jack_connection_manager.py` & `jack_connection_manager-0.0.8/src/jack_connection_manager/jack_connection_manager.py`

 * *Files identical despite different names*

### Comparing `jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/PKG-INFO` & `jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jack_connection_manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for automatically connecting jack clients with lots of ports
 Author-email: Max Weidauer <weidauer@campus.tu-berlin.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jack_connection_manager-0.0.7/src/jack_connection_manager.egg-info/SOURCES.txt` & `jack_connection_manager-0.0.8/src/jack_connection_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

