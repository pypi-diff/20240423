# Comparing `tmp/rich-torndb-0.0.1.tar.gz` & `tmp/rich_torndb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-torndb-0.0.1.tar", last modified: Sun Nov 21 09:56:16 2021, max compression
+gzip compressed data, was "rich_torndb-0.0.2.tar", last modified: Tue Apr 23 07:11:39 2024, max compression
```

## Comparing `rich-torndb-0.0.1.tar` & `rich_torndb-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 walkerjun  (1000) walkerjun  (1000)        0 2021-11-21 09:56:16.377785 rich-torndb-0.0.1/
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     9592 2021-10-11 03:18:15.000000 rich-torndb-0.0.1/LICENSE
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)      288 2021-11-21 09:56:16.377785 rich-torndb-0.0.1/PKG-INFO
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)      937 2021-10-11 03:18:15.000000 rich-torndb-0.0.1/README.md
-drwxrwxr-x   0 walkerjun  (1000) walkerjun  (1000)        0 2021-11-21 09:56:16.373785 rich-torndb-0.0.1/rich_torndb/
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)        0 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/__init__.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     3773 2021-11-14 10:58:17.000000 rich-torndb-0.0.1/rich_torndb/init_tables.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     7260 2021-10-11 03:51:24.000000 rich-torndb-0.0.1/rich_torndb/rich_torndb.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     4832 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/table_joiner.py
-drwxrwxr-x   0 walkerjun  (1000) walkerjun  (1000)        0 2021-11-21 09:56:16.373785 rich-torndb-0.0.1/rich_torndb/utils/
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)        0 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/utils/__init__.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     2870 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/utils/changes_log.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     2352 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/utils/log_helper.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)      899 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/utils/printer.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     3616 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/utils/sql_formatter.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     2089 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/utils/sql_invalid_errors.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     2296 2021-11-13 09:27:54.000000 rich-torndb-0.0.1/rich_torndb/utils/sql_valid_checker.py
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)     9779 2021-10-11 03:45:37.000000 rich-torndb-0.0.1/rich_torndb/utils/torndb.py
-drwxrwxr-x   0 walkerjun  (1000) walkerjun  (1000)        0 2021-11-21 09:56:16.373785 rich-torndb-0.0.1/rich_torndb.egg-info/
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)      288 2021-11-21 09:56:16.000000 rich-torndb-0.0.1/rich_torndb.egg-info/PKG-INFO
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)      572 2021-11-21 09:56:16.000000 rich-torndb-0.0.1/rich_torndb.egg-info/SOURCES.txt
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)        1 2021-11-21 09:56:16.000000 rich-torndb-0.0.1/rich_torndb.egg-info/dependency_links.txt
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)       28 2021-11-21 09:56:16.000000 rich-torndb-0.0.1/rich_torndb.egg-info/requires.txt
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)       30 2021-11-21 09:56:16.000000 rich-torndb-0.0.1/rich_torndb.egg-info/top_level.txt
--rw-rw-r--   0 walkerjun  (1000) walkerjun  (1000)       38 2021-11-21 09:56:16.377785 rich-torndb-0.0.1/setup.cfg
--rwxrwxr-x   0 walkerjun  (1000) walkerjun  (1000)      476 2021-11-21 09:52:45.000000 rich-torndb-0.0.1/setup.py
+drwxrwxr-x   0 lixiang   (1000) lixiang   (1000)        0 2024-04-23 07:11:39.214664 rich_torndb-0.0.2/
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     9592 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/LICENSE
+-rw-r--r--   0 lixiang   (1000) lixiang   (1000)      318 2024-04-23 07:11:39.214664 rich_torndb-0.0.2/PKG-INFO
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)      937 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/README.md
+drwxrwxr-x   0 lixiang   (1000) lixiang   (1000)        0 2024-04-23 07:11:39.214664 rich_torndb-0.0.2/rich_torndb/
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)        0 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/__init__.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     3773 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/init_tables.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     7260 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/rich_torndb.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     4844 2024-04-19 03:27:06.000000 rich_torndb-0.0.2/rich_torndb/table_joiner.py
+drwxrwxr-x   0 lixiang   (1000) lixiang   (1000)        0 2024-04-23 07:11:39.214664 rich_torndb-0.0.2/rich_torndb/utils/
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)        0 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/__init__.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     2870 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/changes_log.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     2352 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/log_helper.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)      899 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/printer.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     3616 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/sql_formatter.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     2089 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/sql_invalid_errors.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     2296 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/sql_valid_checker.py
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)     9779 2024-04-16 06:18:49.000000 rich_torndb-0.0.2/rich_torndb/utils/torndb.py
+drwxrwxr-x   0 lixiang   (1000) lixiang   (1000)        0 2024-04-23 07:11:39.214664 rich_torndb-0.0.2/rich_torndb.egg-info/
+-rw-r--r--   0 lixiang   (1000) lixiang   (1000)      318 2024-04-23 07:11:39.000000 rich_torndb-0.0.2/rich_torndb.egg-info/PKG-INFO
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)      572 2024-04-23 07:11:39.000000 rich_torndb-0.0.2/rich_torndb.egg-info/SOURCES.txt
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)        1 2024-04-23 07:11:39.000000 rich_torndb-0.0.2/rich_torndb.egg-info/dependency_links.txt
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)       28 2024-04-23 07:11:39.000000 rich_torndb-0.0.2/rich_torndb.egg-info/requires.txt
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)       30 2024-04-23 07:11:39.000000 rich_torndb-0.0.2/rich_torndb.egg-info/top_level.txt
+-rw-rw-r--   0 lixiang   (1000) lixiang   (1000)       38 2024-04-23 07:11:39.214664 rich_torndb-0.0.2/setup.cfg
+-rwxrwxr-x   0 lixiang   (1000) lixiang   (1000)      476 2024-04-19 03:27:06.000000 rich_torndb-0.0.2/setup.py
```

### Comparing `rich-torndb-0.0.1/LICENSE` & `rich_torndb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/README.md` & `rich_torndb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/init_tables.py` & `rich_torndb-0.0.2/rich_torndb/init_tables.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/rich_torndb.py` & `rich_torndb-0.0.2/rich_torndb/rich_torndb.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/table_joiner.py` & `rich_torndb-0.0.2/rich_torndb/table_joiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import *
 from tqdm import tqdm
-from rich_torndb import BaseConn
+from rich_torndb.rich_torndb import BaseConn
 
 
 class TableJoiner(object):
 
     @classmethod
     def join_table(cls, base_datas: List[Dict[str, Any]],
                    table: str, fields: List[str], base_join_key: str,
```

### Comparing `rich-torndb-0.0.1/rich_torndb/utils/changes_log.py` & `rich_torndb-0.0.2/rich_torndb/utils/changes_log.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/utils/log_helper.py` & `rich_torndb-0.0.2/rich_torndb/utils/log_helper.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/utils/printer.py` & `rich_torndb-0.0.2/rich_torndb/utils/printer.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/utils/sql_formatter.py` & `rich_torndb-0.0.2/rich_torndb/utils/sql_formatter.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/utils/sql_invalid_errors.py` & `rich_torndb-0.0.2/rich_torndb/utils/sql_invalid_errors.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/utils/sql_valid_checker.py` & `rich_torndb-0.0.2/rich_torndb/utils/sql_valid_checker.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb/utils/torndb.py` & `rich_torndb-0.0.2/rich_torndb/utils/torndb.py`

 * *Files identical despite different names*

### Comparing `rich-torndb-0.0.1/rich_torndb.egg-info/SOURCES.txt` & `rich_torndb-0.0.2/rich_torndb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

