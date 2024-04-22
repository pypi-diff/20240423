# Comparing `tmp/plover-sound-0.0.2.tar.gz` & `tmp/plover-sound-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-sound-0.0.2.tar", last modified: Mon Apr 22 22:01:58 2024, max compression
+gzip compressed data, was "plover-sound-0.0.3.tar", last modified: Mon Apr 22 22:36:16 2024, max compression
```

## Comparing `plover-sound-0.0.2.tar` & `plover-sound-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:01:58.722773 plover-sound-0.0.2/
--rw-r--r--   0 zach      (1000) zach      (1000)     1082 2024-04-22 21:34:13.000000 plover-sound-0.0.2/LICENSE
--rw-r--r--   0 zach      (1000) zach      (1000)       33 2024-04-22 21:41:45.000000 plover-sound-0.0.2/MANIFEST.in
--rw-r--r--   0 zach      (1000) zach      (1000)      881 2024-04-22 22:01:58.722773 plover-sound-0.0.2/PKG-INFO
--rw-r--r--   0 zach      (1000) zach      (1000)      476 2024-04-22 21:34:13.000000 plover-sound-0.0.2/README.md
-drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:01:58.722773 plover-sound-0.0.2/plover_sound/
--rw-r--r--   0 zach      (1000) zach      (1000)        0 2024-04-21 00:26:41.000000 plover-sound-0.0.2/plover_sound/__init__.py
--rw-r--r--   0 zach      (1000) zach      (1000)     8710 2024-04-22 21:03:14.000000 plover-sound-0.0.2/plover_sound/extension.py
--rw-r--r--   0 zach      (1000) zach      (1000)     5020 2024-04-22 21:09:54.000000 plover-sound-0.0.2/plover_sound/tool.py
-drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:01:58.722773 plover-sound-0.0.2/plover_sound.egg-info/
--rw-r--r--   0 zach      (1000) zach      (1000)      881 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/PKG-INFO
--rw-r--r--   0 zach      (1000) zach      (1000)      369 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/SOURCES.txt
--rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/dependency_links.txt
--rw-r--r--   0 zach      (1000) zach      (1000)      144 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/entry_points.txt
--rw-r--r--   0 zach      (1000) zach      (1000)       54 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/requires.txt
--rw-r--r--   0 zach      (1000) zach      (1000)       13 2024-04-22 22:01:58.000000 plover-sound-0.0.2/plover_sound.egg-info/top_level.txt
--rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 18:01:37.000000 plover-sound-0.0.2/plover_sound.egg-info/zip-safe
--rw-r--r--   0 zach      (1000) zach      (1000)      730 2024-04-22 22:01:58.722773 plover-sound-0.0.2/setup.cfg
--rw-r--r--   0 zach      (1000) zach      (1000)       38 2024-04-22 21:40:47.000000 plover-sound-0.0.2/setup.py
+drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:36:16.435228 plover-sound-0.0.3/
+-rw-r--r--   0 zach      (1000) zach      (1000)     1082 2024-04-22 21:34:13.000000 plover-sound-0.0.3/LICENSE
+-rw-r--r--   0 zach      (1000) zach      (1000)       87 2024-04-22 22:34:12.000000 plover-sound-0.0.3/MANIFEST.in
+-rw-r--r--   0 zach      (1000) zach      (1000)      887 2024-04-22 22:36:16.435228 plover-sound-0.0.3/PKG-INFO
+-rw-r--r--   0 zach      (1000) zach      (1000)      476 2024-04-22 21:34:13.000000 plover-sound-0.0.3/README.md
+drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:36:16.435228 plover-sound-0.0.3/plover_sound/
+-rw-r--r--   0 zach      (1000) zach      (1000)        0 2024-04-21 00:26:41.000000 plover-sound-0.0.3/plover_sound/__init__.py
+-rw-r--r--   0 zach      (1000) zach      (1000)     8710 2024-04-22 21:03:14.000000 plover-sound-0.0.3/plover_sound/extension.py
+-rw-r--r--   0 zach      (1000) zach      (1000)     4475 2024-04-22 20:56:22.000000 plover-sound-0.0.3/plover_sound/icon.svg
+-rw-r--r--   0 zach      (1000) zach      (1000)    23359 2024-04-21 02:07:30.000000 plover-sound-0.0.3/plover_sound/keyboard-click.mp3
+-rw-r--r--   0 zach      (1000) zach      (1000)     5020 2024-04-22 21:09:54.000000 plover-sound-0.0.3/plover_sound/tool.py
+drwxr-xr-x   0 zach      (1000) zach      (1000)        0 2024-04-22 22:36:16.435228 plover-sound-0.0.3/plover_sound.egg-info/
+-rw-r--r--   0 zach      (1000) zach      (1000)      887 2024-04-22 22:36:16.000000 plover-sound-0.0.3/plover_sound.egg-info/PKG-INFO
+-rw-r--r--   0 zach      (1000) zach      (1000)      423 2024-04-22 22:36:16.000000 plover-sound-0.0.3/plover_sound.egg-info/SOURCES.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 22:36:16.000000 plover-sound-0.0.3/plover_sound.egg-info/dependency_links.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)      144 2024-04-22 22:36:16.000000 plover-sound-0.0.3/plover_sound.egg-info/entry_points.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)       54 2024-04-22 22:36:16.000000 plover-sound-0.0.3/plover_sound.egg-info/requires.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)       13 2024-04-22 22:36:16.000000 plover-sound-0.0.3/plover_sound.egg-info/top_level.txt
+-rw-r--r--   0 zach      (1000) zach      (1000)        1 2024-04-22 18:01:37.000000 plover-sound-0.0.3/plover_sound.egg-info/zip-safe
+-rw-r--r--   0 zach      (1000) zach      (1000)      731 2024-04-22 22:36:16.435228 plover-sound-0.0.3/setup.cfg
+-rw-r--r--   0 zach      (1000) zach      (1000)       38 2024-04-22 21:40:47.000000 plover-sound-0.0.3/setup.py
```

### Comparing `plover-sound-0.0.2/LICENSE` & `plover-sound-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plover-sound-0.0.2/PKG-INFO` & `plover-sound-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: plover-sound
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plays sound when stroke is registered
+Home-page: https://github.com/raoeus/plover-sound
 Author: Zach Rice
 Author-email: bynxmusic@gmail.com
