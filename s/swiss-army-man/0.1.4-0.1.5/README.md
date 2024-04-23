# Comparing `tmp/swiss_army_man-0.1.4.tar.gz` & `tmp/swiss_army_man-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiss_army_man-0.1.4.tar", max compression
+gzip compressed data, was "swiss_army_man-0.1.5.tar", max compression
```

## Comparing `swiss_army_man-0.1.4.tar` & `swiss_army_man-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      112 2024-04-22 21:27:37.769952 swiss_army_man-0.1.4/README.md
--rw-r--r--   0        0        0      479 2024-04-22 21:54:13.923876 swiss_army_man-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      383 2024-04-22 21:54:14.920129 swiss_army_man-0.1.4/swiss_army_man/__init__.py
--rw-r--r--   0        0        0     5479 2024-04-22 21:53:16.787915 swiss_army_man-0.1.4/swiss_army_man/analyze.py
--rw-r--r--   0        0        0      717 2024-04-22 21:47:53.832258 swiss_army_man-0.1.4/swiss_army_man/database_manager.py
--rw-r--r--   0        0        0      733 2024-04-22 21:47:53.832426 swiss_army_man-0.1.4/swiss_army_man/environment.py
--rw-r--r--   0        0        0     1480 2024-04-22 21:06:47.983399 swiss_army_man-0.1.4/swiss_army_man/file_utils.py
--rw-r--r--   0        0        0      123 2024-04-22 21:03:44.134320 swiss_army_man-0.1.4/swiss_army_man/grep.py
--rw-r--r--   0        0        0      112 2024-04-22 21:03:48.429612 swiss_army_man-0.1.4/swiss_army_man/is_iterable.py
--rw-r--r--   0        0        0      644 2024-04-22 21:03:55.150780 swiss_army_man-0.1.4/swiss_army_man/parse_datetime.py
--rw-r--r--   0        0        0     1054 2024-04-22 21:09:33.740162 swiss_army_man-0.1.4/swiss_army_man/project_root.py
--rw-r--r--   0        0        0      138 2024-04-22 21:04:08.460065 swiss_army_man-0.1.4/swiss_army_man/query_to_df.py
--rw-r--r--   0        0        0     4617 2024-04-22 21:47:53.832676 swiss_army_man-0.1.4/swiss_army_man/redis_cache.py
--rw-r--r--   0        0        0      675 2024-04-22 21:50:07.551457 swiss_army_man-0.1.4/swiss_army_man/sidekiq.py
--rw-r--r--   0        0        0      401 2024-04-22 21:09:51.270537 swiss_army_man-0.1.4/swiss_army_man/singleton.py
--rw-r--r--   0        0        0      605 2024-04-22 21:07:25.215488 swiss_army_man-0.1.4/swiss_army_man/standardize_dates.py
--rw-r--r--   0        0        0      402 2024-04-22 21:10:09.450083 swiss_army_man-0.1.4/swiss_army_man/string_methods.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 swiss_army_man-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-04-22 21:27:37.769952 swiss_army_man-0.1.5/README.md
+-rw-r--r--   0        0        0      479 2024-04-23 13:20:04.877905 swiss_army_man-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      383 2024-04-23 13:19:58.042855 swiss_army_man-0.1.5/swiss_army_man/__init__.py
+-rw-r--r--   0        0        0     5479 2024-04-22 21:53:16.787915 swiss_army_man-0.1.5/swiss_army_man/analyze.py
+-rw-r--r--   0        0        0      716 2024-04-23 13:19:33.338679 swiss_army_man-0.1.5/swiss_army_man/database_manager.py
+-rw-r--r--   0        0        0      733 2024-04-22 21:47:53.832426 swiss_army_man-0.1.5/swiss_army_man/environment.py
+-rw-r--r--   0        0        0     1480 2024-04-22 21:06:47.983399 swiss_army_man-0.1.5/swiss_army_man/file_utils.py
+-rw-r--r--   0        0        0      123 2024-04-22 21:03:44.134320 swiss_army_man-0.1.5/swiss_army_man/grep.py
+-rw-r--r--   0        0        0      112 2024-04-22 21:03:48.429612 swiss_army_man-0.1.5/swiss_army_man/is_iterable.py
+-rw-r--r--   0        0        0      644 2024-04-22 21:03:55.150780 swiss_army_man-0.1.5/swiss_army_man/parse_datetime.py
+-rw-r--r--   0        0        0     1054 2024-04-22 21:09:33.740162 swiss_army_man-0.1.5/swiss_army_man/project_root.py
+-rw-r--r--   0        0        0      138 2024-04-22 21:04:08.460065 swiss_army_man-0.1.5/swiss_army_man/query_to_df.py
+-rw-r--r--   0        0        0     4617 2024-04-22 21:47:53.832676 swiss_army_man-0.1.5/swiss_army_man/redis_cache.py
+-rw-r--r--   0        0        0      675 2024-04-22 21:50:07.551457 swiss_army_man-0.1.5/swiss_army_man/sidekiq.py
+-rw-r--r--   0        0        0      401 2024-04-22 21:09:51.270537 swiss_army_man-0.1.5/swiss_army_man/singleton.py
+-rw-r--r--   0        0        0      605 2024-04-22 21:07:25.215488 swiss_army_man-0.1.5/swiss_army_man/standardize_dates.py
+-rw-r--r--   0        0        0      402 2024-04-22 21:10:09.450083 swiss_army_man-0.1.5/swiss_army_man/string_methods.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 swiss_army_man-0.1.5/PKG-INFO
```

### Comparing `swiss_army_man-0.1.4/swiss_army_man/analyze.py` & `swiss_army_man-0.1.5/swiss_army_man/analyze.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/swiss_army_man/database_manager.py` & `swiss_army_man-0.1.5/swiss_army_man/database_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import psycopg2
 from contextlib import contextmanager
 from . import project_root, db_config
-
 class DatabaseManager():
     @contextmanager
     @staticmethod
     def with_cursor(host=None, dbname=None, port=None):
         if os.path.exists(project_root("db/config.yml")) and host is None:
             config = db_config()
             host = config["host"]
```

### Comparing `swiss_army_man-0.1.4/swiss_army_man/environment.py` & `swiss_army_man-0.1.5/swiss_army_man/environment.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/swiss_army_man/file_utils.py` & `swiss_army_man-0.1.5/swiss_army_man/file_utils.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/swiss_army_man/parse_datetime.py` & `swiss_army_man-0.1.5/swiss_army_man/parse_datetime.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/swiss_army_man/project_root.py` & `swiss_army_man-0.1.5/swiss_army_man/project_root.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/swiss_army_man/redis_cache.py` & `swiss_army_man-0.1.5/swiss_army_man/redis_cache.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/swiss_army_man/sidekiq.py` & `swiss_army_man-0.1.5/swiss_army_man/sidekiq.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/swiss_army_man/standardize_dates.py` & `swiss_army_man-0.1.5/swiss_army_man/standardize_dates.py`

 * *Files identical despite different names*

### Comparing `swiss_army_man-0.1.4/PKG-INFO` & `swiss_army_man-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiss-army-man
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Brett Shollenberger
 Author-email: brettshollenberger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

