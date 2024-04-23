# Comparing `tmp/tabviz-1.1.0.5.tar.gz` & `tmp/tabviz-1.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabviz-1.1.0.5.tar", max compression
+gzip compressed data, was "tabviz-1.1.0.6.tar", max compression
```

## Comparing `tabviz-1.1.0.5.tar` & `tabviz-1.1.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.5/LICENSE
--rw-r--r--   0        0        0     8638 2024-04-23 09:55:23.632400 tabviz-1.1.0.5/pyproject.toml
--rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.5/README.md
--rw-r--r--   0        0        0     2157 2024-04-23 09:55:23.615400 tabviz-1.1.0.5/tabviz/__init__.py
--rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.5/tabviz/static/example.twbx
--rw-r--r--   0        0        0    14559 2024-04-12 13:45:46.447914 tabviz-1.1.0.5/tabviz/tabvizmain.py
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 tabviz-1.1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.6/LICENSE
+-rw-r--r--   0        0        0     8638 2024-04-23 10:10:11.920987 tabviz-1.1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.6/README.md
+-rw-r--r--   0        0        0      114 2024-04-23 10:09:07.303426 tabviz-1.1.0.6/tabviz/__init__.py
+-rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.6/tabviz/static/example.twbx
+-rw-r--r--   0        0        0    14561 2024-04-23 10:09:07.308913 tabviz-1.1.0.6/tabviz/tabvizmain.py
+-rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 tabviz-1.1.0.6/PKG-INFO
```

### Comparing `tabviz-1.1.0.5/LICENSE` & `tabviz-1.1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.5/pyproject.toml` & `tabviz-1.1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tabviz"
-version = "1.1.0.5"
+version = "1.1.0.6"
 description = "A Python module for working with the Tableau"
 authors = ["Ayush Dhiman <ayushdhiman272@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `tabviz-1.1.0.5/tabviz/static/example.twbx` & `tabviz-1.1.0.6/tabviz/static/example.twbx`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.5/tabviz/tabvizmain.py` & `tabviz-1.1.0.6/tabviz/tabvizmain.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,14 @@
 from IPython.display import display, HTML
 import importlib.resources
 import pandas as pd
 import random
 import string
 import hashlib
 
-file_in_static_folder = importlib.resources.files('tabviz').joinpath(os.path.join('static', 'example.twbx'))
-destination_folder = os.getcwd()
-tabviz_folder = os.path.join(destination_folder, 'tabviz')
-if not os.path.exists(tabviz_folder):
-    os.makedirs(tabviz_folder)
-destination_file = os.path.join(tabviz_folder, "example.twbx")
-shutil.copy(file_in_static_folder, destination_file)
-
 
 def tableau_online_signin(site,site_id,token_name,token_secret,api_version):
     signin_url = f'https://{site}/api/{api_version}/auth/signin'
     signin_xml = f'''
     <tsRequest>
       <credentials personalAccessTokenName="{token_name}" personalAccessTokenSecret="{token_secret}">
         <site contentUrl="{site_id}" />
@@ -324,14 +316,23 @@
     replace_table_contents_with_xml_data_for_columns(xml_file,xml_column_data)
     process_file_repack(tabviz_folder)
     workbook_name = generate_random_text(5)
     url = construct_url(site, site_id, workbook_name)
     publish_workbook(token_name,token_secret, site_id, project_id, workbook_name, path_to_workbook,site)
     display_tableau_viz(url)
 
+file_in_static_folder = importlib.resources.files('tabviz').joinpath(os.path.join('static', 'example.twbx'))
+destination_folder = os.getcwd()
+tabviz_folder = os.path.join(destination_folder, 'tabviz')
+if not os.path.exists(tabviz_folder):
+    os.makedirs(tabviz_folder)
+destination_file = os.path.join(tabviz_folder, "example.twbx")
+shutil.copy(file_in_static_folder, destination_file)
+
+
 project_id = " "
 destination_file = os.path.join(tabviz_folder, "example.twbx")
 xml_file = os.path.join(tabviz_folder, "tabviz","example.xml")
 dataset = os.path.join(tabviz_folder, "tabviz", "Data", "1vib26g1r4ena71b8a85o12srz3b", "Product.csv")
 path_to_workbook = os.path.join(tabviz_folder, "..", "Data.twbx")
 table_contents = ""
 table_contents_column = ""
```

### Comparing `tabviz-1.1.0.5/PKG-INFO` & `tabviz-1.1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabviz
-Version: 1.1.0.5
+Version: 1.1.0.6
 Summary: A Python module for working with the Tableau
 License: GNU
 Author: Ayush Dhiman
 Author-email: ayushdhiman272@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

