# Comparing `tmp/vvm_lib-1.0.0.tar.gz` & `tmp/vvm_lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvm_lib-1.0.0.tar", last modified: Mon Apr 22 12:15:32 2024, max compression
+gzip compressed data, was "vvm_lib-1.0.1.tar", last modified: Tue Apr 23 05:45:39 2024, max compression
```

## Comparing `vvm_lib-1.0.0.tar` & `vvm_lib-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 12:15:32.198815 vvm_lib-1.0.0/
--rw-rw-rw-   0        0        0      454 2024-04-22 12:15:32.198815 vvm_lib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-20 07:29:21.000000 vvm_lib-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 12:15:32.200815 vvm_lib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-22 12:15:22.000000 vvm_lib-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 12:15:32.175815 vvm_lib-1.0.0/vvm_lib/
-drwxrwxrwx   0        0        0        0 2024-04-22 12:15:32.196817 vvm_lib-1.0.0/vvm_lib/DB/
--rw-rw-rw-   0        0        0       30 2024-04-22 09:33:28.000000 vvm_lib-1.0.0/vvm_lib/DB/__init__.py
--rw-rw-rw-   0        0        0     5916 2024-04-22 12:14:57.000000 vvm_lib-1.0.0/vvm_lib/DB/db.py
--rw-rw-rw-   0        0        0      229 2024-04-20 07:29:21.000000 vvm_lib-1.0.0/vvm_lib/__init__.py
--rw-rw-rw-   0        0        0     2747 2024-04-20 07:29:21.000000 vvm_lib-1.0.0/vvm_lib/google_book.py
--rw-rw-rw-   0        0        0     3545 2024-04-20 07:29:21.000000 vvm_lib-1.0.0/vvm_lib/greenplum.py
--rw-rw-rw-   0        0        0      654 2024-04-20 07:29:21.000000 vvm_lib-1.0.0/vvm_lib/mssql.py
--rw-rw-rw-   0        0        0      855 2024-04-20 07:29:21.000000 vvm_lib-1.0.0/vvm_lib/vault.py
-drwxrwxrwx   0        0        0        0 2024-04-22 12:15:32.197817 vvm_lib-1.0.0/vvm_lib.egg-info/
--rw-rw-rw-   0        0        0      454 2024-04-22 12:15:32.000000 vvm_lib-1.0.0/vvm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2024-04-22 12:15:32.000000 vvm_lib-1.0.0/vvm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 12:15:32.000000 vvm_lib-1.0.0/vvm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 08:57:19.000000 vvm_lib-1.0.0/vvm_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       94 2024-04-22 12:15:32.000000 vvm_lib-1.0.0/vvm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 12:15:32.000000 vvm_lib-1.0.0/vvm_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.277611 vvm_lib-1.0.1/
+-rw-rw-rw-   0        0        0      454 2024-04-23 05:45:39.277611 vvm_lib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4707 2024-04-23 05:44:57.000000 vvm_lib-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 05:45:39.283541 vvm_lib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      747 2024-04-23 05:28:25.000000 vvm_lib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.253531 vvm_lib-1.0.1/vvm_lib/
+drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.276582 vvm_lib-1.0.1/vvm_lib/DB/
+-rw-rw-rw-   0        0        0       30 2024-04-22 09:33:28.000000 vvm_lib-1.0.1/vvm_lib/DB/__init__.py
+-rw-rw-rw-   0        0        0     6564 2024-04-23 05:43:08.000000 vvm_lib-1.0.1/vvm_lib/DB/db.py
+-rw-rw-rw-   0        0        0      229 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/__init__.py
+-rw-rw-rw-   0        0        0     2747 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/google_book.py
+-rw-rw-rw-   0        0        0     3545 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/greenplum.py
+-rw-rw-rw-   0        0        0      654 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/mssql.py
+-rw-rw-rw-   0        0        0      855 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/vault.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.277611 vvm_lib-1.0.1/vvm_lib.egg-info/
+-rw-rw-rw-   0        0        0      454 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 08:57:19.000000 vvm_lib-1.0.1/vvm_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       94 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/top_level.txt
```

### Comparing `vvm_lib-1.0.0/setup.py` & `vvm_lib-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='vvm_lib',
-      version='1.0.0',
+      version='1.0.1',
       description='my frequently used functions',
       packages=[
           'vvm_lib',
           "vvm_lib.db",
           ],
       package_dir={
         "vvm_lib": "vvm_lib",
```

### Comparing `vvm_lib-1.0.0/vvm_lib/DB/db.py` & `vvm_lib-1.0.1/vvm_lib/DB/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import pandas as pd
 import psycopg2
 import io
 import pymssql
+from clickhouse_connect import get_client, driver
 
 
 class DB:
     """
     Класс для работы с базами данных postgresql и mssql для моего личного пользования
     Конструктор:
         :param dbname: Название БД
         :param user: пользователь
         :param password: пароль
         :param port: порт
         :param host: хост
-        :param what_db: 'postgresql' или 'mssql'
+        :param what_db: 'postgresql' , 'mssql', 'clickhouse'
     """
-    def __init__(self, dbname, user, password, port, host, what_db='postgresql'):
+
+    def __init__(self, dbname, user, password, port, host, what_db='postgresql') -> None:
         """
         :param dbname: Название БД
         :param user: пользователь
         :param password: пароль
         :param port: порт
         :param host: хост
-        :param what_db: 'postgresql' или 'mssql'
+        :param what_db: 'postgresql' , 'mssql', 'clickhouse'
         """
         self.dbname = dbname
         self.user = user
         self.password = password
         self.port = port
         self.host = host
         self.what_db = what_db
@@ -37,40 +39,52 @@
         """
         if self.what_db == 'postgresql':
             return psycopg2.connect(dbname=self.dbname, user=self.user, password=self.password
                                     , port=self.port, host=self.host)
         elif self.what_db == 'mssql':
             return pymssql.connect(server=self.dbname, user=self.user, password=self.password
                                    , port=self.port, host=self.host)
+        elif self.what_db == 'clickhouse':
+            return get_client(database=self.dbname, user=self.user, password=self.password
+                              , port=self.port, host=self.host)
 
     @staticmethod
     def close_connect(connect):
         """
         :param connect:
         :return: закрытие соединения
         """
         connect.close()
         # print(f"Соединение закрыто")
 
-    def select(self, sql: str):
+    def select(self, sql: str) -> pd.DataFrame:
         """
         Если нужно получить DATAFRAME
         :param sql: запрос SQL
         :return: pd.Dastaframe
         """
         connect = self.open_connect()
-        try:
-            with connect.cursor() as cursor:
-                cursor.execute(sql)
-                result = pd.DataFrame(cursor.fetchall(), columns=[col[0] for col in cursor.description])
-        except psycopg2.ProgrammingError as error:
-            raise print(error)
-        finally:
-            self.close_connect(connect)
-        return result
+        if self.what_db == 'clickhouse':
+            try:
+                result = connect.query_df(sql)
+            except driver.exceptions.ProgrammingError as error:
+                raise print(error)
+            finally:
+                self.close_connect(connect)
+            return result
+        else:
+            try:
+                with connect.cursor() as cursor:
+                    cursor.execute(sql)
+                    result = pd.DataFrame(cursor.fetchall(), columns=[col[0] for col in cursor.description])
+            except psycopg2.ProgrammingError as error:
+                raise print(error)
+            finally:
+                self.close_connect(connect)
+            return result
 
     def insert(self, df: pd.DataFrame, table: str):
         """
         Вставка данных
         :param df:
         :param table:
         :return:
@@ -151,8 +165,7 @@
                 cursor.execute(f'truncate table  {table_name}')
                 connect.commit()
         except psycopg2.ProgrammingError as error:
             raise print(error)
         finally:
             self.close_connect(connect)
         print(f'Таблица {table_name} очищена')
-
```

### Comparing `vvm_lib-1.0.0/vvm_lib/google_book.py` & `vvm_lib-1.0.1/vvm_lib/google_book.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-1.0.0/vvm_lib/greenplum.py` & `vvm_lib-1.0.1/vvm_lib/greenplum.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-1.0.0/vvm_lib/mssql.py` & `vvm_lib-1.0.1/vvm_lib/mssql.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-1.0.0/vvm_lib/vault.py` & `vvm_lib-1.0.1/vvm_lib/vault.py`

 * *Files identical despite different names*

