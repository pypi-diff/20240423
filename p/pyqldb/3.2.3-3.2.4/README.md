# Comparing `tmp/pyqldb-3.2.3.tar.gz` & `tmp/pyqldb-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqldb-3.2.3.tar", last modified: Wed May 24 11:38:18 2023, max compression
+gzip compressed data, was "dist/pyqldb-3.2.4.tar", last modified: Wed Apr 17 18:36:07 2024, max compression
```

## Comparing `pyqldb-3.2.3.tar` & `pyqldb-3.2.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.993319 pyqldb-3.2.3/
--rw-r--r--   0 batteson   (504) staff       (20)    10141 2022-11-24 12:16:35.000000 pyqldb-3.2.3/LICENSE
--rw-r--r--   0 batteson   (504) staff       (20)       72 2022-11-24 12:16:35.000000 pyqldb-3.2.3/NOTICE
--rw-r--r--   0 batteson   (504) staff       (20)     6629 2023-05-24 11:38:18.993175 pyqldb-3.2.3/PKG-INFO
--rw-r--r--   0 batteson   (504) staff       (20)     6100 2023-03-24 09:43:15.000000 pyqldb-3.2.3/README.md
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.989116 pyqldb-3.2.3/pyqldb/
--rw-r--r--   0 batteson   (504) staff       (20)      590 2023-05-24 11:32:41.000000 pyqldb-3.2.3/pyqldb/__init__.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.990038 pyqldb-3.2.3/pyqldb/communication/
--rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/communication/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)     8261 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/communication/session_client.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.990300 pyqldb-3.2.3/pyqldb/config/
--rw-r--r--   0 batteson   (504) staff       (20)      562 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/config/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)     3123 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/config/retry_config.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.990834 pyqldb-3.2.3/pyqldb/cursor/
--rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)     2326 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/buffered_cursor.py
--rw-r--r--   0 batteson   (504) staff       (20)     4147 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/read_ahead_cursor.py
--rw-r--r--   0 batteson   (504) staff       (20)     5825 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/stream_cursor.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.991090 pyqldb-3.2.3/pyqldb/driver/
--rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/driver/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)    16772 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/driver/qldb_driver.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.991266 pyqldb-3.2.3/pyqldb/errors/
--rw-r--r--   0 batteson   (504) staff       (20)     5561 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/errors/__init__.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.991702 pyqldb-3.2.3/pyqldb/execution/
--rw-r--r--   0 batteson   (504) staff       (20)      562 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/execution/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)     1409 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/execution/executable.py
--rw-r--r--   0 batteson   (504) staff       (20)     2154 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/execution/executor.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.992135 pyqldb-3.2.3/pyqldb/session/
--rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/session/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)     6383 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/session/qldb_session.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.992415 pyqldb-3.2.3/pyqldb/transaction/
--rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/transaction/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)     5620 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/transaction/transaction.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.992972 pyqldb-3.2.3/pyqldb/util/
--rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/__init__.py
--rw-r--r--   0 batteson   (504) staff       (20)     1495 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/atomic_integer.py
--rw-r--r--   0 batteson   (504) staff       (20)     3790 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/qldb_hash.py
--rw-r--r--   0 batteson   (504) staff       (20)     1503 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/retry.py
-drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.989782 pyqldb-3.2.3/pyqldb.egg-info/
--rw-r--r--   0 batteson   (504) staff       (20)     6629 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/PKG-INFO
--rw-r--r--   0 batteson   (504) staff       (20)      847 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/SOURCES.txt
--rw-r--r--   0 batteson   (504) staff       (20)        1 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/dependency_links.txt
--rw-r--r--   0 batteson   (504) staff       (20)       81 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/requires.txt
--rw-r--r--   0 batteson   (504) staff       (20)        7 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/top_level.txt
--rw-r--r--   0 batteson   (504) staff       (20)       38 2023-05-24 11:38:18.993358 pyqldb-3.2.3/setup.cfg
--rw-r--r--   0 batteson   (504) staff       (20)     1670 2023-05-24 11:26:56.000000 pyqldb-3.2.3/setup.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)    10141 2024-04-16 22:20:25.000000 pyqldb-3.2.4/LICENSE
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)       72 2024-04-16 22:20:25.000000 pyqldb-3.2.4/NOTICE
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     6629 2024-04-17 18:36:06.000000 pyqldb-3.2.4/PKG-INFO
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     6100 2024-04-16 22:20:25.000000 pyqldb-3.2.4/README.md
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      590 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/__init__.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/communication/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      567 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/communication/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     8261 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/communication/session_client.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/config/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      562 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/config/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     3123 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/config/retry_config.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/cursor/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      567 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/cursor/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     2326 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/cursor/buffered_cursor.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     4147 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/cursor/read_ahead_cursor.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     5825 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/cursor/stream_cursor.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/driver/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      567 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/driver/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)    16772 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/driver/qldb_driver.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/errors/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     5561 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/errors/__init__.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/execution/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      562 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/execution/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     1409 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/execution/executable.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     2154 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/execution/executor.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/session/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      567 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/session/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     6383 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/session/qldb_session.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/transaction/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      567 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/transaction/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     5620 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/transaction/transaction.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb/util/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      567 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/util/__init__.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     1495 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/util/atomic_integer.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     3790 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/util/qldb_hash.py
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     1508 2024-04-16 22:20:25.000000 pyqldb-3.2.4/pyqldb/util/retry.py
+drwxr-xr-x   0 sttyle   (6415858) amazon     (100)        0 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb.egg-info/
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     6629 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb.egg-info/PKG-INFO
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)      847 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb.egg-info/SOURCES.txt
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)        1 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb.egg-info/dependency_links.txt
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)       81 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb.egg-info/requires.txt
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)        7 2024-04-17 18:36:06.000000 pyqldb-3.2.4/pyqldb.egg-info/top_level.txt
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)       38 2024-04-17 18:36:06.000000 pyqldb-3.2.4/setup.cfg
+-rw-r--r--   0 sttyle   (6415858) amazon     (100)     1670 2024-04-16 22:20:25.000000 pyqldb-3.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyqldb-3.2.3/LICENSE` & `pyqldb-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/PKG-INFO` & `pyqldb-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqldb
-Version: 3.2.3
+Version: 3.2.4
 Summary: Python driver for Amazon QLDB
 Author: Amazon Web Services
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyqldb-3.2.3/README.md` & `pyqldb-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/__init__.py` & `pyqldb-3.2.4/pyqldb/config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"). You may not use this file except in compliance with
 # the License. A copy of the License is located at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
 # CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions
 # and limitations under the License.
