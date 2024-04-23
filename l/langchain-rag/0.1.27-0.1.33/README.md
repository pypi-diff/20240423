# Comparing `tmp/langchain_rag-0.1.27.tar.gz` & `tmp/langchain_rag-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_rag-0.1.27.tar", max compression
+gzip compressed data, was "langchain_rag-0.1.33.tar", max compression
```

## Comparing `langchain_rag-0.1.27.tar` & `langchain_rag-0.1.33.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.1.27/LICENSE.txt
--rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.1.27/README.md
--rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.1.27/langchain_rag/__init__.py
--rw-r--r--   0        0        0      696 2024-01-29 11:57:32.037286 langchain_rag-0.1.27/langchain_rag/document_transformers/__init__.py
--rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.1.27/langchain_rag/document_transformers/copy_transformer.py
--rw-r--r--   0        0        0     2906 2024-02-27 11:33:44.900653 langchain_rag-0.1.27/langchain_rag/document_transformers/document_transform_pipeline.py
--rw-r--r--   0        0        0     5729 2024-01-29 11:57:32.041286 langchain_rag-0.1.27/langchain_rag/document_transformers/document_transformers.py
--rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.1.27/langchain_rag/document_transformers/generate_questions.py
--rw-r--r--   0        0        0     9198 2024-01-29 11:57:30.045307 langchain_rag-0.1.27/langchain_rag/document_transformers/runnable_document_transformer.py
--rw-r--r--   0        0        0     4706 2024-01-29 12:38:44.614686 langchain_rag-0.1.27/langchain_rag/document_transformers/sumarize_and_questions_transformer.py
--rw-r--r--   0        0        0     3200 2024-01-29 12:38:44.606686 langchain_rag-0.1.27/langchain_rag/document_transformers/sumarize_transformer.py
--rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.1.27/langchain_rag/indexes/__init__.py
--rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.1.27/langchain_rag/indexes/memory_recordmanager.py
--rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.1.27/langchain_rag/storage/__init__.py
--rw-r--r--   0        0        0     7767 2024-01-24 07:31:02.433371 langchain_rag-0.1.27/langchain_rag/storage/sql_docstore.py
--rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.1.27/langchain_rag/vectorstores/__init__.py
--rw-r--r--   0        0        0    31965 2024-02-27 08:39:16.213675 langchain_rag-0.1.27/langchain_rag/vectorstores/rag_vectorstore.py
--rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.1.27/langchain_rag/vectorstores/wrapper_vectorstore.py
--rw-r--r--   0        0        0     3811 2024-02-27 15:44:31.679217 langchain_rag-0.1.27/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 langchain_rag-0.1.27/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.1.33/LICENSE.txt
+-rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.1.33/README.md
+-rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.1.33/langchain_rag/__init__.py
+-rw-r--r--   0        0        0      696 2024-01-29 11:57:32.037286 langchain_rag-0.1.33/langchain_rag/document_transformers/__init__.py
+-rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.1.33/langchain_rag/document_transformers/copy_transformer.py
+-rw-r--r--   0        0        0     2906 2024-02-27 11:33:44.900653 langchain_rag-0.1.33/langchain_rag/document_transformers/document_transform_pipeline.py
+-rw-r--r--   0        0        0     5729 2024-01-29 11:57:32.041286 langchain_rag-0.1.33/langchain_rag/document_transformers/document_transformers.py
+-rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.1.33/langchain_rag/document_transformers/generate_questions.py
+-rw-r--r--   0        0        0     9198 2024-01-29 11:57:30.045307 langchain_rag-0.1.33/langchain_rag/document_transformers/runnable_document_transformer.py
+-rw-r--r--   0        0        0     4706 2024-01-29 12:38:44.614686 langchain_rag-0.1.33/langchain_rag/document_transformers/sumarize_and_questions_transformer.py
+-rw-r--r--   0        0        0     3200 2024-01-29 12:38:44.606686 langchain_rag-0.1.33/langchain_rag/document_transformers/sumarize_transformer.py
+-rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.1.33/langchain_rag/indexes/__init__.py
+-rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.1.33/langchain_rag/indexes/memory_recordmanager.py
+-rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.1.33/langchain_rag/storage/__init__.py
+-rw-r--r--   0        0        0     7807 2024-03-18 16:51:24.598952 langchain_rag-0.1.33/langchain_rag/storage/sql_docstore.py
+-rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.1.33/langchain_rag/vectorstores/__init__.py
+-rw-r--r--   0        0        0    31991 2024-03-18 16:42:17.003830 langchain_rag-0.1.33/langchain_rag/vectorstores/rag_vectorstore.py
+-rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.1.33/langchain_rag/vectorstores/wrapper_vectorstore.py
+-rw-r--r--   0        0        0     3811 2024-02-27 15:44:31.679217 langchain_rag-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 langchain_rag-0.1.33/PKG-INFO
```

### Comparing `langchain_rag-0.1.27/LICENSE.txt` & `langchain_rag-0.1.33/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/README.md` & `langchain_rag-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/__init__.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/copy_transformer.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/copy_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/document_transform_pipeline.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/document_transform_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/document_transformers.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/document_transformers.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/generate_questions.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/generate_questions.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/runnable_document_transformer.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/runnable_document_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/sumarize_and_questions_transformer.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/sumarize_and_questions_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/document_transformers/sumarize_transformer.py` & `langchain_rag-0.1.33/langchain_rag/document_transformers/sumarize_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/indexes/memory_recordmanager.py` & `langchain_rag-0.1.33/langchain_rag/indexes/memory_recordmanager.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/langchain_rag/storage/sql_docstore.py` & `langchain_rag-0.1.33/langchain_rag/storage/sql_docstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,20 +164,21 @@
     #             session.add_all([Value(namespace=self.namespace,
     #                                    key=k,
     #                                    value=v) for k, v in key_value_pairs])
     #             session.commit()
 
     def mset(self, key_value_pairs: Sequence[Tuple[str, bytes]]) -> None:
         # try:
