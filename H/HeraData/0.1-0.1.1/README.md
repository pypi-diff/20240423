# Comparing `tmp/HeraData-0.1.tar.gz` & `tmp/HeraData-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HeraData-0.1.tar", last modified: Mon Apr 22 09:34:30 2024, max compression
+gzip compressed data, was "HeraData-0.1.1.tar", last modified: Tue Apr 23 02:21:37 2024, max compression
```

## Comparing `HeraData-0.1.tar` & `HeraData-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-22 09:34:30.468785 HeraData-0.1/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-22 09:34:30.468785 HeraData-0.1/HeraData.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)      153 2024-04-22 09:34:30.000000 HeraData-0.1/HeraData.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      216 2024-04-22 09:34:30.000000 HeraData-0.1/HeraData.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-22 09:34:30.000000 HeraData-0.1/HeraData.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       14 2024-04-22 09:34:30.000000 HeraData-0.1/HeraData.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-22 09:34:30.000000 HeraData-0.1/HeraData.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      153 2024-04-22 09:34:30.468785 HeraData-0.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-22 09:32:31.000000 HeraData-0.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-22 09:34:30.468785 HeraData-0.1/hera/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-04-22 02:55:07.000000 HeraData-0.1/hera/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      867 2024-04-22 08:43:32.000000 HeraData-0.1/hera/_data_storage.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-22 09:34:30.468785 HeraData-0.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      310 2024-04-22 09:32:52.000000 HeraData-0.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 02:21:37.743590 HeraData-0.1.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      129 2024-04-23 01:24:54.000000 HeraData-0.1.1/.gitignore
+-rw-rw-r--   0 mark      (1000) mark      (1000)      104 2024-04-22 07:50:16.000000 HeraData-0.1.1/.gitmodules
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 02:21:37.743590 HeraData-0.1.1/HeraData.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-23 02:21:37.000000 HeraData-0.1.1/HeraData.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      325 2024-04-23 02:21:37.000000 HeraData-0.1.1/HeraData.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 02:21:37.000000 HeraData-0.1.1/HeraData.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       14 2024-04-23 02:21:37.000000 HeraData-0.1.1/HeraData.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2024-04-23 02:21:37.000000 HeraData-0.1.1/HeraData.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      155 2024-04-23 02:21:37.743590 HeraData-0.1.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)       35 2024-04-22 09:32:31.000000 HeraData-0.1.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 02:21:37.743590 HeraData-0.1.1/hera/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      310 2024-04-23 02:02:41.000000 HeraData-0.1.1/hera/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1050 2024-04-23 02:02:41.000000 HeraData-0.1.1/hera/_data_storage.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1414 2024-04-23 01:37:16.000000 HeraData-0.1.1/main.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       21 2024-04-23 02:00:27.000000 HeraData-0.1.1/requirements.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       79 2024-04-23 02:21:37.743590 HeraData-0.1.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      377 2024-04-23 02:21:32.000000 HeraData-0.1.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 02:21:37.743590 HeraData-0.1.1/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      811 2024-04-23 02:02:41.000000 HeraData-0.1.1/tests/test___init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1173 2024-04-23 01:59:32.000000 HeraData-0.1.1/tests/test__data_storage.py
```

### Comparing `HeraData-0.1/hera/_data_storage.py` & `HeraData-0.1.1/hera/_data_storage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,36 @@
+from enum import Enum
+
 from elasticsearch import Elasticsearch
 
 
+class StorageType(Enum):
+    ELASTICSEARCH = 1
+
+
 class _DataStorage:
     pass
 
 
 class _ElasticSearchDataStorage(_DataStorage):
-    def __init__(self, host="localhost", port=9200):
-        self._host = host
-        self._port = port
-        self._es = Elasticsearch([{"host": host, "port": port}])
+    def __init__(
+            self, host="localhost", port=9200, auth_user='elastic', auth_pass='aoeui123'
+    ):
+        self._es_client = Elasticsearch(
+            ['http://{}:{}'.format(host, port)],
+            basic_auth=(auth_user, auth_pass)
+        )
 
     def store(self, store_name: str, data: dict):
-        self._es.index(index=store_name, body=data)
+        self._es_client.index(index=store_name, body=data)
 
     def get_last(
             self, store_name: str, query: dict, count: int = 1, start_by_id: int = -1
     ):
         query["sort"] = [{'_index': {"order": "desc"}}]
         if start_by_id >= 0:
             query["query"] = {"range": {"_index": {"gt": start_by_id}}}
         query["size"] = count
-        return self._es.search(index=store_name, body=query)
+        return self._es_client.search(index=store_name, body=query)
 
     def search(self, store_name: str, query: dict):
-        return self._es.search(index=store_name, body=query)
+        return self._es_client.search(index=store_name, body=query)
```

