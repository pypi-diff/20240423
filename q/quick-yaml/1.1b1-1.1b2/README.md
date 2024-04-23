# Comparing `tmp/quick_yaml-1.1b1.tar.gz` & `tmp/quick_yaml-1.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_yaml-1.1b1.tar", last modified: Mon Apr 22 05:28:04 2024, max compression
+gzip compressed data, was "quick_yaml-1.1b2.tar", last modified: Tue Apr 23 10:19:35 2024, max compression
```

## Comparing `quick_yaml-1.1b1.tar` & `quick_yaml-1.1b2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     7652 2024-04-02 03:58:22.000000 quick_yaml-1.1b1/LICENSE
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       34 2024-04-12 08:36:58.000000 quick_yaml-1.1b1/MANIFEST.in
--rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13707 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/PKG-INFO
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    12900 2024-04-17 06:06:52.000000 quick_yaml-1.1b1/README.md
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      879 2024-04-22 05:27:53.000000 quick_yaml-1.1b1/pyproject.toml
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       38 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/setup.cfg
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.753146 quick_yaml-1.1b1/src/
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/src/quick_yaml/
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      435 2024-04-12 09:08:35.000000 quick_yaml-1.1b1/src/quick_yaml/Btree.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     8829 2024-04-22 03:40:11.000000 quick_yaml-1.1b1/src/quick_yaml/DatabaseDaemon.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      291 2024-04-18 10:08:18.000000 quick_yaml-1.1b1/src/quick_yaml/__init__.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    22883 2024-04-22 04:20:07.000000 quick_yaml-1.1b1/src/quick_yaml/data_structures.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    35547 2024-04-22 04:18:15.000000 quick_yaml-1.1b1/src/quick_yaml/manager.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     4722 2024-04-12 04:46:47.000000 quick_yaml-1.1b1/src/quick_yaml/mkdocs.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     3905 2024-04-18 10:08:18.000000 quick_yaml-1.1b1/src/quick_yaml/mock_generator.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    10389 2024-04-18 10:08:18.000000 quick_yaml-1.1b1/src/quick_yaml/parser.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      923 2024-04-15 04:28:11.000000 quick_yaml-1.1b1/src/quick_yaml/setup.py
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/src/quick_yaml.egg-info/
--rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13707 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/PKG-INFO
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      653 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/SOURCES.txt
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)        1 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/dependency_links.txt
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       62 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/requires.txt
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       11 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/top_level.txt
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/test/
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1835 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_breeze_query.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1243 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_byaml.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1931 2024-04-22 03:40:11.000000 quick_yaml-1.1b1/test/test_concurrent.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2532 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_dbd.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1441 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_find.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2004 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_query.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2869 2024-04-22 03:41:00.000000 quick_yaml-1.1b1/test/test_transation.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2518 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/testdb_simple.py
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-23 10:19:35.617026 quick_yaml-1.1b2/
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     7652 2024-04-02 03:58:22.000000 quick_yaml-1.1b2/LICENSE
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       34 2024-04-12 08:36:58.000000 quick_yaml-1.1b2/MANIFEST.in
+-rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13708 2024-04-23 10:19:35.613028 quick_yaml-1.1b2/PKG-INFO
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    12900 2024-04-17 06:06:52.000000 quick_yaml-1.1b2/README.md
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      880 2024-04-23 10:18:53.000000 quick_yaml-1.1b2/pyproject.toml
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       38 2024-04-23 10:19:35.617026 quick_yaml-1.1b2/setup.cfg
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-23 10:19:35.613028 quick_yaml-1.1b2/src/
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-23 10:19:35.613028 quick_yaml-1.1b2/src/quick_yaml/
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      435 2024-04-12 09:08:35.000000 quick_yaml-1.1b2/src/quick_yaml/Btree.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     8829 2024-04-22 08:00:53.000000 quick_yaml-1.1b2/src/quick_yaml/DatabaseDaemon.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      291 2024-04-18 10:08:18.000000 quick_yaml-1.1b2/src/quick_yaml/__init__.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    25889 2024-04-23 05:57:15.000000 quick_yaml-1.1b2/src/quick_yaml/data_structures.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    46610 2024-04-23 10:16:25.000000 quick_yaml-1.1b2/src/quick_yaml/manager.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     4722 2024-04-12 04:46:47.000000 quick_yaml-1.1b2/src/quick_yaml/mkdocs.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     3905 2024-04-23 10:16:13.000000 quick_yaml-1.1b2/src/quick_yaml/mock_generator.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    10389 2024-04-23 10:15:27.000000 quick_yaml-1.1b2/src/quick_yaml/parser.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      923 2024-04-15 04:28:11.000000 quick_yaml-1.1b2/src/quick_yaml/setup.py
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-23 10:19:35.613028 quick_yaml-1.1b2/src/quick_yaml.egg-info/
+-rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13708 2024-04-23 10:19:35.000000 quick_yaml-1.1b2/src/quick_yaml.egg-info/PKG-INFO
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      653 2024-04-23 10:19:35.000000 quick_yaml-1.1b2/src/quick_yaml.egg-info/SOURCES.txt
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)        1 2024-04-23 10:19:35.000000 quick_yaml-1.1b2/src/quick_yaml.egg-info/dependency_links.txt
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       62 2024-04-23 10:19:35.000000 quick_yaml-1.1b2/src/quick_yaml.egg-info/requires.txt
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       11 2024-04-23 10:19:35.000000 quick_yaml-1.1b2/src/quick_yaml.egg-info/top_level.txt
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-23 10:19:35.613028 quick_yaml-1.1b2/test/
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1835 2024-04-15 03:31:51.000000 quick_yaml-1.1b2/test/test_breeze_query.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1243 2024-04-15 03:31:51.000000 quick_yaml-1.1b2/test/test_byaml.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1947 2024-04-23 03:34:08.000000 quick_yaml-1.1b2/test/test_concurrent.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2532 2024-04-15 03:31:51.000000 quick_yaml-1.1b2/test/test_dbd.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1441 2024-04-15 03:31:51.000000 quick_yaml-1.1b2/test/test_find.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2004 2024-04-15 03:31:51.000000 quick_yaml-1.1b2/test/test_query.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2869 2024-04-22 03:41:00.000000 quick_yaml-1.1b2/test/test_transation.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2518 2024-04-15 03:31:51.000000 quick_yaml-1.1b2/test/testdb_simple.py
```

### Comparing `quick_yaml-1.1b1/LICENSE` & `quick_yaml-1.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/PKG-INFO` & `quick_yaml-1.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: quick_yaml
-Version: 1.1b1
+Version: 1.1b2
 Summary: A simple Database Management System for users who want self-contained DBMS that uses YAML File format to store values.
 Author-email: Sivarajan R <sivarajan931@gmail.com>