-
-__version__ = '3.2.3'
```

### Comparing `pyqldb-3.2.3/pyqldb/communication/__init__.py` & `pyqldb-3.2.4/pyqldb/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/communication/session_client.py` & `pyqldb-3.2.4/pyqldb/communication/session_client.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/config/__init__.py` & `pyqldb-3.2.4/pyqldb/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/config/retry_config.py` & `pyqldb-3.2.4/pyqldb/config/retry_config.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/cursor/__init__.py` & `pyqldb-3.2.4/pyqldb/cursor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/cursor/buffered_cursor.py` & `pyqldb-3.2.4/pyqldb/cursor/buffered_cursor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/cursor/read_ahead_cursor.py` & `pyqldb-3.2.4/pyqldb/cursor/read_ahead_cursor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/cursor/stream_cursor.py` & `pyqldb-3.2.4/pyqldb/cursor/stream_cursor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/driver/__init__.py` & `pyqldb-3.2.4/pyqldb/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/driver/qldb_driver.py` & `pyqldb-3.2.4/pyqldb/driver/qldb_driver.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/errors/__init__.py` & `pyqldb-3.2.4/pyqldb/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/execution/__init__.py` & `pyqldb-3.2.4/pyqldb/session/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"). You may not use this file except in compliance with
 # the License. A copy of the License is located at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
```

### Comparing `pyqldb-3.2.3/pyqldb/execution/executable.py` & `pyqldb-3.2.4/pyqldb/execution/executable.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/execution/executor.py` & `pyqldb-3.2.4/pyqldb/execution/executor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/session/__init__.py` & `pyqldb-3.2.4/pyqldb/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/session/qldb_session.py` & `pyqldb-3.2.4/pyqldb/session/qldb_session.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/transaction/__init__.py` & `pyqldb-3.2.4/pyqldb/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/transaction/transaction.py` & `pyqldb-3.2.4/pyqldb/transaction/transaction.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/util/__init__.py` & `pyqldb-3.2.4/pyqldb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,7 +4,9 @@
 # the License. A copy of the License is located at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
 # CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions
 # and limitations under the License.
+
+__version__ = '3.2.4'
```

### Comparing `pyqldb-3.2.3/pyqldb/util/atomic_integer.py` & `pyqldb-3.2.4/pyqldb/util/atomic_integer.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/util/qldb_hash.py` & `pyqldb-3.2.4/pyqldb/util/qldb_hash.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/pyqldb/util/retry.py` & `pyqldb-3.2.4/pyqldb/util/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
 
         return delay
 
     @staticmethod
     def _get_delay_with_equal_jitter(retry_attempt, retry_config):
         capped_retries = min(retry_attempt, MAX_POW)
         delay_seed = min(retry_config.base * (1 << capped_retries), MAX_BACKOFF)
-        delay = delay_seed / 2 + random.randint(0, delay_seed / 2)
+        delay = delay_seed / 2 + random.randint(0, int(delay_seed / 2))
 
         return delay
```

### Comparing `pyqldb-3.2.3/pyqldb.egg-info/PKG-INFO` & `pyqldb-3.2.4/pyqldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqldb
-Version: 3.2.3
+Version: 3.2.4
 Summary: Python driver for Amazon QLDB
 Author: Amazon Web Services
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyqldb-3.2.3/pyqldb.egg-info/SOURCES.txt` & `pyqldb-3.2.4/pyqldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.3/setup.py` & `pyqldb-3.2.4/setup.py`

 * *Files identical despite different names*

