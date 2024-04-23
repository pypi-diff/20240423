# Comparing `tmp/thanosql-0.2.1.tar.gz` & `tmp/thanosql-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thanosql-0.2.1.tar", last modified: Fri Apr 12 06:19:59 2024, max compression
+gzip compressed data, was "thanosql-0.2.2.tar", last modified: Tue Apr 23 06:20:33 2024, max compression
```

## Comparing `thanosql-0.2.1.tar` & `thanosql-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:59.526692 thanosql-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 06:19:51.000000 thanosql-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-12 06:19:59.526692 thanosql-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-12 06:19:51.000000 thanosql-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:51.000000 thanosql-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:19:59.526692 thanosql-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-12 06:19:51.000000 thanosql-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:59.518692 thanosql-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-12 06:19:51.000000 thanosql-0.2.1/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-04-12 06:19:51.000000 thanosql-0.2.1/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 06:19:51.000000 thanosql-0.2.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-12 06:19:51.000000 thanosql-0.2.1/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-12 06:19:51.000000 thanosql-0.2.1/tests/test_table_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 06:19:51.000000 thanosql-0.2.1/tests/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:59.518692 thanosql-0.2.1/thanosql/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:59.522692 thanosql-0.2.1/thanosql/magic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/magic/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/magic/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/magic/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/magic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:59.522692 thanosql-0.2.1/thanosql/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-12 06:19:51.000000 thanosql-0.2.1/thanosql/resources/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:19:59.522692 thanosql-0.2.1/thanosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-12 06:19:59.000000 thanosql-0.2.1/thanosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-12 06:19:59.000000 thanosql-0.2.1/thanosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:19:59.000000 thanosql-0.2.1/thanosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:19:59.000000 thanosql-0.2.1/thanosql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 06:19:59.000000 thanosql-0.2.1/thanosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 06:19:59.000000 thanosql-0.2.1/thanosql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.085106 thanosql-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 06:20:27.000000 thanosql-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-23 06:20:33.085106 thanosql-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-23 06:20:27.000000 thanosql-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:27.000000 thanosql-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:20:33.085106 thanosql-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-23 06:20:27.000000 thanosql-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.077106 thanosql-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_table_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-23 06:20:27.000000 thanosql-0.2.2/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.077106 thanosql-0.2.2/thanosql/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.081106 thanosql-0.2.2/thanosql/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/magic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.081106 thanosql-0.2.2/thanosql/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-23 06:20:27.000000 thanosql-0.2.2/thanosql/resources/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:33.081106 thanosql-0.2.2/thanosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:32.000000 thanosql-0.2.2/thanosql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 06:20:33.000000 thanosql-0.2.2/thanosql.egg-info/top_level.txt
```

### Comparing `thanosql-0.2.1/LICENSE` & `thanosql-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/PKG-INFO` & `thanosql-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.2.1
+Version: 0.2.2
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
```

### Comparing `thanosql-0.2.1/README.md` & `thanosql-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/setup.py` & `thanosql-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/tests/test_file.py` & `thanosql-0.2.2/tests/test_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,42 +39,45 @@
     with pytest.raises(ThanoSQLNotFoundError):
         client.file.upload(
             path=file_name,
             db_commit=True,
             table=basic_table_name,
             column=fake.unique.pystr(8),
             dir=dir_name,
+            if_exists="replace",
         )
 
     # trying to insert text into integer column
     with pytest.raises(ThanoSQLValueError):
         client.file.upload(
             path=file_name,
             db_commit=True,
             table=basic_table_name,
             column=int_column_name,
             dir=dir_name,
+            if_exists="replace",
         )
 
     # upload without db_commit and dir
     # note that we cannot check the existence of uploaded files as it requires user_data_root
     # which can technically be saved, but it increases complexity and safety risk
-    res = client.file.upload(path=file_name)
+    res = client.file.upload(path=file_name, if_exists="replace")
     assert res["data"]["file_path"] == default_file_path
 
     # upload with db_commit and dir
     target_table = client.table.get(name=basic_table_name)
     record_count_before = target_table.get_records().total
 
     res = client.file.upload(
         path=file_name,
         db_commit=True,
         table=basic_table_name,
         column=column_name,
         dir=dir_name,
+        if_exists="replace",
     )
     assert res["data"]["file_path"] == f"drive/{dir_name}/{file_name}"
     assert res["data"]["table_name"] == basic_table_name
     assert res["data"]["column_name"] == column_name
 
     record_count_after = target_table.get_records().total
     assert record_count_after == record_count_before + 1