-Project-URL: Homepage, https://gitlab.com/eazy-home-admin/BreezeDB/
-Project-URL: Issues, https://gitlab.com/eazy-home-admin/BreezeDB/issues
+Project-URL: Homepage, https://gitlab.com/eazy-home-admin/QuickYAML
+Project-URL: Issues, https://gitlab.com/eazy-home-admin/QuickYAML/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
```

### Comparing `quick_yaml-1.1b1/README.md` & `quick_yaml-1.1b2/README.md`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/pyproject.toml` & `quick_yaml-1.1b2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "quick_yaml"
-version = "1.1b1"
+version = "1.1b2"
 authors = [
   { name="Sivarajan R", email="sivarajan931@gmail.com" },
 ]
 description = "A simple Database Management System for users who want self-contained DBMS that uses YAML File format to store values."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -19,13 +19,13 @@
     "numpy",
     "pyyaml",
     "setuptools",
     "jmespath",
     "requests"
 ]
 [project.urls]
-Homepage = "https://gitlab.com/eazy-home-admin/BreezeDB/"
-Issues = "https://gitlab.com/eazy-home-admin/BreezeDB/issues"
+Homepage = "https://gitlab.com/eazy-home-admin/QuickYAML"
+Issues = "https://gitlab.com/eazy-home-admin/QuickYAML/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `quick_yaml-1.1b1/src/quick_yaml/DatabaseDaemon.py` & `quick_yaml-1.1b2/src/quick_yaml/DatabaseDaemon.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/src/quick_yaml/data_structures.py` & `quick_yaml-1.1b2/src/quick_yaml/data_structures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__all__ = ['NestedDict', 'BYAML', 'RecordLockManager', 'RecordLock']
+
 import logging
 import threading
 
 import jmespath
 import numpy as np
 import pandas as pd
 import yaml
@@ -401,55 +403,15 @@
                     new_path = path + (key,)
                     self.stack.append((new_path, value))
             else:
                 return '.'.join(path), current
         raise StopIteration
 
 
