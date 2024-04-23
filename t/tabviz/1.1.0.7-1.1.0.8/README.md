# Comparing `tmp/tabviz-1.1.0.7.tar.gz` & `tmp/tabviz-1.1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabviz-1.1.0.7.tar", max compression
+gzip compressed data, was "tabviz-1.1.0.8.tar", max compression
```

## Comparing `tabviz-1.1.0.7.tar` & `tabviz-1.1.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.7/LICENSE
--rw-r--r--   0        0        0     8638 2024-04-23 10:23:06.698047 tabviz-1.1.0.7/pyproject.toml
--rw-r--r--   0        0        0      544 2024-04-23 10:21:04.060281 tabviz-1.1.0.7/README.md
--rw-r--r--   0        0        0      114 2024-04-23 10:09:07.303426 tabviz-1.1.0.7/tabviz/__init__.py
--rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.7/tabviz/static/example.twbx
--rw-r--r--   0        0        0    14561 2024-04-23 10:09:07.308913 tabviz-1.1.0.7/tabviz/tabvizmain.py
--rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 tabviz-1.1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.8/LICENSE
+-rw-r--r--   0        0        0     1162 2024-04-23 10:29:07.234564 tabviz-1.1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      544 2024-04-23 10:21:04.060281 tabviz-1.1.0.8/README.md
+-rw-r--r--   0        0        0      114 2024-04-23 10:09:07.303426 tabviz-1.1.0.8/tabviz/__init__.py
+-rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.8/tabviz/static/example.twbx
+-rw-r--r--   0        0        0    14561 2024-04-23 10:09:07.308913 tabviz-1.1.0.8/tabviz/tabvizmain.py
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 tabviz-1.1.0.8/PKG-INFO
```

### Comparing `tabviz-1.1.0.7/LICENSE` & `tabviz-1.1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.7/README.md` & `tabviz-1.1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.7/tabviz/static/example.twbx` & `tabviz-1.1.0.8/tabviz/static/example.twbx`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.7/tabviz/tabvizmain.py` & `tabviz-1.1.0.8/tabviz/tabvizmain.py`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.7/PKG-INFO` & `tabviz-1.1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabviz
-Version: 1.1.0.7
+Version: 1.1.0.8
 Summary: A Python module for working with the Tableau
 License: GNU
 Author: Ayush Dhiman
 Author-email: ayushdhiman272@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

