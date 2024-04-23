# Comparing `tmp/llama_index_storage_index_store_firestore-0.1.2.tar.gz` & `tmp/llama_index_storage_index_store_firestore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_index_store_firestore-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_storage_index_store_firestore-0.1.3.tar", max compression
```

## Comparing `llama_index_storage_index_store_firestore-0.1.2.tar` & `llama_index_storage_index_store_firestore-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       59 2024-02-13 13:53:01.916309 llama_index_storage_index_store_firestore-0.1.2/README.md
--rw-r--r--   0        0        0      114 2024-02-13 13:53:01.916541 llama_index_storage_index_store_firestore-0.1.2/llama_index/storage/index_store/firestore/__init__.py
--rw-r--r--   0        0        0     1181 2024-02-13 13:53:01.916592 llama_index_storage_index_store_firestore-0.1.2/llama_index/storage/index_store/firestore/base.py
--rw-r--r--   0        0        0     1529 2024-02-21 21:50:49.003555 llama_index_storage_index_store_firestore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 llama_index_storage_index_store_firestore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       59 2024-04-23 21:20:01.672316 llama_index_storage_index_store_firestore-0.1.3/README.md
+-rw-r--r--   0        0        0      114 2024-04-23 21:20:01.672316 llama_index_storage_index_store_firestore-0.1.3/llama_index/storage/index_store/firestore/__init__.py
+-rw-r--r--   0        0        0     1181 2024-04-23 21:20:01.672316 llama_index_storage_index_store_firestore-0.1.3/llama_index/storage/index_store/firestore/base.py
+-rw-r--r--   0        0        0     1528 2024-04-23 21:20:01.672316 llama_index_storage_index_store_firestore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 llama_index_storage_index_store_firestore-0.1.3/PKG-INFO
```

### Comparing `llama_index_storage_index_store_firestore-0.1.2/llama_index/storage/index_store/firestore/base.py` & `llama_index_storage_index_store_firestore-0.1.3/llama_index/storage/index_store/firestore/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_storage_index_store_firestore-0.1.2/pyproject.toml` & `llama_index_storage_index_store_firestore-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index index_store firestore integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-index-store-firestore"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9,<4.0"
 llama-index-core = "^0.10.1"
-llama-index-storage-kvstore-firestore = "^0.1.1"
+llama-index-storage-kvstore-firestore = ">=0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_storage_index_store_firestore-0.1.2/PKG-INFO` & `llama_index_storage_index_store_firestore-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-index-store-firestore
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index index_store firestore integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
-Requires-Dist: llama-index-storage-kvstore-firestore (>=0.1.1,<0.2.0)
+Requires-Dist: llama-index-storage-kvstore-firestore (>=0.1.1)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Index_Store Integration: Firestore Indexstore
```

