# Comparing `tmp/llama_index_storage_kvstore_firestore-0.1.2.tar.gz` & `tmp/llama_index_storage_kvstore_firestore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_kvstore_firestore-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_storage_kvstore_firestore-0.2.0.tar", max compression
```

## Comparing `llama_index_storage_kvstore_firestore-0.1.2.tar` & `llama_index_storage_kvstore_firestore-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       52 2024-02-13 13:53:01.921360 llama_index_storage_kvstore_firestore-0.1.2/README.md
--rw-r--r--   0        0        0      104 2024-02-13 13:53:01.921629 llama_index_storage_kvstore_firestore-0.1.2/llama_index/storage/kvstore/firestore/__init__.py
--rw-r--r--   0        0        0     7539 2024-02-13 13:53:01.921703 llama_index_storage_kvstore_firestore-0.1.2/llama_index/storage/kvstore/firestore/base.py
--rw-r--r--   0        0        0     1500 2024-02-21 21:40:49.590175 llama_index_storage_kvstore_firestore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_firestore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/README.md
+-rw-r--r--   0        0        0      104 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/llama_index/storage/kvstore/firestore/__init__.py
+-rw-r--r--   0        0        0     7983 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/llama_index/storage/kvstore/firestore/base.py
+-rw-r--r--   0        0        0     1498 2024-04-23 21:20:01.676316 llama_index_storage_kvstore_firestore-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_firestore-0.2.0/PKG-INFO
```

### Comparing `llama_index_storage_kvstore_firestore-0.1.2/llama_index/storage/kvstore/firestore/base.py` & `llama_index_storage_kvstore_firestore-0.2.0/llama_index/storage/kvstore/firestore/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict, List, Optional, Tuple
 
+from google.auth.credentials import Credentials
 from google.cloud.firestore_v1.async_client import AsyncClient
 from google.cloud.firestore_v1.client import Client
 from google.cloud.firestore_v1.services.firestore.transports.base import (
     DEFAULT_CLIENT_INFO,
 )
 from llama_index.core.storage.kvstore.types import (
     DEFAULT_BATCH_SIZE,
@@ -23,27 +24,39 @@
 
 class FirestoreKVStore(BaseKVStore):
     """Firestore Key-Value store.
 
     Args:
         project (str): The project which the client acts on behalf of.
         database (str): The database name that the client targets.
+        credentials (google.auth.credentials.Credentials): The OAuth2
+            Credentials to access Firestore. If not passed, falls back
+            to the default inferred from the environment.
     """
 
     def __init__(
         self,
         project: Optional[str] = None,
         database: str = DEFAULT_FIRESTORE_DATABASE,
+        credentials: Optional[Credentials] = None,
     ) -> None:
         client_info = DEFAULT_CLIENT_INFO
         client_info.user_agent = USER_AGENT
         self._adb = AsyncClient(
-            project=project, database=database, client_info=client_info
+            project=project,
+            database=database,
+            client_info=client_info,
+            credentials=credentials,
+        )
+        self._db = Client(
+            project=project,
+            database=database,
+            client_info=client_info,
+            credentials=credentials,
         )
-        self._db = Client(project=project, database=database, client_info=client_info)
 
     def firestore_collection(self, collection: str) -> str:
         return collection.replace("/", SLASH_REPLACEMENT)
 
     def replace_field_name_set(self, val: Dict[str, Any]) -> Dict[str, Any]:
         val = val.copy()
         for k, v in FIELD_NAME_REPLACE_SET.items():
```

### Comparing `llama_index_storage_kvstore_firestore-0.1.2/pyproject.toml` & `llama_index_storage_kvstore_firestore-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index kvstore firestore integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-kvstore-firestore"
 readme = "README.md"
-version = "0.1.2"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9,<4.0"
 llama-index-core = "^0.10.1"
 google-cloud-firestore = "^2.14.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_storage_kvstore_firestore-0.1.2/PKG-INFO` & `llama_index_storage_kvstore_firestore-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-kvstore-firestore
-Version: 0.1.2
+Version: 0.2.0
 Summary: llama-index kvstore firestore integration
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
 Requires-Dist: google-cloud-firestore (>=2.14.0,<3.0.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Kvstore Integration: Firestore Kvstore
```

