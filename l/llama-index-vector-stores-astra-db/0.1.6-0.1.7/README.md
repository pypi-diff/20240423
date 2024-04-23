# Comparing `tmp/llama_index_vector_stores_astra_db-0.1.6.tar.gz` & `tmp/llama_index_vector_stores_astra_db-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_astra_db-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_astra_db-0.1.7.tar", max compression
```

## Comparing `llama_index_vector_stores_astra_db-0.1.6.tar` & `llama_index_vector_stores_astra_db-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      944 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/README.md
--rw-r--r--   0        0        0      105 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/llama_index/vector_stores/astra_db/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/llama_index/vector_stores/astra_db/base.py
--rw-r--r--   0        0        0     1484 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 llama_index_vector_stores_astra_db-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      944 2024-04-23 21:21:28.118175 llama_index_vector_stores_astra_db-0.1.7/README.md
+-rw-r--r--   0        0        0      105 2024-04-23 21:21:28.118175 llama_index_vector_stores_astra_db-0.1.7/llama_index/vector_stores/astra_db/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-23 21:21:28.118175 llama_index_vector_stores_astra_db-0.1.7/llama_index/vector_stores/astra_db/base.py
+-rw-r--r--   0        0        0     1475 2024-04-23 21:21:28.118175 llama_index_vector_stores_astra_db-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 llama_index_vector_stores_astra_db-0.1.7/PKG-INFO
```

### Comparing `llama_index_vector_stores_astra_db-0.1.6/README.md` & `llama_index_vector_stores_astra_db-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_astra_db-0.1.6/llama_index/vector_stores/astra_db/base.py` & `llama_index_vector_stores_astra_db-0.1.7/llama_index/vector_stores/astra_db/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_astra_db-0.1.6/pyproject.toml` & `llama_index_vector_stores_astra_db-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores astra integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-astra-db"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-astrapy = ">=0.7.7, <2"
+astrapy = "^1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_vector_stores_astra_db-0.1.6/PKG-INFO` & `llama_index_vector_stores_astra_db-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-astra-db
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index vector_stores astra integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: astrapy (>=0.7.7,<2)
+Requires-Dist: astrapy (>=1,<2)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Astra DB Vector Store
 
 A LlamaIndex vector store using Astra DB as the backend.
```

