# Comparing `tmp/tabviz-1.1.0.6.tar.gz` & `tmp/tabviz-1.1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabviz-1.1.0.6.tar", max compression
+gzip compressed data, was "tabviz-1.1.0.7.tar", max compression
```

## Comparing `tabviz-1.1.0.6.tar` & `tabviz-1.1.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.6/LICENSE
--rw-r--r--   0        0        0     8638 2024-04-23 10:10:11.920987 tabviz-1.1.0.6/pyproject.toml
--rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.6/README.md
--rw-r--r--   0        0        0      114 2024-04-23 10:09:07.303426 tabviz-1.1.0.6/tabviz/__init__.py
--rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.6/tabviz/static/example.twbx
--rw-r--r--   0        0        0    14561 2024-04-23 10:09:07.308913 tabviz-1.1.0.6/tabviz/tabvizmain.py
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 tabviz-1.1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.7/LICENSE
+-rw-r--r--   0        0        0     8638 2024-04-23 10:23:06.698047 tabviz-1.1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      544 2024-04-23 10:21:04.060281 tabviz-1.1.0.7/README.md
+-rw-r--r--   0        0        0      114 2024-04-23 10:09:07.303426 tabviz-1.1.0.7/tabviz/__init__.py
+-rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.7/tabviz/static/example.twbx
+-rw-r--r--   0        0        0    14561 2024-04-23 10:09:07.308913 tabviz-1.1.0.7/tabviz/tabvizmain.py
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 tabviz-1.1.0.7/PKG-INFO
```

### Comparing `tabviz-1.1.0.6/LICENSE` & `tabviz-1.1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.6/pyproject.toml` & `tabviz-1.1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tabviz"
-version = "1.1.0.6"
+version = "1.1.0.7"
 description = "A Python module for working with the Tableau"
 authors = ["Ayush Dhiman <ayushdhiman272@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `tabviz-1.1.0.6/tabviz/static/example.twbx` & `tabviz-1.1.0.7/tabviz/static/example.twbx`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.6/tabviz/tabvizmain.py` & `tabviz-1.1.0.7/tabviz/tabvizmain.py`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.6/PKG-INFO` & `tabviz-1.1.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabviz
-Version: 1.1.0.6
+Version: 1.1.0.7
 Summary: A Python module for working with the Tableau
 License: GNU
 Author: Ayush Dhiman
 Author-email: ayushdhiman272@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -28,7 +28,11 @@
 poetry build
 ```
 
 ```bash
 poetry publish
 ```
 
+
+# Demo
+
+Try out the demo on [Google Colab](https://colab.research.google.com/drive/1yj_0_T4KUBrWdvrg9TDFUzhavnHZ2Wqe?usp=sharing)
```

