# Comparing `tmp/vlgi_datasets-0.2.0.tar.gz` & `tmp/vlgi_datasets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlgi_datasets-0.2.0.tar", last modified: Mon Apr 22 18:50:38 2024, max compression
+gzip compressed data, was "vlgi_datasets-0.2.1.tar", last modified: Tue Apr 23 18:54:28 2024, max compression
```

## Comparing `vlgi_datasets-0.2.0.tar` & `vlgi_datasets-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 18:50:38.218025 vlgi_datasets-0.2.0/
--rw-rw-rw-   0        0        0     1259 2024-04-22 18:50:38.216023 vlgi_datasets-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      694 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/README.md
--rw-rw-rw-   0        0        0      727 2024-04-22 18:50:05.000000 vlgi_datasets-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 18:50:38.218025 vlgi_datasets-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 18:50:38.200955 vlgi_datasets-0.2.0/vlgi_datasets/
--rw-rw-rw-   0        0        0      453 2024-04-22 18:47:47.000000 vlgi_datasets-0.2.0/vlgi_datasets/__init__.py
--rw-rw-rw-   0        0        0     1398 2024-04-11 11:53:01.000000 vlgi_datasets-0.2.0/vlgi_datasets/open_pyxl_dataset.py
--rw-rw-rw-   0        0        0     2727 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/vlgi_datasets/pdf_dataset.py
--rw-rw-rw-   0        0        0     2090 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/vlgi_datasets/postgres_soft_replace_dataset.py
--rw-rw-rw-   0        0        0     2566 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/vlgi_datasets/postgres_upsert_table.py
--rw-rw-rw-   0        0        0     2475 2024-04-22 18:45:24.000000 vlgi_datasets-0.2.0/vlgi_datasets/sharepoint_excel_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-22 18:50:38.215026 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/
--rw-rw-rw-   0        0        0     1259 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 18:54:28.102473 vlgi_datasets-0.2.1/
+-rw-rw-rw-   0        0        0     1259 2024-04-23 18:54:28.100967 vlgi_datasets-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.1/README.md
+-rw-rw-rw-   0        0        0      727 2024-04-23 18:52:40.000000 vlgi_datasets-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:54:28.102473 vlgi_datasets-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 18:54:28.088312 vlgi_datasets-0.2.1/vlgi_datasets/
+-rw-rw-rw-   0        0        0      453 2024-04-22 18:47:47.000000 vlgi_datasets-0.2.1/vlgi_datasets/__init__.py
+-rw-rw-rw-   0        0        0     1398 2024-04-11 11:53:01.000000 vlgi_datasets-0.2.1/vlgi_datasets/open_pyxl_dataset.py
+-rw-rw-rw-   0        0        0     2727 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.1/vlgi_datasets/pdf_dataset.py
+-rw-rw-rw-   0        0        0     1993 2024-04-23 13:17:21.000000 vlgi_datasets-0.2.1/vlgi_datasets/postgres_soft_replace_dataset.py
+-rw-rw-rw-   0        0        0     2469 2024-04-23 12:32:24.000000 vlgi_datasets-0.2.1/vlgi_datasets/postgres_upsert_table.py
+-rw-rw-rw-   0        0        0     2475 2024-04-22 18:45:24.000000 vlgi_datasets-0.2.1/vlgi_datasets/sharepoint_excel_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:54:28.099968 vlgi_datasets-0.2.1/vlgi_datasets.egg-info/
+-rw-rw-rw-   0        0        0     1259 2024-04-23 18:54:28.000000 vlgi_datasets-0.2.1/vlgi_datasets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-04-23 18:54:28.000000 vlgi_datasets-0.2.1/vlgi_datasets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:54:28.000000 vlgi_datasets-0.2.1/vlgi_datasets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-23 18:54:28.000000 vlgi_datasets-0.2.1/vlgi_datasets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 18:54:28.000000 vlgi_datasets-0.2.1/vlgi_datasets.egg-info/top_level.txt
```

### Comparing `vlgi_datasets-0.2.0/PKG-INFO` & `vlgi_datasets-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlgi-datasets
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package with custom kedro datasets for VLGI
 Author-email: Tecnologia Grupo Sozo <tecnologia@gruposozo.com.br>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `vlgi_datasets-0.2.0/README.md` & `vlgi_datasets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.2.0/pyproject.toml` & `vlgi_datasets-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vlgi-datasets"
-version = "0.2.0"
+version = "0.2.1"
 description = "A package with custom kedro datasets for VLGI"
 authors = [
     { "name" = "Tecnologia Grupo Sozo", "email" = "tecnologia@gruposozo.com.br"}
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `vlgi_datasets-0.2.0/vlgi_datasets/open_pyxl_dataset.py` & `vlgi_datasets-0.2.1/vlgi_datasets/open_pyxl_dataset.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.2.0/vlgi_datasets/pdf_dataset.py` & `vlgi_datasets-0.2.1/vlgi_datasets/pdf_dataset.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.2.0/vlgi_datasets/postgres_soft_replace_dataset.py` & `vlgi_datasets-0.2.1/vlgi_datasets/postgres_soft_replace_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict
 
 import pandas as pd
