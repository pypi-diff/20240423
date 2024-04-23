# Comparing `tmp/wagtail_tabbed_structblock-0.0.5.tar.gz` & `tmp/wagtail_tabbed_structblock-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_tabbed_structblock-0.0.5.tar", max compression
+gzip compressed data, was "wagtail_tabbed_structblock-0.0.6.tar", max compression
```

## Comparing `wagtail_tabbed_structblock-0.0.5.tar` & `wagtail_tabbed_structblock-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1059 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/README.md
--rw-r--r--   0        0        0      323 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/README.md
--rw-r--r--   0        0        0        0 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/__init__.py
--rw-r--r--   0        0        0      167 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/apps.py
--rw-r--r--   0        0        0     1099 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/blocks.py
--rw-r--r--   0        0        0        0 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/migrations/__init__.py
--rw-r--r--   0        0        0    48673 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/poetry.lock
--rw-r--r--   0        0        0      436 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/pyproject.toml
--rw-r--r--   0        0        0      432 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/setup.py
--rw-r--r--   0        0        0      722 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css
--rw-r--r--   0        0        0     1554 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js
--rw-r--r--   0        0        0     1507 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html
--rw-r--r--   0        0        0       60 2024-04-23 20:04:53.129669 wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/tests.py
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 wagtail_tabbed_structblock-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/README.md
+-rw-r--r--   0        0        0      323 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/apps.py
+-rw-r--r--   0        0        0     1099 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/blocks.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/migrations/__init__.py
+-rw-r--r--   0        0        0    48673 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/poetry.lock
+-rw-r--r--   0        0        0      436 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/pyproject.toml
+-rw-r--r--   0        0        0      451 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/setup.py
+-rw-r--r--   0        0        0      722 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css
+-rw-r--r--   0        0        0     1554 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js
+-rw-r--r--   0        0        0     1507 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html
+-rw-r--r--   0        0        0       60 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/tests.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 wagtail_tabbed_structblock-0.0.6/PKG-INFO
```

### Comparing `wagtail_tabbed_structblock-0.0.5/README.md` & `wagtail_tabbed_structblock-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/blocks.py` & `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/poetry.lock` & `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/poetry.lock`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css` & `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js` & `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.5/src/tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html` & `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.5/PKG-INFO` & `wagtail_tabbed_structblock-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-tabbed-structblock
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Eric Kersten
 Author-email: eric.kersten@egodesign.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