-class NestedDictIterator:
-    """
-               An iterator class for NestedDict, allowing iteration over all key-value pairs in the nested dictionary.
-
-               Attributes:
-                   stack (list of tuples): A stack used for depth-first traversal of the dictionary. Each tuple contains a path (as a tuple of keys) and the current dictionary or value to process.
-           """
-
-    def __init__(self, data):
-
-        self.stack = [((), data)]  # Initialize with a tuple of path and data
-
-    def __iter__(self):
-        """
-            Initializes the NestedDictIterator with the nested dictionary data.
-
-            Parameters:
-                data (dict): The nested dictionary data to iterate over.
-        """
-
-        return self
-
-    def __next__(self):
-        """
-              Returns the next key-value pair in the nested dictionary as a dot-separated key string and its value.
-
-              Returns:
-                  A tuple containing a dot-separated key string and its corresponding value.
 
-              Raises:
-                  StopIteration: If there are no more items to iterate over.
-            """
-        while self.stack:
-            path, current = self.stack.pop()
-            if isinstance(current, dict):
-                for key, value in current.items():
-                    new_path = path + (key,)
-                    self.stack.append((new_path, value))
-            else:
-                return '.'.join(path), current
-        raise StopIteration
 
 
 class BYAML:
     """
       A class for handling the encoding and decoding of nested dictionaries into/from an encrypted or plain binary YAML format.
 
       Attributes:
@@ -579,58 +541,178 @@
 class RecordLock:
     def __init__(self):
         self.writer_lock = threading.Semaphore(1)
         self.mutex = threading.Lock()
         self.readers = 0
 
 
+class RecordLock:
+    def __init__(self):
+        self.writer_lock = threading.Semaphore(1)  # Ensure only one writer at a time
+        self.mutex = threading.Lock()  # Mutex for managing readers count
+        self.readers = 0  # Counter for active readers
+
+
 class RecordLockManager:
-    def __init__(self, logger=None):
-        self.records = {}
-        self.mutex = threading.Lock()
-        if logger is None:
+    """
+    A class for managing record-level locks in a thread-safe manner.
+
+    Attributes:
+        - records (dict): A dictionary of record locks, where the keys are table names and the values are dictionaries
+            of record locks.
+        - mutex (threading.Lock): A global mutex for synchronizing access to the records dictionary.
+
+    Methods:
+        make_record_lock(self, table_name, record_id)
+        acquire_writer_lock(self, table_name, record_id)
+        release_writer_lock(self, table_name, record_id)
+        acquire_reader_lock(self, table_name, record_id)
+        release_reader_lock(self, table_name, record_id)
+    """
+
+    def __init__(self, logger=None,create_logger=False):
+        """
+        Initializes a RecordLockManager instance with an optional logger.
+        Parameters:
+            - logger (logging.Logger): An optional logger to use. If not provided, a default logger is created.
+            - create_logger (bool): Whether to create a logger if one is not provided. Defaults to False.
+        """
+        self.records = {}  # Use a dictionary for storing locks
+        self.mutex = threading.Lock()  # Global mutex for synchronizing lock creation
+        if logger is None and create_logger :
             logger = logging.getLogger("RecordLockManager")
             handler = logging.StreamHandler()
             formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
             handler.setFormatter(formatter)
             logger.addHandler(handler)
             logger.setLevel(logging.DEBUG)
         self.logger = logger
 
-    def make_record_lock(self, record_id):
+    def make_record_lock(self, table_name, record_id):
+        """
+        Creates a record lock for the specified table and record ID if it doesn't exist.
+
+        Parameters:
+            - table_name (str): The name of the table.
+            - record_id (str): The ID of the record.
+
+        Returns:
+            None
+
+        """
         with self.mutex:
-            if record_id not in self.records:
-                self.records[record_id] = RecordLock()
-                self.logger.debug(f"Record lock created for ID: {record_id}")
+            if table_name not in self.records:
+                self.records[table_name] = {}
+            if record_id not in self.records[table_name]:
+                self.records[table_name][record_id] = RecordLock()
+                self.logger.debug(f"Record lock created for {table_name} ID: {record_id}")
+
+    def acquire_writer_lock(self, table_name, record_id):
+        """
+        Acquires a writer lock for the specified table and record ID.
+
+        Parameters:
+            - table_name (str): The name of the table.
+            - record_id (str): The ID of the record.
 