-from kedro_datasets.pandas import SQLTableDataset
+from kedro.extras.datasets.pandas import SQLTableDataSet
 from sqlalchemy.dialects.postgresql import insert
 import sqlalchemy
 
 class PostgresSoftReplaceFactory:
     def build(self):
         def postgres_upsert(table, conn, keys, dataframe_values):
             """
@@ -31,25 +31,24 @@
 
             data = [dict(zip(keys, row)) for row in dataframe_values]
             insert_statement = insert(table.table).values(data)
             conn.execute(insert_statement)
 
         return postgres_upsert
 
-class PostgresSoftReplaceDataset(SQLTableDataset):
+class PostgresSoftReplaceDataSet(SQLTableDataSet):
     def __init__(
         self,
         table_name: str,
-        credentials: dict[str, Any],
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        credentials: Dict[str, Any],
+        load_args: Dict[str, Any] = None,
+        save_args: Dict[str, Any] = None,
     ) -> None:
         super().__init__(
-            table_name=table_name, credentials=credentials, load_args=load_args, save_args=save_args, metadata=metadata
+            table_name, credentials, load_args, save_args
         )
 
     def _save(self, data: pd.DataFrame) -> None:
         replace_method_factory = PostgresSoftReplaceFactory()
         replace_method = replace_method_factory.build()
         engine = self.engines[self._connection_str]  # type: ignore
         data.to_sql(con=engine, **self._save_args, method=replace_method)
```

### Comparing `vlgi_datasets-0.2.0/vlgi_datasets/postgres_upsert_table.py` & `vlgi_datasets-0.2.1/vlgi_datasets/postgres_upsert_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict
 
 import numpy as np
 import pandas as pd
-from kedro_datasets.pandas import SQLTableDataset
+from kedro.extras.datasets.pandas import SQLTableDataSet
 from sqlalchemy.dialects.postgresql import insert
 
 class PostgresUpsertFactory:
     def build(self, constraint):
         def postgres_upsert(table, conn, keys, dataframe_values):
             """
             Example
@@ -33,27 +33,26 @@
                 constraint=constraint,
                 set_={c.key: c for c in insert_statement.excluded},
             )
             conn.execute(upsert_statement)
 
         return postgres_upsert
 
-class PostgresTableUpsertDataset(SQLTableDataset):
+class PostgresTableUpsertDataSet(SQLTableDataSet):
     def __init__(
         self,
         table_name: str,
-        credentials: dict[str, Any],
-        load_args: dict[str, Any] = None,
-        save_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        credentials: Dict[str, Any],
+        load_args: Dict[str, Any] = None,
+        save_args: Dict[str, Any] = None,
     ) -> None:
         self.constraint = save_args.pop("constraint")
         self.chunk_size = save_args.pop("chunk_size", None)
         super().__init__(
-            table_name=table_name, credentials=credentials, load_args=load_args, save_args=save_args, metadata=metadata
+            table_name, credentials, load_args, save_args
         )
 
     def _save(self, data: pd.DataFrame) -> None:
         upsert_method_factory = PostgresUpsertFactory()
         upsert_accounts_method = upsert_method_factory.build(self.constraint)
         engine = self.engines[self._connection_str]  # type: ignore
```

### Comparing `vlgi_datasets-0.2.0/vlgi_datasets/sharepoint_excel_dataset.py` & `vlgi_datasets-0.2.1/vlgi_datasets/sharepoint_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.2.0/vlgi_datasets.egg-info/PKG-INFO` & `vlgi_datasets-0.2.1/vlgi_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlgi-datasets
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package with custom kedro datasets for VLGI
 Author-email: Tecnologia Grupo Sozo <tecnologia@gruposozo.com.br>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

