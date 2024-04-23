# Comparing `tmp/rr_connection_manager-0.2.0.tar.gz` & `tmp/rr_connection_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rr_connection_manager-0.2.0.tar", max compression
+gzip compressed data, was "rr_connection_manager-0.3.0.tar", max compression
```

## Comparing `rr_connection_manager-0.2.0.tar` & `rr_connection_manager-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1095 2024-03-07 17:08:52.755956 rr_connection_manager-0.2.0/LICENSE
--rw-r--r--   0        0        0      885 2024-03-14 01:02:06.633700 rr_connection_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      324 2024-03-10 12:26:50.865533 rr_connection_manager-0.2.0/rr_connection_manager/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 11:40:48.701505 rr_connection_manager-0.2.0/rr_connection_manager/classes/__init__.py
--rw-r--r--   0        0        0     1570 2024-03-13 22:02:14.599666 rr_connection_manager-0.2.0/rr_connection_manager/classes/connection.py
--rw-r--r--   0        0        0     3907 2024-03-13 22:02:14.599666 rr_connection_manager-0.2.0/rr_connection_manager/classes/connection_conf.py
--rw-r--r--   0        0        0     2413 2024-03-13 22:02:14.599666 rr_connection_manager-0.2.0/rr_connection_manager/classes/postgres_connection.py
--rw-r--r--   0        0        0     1751 2024-03-14 01:02:06.633700 rr_connection_manager-0.2.0/rr_connection_manager/classes/sql_server_connection.py
--rw-r--r--   0        0        0      555 2024-03-11 23:39:04.899394 rr_connection_manager-0.2.0/rr_connection_manager/classes/sqlite_connection.py
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 rr_connection_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-03-07 17:08:52.755956 rr_connection_manager-0.3.0/LICENSE
+-rw-r--r--   0        0        0      885 2024-04-23 16:39:42.204596 rr_connection_manager-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      324 2024-03-10 12:26:50.865533 rr_connection_manager-0.3.0/rr_connection_manager/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-10 11:40:48.701505 rr_connection_manager-0.3.0/rr_connection_manager/classes/__init__.py
+-rw-r--r--   0        0        0     1570 2024-03-13 22:02:14.599666 rr_connection_manager-0.3.0/rr_connection_manager/classes/connection.py
+-rw-r--r--   0        0        0     4321 2024-04-23 16:39:42.212781 rr_connection_manager-0.3.0/rr_connection_manager/classes/connection_conf.py
+-rw-r--r--   0        0        0     2413 2024-03-13 22:02:14.599666 rr_connection_manager-0.3.0/rr_connection_manager/classes/postgres_connection.py
+-rw-r--r--   0        0        0     1751 2024-03-14 01:02:06.633700 rr_connection_manager-0.3.0/rr_connection_manager/classes/sql_server_connection.py
+-rw-r--r--   0        0        0      555 2024-03-11 23:39:04.899394 rr_connection_manager-0.3.0/rr_connection_manager/classes/sqlite_connection.py
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 rr_connection_manager-0.3.0/PKG-INFO
```

### Comparing `rr_connection_manager-0.2.0/LICENSE` & `rr_connection_manager-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rr_connection_manager-0.2.0/pyproject.toml` & `rr_connection_manager-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rr-connection-manager"
-version = "0.2.0"
+version = "0.3.0"
 description = "A package to help you connect to all Registry databases"
 authors = ["andrew atterton <andrew.atterton@renalregistry.nhs.uk>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 SQLAlchemy = "^2.0.23"
```

### Comparing `rr_connection_manager-0.2.0/rr_connection_manager/classes/connection.py` & `rr_connection_manager-0.3.0/rr_connection_manager/classes/connection.py`

 * *Files identical despite different names*

### Comparing `rr_connection_manager-0.2.0/rr_connection_manager/classes/connection_conf.py` & `rr_connection_manager-0.3.0/rr_connection_manager/classes/connection_conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import hashlib
 import json
 import os
+import getpass
 
 from dotenv import dotenv_values
 from pykeepass import PyKeePass
 
 
 class ConnectionConf:
     def __init__(self, app, via_app) -> None:
         self.app = app
-        self.conf = dotenv_values(".env")
+        self.conf = dotenv_values(".connection_env")
         self.via_app_server = via_app
         self.app_host = None
         self.db_host = None
         self.db_user = None
         self.database = None
         self.db_password = None
         self.tunnel_user = None
@@ -29,20 +30,55 @@
 
         sha256_hash = hashlib.sha256()
         sha256_hash.update(public_key.encode("utf-8"))
 
         return sha256_hash.hexdigest()
 
     def _set_attributes(self):
-        if "KEEPASS_FILE_PATH" not in self.conf and "DB_HOST" not in self.conf:
-            raise ValueError("Missing vital attributes in the env file")
+        if len(self.conf) > 0:
+            if "APP_HOST" in self.conf:
+                self.app_host = self.conf["APP_HOST"]
+            if "DB_HOST" in self.conf:
+                self.db_host = self.conf["DB_HOST"]
+            else:
+                # This might not be the case for SQLite
+                raise ValueError(
+                    "DB_HOST is a required variable if you are using a .connection_env file"
+                )
+            if "DB_USER" in self.conf:
+                self.db_user = self.conf["DB_USER"]
+            if "DATABASE" in self.conf:
+                self.database = self.conf["DATABASE"]
+            else:
+                # This might not be the case for SQLite
+                raise ValueError(
+                    "DATABASE is a variable if you are using a .connection_env file"
+                )
+            if "DB_PASSWORD" in self.conf:
+                self.db_password = self.conf["DB_PASSWORD"]
+            if "TUNNEL_USER" in self.conf:
+                self.tunnel_user = self.conf["TUNNEL_USER"]
+            if "DB_PORT" in self.conf:
+                self.db_port = self.conf["DB_PORT"]
+            if "TUNNEL_PORT" in self.conf:
+                self.tunnel_port = self.conf["TUNNEL_PORT"]
+
+        else:
+            user = getpass.getuser().replace(".", "_")
+            keepass_file_path = os.path.abspath(
+                os.path.join("R:", "Connection Manager", user, f"{user}.kdbx ")
+            )
+
+            if not os.path.exists(keepass_file_path):
+                raise FileExistsError(
+                    "Can't find your keepass file. You might need to run rr-key-manager"
+                )
 
-        if "KEEPASS_FILE_PATH" in self.conf:
             kp = PyKeePass(
-                self.conf["KEEPASS_FILE_PATH"],
+                keepass_file_path,
                 password=self._get_keepass_key(),
             )
 
             group = kp.find_groups(name=self.app, first=True)
 
             if any(e for e in group.entries if "db_server" in e.path):
                 db_server = next((e for e in group.entries if "db_server" in e.path))
@@ -68,31 +104,7 @@
                 if (
                     self.via_app_server == "true"
                     and app_server.notes
                     and "PORTS" in app_server.notes
                 ):
                     self.tunnel_user = app_server.username
                     self.tunnel_port = json.loads(app_server.notes)["PORTS"]["SSH_PORT"]
-
-        else:
-            if "APP_HOST" in self.conf:
-                self.app_host = self.conf["APP_HOST"]
-            if "DB_HOST" in self.conf:
-                self.db_host = self.conf["DB_HOST"]
-            else:
-                # This might not be the case for SQLite
-                raise ValueError("DB_HOST is a required env")
-            if "DB_USER" in self.conf:
-                self.db_user = self.conf["DB_USER"]
-            if "DATABASE" in self.conf:
-                self.database = self.conf["DATABASE"]
-            else:
-                # This might not be the case for SQLite
-                raise ValueError("DATABASE is a required env")
-            if "DB_PASSWORD" in self.conf:
-                self.db_password = self.conf["DB_PASSWORD"]
-            if "TUNNEL_USER" in self.conf:
-                self.tunnel_user = self.conf["TUNNEL_USER"]
-            if "DB_PORT" in self.conf:
-                self.db_port = self.conf["DB_PORT"]
-            if "TUNNEL_PORT" in self.conf:
-                self.tunnel_port = self.conf["TUNNEL_PORT"]
```

### Comparing `rr_connection_manager-0.2.0/rr_connection_manager/classes/postgres_connection.py` & `rr_connection_manager-0.3.0/rr_connection_manager/classes/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `rr_connection_manager-0.2.0/rr_connection_manager/classes/sql_server_connection.py` & `rr_connection_manager-0.3.0/rr_connection_manager/classes/sql_server_connection.py`

 * *Files identical despite different names*

### Comparing `rr_connection_manager-0.2.0/rr_connection_manager/classes/sqlite_connection.py` & `rr_connection_manager-0.3.0/rr_connection_manager/classes/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `rr_connection_manager-0.2.0/PKG-INFO` & `rr_connection_manager-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rr-connection-manager
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package to help you connect to all Registry databases
 License: MIT
 Author: andrew atterton
 Author-email: andrew.atterton@renalregistry.nhs.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

