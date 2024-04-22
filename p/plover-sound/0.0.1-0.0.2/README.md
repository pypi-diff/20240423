# Comparing `tmp/plover-sound-0.0.1.tar.gz` & `tmp/plover-sound-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-sound-0.0.1.tar", last modified: Mon Apr 22 21:43:05 2024, max compression
+gzip compressed data, was "plover-sound-0.0.2.tar", last modified: Mon Apr 22 22:01:58 2024, max compression
```

## Comparing `plover-sound-0.0.1.tar` & `plover-sound-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 21:43:05.327899 plover-sound-0.0.1/
--rw-r--r--   0 zach      (1000) zach      (1000)     1082 2024-04-22 21:34:13.000000 plover-sound-0.0.1/LICENSE
--rw-r--r--   0 zach      (1000) zach      (1000)       33 2024-04-22 21:41:45.000000 plover-sound-0.0.1/MANIFEST.in
--rw-r--r--   0 zach      (1000) zach      (1000)      881 2024-04-22 21:43:05.327899 plover-sound-0.0.1/PKG-INFO
--rw-r--r--   0 zach      (1000) zach      (1000)      476 2024-04-22 21:34:13.000000 plover-sound-0.0.1/README.md
-drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 21:43:05.327899 plover-sound-0.0.1/plover_sound/
--rw-r--r--   0 zach      (1000) zach      (1000)        0 2024-04-21 00:26:41.000000 plover-sound-0.0.1/plover_sound/__init__.py
--rw-r--r--   0 zach      (1000) zach      (1000)     8710 2024-04-22 21:03:14.000000 plover-sound-0.0.1/plover_sound/extension.py
--rw-r--r--   0 zach      (1000) zach      (1000)     5020 2024-04-22 21:09:54.000000 plover-sound-0.0.1/plover_sound/tool.py
-drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 21:43:05.327899 plover-sound-0.0.1/plover_sound.egg-info/
--rw-r--r--   0 zach      (1000) zach      (1000)      881 2024-04-22 21:43:05.000000 plover-sound-0.0.1/plover_sound.egg-info/PKG-INFO
--rw-r--r--   0 zach      (1000) zach      (1000)      369 2024-04-22 21:43:05.000000 plover-sound-0.0.1/plover_sound.egg-info/SOURCES.txt
--rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 21:43:05.000000 plover-sound-0.0.1/plover_sound.egg-info/dependency_links.txt
--rw-r--r--   0 zach      (1000) zach      (1000)      144 2024-04-22 21:43:05.000000 plover-sound-0.0.1/plover_sound.egg-info/entry_points.txt
--rw-r--r--   0 zach      (1000) zach      (1000)       54 2024-04-22 21:43:05.000000 plover-sound-0.0.1/plover_sound.egg-info/requires.txt
--rw-r--r--   0 zach      (1000) zach      (1000)       13 2024-04-22 21:43:05.000000 plover-sound-0.0.1/plover_sound.egg-info/top_level.txt
--rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 18:01:37.000000 plover-sound-0.0.1/plover_sound.egg-info/zip-safe
--rw-r--r--   0 zach      (1000) zach      (1000)      730 2024-04-22 21:43:05.327899 plover-sound-0.0.1/setup.cfg
--rw-r--r--   0 zach      (1000) zach      (1000)       38 2024-04-22 21:40:47.000000 plover-sound-0.0.1/setup.py
+drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:01:58.722773 plover-sound-0.0.2/
+-rw-r--r--   0 zach      (1000) zach      (1000)     1082 2024-04-22 21:34:13.000000 plover-sound-0.0.2/LICENSE
+-rw-r--r--   0 zach      (1000) zach      (1000)       33 2024-04-22 21:41:45.000000 plover-sound-0.0.2/MANIFEST.in
+-rw-r--r--   0 zach      (1000) zach      (1000)      881 2024-04-22 22:01:58.722773 plover-sound-0.0.2/PKG-INFO
+-rw-r--r--   0 zach      (1000) zach      (1000)      476 2024-04-22 21:34:13.000000 plover-sound-0.0.2/README.md
+drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:01:58.722773 plover-sound-0.0.2/plover_sound/
+-rw-r--r--   0 zach      (1000) zach      (1000)        0 2024-04-21 00:26:41.000000 plover-sound-0.0.2/plover_sound/__init__.py
+-rw-r--r--   0 zach      (1000) zach      (1000)     8710 2024-04-22 21:03:14.000000 plover-sound-0.0.2/plover_sound/extension.py
+-rw-r--r--   0 zach      (1000) zach      (1000)     5020 2024-04-22 21:09:54.000000 plover-sound-0.0.2/plover_sound/tool.py
+drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:01:58.722773 plover-sound-0.0.2/plover_sound.egg-info/
+-rw-r--r--   0 zach      (1000) zach      (1000)      881 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/PKG-INFO
+-rw-r--r--   0 zach      (1000) zach      (1000)      369 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/SOURCES.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/dependency_links.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)      144 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/entry_points.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)       54 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/requires.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)       13 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/top_level.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 18:01:37.000000 plover-sound-0.0.2/plover_sound.egg-info/zip-safe
+-rw-r--r--   0 zach      (1000) zach      (1000)      730 2024-04-22 22:01:58.722773 plover-sound-0.0.2/setup.cfg
+-rw-r--r--   0 zach      (1000) zach      (1000)       38 2024-04-22 21:40:47.000000 plover-sound-0.0.2/setup.py
```

### Comparing `plover-sound-0.0.1/LICENSE` & `plover-sound-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plover-sound-0.0.1/PKG-INFO` & `plover-sound-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-sound
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plays sound when stroke is registered
 Author: Zach Rice
 Author-email: bynxmusic@gmail.com
 License: GNU General Public License v2 or later (GPLv2+)
 Keywords: plover plover_plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plover-sound-0.0.1/plover_sound/extension.py` & `plover-sound-0.0.2/plover_sound/extension.py`

 * *Files identical despite different names*

### Comparing `plover-sound-0.0.1/plover_sound/tool.py` & `plover-sound-0.0.2/plover_sound/tool.py`

 * *Files identical despite different names*

### Comparing `plover-sound-0.0.1/plover_sound.egg-info/PKG-INFO` & `plover-sound-0.0.2/plover_sound.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-sound
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plays sound when stroke is registered
 Author: Zach Rice
 Author-email: bynxmusic@gmail.com
 License: GNU General Public License v2 or later (GPLv2+)
 Keywords: plover plover_plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plover-sound-0.0.1/setup.cfg` & `plover-sound-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-sound
-version = 0.0.1
+version = 0.0.2
 description = Plays sound when stroke is registered
 author = Zach Rice
 author_email = bynxmusic@gmail.com
 license = GNU General Public License v2 or later (GPLv2+)
 keywords = plover plover_plugin
 long_description = file: README.md
 long_description_content_type = text/markdown
```

