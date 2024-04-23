# Comparing `tmp/neon-enclosure-1.6.2a4.tar.gz` & `tmp/neon-enclosure-1.6.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-enclosure-1.6.2a4.tar", last modified: Thu Feb 22 18:44:22 2024, max compression
+gzip compressed data, was "neon-enclosure-1.6.2a5.tar", last modified: Tue Apr 23 17:48:00 2024, max compression
```

## Comparing `neon-enclosure-1.6.2a4.tar` & `neon-enclosure-1.6.2a5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:44:22.543758 neon-enclosure-1.6.2a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-22 18:44:22.543758 neon-enclosure-1.6.2a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:44:22.539758 neon-enclosure-1.6.2a4/neon_enclosure/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:44:22.543758 neon-enclosure-1.6.2a4/neon_enclosure/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/admin/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/neon_enclosure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:44:22.543758 neon-enclosure-1.6.2a4/neon_enclosure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-22 18:44:22.000000 neon-enclosure-1.6.2a4/neon_enclosure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-22 18:44:22.000000 neon-enclosure-1.6.2a4/neon_enclosure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:44:22.000000 neon-enclosure-1.6.2a4/neon_enclosure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-22 18:44:22.000000 neon-enclosure-1.6.2a4/neon_enclosure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-22 18:44:22.000000 neon-enclosure-1.6.2a4/neon_enclosure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-22 18:44:22.000000 neon-enclosure-1.6.2a4/neon_enclosure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 18:44:22.543758 neon-enclosure-1.6.2a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-22 18:44:19.000000 neon-enclosure-1.6.2a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:48:00.500912 neon-enclosure-1.6.2a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-23 17:48:00.500912 neon-enclosure-1.6.2a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:48:00.496912 neon-enclosure-1.6.2a5/neon_enclosure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:48:00.500912 neon-enclosure-1.6.2a5/neon_enclosure/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/admin/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/neon_enclosure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:48:00.500912 neon-enclosure-1.6.2a5/neon_enclosure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-23 17:48:00.000000 neon-enclosure-1.6.2a5/neon_enclosure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 17:48:00.000000 neon-enclosure-1.6.2a5/neon_enclosure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:48:00.000000 neon-enclosure-1.6.2a5/neon_enclosure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-23 17:48:00.000000 neon-enclosure-1.6.2a5/neon_enclosure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-23 17:48:00.000000 neon-enclosure-1.6.2a5/neon_enclosure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 17:48:00.000000 neon-enclosure-1.6.2a5/neon_enclosure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:48:00.500912 neon-enclosure-1.6.2a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-23 17:47:54.000000 neon-enclosure-1.6.2a5/setup.py
```

### Comparing `neon-enclosure-1.6.2a4/LICENSE.md` & `neon-enclosure-1.6.2a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/PKG-INFO` & `neon-enclosure-1.6.2a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.6.2a4
+Version: 1.6.2a5
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.6.2a4/README.md` & `neon-enclosure-1.6.2a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/__init__.py` & `neon-enclosure-1.6.2a5/neon_enclosure/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/__main__.py` & `neon-enclosure-1.6.2a5/neon_enclosure/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/admin/__init__.py` & `neon-enclosure-1.6.2a5/neon_enclosure/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/admin/__main__.py` & `neon-enclosure-1.6.2a5/neon_enclosure/admin/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/admin/service.py` & `neon-enclosure-1.6.2a5/neon_enclosure/admin/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/cli.py` & `neon-enclosure-1.6.2a5/neon_enclosure/cli.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/service.py` & `neon-enclosure-1.6.2a5/neon_enclosure/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure/utils.py` & `neon-enclosure-1.6.2a5/neon_enclosure/utils.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.6.2a4/neon_enclosure.egg-info/PKG-INFO` & `neon-enclosure-1.6.2a5/neon_enclosure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.6.2a4
+Version: 1.6.2a5
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.6.2a4/setup.py` & `neon-enclosure-1.6.2a5/setup.py`

 * *Files identical despite different names*