-    def acquire_writer_lock(self, record_id):
+        Returns:
+            None
+        """
         with self.mutex:
-            if record_id not in self.records:
-                self.make_record_lock(record_id)
-            self.logger.debug(f"Writer waiting to acquire lock for record {record_id}")
-        self.records[record_id].writer_lock.acquire()
-        self.logger.debug(f"Writer acquired lock for record {record_id}")
-
-    def release_writer_lock(self, record_id):
-        self.records[record_id].writer_lock.release()
-        self.logger.debug(f"Writer released lock for record {record_id}")
+            if table_name not in self.records or record_id not in self.records[table_name]:
+                self.make_record_lock(table_name, record_id)
+            self.logger.debug(f"Writer waiting to acquire lock for {table_name} record {record_id}")
+        self.records[table_name][record_id].writer_lock.acquire()
+        self.logger.debug(f"Writer acquired lock for {table_name} record {record_id}")
+
+    def release_writer_lock(self, table_name, record_id):
+        """
+        Releases a writer lock for the specified table and record ID.
+
+        Parameters:
+            - table_name (str): The name of the table.
+            - record_id (str): The ID of the record.
+
+        Returns:
+            None
+        """
+        self.records[table_name][record_id].writer_lock.release()
+        self.logger.debug(f"Writer released lock for {table_name} record {record_id}")
+
+    def acquire_reader_lock(self, table_name, record_id):
+        """
+        Acquires a reader lock for the specified table and record ID.
+
+        Parameters:
+            - table_name (str): The name of the table.
+            - record_id (str): The ID of the record.
 
-    def acquire_reader_lock(self, record_id):
+        Returns:
+            None
+        """
         with self.mutex:
-            if record_id not in self.records:
-                self.make_record_lock(record_id)
-            record = self.records[record_id]
-            record.mutex.acquire()
-
-        record.readers += 1
-        if record.readers == 1:
-            record.writer_lock.acquire()
-        record.mutex.release()
-        self.logger.debug(f"Reader acquired lock for record {record_id}, total readers: {record.readers}")
-
-    def release_reader_lock(self, record_id):
-        with self.records[record_id].mutex:
-            record = self.records[record_id]
+            if table_name not in self.records or record_id not in self.records[table_name]:
+                self.make_record_lock(table_name, record_id)
+            record = self.records[table_name][record_id]
+        with record.mutex:
+            record.readers += 1
+            if record.readers == 1:
+                record.writer_lock.acquire()
+        self.logger.debug(f"Reader acquired lock for {table_name} record {record_id}, total readers: {record.readers}")
+
+    def release_reader_lock(self, table_name, record_id):
+        """
+        Releases a reader lock for the specified table and record ID.
+
+        Parameters:
+            - table_name (str): The name of the table.
+            - record_id (str): The ID of the record.
+
+        Returns:
+            None
+        """
+        with self.records[table_name][record_id].mutex:
+            record = self.records[table_name][record_id]
             record.readers -= 1
-            self.logger.debug(f"Reader released lock for record {record_id}, remaining readers: {record.readers}")
             if record.readers == 0:
                 record.writer_lock.release()
+            self.logger.debug(
+                f"Reader released lock for {table_name} record {record_id}, remaining readers: {record.readers}")
+
+    def delete_lock_id(self, table_name, record_id):
+        """
+        Deletes a lock for the specified table and record ID.
+
+        Parameters:
+            - table_name (str): The name of the table.
+            - record_id (str): The ID of the record.
+
+        Returns:
+            None
+        """
+        with self.mutex:
+            if table_name in self.records and record_id in self.records[table_name]:
+                del self.records[table_name][record_id]
+                self.logger.debug(f"Record lock deleted for {table_name} ID: {record_id}")
+
+    def delete_lock_table(self,table_name):
+        """
+        Deletes all locks for the specified table.
+
+        Parameters:
+            - table_name (str): The name of the table.
+
+        Returns:
+            None
+        """
+        with self.mutex:
+            if table_name in self.records:
+                # before that release all the locks
+                for record_id in list(self.records[table_name]):
+                    try:
+                        self.release_reader_lock(table_name, record_id)
+                        self.release_writer_lock(table_name, record_id)
+                    except:
+
+                        continue
+                del self.records[table_name]
+                self.logger.debug(f"Record lock table deleted for {table_name}")
```

### Comparing `quick_yaml-1.1b1/src/quick_yaml/manager.py` & `quick_yaml-1.1b2/src/quick_yaml/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+# __all__ = ['QYAMLDB', 'QYAMLDBCoarse', 'MetaData']
+
 import logging
 import time
 from threading import Semaphore, Lock
 
 import jmespath
+import sys
 
-from .data_structures import BYAML, NestedDict
+from .data_structures import BYAML, NestedDict, RecordLockManager
 from .parser import QueryProcessor
 import pandas as pd
 import copy
 
 
 class MetaData:
     """
