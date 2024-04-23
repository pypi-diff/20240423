# Comparing `tmp/SQLLite3HelperClass-0.1.3.tar.gz` & `tmp/SQLLite3HelperClass-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLLite3HelperClass-0.1.3.tar", last modified: Mon Sep 11 13:32:39 2023, max compression
+gzip compressed data, was "SQLLite3HelperClass-0.5.tar", last modified: Tue Apr 23 13:53:40 2024, max compression
```

## Comparing `SQLLite3HelperClass-0.1.3.tar` & `SQLLite3HelperClass-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-09-11 13:32:39.438824 SQLLite3HelperClass-0.1.3/
--rw-rw-rw-   0        0        0     1084 2023-09-11 11:42:18.000000 SQLLite3HelperClass-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      535 2023-09-11 13:32:39.439860 SQLLite3HelperClass-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-09-11 11:44:04.000000 SQLLite3HelperClass-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-09-11 13:32:39.418861 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass/
--rw-rw-rw-   0        0        0     2024 2023-09-11 11:30:22.000000 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass/SQLLite3HelperClass.py
--rw-rw-rw-   0        0        0       66 2023-09-11 13:26:16.000000 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-11 13:32:39.435870 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass.egg-info/
--rw-rw-rw-   0        0        0      535 2023-09-11 13:32:39.000000 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-09-11 13:32:39.000000 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-11 13:32:39.000000 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-09-11 13:32:39.000000 SQLLite3HelperClass-0.1.3/SQLLite3HelperClass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-09-11 13:32:39.441817 SQLLite3HelperClass-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-09-11 13:28:41.000000 SQLLite3HelperClass-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:53:40.548902 SQLLite3HelperClass-0.5/
+-rw-rw-rw-   0        0        0     1084 2023-09-11 14:39:05.000000 SQLLite3HelperClass-0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      531 2024-04-23 13:53:40.549942 SQLLite3HelperClass-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-09-11 14:39:05.000000 SQLLite3HelperClass-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 13:53:40.534939 SQLLite3HelperClass-0.5/SQLLite3HelperClass/
+-rw-rw-rw-   0        0        0     3297 2024-04-23 12:36:38.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass/SQLLite3HelperClass.py
+-rw-rw-rw-   0        0        0       66 2023-09-11 14:39:05.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:53:40.546907 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/
+-rw-rw-rw-   0        0        0      531 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-23 13:53:40.550924 SQLLite3HelperClass-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      587 2024-04-23 12:19:49.000000 SQLLite3HelperClass-0.5/setup.py
```

### Comparing `SQLLite3HelperClass-0.1.3/LICENSE.txt` & `SQLLite3HelperClass-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SQLLite3HelperClass-0.1.3/PKG-INFO` & `SQLLite3HelperClass-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: SQLLite3HelperClass
-Version: 0.1.3
+Version: 0.5
 Summary: Initializes an sqlite3 database and has a basic query method. This class is meant to be subclassed and expanded.
 Home-page: https://github.com/amcsparron2793-Water/SQLLite3HelperClass
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.5.tar.gz
 Keywords: Sqlite3,database
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `SQLLite3HelperClass-0.1.3/SQLLite3HelperClass/SQLLite3HelperClass.py` & `SQLLite3HelperClass-0.5/SQLLite3HelperClass/SQLLite3HelperClass.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import sqlite3
 from logging import Logger
+from typing import List
+from collections import ChainMap
 
 
 class SQLlite3Helper:
     """ Initializes an SQLlite3 database and has a basic query method.
     This class is meant to be subclassed and expanded.
 
     IF NO LOGGER IS SPECIFIED, A DUMMY LOGGER IS USED. """
@@ -35,23 +37,58 @@
         except sqlite3.IntegrityError as e:
             self._logger.error(e, exc_info=True)
             raise e
         except sqlite3.OperationalError as e:
             self._logger.error(e, exc_info=True)
             raise e
 
-    def Query(self, sql_string: str):
+    @property
+    def results_column_names(self) -> List[str] or None:
+        try:
+            return [d[0] for d in self._cursor.description]
+        except AttributeError as e:
+            return None
+
+    def _ConvertToFinalListDict(self, results: List[tuple]) -> List[dict] or None:
+        row_list_dict = []
+        final_list_dict = []
+
+        for row in results:
+            if self.results_column_names:
+                for cell, col in zip(row, self.results_column_names):
+                    row_list_dict.append({col: cell})
+                final_list_dict.append(dict(ChainMap(*row_list_dict)))
+                row_list_dict.clear()
+            else:
+                raise AttributeError("A query has not been executed, "
+                                     "please execute a query before calling this function.")
+        if len(final_list_dict) > 0:
+            return final_list_dict
+        else:
+            return None
+
+    def Query(self, sql_string: str, **kwargs):
+        return_dict = False
+        if kwargs:
+            if 'return_dict' in kwargs:
+                return_dict = kwargs['return_dict']
         try:
             self._cursor.execute(sql_string)
+
             res = self._cursor.fetchall()
+
             if res:
                 self._logger.info(f"{len(res)} item(s) returned.")
-                return res
             else:
                 self._logger.warning(f"query returned no results")
-                return None
+
+            if return_dict:
+                return self._ConvertToFinalListDict(res)
+            else:
+                return res or None
+
         except sqlite3.IntegrityError as e:
             self._logger.error(e, exc_info=True)
             raise e
         except sqlite3.OperationalError as e:
             self._logger.error(e, exc_info=True)
-            raise e
+            raise e
```

### Comparing `SQLLite3HelperClass-0.1.3/SQLLite3HelperClass.egg-info/PKG-INFO` & `SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: SQLLite3HelperClass
-Version: 0.1.3
+Version: 0.5
 Summary: Initializes an sqlite3 database and has a basic query method. This class is meant to be subclassed and expanded.
 Home-page: https://github.com/amcsparron2793-Water/SQLLite3HelperClass
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.5.tar.gz
 Keywords: Sqlite3,database
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `SQLLite3HelperClass-0.1.3/setup.py` & `SQLLite3HelperClass-0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='SQLLite3HelperClass',
-    version='0.1.3',
+    version='0.5',
     packages=['SQLLite3HelperClass'],
     url='https://github.com/amcsparron2793-Water/SQLLite3HelperClass',
-    download_url='https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.1.3.tar.gz',
+    download_url='https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.5.tar.gz',
     keywords=["Sqlite3", "database"],
     license='MIT License',
     author='Amcsparron',
     author_email='amcsparron@albanyny.gov',
     description='Initializes an sqlite3 database and has a basic query method. This class is meant to be subclassed and expanded.'
 )
```

