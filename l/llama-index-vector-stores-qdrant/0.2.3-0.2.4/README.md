# Comparing `tmp/llama_index_vector_stores_qdrant-0.2.3.tar.gz` & `tmp/llama_index_vector_stores_qdrant-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_qdrant-0.2.3.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_qdrant-0.2.4.tar", max compression
```

## Comparing `llama_index_vector_stores_qdrant-0.2.3.tar` & `llama_index_vector_stores_qdrant-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-04-22 18:39:39.729173 llama_index_vector_stores_qdrant-0.2.3/README.md
--rw-r--r--   0        0        0      101 2024-04-22 18:39:39.729173 llama_index_vector_stores_qdrant-0.2.3/llama_index/vector_stores/qdrant/__init__.py
--rw-r--r--   0        0        0    33434 2024-04-22 18:39:39.729173 llama_index_vector_stores_qdrant-0.2.3/llama_index/vector_stores/qdrant/base.py
--rw-r--r--   0        0        0     6897 2024-04-22 18:39:39.729173 llama_index_vector_stores_qdrant-0.2.3/llama_index/vector_stores/qdrant/utils.py
--rw-r--r--   0        0        0     1600 2024-04-22 18:39:39.729173 llama_index_vector_stores_qdrant-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-22 20:50:53.236409 llama_index_vector_stores_qdrant-0.2.4/README.md
+-rw-r--r--   0        0        0      101 2024-04-22 20:50:53.236409 llama_index_vector_stores_qdrant-0.2.4/llama_index/vector_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0    34174 2024-04-22 20:50:53.236409 llama_index_vector_stores_qdrant-0.2.4/llama_index/vector_stores/qdrant/base.py
+-rw-r--r--   0        0        0     6897 2024-04-22 20:50:53.236409 llama_index_vector_stores_qdrant-0.2.4/llama_index/vector_stores/qdrant/utils.py
+-rw-r--r--   0        0        0     1600 2024-04-22 20:50:53.236409 llama_index_vector_stores_qdrant-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.2.4/PKG-INFO
```

### Comparing `llama_index_vector_stores_qdrant-0.2.3/llama_index/vector_stores/qdrant/base.py` & `llama_index_vector_stores_qdrant-0.2.4/llama_index/vector_stores/qdrant/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,15 +200,17 @@
         sparse_query_fn: Optional[SparseEncoderCallable] = None,
         hybrid_fusion_fn: Optional[HybridFusionCallable] = None,
     ):
         self._sparse_doc_fn = sparse_doc_fn
         self._sparse_query_fn = sparse_query_fn
         self._hybrid_fusion_fn = hybrid_fusion_fn
 
-    def _build_points(self, nodes: List[BaseNode]) -> Tuple[List[Any], List[str]]:
+    def _build_points(
+        self, nodes: List[BaseNode], sparse_vector_name: str
+    ) -> Tuple[List[Any], List[str]]:
         ids = []
         points = []
         for node_batch in iter_batch(nodes, self.batch_size):
             node_ids = []
             vectors: List[Any] = []
             sparse_vectors: List[List[float]] = []
             sparse_indices: List[List[int]] = []