@@ -186,14 +189,29 @@
                 self.tables[table_name] = {
                     'metadata': metadata,
                     'data': NestedDict(table_info['data'])
                 }
         except Exception:
             print("WARNING CANNOT LOAD META DATA")
 
+    def generate_new_id(self, table_name):
+        """
+        Generates new ID for records
+        """
+        # Get existing IDs as integers
+        existing_ids = [int(key) for key in self.tables[table_name]['data'].get_dict().keys()]
+
+        # Find missing IDs if there are any gaps
+        missing_ids = [i for i in range(1, max(existing_ids) + 1) if i not in existing_ids] if existing_ids else []
+
+        # Use the first missing ID if available; otherwise, use the next highest ID
+        entry_id = str(missing_ids[0]) if missing_ids else str(max(existing_ids) + 1 if existing_ids else 1)
+
+        return entry_id
+
     def insert_new_data(self, table_name, data):
         """
         Insert new data into the specified table.
 
         Parameters:
             table_name (str): Name of the table to insert data into.
             data (dict): Data to be inserted into the table.
@@ -211,23 +229,15 @@
         # Check for unique constraints
         unique_columns = self.tables[table_name]['metadata'].get_unique_columns(table_name)
         for column in unique_columns:
             if column in data and any(
                     data[column] == row.get(column) for row in self.tables[table_name]['data'].get_dict().values()):
                 raise ValueError(f"Unique constraint violated for column: {column}")
 
-        # Get existing IDs as integers
-        existing_ids = [int(key) for key in self.tables[table_name]['data'].get_dict().keys()]
-
-        # Find missing IDs if there are any gaps
-        missing_ids = [i for i in range(1, max(existing_ids) + 1) if i not in existing_ids] if existing_ids else []
-
-        # Use the first missing ID if available; otherwise, use the next highest ID
-        entry_id = str(missing_ids[0]) if missing_ids else str(max(existing_ids) + 1 if existing_ids else 1)
-
+        entry_id = self.generate_new_id(table_name)
         # Insert the data with the new entry_id
         self.tables[table_name]['data'][entry_id] = data
         self.save_db()
         return 'done'
 
     def insert_many(self, table_name, list_of_values):
         """
@@ -525,14 +535,16 @@
                     elif on_invalid_command == 'continue':
                         transaction_report['list_of_failed_operations_id'].append(transaction_id)
                         continue
                 transaction_report['successful_operations'] += 1
             except Exception as e:
                 if error_strategy == 'rollback':
                     self.tables = self._backup_table
+                    self.save_db()  # Save roll-backed DB.
+                    del self._backup_table
                     transaction_report['failed_operation'] += len(transactional_data) - transaction_report[
                         'successful_operations']
                     return {'status': 'Failure', 'error_message': str(e), 'details': transaction_report}
                 elif error_strategy == 'break':
                     transaction_report['failed_operation'] += len(transactional_data) - transaction_report[
                         'successful_operations']
                     return {'status': 'Failure', 'error_message': str(e), 'details': transaction_report}
@@ -634,22 +646,21 @@
         self._log(f'Released writer lock.With {self._readers} _readers', 'debug')
 
     def _start_read(self):
         """
         Function to acquire the reader lock.
         """
         self._log('Waiting to acquire reader lock', 'debug')
-        self._mutex.acquire() # Acquire mutex lock to synchronize readers attaining lock
+        self._mutex.acquire()  # Acquire mutex lock to synchronize readers attaining lock
         while self._writers_waiting:
             # Release all the readers until writers are finished.
             self._log(f'Lock Released due to waiting of writers. No of _readers {self._readers}')
-            self._mutex.release() # Release mutex in favor of writers
+            self._mutex.release()  # Release mutex in favor of writers
             time.sleep(0.1)  # Sleep to prevent busy waiting
