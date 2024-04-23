# Comparing `tmp/llama_index_storage_docstore_firestore-0.1.2.tar.gz` & `tmp/llama_index_storage_docstore_firestore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_docstore_firestore-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_storage_docstore_firestore-0.1.3.tar", max compression
```

## Comparing `llama_index_storage_docstore_firestore-0.1.2.tar` & `llama_index_storage_docstore_firestore-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       54 2024-02-13 13:53:01.910770 llama_index_storage_docstore_firestore-0.1.2/README.md
--rw-r--r--   0        0        0      117 2024-02-13 13:53:01.911016 llama_index_storage_docstore_firestore-0.1.2/llama_index/storage/docstore/firestore/__init__.py
--rw-r--r--   0        0        0     1391 2024-02-13 13:53:01.911064 llama_index_storage_docstore_firestore-0.1.2/llama_index/storage/docstore/firestore/base.py
--rw-r--r--   0        0        0     1523 2024-02-21 22:00:22.291166 llama_index_storage_docstore_firestore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 llama_index_storage_docstore_firestore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-23 21:20:01.668316 llama_index_storage_docstore_firestore-0.1.3/README.md
+-rw-r--r--   0        0        0      117 2024-04-23 21:20:01.668316 llama_index_storage_docstore_firestore-0.1.3/llama_index/storage/docstore/firestore/__init__.py
+-rw-r--r--   0        0        0     1391 2024-04-23 21:20:01.668316 llama_index_storage_docstore_firestore-0.1.3/llama_index/storage/docstore/firestore/base.py
+-rw-r--r--   0        0        0     1522 2024-04-23 21:20:01.668316 llama_index_storage_docstore_firestore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 llama_index_storage_docstore_firestore-0.1.3/PKG-INFO
```

### Comparing `llama_index_storage_docstore_firestore-0.1.2/llama_index/storage/docstore/firestore/base.py` & `llama_index_storage_docstore_firestore-0.1.3/llama_index/storage/docstore/firestore/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_storage_docstore_firestore-0.1.2/pyproject.toml` & `llama_index_storage_docstore_firestore-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index docstore firestore integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-docstore-firestore"
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

### Comparing `llama_index_storage_docstore_firestore-0.1.2/PKG-INFO` & `llama_index_storage_docstore_firestore-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-docstore-firestore
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index docstore firestore integration
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
 
 # LlamaIndex Docstore Integration: Firestore Docstore
```

