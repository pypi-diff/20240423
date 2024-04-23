# Comparing `tmp/tidb_vector-0.0.7.tar.gz` & `tmp/tidb_vector-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidb_vector-0.0.7.tar", max compression
+gzip compressed data, was "tidb_vector-0.0.8.tar", max compression
```

## Comparing `tidb_vector-0.0.7.tar` & `tidb_vector-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11294 2024-03-04 08:01:44.610607 tidb_vector-0.0.7/LICENSE
--rw-r--r--   0        0        0     4617 2024-03-18 06:08:42.030577 tidb_vector-0.0.7/README.md
--rw-r--r--   0        0        0      852 2024-04-01 08:18:14.580905 tidb_vector-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-03 09:41:38.451647 tidb_vector-0.0.7/tidb_vector/__init__.py
--rw-r--r--   0        0        0      109 2024-03-14 03:53:20.150919 tidb_vector-0.0.7/tidb_vector/constants.py
--rw-r--r--   0        0        0      356 2024-03-05 22:28:11.819145 tidb_vector-0.0.7/tidb_vector/integrations/__init__.py
--rw-r--r--   0        0        0     3478 2024-04-03 09:40:56.455876 tidb_vector-0.0.7/tidb_vector/integrations/utils.py
--rw-r--r--   0        0        0    18592 2024-04-01 07:50:10.331513 tidb_vector-0.0.7/tidb_vector/integrations/vector_client.py
--rw-r--r--   0        0        0      962 2024-03-14 03:59:19.124632 tidb_vector-0.0.7/tidb_vector/peewee/__init__.py
--rw-r--r--   0        0        0     2775 2024-03-16 06:37:36.615096 tidb_vector-0.0.7/tidb_vector/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      863 2024-03-14 03:59:19.126501 tidb_vector-0.0.7/tidb_vector/utils.py
--rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 tidb_vector-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11294 2024-03-04 08:01:44.610607 tidb_vector-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6872 2024-04-22 13:07:11.269379 tidb_vector-0.0.8/README.md
+-rw-r--r--   0        0        0      852 2024-04-01 08:18:14.580905 tidb_vector-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-23 11:11:43.858106 tidb_vector-0.0.8/tidb_vector/__init__.py
+-rw-r--r--   0        0        0      109 2024-03-14 03:53:20.150919 tidb_vector-0.0.8/tidb_vector/constants.py
+-rw-r--r--   0        0        0      356 2024-03-05 22:28:11.819145 tidb_vector-0.0.8/tidb_vector/integrations/__init__.py
+-rw-r--r--   0        0        0     3666 2024-04-23 03:30:37.756240 tidb_vector-0.0.8/tidb_vector/integrations/utils.py
+-rw-r--r--   0        0        0    18701 2024-04-23 03:30:37.757294 tidb_vector-0.0.8/tidb_vector/integrations/vector_client.py
+-rw-r--r--   0        0        0      962 2024-03-14 03:59:19.124632 tidb_vector-0.0.8/tidb_vector/peewee/__init__.py
+-rw-r--r--   0        0        0     2775 2024-03-16 06:37:36.615096 tidb_vector-0.0.8/tidb_vector/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      863 2024-03-14 03:59:19.126501 tidb_vector-0.0.8/tidb_vector/utils.py
+-rw-r--r--   0        0        0     7540 1970-01-01 00:00:00.000000 tidb_vector-0.0.8/PKG-INFO
```

### Comparing `tidb_vector-0.0.7/LICENSE` & `tidb_vector-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.7/pyproject.toml` & `tidb_vector-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.7/tidb_vector/integrations/utils.py` & `tidb_vector-0.0.8/tidb_vector/integrations/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,27 +40,33 @@
     try:
         inspector = sqlalchemy.inspect(engine)
         return table_name in inspector.get_table_names()
     finally:
         engine.dispose()
 
 