+        values: Dict[str, bytes] = dict(key_value_pairs)
         with self._make_session() as session:
-            self._mdetete([key for key, _ in key_value_pairs], session)
+            self._mdetete(list(values.keys()), session)
             session.add_all(
                 [
                     Value(namespace=self.namespace, key=k, value=v)
-                    for k, v in key_value_pairs
+                    for k, v in values.items()
                 ]
             )
 
     def _mdetete(self, keys: Sequence[str], session: Session) -> None:
         with session.begin():
             session.query(Value).filter(  # type: ignore
                 and_(
```

### Comparing `langchain_rag-0.1.27/langchain_rag/vectorstores/rag_vectorstore.py` & `langchain_rag-0.1.33/langchain_rag/vectorstores/rag_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
                 chunk_s = scores.get(id, 1.0)
                 scores[id] = min(chunk_s, s)
         docs = cast(Sequence[Document], self.docstore.mget(ids))
         map_ids = {doc.metadata[key]: i for doc, i in zip(docs, ids) if doc}
         return sorted(
             [(d, scores[map_ids[d.metadata[key]]]) for d in docs if d is not None],
             key=lambda x: x[1],
+            reverse=True,
         )
 
     def _get_trunk_from_sub_docs_and_score(
         self, sub_docs_and_score: List[Tuple[Document, float]], k: int, **kwargs: Any
     ) -> List[Tuple[Document, float]]:
         if self.chunk_transformer:
             result = self._update_score_of_chunk(sub_docs_and_score)
```

### Comparing `langchain_rag-0.1.27/langchain_rag/vectorstores/wrapper_vectorstore.py` & `langchain_rag-0.1.33/langchain_rag/vectorstores/wrapper_vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/pyproject.toml` & `langchain_rag-0.1.33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.27/PKG-INFO` & `langchain_rag-0.1.33/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-rag
-Version: 0.1.27
+Version: 0.1.33
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/langchain-ai/langchain/pull/7278) to be validated.
 Home-page: https://www.github.com/pprados/langchain-rag
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