-            self._mutex.acquire() # Again Try to aqquire locks.
-
+            self._mutex.acquire()  # Again Try to acquire locks.
 
         self._log('Acquired reader lock', 'debug')
         self._readers += 1
 
         if self._readers == 1:
             self._log('Waiting for writers lock by _readers', 'debug')
             self._writers_lock.acquire()
@@ -951,9 +962,326 @@
 
         return result
 
 
 class QYAMLDBFine(QYAMLDB):
     """
     A subclass of QYAMLDB that implements fine-grained locking. It implements read/write lock in record level.
+
     """
-    pass
+
+    def __init__(self, path, key_file='key.file', encrypted=False, byaml=None, log_file='qyaml.log',
+                 enable_logging=True,
+                 log_level=logging.DEBUG, silent=False):
+
+        super().__init__(path, key_file, encrypted, byaml, log_file, enable_logging, log_level, silent)
+        self._lock_manager = RecordLockManager(self._logger)
+
+    def insert_new_data(self, table_name, data):
+        """
+        Insert new data into the table in a thread-safe manner.
+
+        Parameters:
+            table_name (str): Name of the table.
+            data (dict): Data to insert.
+
+        Returns:
+            str: A message indicating the insertion operation is done.
+
+        Raises:
+            ValueError: If the table does not exist, the entry does not exist, or a unique constraint is violated.
+        """
+        if table_name not in self.tables:
+            raise ValueError("Table does not exist.")
+
+        # Generate a unique Record ID for the new data
+        entry_id = self.generate_new_id(table_name)
+
+        # Acquire a write lock for the newly generated ID
+        self._lock_manager.acquire_writer_lock(entry_id)
+
+        try:
+            # Check for unique constraints
+            unique_columns = self.tables[table_name]['metadata'].get_unique_columns()
+            if any(data.get(column) in [row.get(column) for row in self.tables[table_name]['data'].values()] for column
+                   in unique_columns):
+                raise ValueError("Unique constraint violated.")
+
+            # Insert the data
+            self.tables[table_name]['data'][entry_id] = data
+            self.save_db()
+            self._logger.debug(f"Inserted data for record {entry_id} into table {table_name}")
+        except Exception as e:
+            raise e
+        finally:
+            # Release the write lock
+            self._lock_manager.release_writer_lock(table_name, entry_id)
+
+        return "done."
+
+    def update_entry(self, table_name, entry_id, updated_data):
+        """"""
+        if table_name not in self.tables or entry_id not in self.tables[table_name]['data'].keys():
+            raise ValueError("Table or entry does not exist.")
+        try:
+            self._lock_manager.acquire_writer_lock(table_name, entry_id)
+            self.tables[table_name]['data'][entry_id].update(updated_data)
+            self.save_db()
+            self.save_db()
+        except Exception as e:
+            raise e
+        finally:
+            # Release the lock
+            self._lock_manager.release_writer_lock(table_name, entry_id)
+
+        return "done."
+
+    def update_many(self, table_name, condition, update_data, flags=None):
+        """ Updates data based on given condition.
+        Parameters:
+            condition (dict): Filtering Conditions.
+            update_data (dict): Data to be updated.
+            flags: Additional flags (Supported: { add_missing_values : 'True'/False}).
+            table_name: Name of table.
+        """
+        if flags is None:
+            flags = {'add_missing_values': True}
+        if table_name not in self.tables:
+            raise ValueError(f"Table '{table_name}' does not exist.")
+
+        # Retrieve the metadata to check for unique constraints
+        unique_columns = self.tables[table_name]['metadata'].get_unique_columns(table_name)
+        qp = QueryProcessor(self.tables[table_name])
+        qp.filter_id(condition)
+        matching_ids = qp.results
+
+        if not matching_ids:
+            return None  # No data matching the condition
+
+        # Sort IDs to avoid deadlock
+        matching_ids.sort()
+
+        locked_ids = []
+        try:
+            # Acquire locks for all relevant records
+            for entry_id in matching_ids:
+                self._lock_manager.acquire_writer_lock(table_name, entry_id)
+                locked_ids.append(entry_id)
+
+            # Perform updates
+            super().update_many(table_name, condition, update_data, flags)
+
+            # Release locks
+            for entry_id in locked_ids:
+                self._lock_manager.release_writer_lock(table_name, entry_id)
+        except Exception as e:
+            raise e
+        finally:
+            # Release locks
+            for entry_id in locked_ids:
+                self._lock_manager.release_writer_lock(table_name, entry_id)
+
+        return "done."
+
+    def delete_entry(self, table_name, entry_id):
+        """"""
+        if table_name not in self.tables or entry_id not in self.tables[table_name]['data'].keys():
+            raise ValueError("Table or entry does not exist.")
+        try:
+            self._lock_manager.acquire_writer_lock(table_name, entry_id)
+            del self.tables[table_name]['data'][entry_id]
+
+            self.save_db()
+        except Exception as e:
+            raise e
+        finally:
+            # Release the lock
+            self._lock_manager.release_writer_lock(table_name, entry_id)
+            self._lock_manager.delete_lock_id(table_name, entry_id)
+
+        return "done."
+
+    def delete_table(self, table_name):
+        """"""
+
+        if table_name not in self.tables:
+            raise ValueError("Table does not exist.")
+
+        # Acquire lock for entire id
+        for i in self.tables[table_name]['data'].keys():
+            self._lock_manager.acquire_writer_lock(table_name, i)
+        del self.tables[table_name]
+
+        self.save_db()
+
+        # Delete the tab
+
+    def delete_many(self, table_name, condition):
+        """
+        Delete multiple records from a table based on a given condition.
+        Threadsafe
+        Parameters:
+            table_name (str): The name of the table to delete records from.
+            condition (dict): The condition to filter the records to be deleted.
+        Raises:
+            ValueError: If the table does not exist in the database.
+        Returns:
+            str: A message confirming the deletion process is done.
+        """
+        if table_name not in self.tables:
+            raise ValueError(f"Table '{table_name}' does not exist.")
+
+        # Retrieve the metadata to check for unique constraints
+        qp = QueryProcessor(self.tables[table_name])
+        qp.filter_id(condition)
+        matching_ids = qp.result
+
+        if not matching_ids:
+            return None  # No data matching the condition
+
+        # Sort IDs to avoid deadlock
+        matching_ids.sort()
+
+        locked_ids = []
+        try:
+            # Acquire locks for all relevant records
+            for entry_id in matching_ids:
+                self._lock_manager.acquire_writer_lock(table_name, entry_id)
+                locked_ids.append(entry_id)
+
+            # Perform updates
+            for entry_id in matching_ids:
+                del self.tables[table_name]['data'][entry_id]
+
+            self.save_db()
+
+        except Exception as e:
+            raise e
+        finally:
+            # Release locks
+            for entry_id in locked_ids:
+                self._lock_manager.release_writer_lock(table_name, entry_id)
+                # remove all the locks associated with id
+                self._lock_manager.delete_lock_id(table_name, entry_id)
+
+        return "done."
+
+    def find_all(self, table_name):
+        """
+        Returns all the record.
+        Returns:
+            list: A list of all the records in the table.
+        Raises:
+            ValueError: If the table does not exist in the database.
+        """
+        if table_name not in self.tables:
+            raise ValueError("Table does not exist.")
+
+        self._lock_for_read(table_name)
+        results = self.tables[table_name]['data'].values()
+        self._release_read(table_name)
+        return results
+
+    def find(self, table_name, query):
+        """
+        Find for specific records based on $filter query
+
+        Parameters:
+            table_name (str): The name of the table to search in.
+            query (dict): The query to filter the data.
+
+        Returns:
+            list: The results of the query execution.
+        Raises:
+            ValueError: If the table does not exist in the database.
+        """
+        if table_name not in self.tables:
+            raise ValueError("Table does not exist.")
+
+        self._lock_for_read(table_name)
+        qp = QueryProcessor(self.tables[table_name])
+        results = qp.filter(query)
+        self._release_read(table_name)
+        return results
+
+    def _lock_for_read(self, table_name):
+        """
+        Lock All the record in the table for reading
+
+       **DO NOT USE THIS FUNCTION. IT IS MEANT FOR INTERNAL PURPOSES.**
+
+        Parameters:
+            table_name (str): The name of the table to lock.
+
+        Returns:
+            None
+        """
+
+        if table_name not in self.tables:
+            raise ValueError(f"Table '{table_name}' does not exist.")
+
+        # lock for all data
+        for i in self.tables[table_name]['data'].keys():
+            self._lock_manager.acquire_reader_lock(table_name, i)
+
+    def _release_read(self, table_name):
+        """
+        Release All the record in the table for reading
+
+       **DO NOT USE THIS FUNCTION.
+       IT IS MEANT FOR INTERNAL PURPOSES.**
+
+        Parameters:
+            table_name (str): The name of the table to lock.
+
+        Returns:
+            None
+        """
+
+        if table_name not in self.tables:
+            raise ValueError(f"Table '{table_name}' does not exist.")
+
+        # lock for all data
+        for i in self.tables[table_name]['data'].keys():
+            self._lock_manager.release_reader_lock(table_name, i)
+
+    # _lock_write
+
+    def _lock_for_write(self, table_name):
+        """
+        Lock All the record in the table for writing
+
+       **DO NOT USE THIS FUNCTION. IT IS MEANT FOR INTERNAL PURPOSES.**
+
+        Parameters:
+            table_name (str): The name of the table to lock.
+
+        Returns:
+            None
+        """
+
+        if table_name not in self.tables:
+            raise ValueError(f"Table '{table_name}' does not exist.")
+
+        # lock for all data
+        for i in self.tables[table_name]['data'].keys():
+            self._lock_manager.acquire_writer_lock(table_name, i)
+
+    def _release_write(self, table_name):
+        """
+        Release All the record in the table for writing
+
+       **DO NOT USE THIS FUNCTION. IT IS MEANT FOR INTERNAL PURPOSES.**
+
+        Parameters:
+            table_name (str): The name of the table to lock.
+
+        Returns:
+            None
+        """
+
+        if table_name not in self.tables:
+            raise ValueError(f"Table '{table_name}' does not exist.")
+
+        # lock for all data
+        for i in self.tables[table_name]['data'].keys():
+            self._lock_manager.release_writer_lock(table_name, i)
```

### Comparing `quick_yaml-1.1b1/src/quick_yaml/mkdocs.py` & `quick_yaml-1.1b2/src/quick_yaml/mkdocs.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/src/quick_yaml/mock_generator.py` & `quick_yaml-1.1b2/src/quick_yaml/mock_generator.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/src/quick_yaml/parser.py` & `quick_yaml-1.1b2/src/quick_yaml/parser.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/src/quick_yaml/setup.py` & `quick_yaml-1.1b2/src/quick_yaml/setup.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/src/quick_yaml.egg-info/PKG-INFO` & `quick_yaml-1.1b2/src/quick_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: quick_yaml
-Version: 1.1b1
+Version: 1.1b2
 Summary: A simple Database Management System for users who want self-contained DBMS that uses YAML File format to store values.
 Author-email: Sivarajan R <sivarajan931@gmail.com>