-License: GNU General Public License v2 or later (GPLv2+)
+License: MIT
 Keywords: plover plover_plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover[gui_qt]>=4.0.0.rc2
 Requires-Dist: pygame>=2.5.2
 Requires-Dist: numpy>=1.26.4
```

### Comparing `plover-sound-0.0.2/plover_sound/extension.py` & `plover-sound-0.0.3/plover_sound/extension.py`

 * *Files identical despite different names*

### Comparing `plover-sound-0.0.2/plover_sound/tool.py` & `plover-sound-0.0.3/plover_sound/tool.py`

 * *Files identical despite different names*

### Comparing `plover-sound-0.0.2/plover_sound.egg-info/PKG-INFO` & `plover-sound-0.0.3/plover_sound.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: plover-sound
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plays sound when stroke is registered
+Home-page: https://github.com/raoeus/plover-sound
 Author: Zach Rice
 Author-email: bynxmusic@gmail.com
-License: GNU General Public License v2 or later (GPLv2+)
+License: MIT
 Keywords: plover plover_plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover[gui_qt]>=4.0.0.rc2
 Requires-Dist: pygame>=2.5.2
 Requires-Dist: numpy>=1.26.4
```

### Comparing `plover-sound-0.0.2/setup.cfg` & `plover-sound-0.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [metadata]
 name = plover-sound
-version = 0.0.2
+version = 0.0.3
 description = Plays sound when stroke is registered
 author = Zach Rice
 author_email = bynxmusic@gmail.com
-license = GNU General Public License v2 or later (GPLv2+)
+license = MIT
+url = https://github.com/raoeus/plover-sound
 keywords = plover plover_plugin
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = True
 setup_requires =
```

