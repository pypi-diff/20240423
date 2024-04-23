# Comparing `tmp/msg2po-1.2.0.tar.gz` & `tmp/msg2po-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msg2po-1.2.0.tar", max compression
+gzip compressed data, was "msg2po-1.2.1.tar", max compression
```

## Comparing `msg2po-1.2.0.tar` & `msg2po-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2038 2024-04-22 04:13:33.754976 msg2po-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/__init__.py
--rwxr-xr-x   0        0        0     1623 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/bgforge_config.py
--rw-r--r--   0        0        0      511 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/common.py
--rw-r--r--   0        0        0     2364 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/config.py
--rw-r--r--   0        0        0    32070 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/core.py
--rwxr-xr-x   0        0        0      746 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/diff_male_female_po_to_csv.py
--rwxr-xr-x   0        0        0     4017 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/dir2msgstr.py
--rwxr-xr-x   0        0        0     1162 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/female_csv2po.py
--rwxr-xr-x   0        0        0     1334 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/file2msgstr.py
--rwxr-xr-x   0        0        0      731 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/file2po.py
--rwxr-xr-x   0        0        0     1756 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/lowercase.py
--rwxr-xr-x   0        0        0     2447 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/msgmerge.py
--rwxr-xr-x   0        0        0      892 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/po2file.py
--rwxr-xr-x   0        0        0     4659 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/poify.py
--rwxr-xr-x   0        0        0      702 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/resave_po.py
--rwxr-xr-x   0        0        0     2193 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unfuzzy.py
--rw-r--r--   0        0        0     1336 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unfuzzy.yml
--rwxr-xr-x   0        0        0     1122 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unfuzzy_cassidy.py
--rwxr-xr-x   0        0        0     2272 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unpoify.py
--rw-r--r--   0        0        0     1218 2024-04-22 04:13:33.754976 msg2po-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 msg2po-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2038 2024-04-23 10:40:25.133746 msg2po-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 10:40:25.133746 msg2po-1.2.1/msg2po/__init__.py
+-rwxr-xr-x   0        0        0     1623 2024-04-23 10:40:25.133746 msg2po-1.2.1/msg2po/bgforge_config.py
+-rw-r--r--   0        0        0      511 2024-04-23 10:40:25.133746 msg2po-1.2.1/msg2po/common.py
+-rw-r--r--   0        0        0     2364 2024-04-23 10:40:25.133746 msg2po-1.2.1/msg2po/config.py
+-rw-r--r--   0        0        0    32098 2024-04-23 10:40:25.133746 msg2po-1.2.1/msg2po/core.py
+-rwxr-xr-x   0        0        0      746 2024-04-23 10:40:25.133746 msg2po-1.2.1/msg2po/diff_male_female_po_to_csv.py
+-rwxr-xr-x   0        0        0     4017 2024-04-23 10:40:25.133746 msg2po-1.2.1/msg2po/dir2msgstr.py
+-rwxr-xr-x   0        0        0     1162 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/female_csv2po.py
+-rwxr-xr-x   0        0        0     1334 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/file2msgstr.py
+-rwxr-xr-x   0        0        0      731 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/file2po.py
+-rwxr-xr-x   0        0        0     1756 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/lowercase.py
+-rwxr-xr-x   0        0        0     2447 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/msgmerge.py
+-rwxr-xr-x   0        0        0      892 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/po2file.py
+-rwxr-xr-x   0        0        0     4659 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/poify.py
+-rwxr-xr-x   0        0        0      702 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/resave_po.py
+-rwxr-xr-x   0        0        0     2193 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/unfuzzy.py
+-rw-r--r--   0        0        0     1336 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/unfuzzy.yml
+-rwxr-xr-x   0        0        0     1122 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/unfuzzy_cassidy.py
+-rwxr-xr-x   0        0        0     2272 2024-04-23 10:40:25.137745 msg2po-1.2.1/msg2po/unpoify.py
+-rw-r--r--   0        0        0     1218 2024-04-23 10:40:25.137745 msg2po-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 msg2po-1.2.1/PKG-INFO
```

### Comparing `msg2po-1.2.0/README.md` & `msg2po-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/bgforge_config.py` & `msg2po-1.2.1/msg2po/bgforge_config.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/config.py` & `msg2po-1.2.1/msg2po/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ruamel.yaml
 import sys
 import os
 
-VERSION = "1.2.0"
+VERSION = "1.2.1"
 
 
 class Config:
     def __init__(self):
         yml = ".bgforge.yml"
         translation_defaults = {
             "encoding": "cp1252",
```

### Comparing `msg2po-1.2.0/msg2po/core.py` & `msg2po-1.2.1/msg2po/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -842,14 +842,15 @@
         "pt_br": "portuguese",
         "it": "italian",
         "pl": "polish",
         "es": "spanish",
         "ru": "russian",
         "sv": "swedish",
         "uk": "ukrainian",
+        "vi": "vietnamese",
     }
     slug = strip_ext(basename(po_filename)).lower()
     if CONFIG.simple_languages:
         try:
             slug = slug_map[slug]
         except:
             pass
```

### Comparing `msg2po-1.2.0/msg2po/diff_male_female_po_to_csv.py` & `msg2po-1.2.1/msg2po/diff_male_female_po_to_csv.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/dir2msgstr.py` & `msg2po-1.2.1/msg2po/dir2msgstr.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/female_csv2po.py` & `msg2po-1.2.1/msg2po/female_csv2po.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/file2msgstr.py` & `msg2po-1.2.1/msg2po/file2msgstr.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/file2po.py` & `msg2po-1.2.1/msg2po/file2po.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/lowercase.py` & `msg2po-1.2.1/msg2po/lowercase.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/msgmerge.py` & `msg2po-1.2.1/msg2po/msgmerge.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/po2file.py` & `msg2po-1.2.1/msg2po/po2file.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/poify.py` & `msg2po-1.2.1/msg2po/poify.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/resave_po.py` & `msg2po-1.2.1/msg2po/resave_po.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/unfuzzy.py` & `msg2po-1.2.1/msg2po/unfuzzy.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/unfuzzy.yml` & `msg2po-1.2.1/msg2po/unfuzzy.yml`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/unfuzzy_cassidy.py` & `msg2po-1.2.1/msg2po/unfuzzy_cassidy.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/msg2po/unpoify.py` & `msg2po-1.2.1/msg2po/unpoify.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.2.0/pyproject.toml` & `msg2po-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msg2po"
-version = "1.2.0"
+version = "1.2.1"
 description = "A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back."
 authors = ["BGforge <dev@bgforge.net>"]
 keywords = ["Fallout", "Fallout 2", "Baldur's Gate", "Infinity Engine", "WeiDU"]
 readme = "README.md"
 homepage = "https://github.com/BGforgeNet/msg2po"
 repository = "https://github.com/BGforgeNet/msg2po"
```

### Comparing `msg2po-1.2.0/PKG-INFO` & `msg2po-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msg2po
-Version: 1.2.0
+Version: 1.2.1
 Summary: A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back.
 Home-page: https://github.com/BGforgeNet/msg2po
 Keywords: Fallout,Fallout 2,Baldur's Gate,Infinity Engine,WeiDU
 Author: BGforge
 Author-email: dev@bgforge.net
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
```

