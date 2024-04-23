# Comparing `tmp/database-common-tools-1.1.4.tar.gz` & `tmp/database-common-tools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-common-tools-1.1.4.tar", last modified: Tue Apr 23 10:07:23 2024, max compression
+gzip compressed data, was "database-common-tools-1.1.5.tar", last modified: Tue Apr 23 10:17:17 2024, max compression
```

## Comparing `database-common-tools-1.1.4.tar` & `database-common-tools-1.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:07:23.912642 database-common-tools-1.1.4/
--rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.1.4/LICENSE
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-23 10:07:23.912056 database-common-tools-1.1.4/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.1.4/README.md
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:07:23.896165 database-common-tools-1.1.4/database_common_tools.egg-info/
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-23 10:07:23.000000 database-common-tools-1.1.4/database_common_tools.egg-info/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-23 10:07:23.000000 database-common-tools-1.1.4/database_common_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-23 10:07:23.000000 database-common-tools-1.1.4/database_common_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-23 10:07:23.000000 database-common-tools-1.1.4/database_common_tools.egg-info/requires.txt
--rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-23 10:07:23.000000 database-common-tools-1.1.4/database_common_tools.egg-info/top_level.txt
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:07:23.910074 database-common-tools-1.1.4/databasetools/
--rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.1.4/databasetools/__init__.py
--rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.1.4/databasetools/analysis_json.py
--rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 11:58:05.000000 database-common-tools-1.1.4/databasetools/analysis_json_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     2529 2024-04-18 06:06:35.000000 database-common-tools-1.1.4/databasetools/analysis_json_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.1.4/databasetools/data_analysis.py
--rw-r--r--   0 yangming   (501) staff       (20)     3562 2024-04-16 12:39:11.000000 database-common-tools-1.1.4/databasetools/data_analysis_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     4515 2024-04-17 05:55:14.000000 database-common-tools-1.1.4/databasetools/data_analysis_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)      794 2024-04-23 10:06:19.000000 database-common-tools-1.1.4/databasetools/kafka_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.1.4/databasetools/mongo_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.1.4/databasetools/mt_wx_message.py
--rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.1.4/databasetools/mysql_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.1.4/databasetools/opensearch_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.1.4/databasetools/redis_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-23 10:07:23.912798 database-common-tools-1.1.4/setup.cfg
--rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-23 10:06:45.000000 database-common-tools-1.1.4/setup.py
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:07:23.911338 database-common-tools-1.1.4/test/
--rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.1.4/test/__init__.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:17:17.316546 database-common-tools-1.1.5/
+-rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.1.5/LICENSE
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-23 10:17:17.316012 database-common-tools-1.1.5/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.1.5/README.md
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:17:17.302734 database-common-tools-1.1.5/database_common_tools.egg-info/
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-23 10:17:17.000000 database-common-tools-1.1.5/database_common_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-23 10:17:17.000000 database-common-tools-1.1.5/database_common_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-23 10:17:17.000000 database-common-tools-1.1.5/database_common_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-23 10:17:17.000000 database-common-tools-1.1.5/database_common_tools.egg-info/requires.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-23 10:17:17.000000 database-common-tools-1.1.5/database_common_tools.egg-info/top_level.txt
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:17:17.314556 database-common-tools-1.1.5/databasetools/
+-rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.1.5/databasetools/__init__.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.1.5/databasetools/analysis_json.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 11:58:05.000000 database-common-tools-1.1.5/databasetools/analysis_json_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2529 2024-04-18 06:06:35.000000 database-common-tools-1.1.5/databasetools/analysis_json_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.1.5/databasetools/data_analysis.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3562 2024-04-16 12:39:11.000000 database-common-tools-1.1.5/databasetools/data_analysis_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     4515 2024-04-17 05:55:14.000000 database-common-tools-1.1.5/databasetools/data_analysis_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1044 2024-04-23 10:17:01.000000 database-common-tools-1.1.5/databasetools/kafka_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.1.5/databasetools/mongo_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.1.5/databasetools/mt_wx_message.py
+-rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.1.5/databasetools/mysql_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.1.5/databasetools/opensearch_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.1.5/databasetools/redis_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-23 10:17:17.316720 database-common-tools-1.1.5/setup.cfg
+-rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-23 10:17:12.000000 database-common-tools-1.1.5/setup.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-23 10:17:17.315485 database-common-tools-1.1.5/test/
+-rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.1.5/test/__init__.py
```

### Comparing `database-common-tools-1.1.4/LICENSE` & `database-common-tools-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/PKG-INFO` & `database-common-tools-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.1.4
+Version: 1.1.5
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.1.4/database_common_tools.egg-info/PKG-INFO` & `database-common-tools-1.1.5/database_common_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.1.4
+Version: 1.1.5
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.1.4/database_common_tools.egg-info/SOURCES.txt` & `database-common-tools-1.1.5/database_common_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/__init__.py` & `database-common-tools-1.1.5/databasetools/__init__.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/analysis_json.py` & `database-common-tools-1.1.5/databasetools/analysis_json.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/analysis_json_v2.py` & `database-common-tools-1.1.5/databasetools/analysis_json_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/analysis_json_v3.py` & `database-common-tools-1.1.5/databasetools/analysis_json_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/data_analysis.py` & `database-common-tools-1.1.5/databasetools/data_analysis.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/data_analysis_v2.py` & `database-common-tools-1.1.5/databasetools/data_analysis_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/data_analysis_v3.py` & `database-common-tools-1.1.5/databasetools/data_analysis_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/mongo_connect.py` & `database-common-tools-1.1.5/databasetools/mongo_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/mt_wx_message.py` & `database-common-tools-1.1.5/databasetools/mt_wx_message.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/opensearch_connect.py` & `database-common-tools-1.1.5/databasetools/opensearch_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/databasetools/redis_connect.py` & `database-common-tools-1.1.5/databasetools/redis_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.4/setup.py` & `database-common-tools-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'database-common-tools'
 DESCRIPTION = 'let message middleware and use database more easy'
 URL = 'https://github.com/yangming9/database-common-tools.git'
 EMAIL = 'yma91412@gmail.com'
 AUTHOR = 'Coder Yang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'jsonpath',
     'pymongo',
     'redis',
```

