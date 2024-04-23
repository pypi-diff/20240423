# Comparing `tmp/llama_index_readers_astra_db-0.1.5.tar.gz` & `tmp/llama_index_readers_astra_db-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_astra_db-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_readers_astra_db-0.1.6.tar", max compression
```

## Comparing `llama_index_readers_astra_db-0.1.5.tar` & `llama_index_readers_astra_db-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1584 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/README.md
--rw-r--r--   0        0        0       89 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/llama_index/readers/astra_db/__init__.py
--rw-r--r--   0        0        0     2945 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/llama_index/readers/astra_db/base.py
--rw-r--r--   0        0        0     1491 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2198 1970-01-01 00:00:00.000000 llama_index_readers_astra_db-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1584 2024-04-23 21:21:27.966176 llama_index_readers_astra_db-0.1.6/README.md
+-rw-r--r--   0        0        0       89 2024-04-23 21:21:27.966176 llama_index_readers_astra_db-0.1.6/llama_index/readers/astra_db/__init__.py
+-rw-r--r--   0        0        0     2945 2024-04-23 21:21:27.966176 llama_index_readers_astra_db-0.1.6/llama_index/readers/astra_db/base.py
+-rw-r--r--   0        0        0     1482 2024-04-23 21:21:27.966176 llama_index_readers_astra_db-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 llama_index_readers_astra_db-0.1.6/PKG-INFO
```

### Comparing `llama_index_readers_astra_db-0.1.5/README.md` & `llama_index_readers_astra_db-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_astra_db-0.1.5/llama_index/readers/astra_db/base.py` & `llama_index_readers_astra_db-0.1.6/llama_index/readers/astra_db/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_astra_db-0.1.5/pyproject.toml` & `llama_index_readers_astra_db-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers astra_db integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["erichare"]
 name = "llama-index-readers-astra-db"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
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

### Comparing `llama_index_readers_astra_db-0.1.5/PKG-INFO` & `llama_index_readers_astra_db-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-astra-db
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index readers astra_db integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: erichare
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
 
 # Astra DB Loader
 
 ```bash
 pip install llama-index-readers-astra-db
```