-Project-URL: Homepage, https://gitlab.com/eazy-home-admin/BreezeDB/
-Project-URL: Issues, https://gitlab.com/eazy-home-admin/BreezeDB/issues
+Project-URL: Homepage, https://gitlab.com/eazy-home-admin/QuickYAML
+Project-URL: Issues, https://gitlab.com/eazy-home-admin/QuickYAML/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
```

### Comparing `quick_yaml-1.1b1/src/quick_yaml.egg-info/SOURCES.txt` & `quick_yaml-1.1b2/src/quick_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/test/test_breeze_query.py` & `quick_yaml-1.1b2/test/test_breeze_query.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/test/test_byaml.py` & `quick_yaml-1.1b2/test/test_byaml.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/test/test_concurrent.py` & `quick_yaml-1.1b2/test/test_concurrent.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from random import randint
 
 from src.quick_yaml.manager import QYAMLDB, QYAMLDBCoarse
 
 # Initialize the database
 db_path = "test_db.ezdb"
-db = QYAMLDBCoarse(path=db_path)
+db = QYAMLDBCoarse(path=db_path,encrypted=False)
 
 # Setup initial tables and data
 db.create_table("test_table")
 for i in range(10):
     db.insert_new_data("test_table", {"id": i, "value": f"initial_data_{i}"})
```

### Comparing `quick_yaml-1.1b1/test/test_dbd.py` & `quick_yaml-1.1b2/test/test_dbd.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/test/test_find.py` & `quick_yaml-1.1b2/test/test_find.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/test/test_query.py` & `quick_yaml-1.1b2/test/test_query.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/test/test_transation.py` & `quick_yaml-1.1b2/test/test_transation.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.1b1/test/testdb_simple.py` & `quick_yaml-1.1b2/test/testdb_simple.py`

 * *Files identical despite different names*

