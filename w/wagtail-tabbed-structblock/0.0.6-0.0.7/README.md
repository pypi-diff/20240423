# Comparing `tmp/wagtail_tabbed_structblock-0.0.6.tar.gz` & `tmp/wagtail_tabbed_structblock-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_tabbed_structblock-0.0.6.tar", max compression
+gzip compressed data, was "wagtail_tabbed_structblock-0.0.7.tar", max compression
```

## Comparing `wagtail_tabbed_structblock-0.0.6.tar` & `wagtail_tabbed_structblock-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1059 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/README.md
--rw-r--r--   0        0        0      323 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/README.md
--rw-r--r--   0        0        0        0 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/__init__.py
--rw-r--r--   0        0        0      167 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/apps.py
--rw-r--r--   0        0        0     1099 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/blocks.py
--rw-r--r--   0        0        0        0 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/migrations/__init__.py
--rw-r--r--   0        0        0    48673 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/poetry.lock
--rw-r--r--   0        0        0      436 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/pyproject.toml
--rw-r--r--   0        0        0      451 2024-04-23 20:14:43.094055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/setup.py
--rw-r--r--   0        0        0      722 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css
--rw-r--r--   0        0        0     1554 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js
--rw-r--r--   0        0        0     1507 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html
--rw-r--r--   0        0        0       60 2024-04-23 20:14:43.098055 wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/tests.py
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 wagtail_tabbed_structblock-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/README.md
+-rw-r--r--   0        0        0      346 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/apps.py
+-rw-r--r--   0        0        0     1099 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/blocks.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/migrations/__init__.py
+-rw-r--r--   0        0        0    48673 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/poetry.lock
+-rw-r--r--   0        0        0      436 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/pyproject.toml
+-rw-r--r--   0        0        0      377 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/setup.py
+-rw-r--r--   0        0        0      722 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css
+-rw-r--r--   0        0        0     1554 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js
+-rw-r--r--   0        0        0     1507 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html
+-rw-r--r--   0        0        0       60 2024-04-23 20:25:06.531940 wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/tests.py
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 wagtail_tabbed_structblock-0.0.7/PKG-INFO
```

### Comparing `wagtail_tabbed_structblock-0.0.6/README.md` & `wagtail_tabbed_structblock-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 As custom blocks grow in fields it becomes necessary to group and hide some of the block fields. Tabbed StrucBlock allows such grouping into a tabbed UI.
 
 
 ## Installation
 
 1. Install the package with `pip install wagtail-tabbed-strucblock`.
-2. Add to `INSTALLED_ADD` as `tabbed_structblock`.
+2. Add to `INSTALLED_ADD` as `wagtail_tabbed_structblock`.
 
 
 ## Usage
 
-1. Import the class with `from tabbed_structblock.blocks import TabbedStructBlock`.
+1. Import the class with `from wagtail_tabbed_structblock.blocks import TabbedStructBlock`.
 2. Create your `StructBlock` as usual extending `TabbedStructBlock`.
 3. Define the tabs in the `Meta` class of the block as shown in the example below.
 
 ```python
 from wagtail import blocks
 
-from tabbed_structblock.blocks import TabbedStructBlock
+from wagtail_tabbed_structblock.blocks import TabbedStructBlock
 
 
 class ExampleBlock(TabbedStructBlock):
     title = blocks.CharBlock()
     content = blocks.RichTextBlock()
```

### Comparing `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/blocks.py` & `wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/poetry.lock` & `wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/poetry.lock`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css` & `wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/static/tabbed_structblock/css/tabbed_structblock.css`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js` & `wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/static/tabbed_structblock/js/tabbed_structblock.js`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.6/src/tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html` & `wagtail_tabbed_structblock-0.0.7/wagtail_tabbed_structblock/templates/tabbed_structblock/tabbed_struct_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_tabbed_structblock-0.0.6/PKG-INFO` & `wagtail_tabbed_structblock-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-tabbed-structblock
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Eric Kersten
 Author-email: eric.kersten@egodesign.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,27 +16,27 @@
 
 As custom blocks grow in fields it becomes necessary to group and hide some of the block fields. Tabbed StrucBlock allows such grouping into a tabbed UI.
 
 
 ## Installation
 
 1. Install the package with `pip install wagtail-tabbed-strucblock`.
-2. Add to `INSTALLED_ADD` as `tabbed_structblock`.
+2. Add to `INSTALLED_ADD` as `wagtail_tabbed_structblock`.
 
 
 ## Usage
 
-1. Import the class with `from tabbed_structblock.blocks import TabbedStructBlock`.
+1. Import the class with `from wagtail_tabbed_structblock.blocks import TabbedStructBlock`.
 2. Create your `StructBlock` as usual extending `TabbedStructBlock`.
 3. Define the tabs in the `Meta` class of the block as shown in the example below.
 
 ```python
 from wagtail import blocks
 
-from tabbed_structblock.blocks import TabbedStructBlock
+from wagtail_tabbed_structblock.blocks import TabbedStructBlock
 
 
 class ExampleBlock(TabbedStructBlock):
     title = blocks.CharBlock()
     content = blocks.RichTextBlock()
```

