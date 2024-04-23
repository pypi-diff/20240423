# Comparing `tmp/tabviz-1.1.0.3.tar.gz` & `tmp/tabviz-1.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabviz-1.1.0.3.tar", max compression
+gzip compressed data, was "tabviz-1.1.0.4.tar", max compression
```

## Comparing `tabviz-1.1.0.3.tar` & `tabviz-1.1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.3/LICENSE
--rw-r--r--   0        0        0     8615 2024-04-12 13:45:46.456443 tabviz-1.1.0.3/pyproject.toml
--rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-03-19 00:43:43.742786 tabviz-1.1.0.3/tabviz/__init__.py
--rw-r--r--   0        0        0    14559 2024-04-12 13:45:46.447914 tabviz-1.1.0.3/tabviz/__main__.py
--rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.3/tabviz/static/example.twbx
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 tabviz-1.1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.4/LICENSE
+-rw-r--r--   0        0        0     8638 2024-04-23 09:50:16.208896 tabviz-1.1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.4/README.md
+-rw-r--r--   0        0        0     2153 2024-04-23 09:49:12.985507 tabviz-1.1.0.4/tabviz/__init__.py
+-rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.4/tabviz/static/example.twbx
+-rw-r--r--   0        0        0    14559 2024-04-12 13:45:46.447914 tabviz-1.1.0.4/tabviz/tabvizmain.py
+-rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 tabviz-1.1.0.4/PKG-INFO
```

### Comparing `tabviz-1.1.0.3/LICENSE` & `tabviz-1.1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.3/pyproject.toml` & `tabviz-1.1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tabviz"
-version = "1.1.0.3"
+version = "1.1.0.4"
 description = "A Python module for working with the Tableau"
 authors = ["Ayush Dhiman <ayushdhiman272@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tableauserverclient = "^0.30"
+starlette = "^0.37.2"
 
 [tool.poetry.dev-dependencies]
 argparse = "^1.4.0"
 black = "23.7"
 mock = "^4.0.3"
 mypy = "1.4"
 pytest = "^7.0"
```

### Comparing `tabviz-1.1.0.3/tabviz/__main__.py` & `tabviz-1.1.0.4/tabviz/tabvizmain.py`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.3/tabviz/static/example.twbx` & `tabviz-1.1.0.4/tabviz/static/example.twbx`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.3/PKG-INFO` & `tabviz-1.1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tabviz
-Version: 1.1.0.3
+Version: 1.1.0.4
 Summary: A Python module for working with the Tableau
 License: GNU
 Author: Ayush Dhiman
 Author-email: ayushdhiman272@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: starlette (>=0.37.2,<0.38.0)
 Requires-Dist: tableauserverclient (>=0.30,<0.31)
 Description-Content-Type: text/markdown
 
 # Tabviz
 
 TabViz is a [pip library](https://pypi.org/project/tabviz/) which simplifies the process of creating interactive data visualization in your jupyter notebook automatically using tableau and Gen-AI, all you have to do is provide a dataset(in csv)  and wait for TabViz to generate you a useful enough visualization.
```