@@ -83,14 +86,15 @@
 def test_get_files(client: ThanoSQL):
     # path must start with drive/
     with pytest.raises(ThanoSQLValueError):
         client.file.list(path=dir_name)
 
     res = client.file.list(path=f"drive/{dir_name}/*")
     # at least the file we just uploaded
+    assert isinstance(res["data"]["matched_pathnames"], list)
     assert len(res["data"]["matched_pathnames"]) >= 1
 
 
 def test_delete_file(client: ThanoSQL, basic_table_name: str):
     # path must start with drive/
     with pytest.raises(ThanoSQLValueError):
         client.file.delete(path=dir_name)
```

### Comparing `thanosql-0.2.1/tests/test_query.py` & `thanosql-0.2.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/tests/test_schema.py` & `thanosql-0.2.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/tests/test_table.py` & `thanosql-0.2.2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/tests/test_table_template.py` & `thanosql-0.2.2/tests/test_table_template.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/tests/test_view.py` & `thanosql-0.2.2/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql/_base_client.py` & `thanosql-0.2.2/thanosql/_base_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,45 @@
 import requests
 from tqdm import tqdm
 
 import thanosql._error as thanosql_error
 
 
 class ThanoSQLBaseClient:
+    """Base client for accessing various ThanoSQL services.
+
+    Attributes
+    ----------
+    token: str
+        Access token to be used in the request header.
+    base_url: str
+        Base URL of the ThanoSQL service.
+    version: str
+        Version of the API.
+    url: str
+        Base API URL of the ThanoSQL service that contains the base_url
+        and version.
+
+    Raises
+    ------
+    ThanoSQLPermissionError
+        - If an invalid API token is provided.
+        - If an operation is forbidden.
+    ThanoSQLAlreadyExistsError
+        If an object with the same name already exists.
+    ThanoSQLNotFoundError
+        If a requested object is not found.
+    ThanoSQLValueError
+        If input values are in incorrect format.
+    ThanoSQLInternalError
+        If an error happens while doing operations on the workspace
+        or fetching data from the database.
+
+    """
+
     def __init__(self, token: str, base_url: str, version: str) -> None:
         self.token: str = token
         self.base_url: str = base_url.strip("/")
         self.version: str = version
 
         self.url: str = f"{self.base_url}/api/{version}"
```

### Comparing `thanosql-0.2.1/thanosql/_client.py` & `thanosql-0.2.2/thanosql/_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,48 @@
     SchemaService,
     TableService,
     ViewService,
 )
 
 
 class ThanoSQL(ThanoSQLBaseClient):
+    """Client for accessing the ThanoSQL engine.
+
+    Parameters
+    ----------
+    api_token: str, optional
+        The workspace/engine API token. If not supplied, will be retrieved
+        from the THANOSQL_API_TOKEN environment variable.
+    engine_url: str, optional
+        The workspace engine URL. If not supplied, will be retrieved from
+        the THANOSQL_ENGINE_URL environment variable.
+    api_version: str, default "v1"
+        The version of the API used.
+
+    Attributes
+    ----------
+    query: QueryService
+        The service layer for query APIs.
+    file: FileService
+        The service layer for file APIs.
+    schema: SchemaService
+        The service layer for schema APIs.
+    table: TableService
+        The service layer for table APIs.
+    view: ViewService
+        The service layer for view APIs.
+
+    Raises
+    ------
+    ThanoSQLValueError
+        If API token and/or engine URL is neither passed in as parameters
+        nor set as environment variables.
+
+    """
+
     def __init__(
         self,
         api_token: Optional[str] = None,
         engine_url: Optional[str] = None,
         api_version: str = "v1",
     ) -> None:
         if api_token is None:
```

### Comparing `thanosql-0.2.1/thanosql/_error.py` & `thanosql-0.2.2/thanosql/_error.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql/_service.py` & `thanosql-0.2.2/thanosql/_service.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql/magic/magic.py` & `thanosql-0.2.2/thanosql/magic/magic.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql/magic/parse.py` & `thanosql-0.2.2/thanosql/magic/parse.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql/magic/util.py` & `thanosql-0.2.2/thanosql/magic/util.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql/resources/__init__.py` & `thanosql-0.2.2/thanosql/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql/resources/_record.py` & `thanosql-0.2.2/thanosql/resources/_record.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.2.1/thanosql.egg-info/PKG-INFO` & `thanosql-0.2.2/thanosql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.2.1
+Version: 0.2.2
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
```

### Comparing `thanosql-0.2.1/thanosql.egg-info/SOURCES.txt` & `thanosql-0.2.2/thanosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

