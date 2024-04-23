# Comparing `tmp/tabviz-1.1.0.4.tar.gz` & `tmp/tabviz-1.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabviz-1.1.0.4.tar", max compression
+gzip compressed data, was "tabviz-1.1.0.5.tar", max compression
```

## Comparing `tabviz-1.1.0.4.tar` & `tabviz-1.1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.4/LICENSE
--rw-r--r--   0        0        0     8638 2024-04-23 09:50:16.208896 tabviz-1.1.0.4/pyproject.toml
--rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.4/README.md
--rw-r--r--   0        0        0     2153 2024-04-23 09:49:12.985507 tabviz-1.1.0.4/tabviz/__init__.py
--rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.4/tabviz/static/example.twbx
--rw-r--r--   0        0        0    14559 2024-04-12 13:45:46.447914 tabviz-1.1.0.4/tabviz/tabvizmain.py
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 tabviz-1.1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.5/LICENSE
+-rw-r--r--   0        0        0     8638 2024-04-23 09:55:23.632400 tabviz-1.1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.5/README.md
+-rw-r--r--   0        0        0     2157 2024-04-23 09:55:23.615400 tabviz-1.1.0.5/tabviz/__init__.py
+-rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.5/tabviz/static/example.twbx
+-rw-r--r--   0        0        0    14559 2024-04-12 13:45:46.447914 tabviz-1.1.0.5/tabviz/tabvizmain.py
+-rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 tabviz-1.1.0.5/PKG-INFO
```

### Comparing `tabviz-1.1.0.4/LICENSE` & `tabviz-1.1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.4/pyproject.toml` & `tabviz-1.1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tabviz"
-version = "1.1.0.4"
+version = "1.1.0.5"
 description = "A Python module for working with the Tableau"
 authors = ["Ayush Dhiman <ayushdhiman272@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `tabviz-1.1.0.4/tabviz/__init__.py` & `tabviz-1.1.0.5/tabviz/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from starlette import status as status
 import importlib
 import os
 import shutil
-from .tabviz import main
+from .tabvizmain import main
 
 
 file_in_static_folder = importlib.resources.files('tabviz').joinpath(os.path.join('static', 'example.twbx'))
 destination_folder = os.getcwd()
 tabviz_folder = os.path.join(destination_folder, 'tabviz')
 if not os.path.exists(tabviz_folder):
     os.makedirs(tabviz_folder)
```

### Comparing `tabviz-1.1.0.4/tabviz/static/example.twbx` & `tabviz-1.1.0.5/tabviz/static/example.twbx`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.4/tabviz/tabvizmain.py` & `tabviz-1.1.0.5/tabviz/tabvizmain.py`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.4/PKG-INFO` & `tabviz-1.1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabviz
-Version: 1.1.0.4
+Version: 1.1.0.5
 Summary: A Python module for working with the Tableau
 License: GNU
 Author: Ayush Dhiman
 Author-email: ayushdhiman272@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

