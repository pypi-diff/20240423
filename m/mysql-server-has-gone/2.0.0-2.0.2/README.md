# Comparing `tmp/mysql_server_has_gone-2.0.0.tar.gz` & `tmp/mysql_server_has_gone-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_server_has_gone-2.0.0.tar", last modified: Thu Apr 11 07:01:06 2024, max compression
+gzip compressed data, was "mysql_server_has_gone-2.0.2.tar", last modified: Tue Apr 23 01:46:41 2024, max compression
```

## Comparing `mysql_server_has_gone-2.0.0.tar` & `mysql_server_has_gone-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 07:01:06.968436 mysql_server_has_gone-2.0.0/
--rw-rw-rw-   0        0        0     1082 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1090 2024-04-11 07:01:06.967437 mysql_server_has_gone-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      750 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 07:01:06.966438 mysql_server_has_gone-2.0.0/mysql_server_has_gone.egg-info/
--rw-rw-rw-   0        0        0     1090 2024-04-11 07:01:06.000000 mysql_server_has_gone-2.0.0/mysql_server_has_gone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-11 07:01:06.000000 mysql_server_has_gone-2.0.0/mysql_server_has_gone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 07:01:06.000000 mysql_server_has_gone-2.0.0/mysql_server_has_gone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-11 07:01:06.000000 mysql_server_has_gone-2.0.0/mysql_server_has_gone.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 07:01:06.964442 mysql_server_has_gone-2.0.0/mysql_server_has_gone_away/
--rw-rw-rw-   0        0        0        0 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.0/mysql_server_has_gone_away/__init__.py
--rw-rw-rw-   0        0        0     1907 2024-04-11 06:35:24.000000 mysql_server_has_gone-2.0.0/mysql_server_has_gone_away/base.py
--rw-rw-rw-   0        0        0       42 2024-04-11 07:01:06.968436 mysql_server_has_gone-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-04-11 07:01:04.000000 mysql_server_has_gone-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 01:46:41.805828 mysql_server_has_gone-2.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1090 2024-04-23 01:46:41.805297 mysql_server_has_gone-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 01:46:41.804272 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/
+-rw-rw-rw-   0        0        0     1090 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 01:46:41.803151 mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/
+-rw-rw-rw-   0        0        0        0 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/__init__.py
+-rw-rw-rw-   0        0        0     1973 2024-04-23 01:44:06.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/base.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 01:46:41.805828 mysql_server_has_gone-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-04-23 01:46:38.000000 mysql_server_has_gone-2.0.2/setup.py
```

### Comparing `mysql_server_has_gone-2.0.0/LICENSE` & `mysql_server_has_gone-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_server_has_gone-2.0.0/PKG-INFO` & `mysql_server_has_gone-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_server_has_gone
-Version: 2.0.0
+Version: 2.0.2
 Summary: Django myslq backend that fixes issue with long living connection
 Home-page: https://github.com/maiyajj/MySQL-server-has-gone-away
 Author: maiyajj
 Author-email: 1045373828@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysql_server_has_gone-2.0.0/README.md` & `mysql_server_has_gone-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mysql_server_has_gone-2.0.0/mysql_server_has_gone.egg-info/PKG-INFO` & `mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_server_has_gone
-Version: 2.0.0
+Version: 2.0.2
 Summary: Django myslq backend that fixes issue with long living connection
 Home-page: https://github.com/maiyajj/MySQL-server-has-gone-away
 Author: maiyajj
 Author-email: 1045373828@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysql_server_has_gone-2.0.0/mysql_server_has_gone_away/base.py` & `mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """
 https://stackoverflow.com/a/60894948/3872976
 """
 
 import logging
 
-from django.db import OperationalError, InterfaceError, IntegrityError
+from django.db import IntegrityError, InterfaceError, OperationalError
 from django.db.backends.mysql import base
+from retry import retry
+
+logger = logging.getLogger("mysql_server_has_gone_away")
 
-logger = logging.getLogger('mysql_server_has_gone_away')
 
 def check_mysql_gone_away(db_wrapper):
     def decorate(f):
+        @retry(tries=3)
         def wrapper(self, query, args=None):
             try:
                 return f(self, query, args)
             except (OperationalError, InterfaceError) as e:
-                logger.warn("MySQL server has gone away. Rerunning query: %s", query)
+                logger.error(f"MySQL server has gone away. Rerunning query: {query}; Error: {e}")
                 if (
-                    'MySQL server has gone away' in str(e) or
-                    'Server has gone away' in str(e) or
-                    'Lost connection to MySQL server during query' in str(e)
+                    "MySQL server has gone away" in str(e)
+                    or "Server has gone away" in str(e)
+                    or "Lost connection to MySQL server during query" in str(e)
                 ):
                     db_wrapper.connection.close()
                     db_wrapper.connect()
                     self.cursor = db_wrapper.connection.cursor()
                     return f(self, query, args)
                 # Map some error codes to IntegrityError, since they seem to be
                 # misclassified and Django would prefer the more logical place.
                 if e.args[0] in self.codes_for_integrityerror:
                     raise IntegrityError(*tuple(e.args))
                 raise
+
         return wrapper
 
     return decorate
 
 
 class DatabaseWrapper(base.DatabaseWrapper):
```

### Comparing `mysql_server_has_gone-2.0.0/setup.py` & `mysql_server_has_gone-2.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mysql_server_has_gone",
-    version="2.0.0",
+    version="2.0.2",
     description="Django myslq backend that fixes issue with long living connection",
-    author='maiyajj',
-    author_email='1045373828@qq.com',
+    author="maiyajj",
+    author_email="1045373828@qq.com",
     license="MIT",
-    url='https://github.com/maiyajj/MySQL-server-has-gone-away',
+    url="https://github.com/maiyajj/MySQL-server-has-gone-away",
     long_description=long_description,
     packages=find_packages(),
     long_description_content_type="text/markdown",
 )
```