-def get_embedding_column_definition(connection_string, table_name, column_name):
+def get_embedding_column_definition(
+    connection_string: str,
+    table_name: str,
+    column_name: str,
+    engine_args: Optional[Dict[str, Any]] = None,
+):
     """
     Retrieves the column definition of an embedding column from a database table.
 
     Args:
         connection_string (str): The connection string to the database.
         table_name (str): The name of the table.
         column_name (str): The name of the column.
+        engine_args (Optional[Dict[str, Any]]): Additional arguments for the engine.
 
     Returns:
         tuple: A tuple containing the dimension (int or None) and distance metric (str or None).
     """
-    engine = sqlalchemy.create_engine(connection_string)
+    engine = sqlalchemy.create_engine(connection_string, **(engine_args or {}))
     try:
         with engine.connect() as connection:
             query = f"""SELECT COLUMN_TYPE, COLUMN_COMMENT
                         FROM INFORMATION_SCHEMA.COLUMNS
                         WHERE TABLE_NAME = '{table_name}' AND COLUMN_NAME = '{column_name}'"""
             result = connection.execute(sqlalchemy.text(query)).fetchone()
             if result:
```

### Comparing `tidb_vector-0.0.7/tidb_vector/integrations/vector_client.py` & `tidb_vector-0.0.8/tidb_vector/integrations/vector_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,18 @@
         """
         Check if the table is compatible with the current configuration.
         """
         if self._drop_existing_table:
             return
 
         actual_dim, actual_distance_strategy = get_embedding_column_definition(
-            self.connection_string, self._table_name, "embedding"
+            connection_string=self.connection_string,
+            table_name=self._table_name,
+            column_name="embedding",
+            engine_args=self._engine_args,
         )
         if actual_dim is not None:
             # If the vector dimension is not set, set it to the actual dimension
             if self._vector_dimension is None:
                 self._vector_dimension = actual_dim
             elif actual_dim != self._vector_dimension:
                 raise EmbeddingColumnMismatchError(
```

### Comparing `tidb_vector-0.0.7/tidb_vector/peewee/__init__.py` & `tidb_vector-0.0.8/tidb_vector/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.7/tidb_vector/sqlalchemy/__init__.py` & `tidb_vector-0.0.8/tidb_vector/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.7/tidb_vector/utils.py` & `tidb_vector-0.0.8/tidb_vector/utils.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.7/PKG-INFO` & `tidb_vector-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidb-vector
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python client for TiDB Vector
 License: Apache-2.0
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -34,36 +34,49 @@
 TiDB vector supports below distance functions:
 
 - `L1Distance`
 - `L2Distance`
 - `CosineDistance`
 - `NegativeInnerProduct`
 
-supports following orm or framework:
+It also supports using hnsw index with l2 or cosine distance to speed up the search, for more details see [Vector Search Indexes in TiDB](https://docs.google.com/document/d/15eAO0xrvEd6_tTxW_zEko4CECwnnSwQg8GGrqK1Caiw)
+
+Supports following orm or framework:
 
 - [SQLAlchemy](#sqlalchemy)
 - [Django](#django)
 - [Peewee](#peewee)
 - [TiDB Vector Client](#tidb-vector-client)
 
 ### SQLAlchemy
 
+Learn how to connect to TiDB Serverless in the [TiDB Cloud documentation](https://docs.pingcap.com/tidbcloud/dev-guide-sample-application-python-sqlalchemy).
+
 Define table with vector field
 
 ```python
-from sqlalchemy import Column, Integer
+from sqlalchemy import Column, Integer, create_engine
 from sqlalchemy.orm import declarative_base
 from tidb_vector.sqlalchemy import VectorType
 
+engine = create_engine('mysql://****.root:******@gateway01.xxxxxx.shared.aws.tidbcloud.com:4000/test')
 Base = declarative_base()
 
 class Test(Base):
     __tablename__ = 'test'
     id = Column(Integer, primary_key=True)
     embedding = Column(VectorType(3))
+
+# or add hnsw index when creating table
+class TestWithIndex(Base):
+    __tablename__ = 'test_with_index'
+    id = Column(Integer, primary_key=True)
+    embedding = Column(VectorType(3), comment="hnsw(distance=l2)")
+
+Base.metadata.create_all(engine)
 ```
 
 Insert vector data
 
 ```python
 test = Test(embedding=[1, 2, 3])
 session.add(test)
@@ -96,28 +109,57 @@
 
 Define peewee table with vector field
 
 ```python
 from peewee import Model, MySQLDatabase
 from tidb_vector.peewee import VectorField
 
+# Using `pymysql` as the driver
+connect_kwargs = {
+    'ssl_verify_cert': True,
+    'ssl_verify_identity': True,
+}
+
+# Using `mysqlclient` as the driver
+connect_kwargs = {
+    'ssl_mode': 'VERIFY_IDENTITY',
+    'ssl': {
+        # Root certificate default path
+        # https://docs.pingcap.com/tidbcloud/secure-connections-to-serverless-clusters/#root-certificate-default-path
+        'ca': '/etc/ssl/cert.pem'  # MacOS
+    },
+}
+
 db = MySQLDatabase(
     'peewee_test',
     user='xxxxxxxx.root',
     password='xxxxxxxx',
     host='xxxxxxxx.shared.aws.tidbcloud.com',
     port=4000,
+    **connect_kwargs,
 )
 
 class TestModel(Model):
     class Meta:
         database = db
         table_name = 'test'
 
     embedding = VectorField(3)
+
+# or add hnsw index when creating table
+class TestModelWithIndex(Model):
+    class Meta:
+        database = db
+        table_name = 'test_with_index'
+
+    embedding = VectorField(3, constraints=[SQL("COMMENT 'hnsw(distance=l2)'")])
+
+
+db.connect()
+db.create_tables([TestModel, TestModelWithIndex])
 ```
 
 Insert vector data
 
 ```python
 TestModel.create(embedding=[1, 2, 3])
 ```
@@ -148,15 +190,15 @@
 
 Create a `TiDBVectorClient` instance:
 
 ```python
 from tidb_vector.integrations import TiDBVectorClient
 
 TABLE_NAME = 'vector_test'
-CONNECTION_STRING = 'mysql+pymysql://<USER>:<PASSWORD>@<HOST>:4000/<DB>?ssl_ca=/etc/ssl/cert.pem&ssl_verify_cert=true&ssl_verify_identity=true'
+CONNECTION_STRING = 'mysql+pymysql://<USER>:<PASSWORD>@<HOST>:4000/<DB>?ssl_verify_cert=true&ssl_verify_identity=true'
 
 tidb_vs = TiDBVectorClient(
     # the table which will store the vector data
     table_name=TABLE_NAME,
     # tidb connection string
     connection_string=CONNECTION_STRING,
     # the dimension of the vector, in this example, we use the ada model, which has 1536 dimensions
@@ -208,7 +250,17 @@
 ```python
 tidb_vs.delete(["f8e7dee2-63b6-42f1-8b60-2d46710c1971"])
 
 # delete with filter
 tidb_vs.delete(["f8e7dee2-63b6-42f1-8b60-2d46710c1971"], filter={"category": "P1"})
 ```
 
+## Examples
+
+There are some examples to show how to use the tidb-vector-python to interact with TiDB Vector in different scenarios.
+
+- [OpenAI Embedding](./examples/openai_embedding/README.md): use the OpenAI embedding model to generate vectors for text data, store them in TiDB Vector, and search for similar text.
+- [Image Search](./examples/image_search/README.md): use the OpenAI CLIP model to generate vectors for image and text, store them in TiDB Vector, and search for similar images.
+- [LlamaIndex RAG with UI](./examples/llamaindex-tidb-vector-with-ui/README.md): use the LlamaIndex to build an [RAG(Retrieval-Augmented Generation)](https://docs.llamaindex.ai/en/latest/getting_started/concepts/) application.
+
+for more examples, see the [examples](./examples) directory.
+
```

