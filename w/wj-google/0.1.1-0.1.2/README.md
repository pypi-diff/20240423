# Comparing `tmp/wj_google-0.1.1.tar.gz` & `tmp/wj_google-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wj_google-0.1.1.tar", max compression
+gzip compressed data, was "wj_google-0.1.2.tar", max compression
```

## Comparing `wj_google-0.1.1.tar` & `wj_google-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     5764 2024-04-19 01:01:58.122781 wj_google-0.1.1/README.md
--rw-r--r--   0        0        0      602 2024-04-19 01:01:58.122781 wj_google-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 01:01:58.144780 wj_google-0.1.1/wj_google/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 01:01:58.145781 wj_google-0.1.1/wj_google/examples/__init__.py
--rw-r--r--   0        0        0     1961 2024-04-19 01:01:58.123781 wj_google-0.1.1/wj_google/examples/bigquery.py
--rw-r--r--   0        0        0     2736 2024-04-19 01:01:58.123781 wj_google-0.1.1/wj_google/examples/sorage_and_drive.py
--rw-r--r--   0        0        0     1522 2024-04-19 01:01:58.123781 wj_google-0.1.1/wj_google/google_api/Google.py
--rw-r--r--   0        0        0        0 2024-04-19 01:01:58.145781 wj_google-0.1.1/wj_google/google_api/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-19 01:01:58.123781 wj_google-0.1.1/wj_google/google_api/google_api.py
--rw-r--r--   0        0        0        0 2024-04-19 01:01:58.145781 wj_google-0.1.1/wj_google/google_cloud/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-19 01:01:58.123781 wj_google-0.1.1/wj_google/google_cloud/cloud_connector.py
--rw-r--r--   0        0        0     3227 2024-04-19 01:01:58.123781 wj_google-0.1.1/wj_google/main.py
--rw-r--r--   0        0        0        0 2024-04-19 01:01:58.145781 wj_google-0.1.1/wj_google/tools/__init__.py
--rw-r--r--   0        0        0      384 2024-04-19 01:01:58.123781 wj_google-0.1.1/wj_google/tools/files_manage.py
--rw-r--r--   0        0        0     6641 1970-01-01 00:00:00.000000 wj_google-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5429 2024-04-23 01:58:59.402346 wj_google-0.1.2/README.md
+-rw-r--r--   0        0        0      584 2024-04-23 01:58:59.402346 wj_google-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/examples/__init__.py
+-rw-r--r--   0        0        0     1961 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/examples/bigquery.py
+-rw-r--r--   0        0        0     2736 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/examples/sorage_and_drive.py
+-rw-r--r--   0        0        0     1522 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/google_api/Google.py
+-rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/google_api/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/google_api/google_api.py
+-rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/google_cloud/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/google_cloud/cloud_connector.py
+-rw-r--r--   0        0        0     3227 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/main.py
+-rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/tools/__init__.py
+-rw-r--r--   0        0        0      384 2024-04-23 01:58:59.404346 wj_google-0.1.2/wj_google/tools/files_manage.py
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 wj_google-0.1.2/PKG-INFO
```

### Comparing `wj_google-0.1.1/README.md` & `wj_google-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -178,20 +178,7 @@
 )
 
 ```
 #### Delete label to bigquery table:
 ```
 delete_labels_in_table(dataset_name, table_name)
 ```
-
-#### Export queries to excel(Depreciated!):
-You can use multiple queries and add it in a excel document, every query will be converted in a worksheet.
-```
-query1 = """
-SELECT * FROM `test.tw` LIMIT 10
-"""
-query2 = """
-SELECT * FROM `reports.reports` LIMIT 10
-"""
-queries = [query1, query2]
-export_queries_to_excel(queries=queries)
-```
```

### Comparing `wj_google-0.1.1/pyproject.toml` & `wj_google-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wj-google"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Johan <mantimanti89@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "wj_google" },
 ]
 
@@ -16,14 +16,13 @@
 python-dotenv = "^1.0.1"
 google-cloud-storage = "^2.15.0"
 flake8 = "^7.0.0"
 black = "^24.2.0"
 google-cloud-bigquery = "^3.18.0"
 pandas = "^2.2.1"
 db-dtypes = "^1.2.0"
-unittest = "^0.0"
 pytest = "^8.1.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wj_google-0.1.1/wj_google/examples/bigquery.py` & `wj_google-0.1.2/wj_google/examples/bigquery.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.1/wj_google/examples/sorage_and_drive.py` & `wj_google-0.1.2/wj_google/examples/sorage_and_drive.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.1/wj_google/google_api/Google.py` & `wj_google-0.1.2/wj_google/google_api/Google.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.1/wj_google/google_api/google_api.py` & `wj_google-0.1.2/wj_google/google_api/google_api.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.1/wj_google/google_cloud/cloud_connector.py` & `wj_google-0.1.2/wj_google/google_cloud/cloud_connector.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.1/wj_google/main.py` & `wj_google-0.1.2/wj_google/main.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.1/PKG-INFO` & `wj_google-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wj-google
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Johan
 Author-email: mantimanti89@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -15,15 +15,14 @@
 Requires-Dist: google-api-python-client (>=2.121.0,<3.0.0)
 Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.18.0,<4.0.0)
 Requires-Dist: google-cloud-storage (>=2.15.0,<3.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: unittest (>=0.0,<0.1)
 Description-Content-Type: text/markdown
 
 # wj_google
 
 
 
 ## Getting started
@@ -203,19 +202,7 @@
 
 ```
 #### Delete label to bigquery table:
 ```
 delete_labels_in_table(dataset_name, table_name)
 ```
 
-#### Export queries to excel(Depreciated!):
-You can use multiple queries and add it in a excel document, every query will be converted in a worksheet.
-```
-query1 = """
-SELECT * FROM `test.tw` LIMIT 10
-"""
-query2 = """
-SELECT * FROM `reports.reports` LIMIT 10
-"""
-queries = [query1, query2]
-export_queries_to_excel(queries=queries)
-```
```

