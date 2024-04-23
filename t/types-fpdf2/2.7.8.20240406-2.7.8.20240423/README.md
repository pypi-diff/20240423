# Comparing `tmp/types-fpdf2-2.7.8.20240406.tar.gz` & `tmp/types-fpdf2-2.7.8.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-fpdf2-2.7.8.20240406.tar", last modified: Sat Apr  6 02:13:28 2024, max compression
+gzip compressed data, was "types-fpdf2-2.7.8.20240423.tar", last modified: Tue Apr 23 02:19:52 2024, max compression
```

## Comparing `types-fpdf2-2.7.8.20240406.tar` & `types-fpdf2-2.7.8.20240423.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:28.154627 types-fpdf2-2.7.8.20240406/
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-06 02:13:27.000000 types-fpdf2-2.7.8.20240406/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-06 02:13:27.000000 types-fpdf2-2.7.8.20240406/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-06 02:13:28.154627 types-fpdf2-2.7.8.20240406/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:28.154627 types-fpdf2-2.7.8.20240406/fpdf-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 02:13:27.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/_fonttools_shims.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/annotations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/bidi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/deprecation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15139 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/encryption.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/fpdf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/graphics_state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/image_datastructures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/image_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/line_break.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/linearization.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/outline.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/output.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/prefs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:27.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/recorder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/sign.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/structure_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/svg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/syntax.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/template.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/text_region.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/transitions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-06 02:12:57.000000 types-fpdf2-2.7.8.20240406/fpdf-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:13:28.154627 types-fpdf2-2.7.8.20240406/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-06 02:13:27.000000 types-fpdf2-2.7.8.20240406/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:28.154627 types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-06 02:13:28.000000 types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-06 02:13:28.000000 types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:13:28.000000 types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 02:13:28.000000 types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 02:13:28.000000 types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/fpdf-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/_fonttools_shims.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/annotations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/bidi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15139 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/encryption.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/fpdf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/graphics_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/image_datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/image_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/line_break.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/linearization.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/outline.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/output.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/prefs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/sign.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/structure_tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/svg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/syntax.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/text_region.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/transitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/top_level.txt
```

### Comparing `types-fpdf2-2.7.8.20240406/CHANGELOG.md` & `types-fpdf2-2.7.8.20240423/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 2.7.8.20240423 (2024-04-23)
+
+Add precise values for enum members where possible (#11299)
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+Co-authored-by: Alex Waygood <alex.waygood@gmail.com>
+
 ## 2.7.8.20240406 (2024-04-06)
 
 Depend on Pillow instead of types-Pillow (#11720)
 
 ## 2.7.8.20240331 (2024-03-31)
 
 Remove bare Incomplete annotations in third-party stubs (#11671)
```

### Comparing `types-fpdf2-2.7.8.20240406/PKG-INFO` & `types-fpdf2-2.7.8.20240423/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.7.8.20240406
+Version: 2.7.8.20240423
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-fpdf2` aims to provide accurate annotations
 for `fpdf2==2.7.8`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/__init__.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/_fonttools_shims.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/_fonttools_shims.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/actions.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/actions.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/annotations.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/annotations.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/bidi.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/bidi.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/drawing.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/drawing.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/encryption.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/encryption.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/fonts.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/fonts.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/fpdf.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/fpdf.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/graphics_state.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/graphics_state.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/html.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/html.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/image_datastructures.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/image_datastructures.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/image_parsing.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/image_parsing.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/line_break.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/line_break.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/linearization.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/linearization.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/outline.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/outline.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/output.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/output.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/prefs.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/prefs.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/sign.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/sign.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/structure_tree.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/structure_tree.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/svg.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/svg.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/syntax.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/syntax.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/table.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/table.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/template.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/template.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/text_region.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/text_region.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/transitions.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/transitions.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/fpdf-stubs/util.pyi` & `types-fpdf2-2.7.8.20240423/fpdf-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240406/setup.py` & `types-fpdf2-2.7.8.20240423/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-fpdf2` aims to provide accurate annotations
 for `fpdf2==2.7.8`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.7.8.20240406",
+      version="2.7.8.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md",
```

### Comparing `types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/PKG-INFO` & `types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.7.8.20240406
+Version: 2.7.8.20240423
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-fpdf2` aims to provide accurate annotations
 for `fpdf2==2.7.8`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-fpdf2-2.7.8.20240406/types_fpdf2.egg-info/SOURCES.txt` & `types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