@@ -231,15 +233,15 @@
                         len(sparse_vectors) > 0
                         and len(sparse_indices) > 0
                         and len(sparse_vectors) == len(sparse_indices)
                     ):
                         vectors.append(
                             {
                                 # Dynamically switch between the old and new sparse vector name
-                                self.sparse_vector_name: rest.SparseVector(
+                                sparse_vector_name: rest.SparseVector(
                                     indices=sparse_indices[i],
                                     values=sparse_vectors[i],
                                 ),
                                 DENSE_VECTOR_NAME: node.get_embedding(),
                             }
                         )
                     else:
@@ -278,15 +280,16 @@
         """
         if len(nodes) > 0 and not self._collection_initialized:
             self._create_collection(
                 collection_name=self.collection_name,
                 vector_size=len(nodes[0].get_embedding()),
             )
 
-        points, ids = self._build_points(nodes)
+        sparse_vector_name = self.sparse_vector_name()
+        points, ids = self._build_points(nodes, sparse_vector_name)
 
         self._client.upload_points(
             collection_name=self.collection_name,
             points=points,
             batch_size=self.batch_size,
             parallel=self.parallel,
             max_retries=self.max_retries,
@@ -312,15 +315,16 @@
 
         if len(nodes) > 0 and not collection_initialized:
             await self._acreate_collection(
                 collection_name=self.collection_name,
                 vector_size=len(nodes[0].get_embedding()),
             )
 
-        points, ids = self._build_points(nodes)
+        sparse_vector_name = await self.asparse_vector_name()
+        points, ids = self._build_points(nodes, sparse_vector_name)
 
         await self._aclient.upload_points(
             collection_name=self.collection_name,
             points=points,
             batch_size=self.batch_size,
             parallel=self.parallel,
             max_retries=self.max_retries,
@@ -509,15 +513,15 @@
                         limit=query.similarity_top_k,
                         filter=query_filter,
                         with_payload=True,
                     ),
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
                             # Dynamically switch between the old and new sparse vector name
-                            name=self.sparse_vector_name,
+                            name=self.sparse_vector_name(),
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -552,15 +556,15 @@
 
             sparse_response = self._client.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
                             # Dynamically switch between the old and new sparse vector name
-                            name=self.sparse_vector_name,
+                            name=self.sparse_vector_name(),
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -643,15 +647,15 @@
                         limit=query.similarity_top_k,
                         filter=query_filter,
                         with_payload=True,
                     ),
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
                             # Dynamically switch between the old and new sparse vector name
-                            name=self.sparse_vector_name,
+                            name=await self.asparse_vector_name(),
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -685,15 +689,15 @@
 
             sparse_response = await self._aclient.search_batch(
                 collection_name=self.collection_name,
                 requests=[
                     rest.SearchRequest(
                         vector=rest.NamedSparseVector(
                             # Dynamically switch between the old and new sparse vector name
-                            name=self.sparse_vector_name,
+                            name=await self.sparse_vector_name(),
                             vector=rest.SparseVector(
                                 indices=sparse_indices[0],
                                 values=sparse_embedding[0],
                             ),
                         ),
                         limit=sparse_top_k,
                         filter=query_filter,
@@ -869,22 +873,37 @@
     def use_old_sparse_encoder(self, collection_name: str) -> bool:
         return (
             self._collection_exists(collection_name)
             and SPARSE_VECTOR_NAME_OLD
             in self.client.get_collection(collection_name).config.params.vectors
         )
 
-    @property
     def sparse_vector_name(self) -> str:
         return (
             SPARSE_VECTOR_NAME_OLD
             if self.use_old_sparse_encoder(self.collection_name)
             else SPARSE_VECTOR_NAME
         )
 
+    async def ause_old_sparse_encoder(self, collection_name: str) -> bool:
+        return (
+            await self._acollection_exists(collection_name)
+            and SPARSE_VECTOR_NAME_OLD
+            in (
+                await self._aclient.get_collection(collection_name)
+            ).config.params.vectors
+        )
+
+    async def asparse_vector_name(self) -> str:
+        return (
+            SPARSE_VECTOR_NAME_OLD
+            if await self.ause_old_sparse_encoder(self.collection_name)
+            else SPARSE_VECTOR_NAME
+        )
+
     def get_default_sparse_doc_encoder(
         self, collection_name: str
     ) -> SparseEncoderCallable:
         if self.use_old_sparse_encoder(collection_name):
             return default_sparse_encoder("naver/efficient-splade-VI-BT-large-doc")
 
         return fastembed_sparse_encoder(model_name="prithvida/Splade_PP_en_v1")
```

### Comparing `llama_index_vector_stores_qdrant-0.2.3/llama_index/vector_stores/qdrant/utils.py` & `llama_index_vector_stores_qdrant-0.2.4/llama_index/vector_stores/qdrant/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_qdrant-0.2.3/pyproject.toml` & `llama_index_vector_stores_qdrant-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores qdrant integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-qdrant"
 readme = "README.md"
-version = "0.2.3"
+version = "0.2.4"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 llama-index-core = "^0.10.1"
 qdrant-client = "^1.7.1"
 grpcio = "^1.60.0"
```

### Comparing `llama_index_vector_stores_qdrant-0.2.3/PKG-INFO` & `llama_index_vector_stores_qdrant-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-qdrant
-Version: 0.2.3
+Version: 0.2.4
 Summary: llama-index vector_stores qdrant integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

