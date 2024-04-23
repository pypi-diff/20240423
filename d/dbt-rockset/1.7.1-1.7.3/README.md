# Comparing `tmp/dbt-rockset-1.7.1.tar.gz` & `tmp/dbt_rockset-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-rockset-1.7.1.tar", last modified: Fri Mar 22 21:25:46 2024, max compression
+gzip compressed data, was "dbt_rockset-1.7.3.tar", last modified: Tue Apr 23 17:41:15 2024, max compression
```

## Comparing `dbt-rockset-1.7.1.tar` & `dbt_rockset-1.7.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.261937 dbt-rockset-1.7.1/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       47 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/MANIFEST.in
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      315 2024-03-22 21:25:46.261937 dbt-rockset-1.7.1/PKG-INFO
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)    11300 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/README.md
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.253937 dbt-rockset-1.7.1/dbt/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-03-22 18:35:34.000000 dbt-rockset-1.7.1/dbt/__init__.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.253937 dbt-rockset-1.7.1/dbt/adapters/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-03-22 18:35:34.000000 dbt-rockset-1.7.1/dbt/adapters/__init__.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.257937 dbt-rockset-1.7.1/dbt/adapters/rockset/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      505 2024-03-22 18:35:34.000000 dbt-rockset-1.7.1/dbt/adapters/rockset/__init__.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       18 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/adapters/rockset/__version__.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      694 2024-03-22 18:35:34.000000 dbt-rockset-1.7.1/dbt/adapters/rockset/column.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     4667 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/adapters/rockset/connections.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)    34774 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/adapters/rockset/impl.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1154 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/adapters/rockset/relation.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.257937 dbt-rockset-1.7.1/dbt/include/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-03-22 18:35:34.000000 dbt-rockset-1.7.1/dbt/include/__init__.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.257937 dbt-rockset-1.7.1/dbt/include/rockset/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       51 2024-03-22 18:35:34.000000 dbt-rockset-1.7.1/dbt/include/rockset/__init__.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       91 2024-01-12 19:22:23.000000 dbt-rockset-1.7.1/dbt/include/rockset/dbt_project.yml
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.257937 dbt-rockset-1.7.1/dbt/include/rockset/macros/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      132 2024-01-12 19:22:23.000000 dbt-rockset-1.7.1/dbt/include/rockset/macros/catalog.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       82 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/include/rockset/macros/current_ts.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      475 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/include/rockset/macros/macros.sql
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.257937 dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1040 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/incremental.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1605 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/seed.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      658 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/table.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      934 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/view.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      463 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/dbt/include/rockset/profile_template.yml
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-03-22 21:25:46.261937 dbt-rockset-1.7.1/dbt_rockset.egg-info/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      315 2024-03-22 21:25:46.000000 dbt-rockset-1.7.1/dbt_rockset.egg-info/PKG-INFO
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      915 2024-03-22 21:25:46.000000 dbt-rockset-1.7.1/dbt_rockset.egg-info/SOURCES.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)        1 2024-03-22 21:25:46.000000 dbt-rockset-1.7.1/dbt_rockset.egg-info/dependency_links.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       42 2024-03-22 21:25:46.000000 dbt-rockset-1.7.1/dbt_rockset.egg-info/requires.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)        4 2024-03-22 21:25:46.000000 dbt-rockset-1.7.1/dbt_rockset.egg-info/top_level.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       38 2024-03-22 21:25:46.261937 dbt-rockset-1.7.1/setup.cfg
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      690 2024-03-22 21:23:22.000000 dbt-rockset-1.7.1/setup.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       47 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/MANIFEST.in
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      315 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/PKG-INFO
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)    11253 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/README.md
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.923008 dbt_rockset-1.7.3/dbt/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/__init__.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.923008 dbt_rockset-1.7.3/dbt/adapters/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/__init__.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.927008 dbt_rockset-1.7.3/dbt/adapters/rockset/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      507 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/__init__.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       18 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/__version__.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      694 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/column.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     4653 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/connections.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)    37792 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/impl.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1157 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/relation.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.927008 dbt_rockset-1.7.3/dbt/include/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/include/__init__.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.927008 dbt_rockset-1.7.3/dbt/include/rockset/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       52 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/include/rockset/__init__.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       91 2024-01-12 19:22:23.000000 dbt_rockset-1.7.3/dbt/include/rockset/dbt_project.yml
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.931008 dbt_rockset-1.7.3/dbt/include/rockset/macros/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      132 2024-01-12 19:22:23.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/catalog.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       82 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/current_ts.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      475 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/macros.sql
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.931008 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1040 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/incremental.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      664 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/query_lambda.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1605 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/seed.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      658 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/table.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      934 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/view.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      463 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/profile_template.yml
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/dbt_rockset.egg-info/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      315 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/PKG-INFO
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      976 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/SOURCES.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)        1 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/dependency_links.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       42 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/requires.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)        4 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/top_level.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       38 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/setup.cfg
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      668 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/setup.py
```

### Comparing `dbt-rockset-1.7.1/README.md` & `dbt_rockset-1.7.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 Type | Supported? | Details
 -----|------------|----------------
 [Table](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#table) | YES | Creates a [Rockset collection](https://docs.rockset.com/collections/).
 [View](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#view) | YES | Creates a [Rockset view](https://rockset.com/docs/views/#gatsby-focus-wrapper).
 [Ephemeral](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#ephemeral) | Yes | Create a CTE.
 [Incremental](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#incremental) | YES | Creates a [Rockset collection](https://docs.rockset.com/collections/) if it doesn't exist, and writes to it.
 
+Query Lambda can be created and updated using dbt. See the tests for an example usage.
+
 ## Real-Time Streaming ELT Using dbt + Rockset
 
 As data is ingested, Rockset performs the following:
 * The data is automatically indexed in at least three different ways using Rockset’s [Converged Index™](https://rockset.com/blog/converged-indexing-the-secret-sauce-behind-rocksets-fast-queries/) technology.
 * Your write-time data transformations are performed.
 * The data is made available for queries within seconds.
 
@@ -134,30 +136,26 @@
 * Transform and persist them into Rockset collections via Incremental or Table Models.
 * Execute a sequence of view models during read-time to transform your data again.
 
 ## Testing, Formatting, & Caveats
 
 ### Testing Changes
 
-Install [dbt-adapter-tests](https://github.com/dbt-labs/dbt-adapter-tests) in order to run the tests:
-```
-pip3 install pytest-dbt-adapter
-```
-
-Before landing a commit, ensure that your changes pass tests by inserting an api key for any active Rockset org in `test/rockset.dbtspec`, and then running these two commands to install your changes in your local environment and run our test suite:
+Before landing a commit, ensure that your changes pass tests. Your credentials should be set in the .env file in the repo root. See the test.env file for an example. Once the .env file is set, you can run the tests using the following command.
 ```
-pip3 install .
-pytest test/rockset.dbtspec
+pytest -s tests/functional
 ```
 
 ### Formatting
 
-Before landing a commit, format changes according to pep8 using these commands:
+Before landing a commit format changes using [black](https://github.com/psf/black).
 ```
-pip3 install autopep8
-autopep8 --in-place --recursive .
+# Install
+python -m pip install black
+# Usage (From repo root)
+python -m black .
 ```
 
 ### Caveats
 1. `unique_key` is not supported with incremental, unless it is set to [_id](https://rockset.com/docs/special-fields/#the-_id-field), which acts as a natural `unique_key` in Rockset anyway.
 2. The `table` materialization is slower in Rockset than most due to Rockset's architecture as a low-latency, real-time database. Creating new collections requires provisioning hot storage to index and serve fresh data, which takes about a minute.
 3. Rockset queries have a two-minute timeout unless run asynchronously. You can extend this limit to 30 minutes by setting the run_async_iis to true. However, if the query ends up in the queue because you have hit your org's Concurrent Query Execution Limit (CQEL), the query must at least start execution before 2 minutes have passed. Otherwise, your IIS query will error. If the query leaves the queue and begins execution before 2 minutes have passed, the normal 30 minute time limit will apply.
```

### Comparing `dbt-rockset-1.7.1/dbt/adapters/rockset/column.py` & `dbt_rockset-1.7.3/dbt/adapters/rockset/column.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 import rockset
 
 
 @dataclass
 class RocksetColumn(Column):
     def is_integer(self) -> bool:
-        return self.dtype.lower() in ['int']
+        return self.dtype.lower() in ["int"]
 
     def is_numeric(self) -> bool:
-        return self.dtype.lower() in ['int', 'float']
+        return self.dtype.lower() in ["int", "float"]
 
     def is_float(self):
-        return self.dtype.lower() in ['float']
+        return self.dtype.lower() in ["float"]
 
     def is_string(self):
-        return self.dtype.lower() in ['string']
+        return self.dtype.lower() in ["string"]
 
     def string_size(self) -> int:
         if not self.is_string():
             raise DbtRuntimeError("Called string_size() on non-string field!")
 
         return rockset.Client.MAX_FIELD_VALUE_BYTES
```

### Comparing `dbt-rockset-1.7.1/dbt/adapters/rockset/connections.py` & `dbt_rockset-1.7.3/dbt/adapters/rockset/connections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,119 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from dbt.adapters.base import Credentials
 from dbt.adapters.base import BaseConnectionManager
 from dbt.clients import agate_helper
 from dbt.contracts.connection import AdapterResponse, Connection
 from dbt.logger import GLOBAL_LOGGER as logger
+from dbt.exceptions import NotImplementedError, DbtValidationError
 
 import agate
 import dbt
 import rockset_sqlalchemy as sql
 from .__version__ import version as rs_version
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 
 @dataclass
 class RocksetCredentials(Credentials):
     database: str = "db"
     vi_rrn: Optional[str] = None
     run_async_iis: Optional[bool] = False
-    api_server: Optional[str] = 'api.usw2a1.rockset.com'
+    api_server: Optional[str] = "api.usw2a1.rockset.com"
     api_key: Optional[str] = None
     schema: Optional[str] = None
 
     @property
     def type(self):
-        return 'rockset'
+        return "rockset"
 
     @property
     def unique_field(self):
         return self.api_key
 
     def _connection_keys(self):
-        return ('api_key', 'apiserver', 'schema')
+        return ("api_key", "apiserver", "schema")
 
-    _ALIASES = {
-        'workspace': 'schema'
-    }
+    _ALIASES = {"workspace": "schema"}
 
 
 class RocksetConnectionManager(BaseConnectionManager):
-    TYPE = 'rockset'
+    TYPE = "rockset"
 
     @classmethod
     def open(cls, connection: Connection) -> Connection:
-        if connection.state == 'open':
-            logger.debug('Connection is already open, skipping open.')
+        if connection.state == "open":
+            logger.debug("Connection is already open, skipping open.")
             return connection
 
         credentials = connection.credentials
 
         # Ensure the credentials have a valid apiserver before connecting to rockset
-        if not (credentials.api_server is not None and 'api' in credentials.api_server and credentials.api_server.endswith("rockset.com")):
-            raise dbt.exceptions.NotImplementedException(
-                f'Invalid apiserver `{credentials.api_server}` specified in profile. Expecting a server of the form api.<region>.rockset.com')
+        if not (
+            credentials.api_server is not None
+            and "api" in credentials.api_server
+            and credentials.api_server.endswith("rockset.com")
+        ):
+            raise DbtValidationError(
+                f"Invalid apiserver `{credentials.api_server}` specified in profile. Expecting a server of the form api.<region>.rockset.com"
+            )
 
         try:
             handle = sql.connect(
-                api_server=credentials.api_server,
-                api_key=credentials.api_key
+                api_server=credentials.api_server, api_key=credentials.api_key
             )
-            handle._client.api_client.user_agent = 'dbt/' + rs_version
+            handle._client.api_client.user_agent = "dbt/" + rs_version
 
-            connection.state = 'open'
+            connection.state = "open"
             connection.handle = handle
             return connection
         except Exception as e:
-            connection.state = 'fail'
+            connection.state = "fail"
             connection.handle = None
             raise dbt.exceptions.FailedToConnectException(e)
 
     @classmethod
     def get_status(cls, cursor) -> str:
         # Rockset cursors don't have a status_message
-        return 'OK'
+        return "OK"
 
     def cancel_open(self) -> Optional[List[str]]:
-        raise dbt.exceptions.NotImplementedException(
-            '`cancel_open` is not implemented for this adapter!'
-        )
+        raise NotImplementedError("`cancel_open` is not implemented for this adapter!")
 
     def begin(self) -> None:
         """Begin a transaction. (passable)"""
-        raise dbt.exceptions.NotImplementedException(
-            '`begin` is not implemented for this adapter!'
-        )
+        raise NotImplementedError("`begin` is not implemented for this adapter!")
 
     def commit(self) -> None:
         """Commit a transaction. (passable)"""
-        raise dbt.exceptions.NotImplementedException(
-            '`commit` is not implemented for this adapter!'
-        )
+        raise NotImplementedError("`commit` is not implemented for this adapter!")
 
     def clear_transaction(self) -> None:
         pass
 
     # auto_begin is ignored in Rockset, and only included for consistency
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
+        self,
+        sql: str,
+        auto_begin: bool = False,
+        fetch: bool = False,
+        limit: Optional[int] = None,
     ) -> Tuple[Union[AdapterResponse, str], agate.Table]:
         sql = self._add_query_comment(sql)
         cursor = self.get_thread_connection().handle.cursor()
 
         if fetch:
             rows, field_names = self._sql_to_results(cursor, sql, limit)
             table = agate_helper.table_from_data_flat(rows, field_names)
         else:
             cursor.execute(sql)
             table = agate_helper.empty_table()
 
-        return AdapterResponse(_message='OK'), table
+        return AdapterResponse(_message="OK"), table
 
     def _sql_to_results(self, cursor, sql, limit):
         cursor.execute(sql)
         field_names = self._description_to_field_names(cursor.description)
         json_results = []
         if limit is None:
             rows = cursor.fetchall()
@@ -136,8 +137,8 @@
         try:
             yield
         except Exception as e:
             raise e
 
     @classmethod
     def get_response(cls, cursor) -> str:
-        return 'OK'
+        return "OK"
```

### Comparing `dbt-rockset-1.7.1/dbt/adapters/rockset/impl.py` & `dbt_rockset-1.7.3/dbt/adapters/rockset/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.rockset.connections import RocksetConnectionManager
 from dbt.adapters.rockset.relation import RocksetQuotePolicy, RocksetRelation
 from dbt.contracts.graph.manifest import Manifest
 from dbt.adapters.rockset.column import RocksetColumn
 from dbt.logger import GLOBAL_LOGGER as logger
 from dbt.adapters.base import BaseRelation
+from dbt.exceptions import NotImplementedError
 from .__version__ import version as rs_version
 
 import agate
 import datetime
 import dbt
 import json
 import collections
-import os
 import requests
 import rockset
+from rockset.models import *
+from rockset import ApiException
 from decimal import Decimal
-from time import sleep, time
+from time import sleep
 from typing import List, Optional, Set
 
 
 OK = 200
 NOT_FOUND = 404
 ASYNC_OPTIONS = {
     "client_timeout_ms": 1000,  # arbitrary
@@ -96,30 +98,30 @@
         # Drop all views in the ws
         for view in self._list_views(ws):
             self._delete_view_recursively(ws, view)
 
         # Drop all aliases in the ws
         for alias in rs.Aliases.workspace_aliases(workspace=ws).data:
             self._delete_alias(ws, alias.name)
-
         # Drop all collections in the ws
         for collection in rs.Collections.workspace_collections(workspace=ws).data:
-            self._delete_collection(
-                ws, collection.name, wait_until_deleted=False)
+            self._delete_collection(ws, collection.name, wait_until_deleted=False)
+        # Drop all QLs in the ws
+        for ql in rs.QueryLambdas.list_query_lambdas_in_workspace(workspace=ws).data:
+            self._delete_ql(ws, ql.name)
 
         try:
             # Wait until the ws has 0 collections. We do this so deletion of multiple collections
             # can happen in parallel
             while True:
                 workspace = rs.Workspaces.get(workspace=ws).data
                 if workspace.collection_count == 0:
                     break
                 logger.debug(
-                    f"Waiting for ws {ws} to have 0 collections, has {
-                        workspace.collection_count}"
+                    f"Waiting for ws {ws} to have 0 collections, has {workspace.collection_count}"
                 )
                 sleep(3)
 
             rs.Workspaces.delete(workspace=ws)
             sleep(4)  # Wait for workspace to be deleted
         except Exception as e:
             logger.debug(f"Caught exception of type {e.__class__}")
@@ -133,17 +135,15 @@
     @available
     def list_schemas(self, database: str) -> List[str]:
         rs = self._rs_client()
         return [ws.name for ws in rs.Workspaces.list().data]
 
     # Relation/Collection related methods
     def truncate_relation(self, relation: RocksetRelation) -> None:
-        raise dbt.exceptions.NotImplementedException(
-            "`truncate` is not implemented for this adapter!"
-        )
+        raise NotImplementedError("`truncate` is not implemented for this adapter!")
 
     @available.parse(lambda *a, **k: "")
     def get_dummy_sql(self):
         return f"""
             /* Placeholder Query  */
             SELECT 3;
         """
@@ -155,37 +155,35 @@
 
         if self._does_view_exist(ws, identifier):
             self._delete_view_recursively(ws, identifier)
         elif self._does_collection_exist(ws, identifier):
             self._delete_collection(ws, identifier)
         else:
             raise dbt.exceptions.Exception(
-                f"Tried to drop relation {ws}.{
-                    identifier} that does not exist!"
+                f"Tried to drop relation {ws}.{identifier} that does not exist!"
             )
 
     def rename_relation(
         self, from_relation: RocksetRelation, to_relation: RocksetRelation
     ) -> None:
-        raise dbt.exceptions.NotImplementedException(
-            "`rename` is not implemented for this adapter!"
-        )
+        raise NotImplementedError("`rename` is not implemented for this adapter!")
 
     @available.parse(lambda *a, **k: "")
     def get_collection(self, relation) -> RocksetRelation:
         ws = relation.schema
         cname = relation.identifier
 
         try:
             rs = self._rs_client()
-            existing_collection = rs.Collections.get(
-                collection=cname, workspace=ws)
+            existing_collection = rs.Collections.get(collection=cname, workspace=ws)
             return self._rs_collection_to_relation(existing_collection)
         except Exception as e:
-            if hasattr(e, "status") and e.status == NOT_FOUND:  # Collection does not exist
+            if (
+                hasattr(e, "status") and e.status == NOT_FOUND
+            ):  # Collection does not exist
                 return None
             else:  # Unexpected error
                 raise e
 
     # Required by BaseAdapter
     def list_relations_without_caching(
         self, schema_relation: RocksetRelation
@@ -200,16 +198,15 @@
     def list_relations(
         self, database: Optional[str], schema: str
     ) -> List[RocksetRelation]:
 
         rs = self._rs_client()
         relations = []
 
-        collections = rs.Collections.workspace_collections(
-            workspace=schema).data
+        collections = rs.Collections.workspace_collections(workspace=schema).data
         for collection in collections:
             relations.append(self._rs_collection_to_relation(collection))
         return relations
 
     # Required by BaseAdapter
     def get_columns_in_relation(self, relation: RocksetRelation) -> List[RocksetColumn]:
         logger.debug(f"Getting columns in relation {relation.identifier}")
@@ -246,25 +243,21 @@
             for k, v in field_types.items()
         ]
 
     def get_filtered_catalog(
         self, manifest: Manifest, relations: Optional[Set[BaseRelation]] = None
     ):
         catalogs: agate.Table
-        if (
-            relations is None
-            or len(relations) > 100
-        ):
+        if relations is None or len(relations) > 100:
             # Do it the traditional way. We get the full catalog.
             catalogs, exceptions = self.get_catalog(manifest)
         else:
             # Do it the new way. We try to save time by selecting information
             # only for the exact set of relations we are interested in.
-            catalogs, exceptions = self.get_catalog_by_relations(
-                manifest, relations)
+            catalogs, exceptions = self.get_catalog_by_relations(manifest, relations)
 
         if relations and catalogs:
             relation_map = {
                 (
                     r.schema.casefold() if r.schema else None,
                     r.identifier.casefold() if r.identifier else None,
                 )
@@ -278,15 +271,17 @@
                 i = i.casefold() if i is not None else None
                 return (s, i) in relation_map
 
             catalogs = catalogs.where(in_map)
 
         return catalogs, exceptions
 
-    def get_catalog_by_relations(self, manifest: Manifest, relations: List[RocksetRelation]):
+    def get_catalog_by_relations(
+        self, manifest: Manifest, relations: List[RocksetRelation]
+    ):
         rs = self._rs_client()
 
         columns = [
             "table_database",
             "table_name",
             "table_schema",
             "table_type",
@@ -300,18 +295,21 @@
             "stats:bytes:include",
             "column_type",
             "column_name",
             "column_index",
         ]
         catalog_rows = []
         databases = {x.database for x in manifest.sources.values()} | {
-            x.database for x in manifest.nodes.values()}
+            x.database for x in manifest.nodes.values()
+        }
         # DB is not a thing in RS. Include all DBs to be filtered out in later stages of catalog generation
         for relation in relations:
-            for collection in rs.Collections.workspace_collections(workspace=relation.schema).data:
+            for collection in rs.Collections.workspace_collections(
+                workspace=relation.schema
+            ).data:
                 rel = self.Relation.create(
                     schema=collection.workspace, identifier=collection.name
                 )
                 col_types = self._get_types_in_relation(rel)
                 for i, c in enumerate(col_types):
                     for db in databases:
                         catalog_rows.append(
@@ -333,57 +331,135 @@
                                 i,
                             ]
                         )
         catalog_table = agate.Table(
             rows=catalog_rows,
             column_names=columns,
             column_types=agate.TypeTester(
-                force={"table_database": agate.Text(
-                    cast_nulls=False, null_values=[])}
+                force={"table_database": agate.Text(cast_nulls=False, null_values=[])}
             ),
         )
 
         return catalog_table, []
 
     # Rockset doesn't support DESCRIBE on views, so those are not included in the catalog information
     def get_catalog(self, manifest: Manifest) -> agate.Table:
         schemas = super()._get_cache_schemas(manifest)
         return self.get_catalog_by_relations(manifest, schemas)
 
     def expand_column_types(
         self, goal: RocksetRelation, current: RocksetRelation
     ) -> None:
-        raise dbt.exceptions.NotImplementedException(
+        raise NotImplementedError(
             "`expand_column_types` is not implemented for this adapter!"
         )
 
     def expand_target_column_types(
         self, from_relation: RocksetRelation, to_relation: RocksetRelation
     ) -> None:
-        raise dbt.exceptions.NotImplementedException(
+        raise NotImplementedError(
             "`expand_target_column_types` is not implemented for this adapter!"
         )
 
     @classmethod
     def quote(cls, identifier: str) -> str:
         return "`{}`".format(identifier)
 
     ###
     # Special Rockset implementations
     ###
 
     @available.parse(lambda *a, **k: "")
     def do_debug(self, obj):
         import pdb
+
         pdb.set_trace()
 
     @available.parse(lambda *a, **k: "")
     def apply_snapshot(self, relation, sql):
         raise dbt.exceptions.Exception("Snapshots unsupported")
 
+    # Query Lambda materialization
+    @available.parse(lambda *a, **k: "")
+    def create_or_update_query_lambda(self, relation, sql, tags, parameters):
+        ws = relation.schema
+        name = relation.identifier
+        # Ensure workspace exists
+        self.create_schema(relation)
+
+        if self._query_lambda_exists(ws, name):
+            self._update_query_lambda(ws, name, sql, tags, parameters)
+        else:
+            self._create_query_lambda(ws, name, sql, tags, parameters)
+
+    def _update_query_lambda(self, ws, name, sql, tags, parameters):
+        rs = self._rs_client()
+        query_params = [QueryParameter(**qp) for qp in parameters]
+        try:
+            api_response = rs.QueryLambdas.update_query_lambda(
+                workspace=ws,
+                description="Created via DBT",
+                is_public=False,
+                query_lambda=name,
+                sql=QueryLambdaSql(
+                    default_parameters=query_params,
+                    query=sql,
+                ),
+            )
+            ql_version = api_response.data.version
+            for t in tags:
+                self._add_query_lambda_tag(ws, name, ql_version, t)
+        except ApiException as e:
+            logger.error(e)
+            raise e
+
+    def _create_query_lambda(self, ws, name, sql, tags, parameters):
+        rs = self._rs_client()
+        query_params = [QueryParameter(**qp) for qp in parameters]
+        try:
+            api_response = rs.QueryLambdas.create_query_lambda(
+                workspace=ws,
+                description="Created via DBT",
+                is_public=False,
+                name=name,
+                sql=QueryLambdaSql(
+                    default_parameters=query_params,
+                    query=sql,
+                ),
+            )
+            ql_version = api_response.data.version
+            for t in tags:
+                self._add_query_lambda_tag(ws, name, ql_version, t)
+        except ApiException as e:
+            logger.error(e)
+            raise e
+
+    def _add_query_lambda_tag(self, ws, name, version, tag):
+        rs = self._rs_client()
+        api_response = rs.QueryLambdas.create_query_lambda_tag(
+            workspace=ws,
+            query_lambda=name,
+            tag_name=tag,
+            version=version,
+        )
+
+    def _query_lambda_exists(self, ws, name):
+        # Check if latest tag exists
+        rs = self._rs_client()
+        try:
+            resp = rs.QueryLambdas.get_query_lambda_tag_version(
+                workspace=ws, query_lambda=name, tag="latest"
+            )
+            return True
+        except ApiException as e:
+            if e.status == 404:
+                return False
+            else:
+                raise e
+
     # Table materialization
     @available.parse(lambda *a, **k: "")
     def create_table(self, relation, sql):
         ws = relation.schema
         cname = relation.identifier
         rs = self._rs_client()
 
@@ -419,28 +495,26 @@
             d = dict(row.dict())
             for k, v in d.items():
                 d[k] = self._convert_agate_data_type(v)
             json_docs.append(d)
 
         # The check for a view should happen before this point
         if self._does_view_exist(ws, cname):
-            raise dbt.exceptions.Exception(
-                f"InternalError : View {ws}.{cname} exists")
+            raise dbt.exceptions.Exception(f"InternalError : View {ws}.{cname} exists")
 
         # Create the Rockset collection
         if not self._does_collection_exist(ws, cname):
             rs = self._rs_client()
             rs.Collections.create_s3_collection(name=cname, workspace=ws)
         self._wait_until_collection_ready(ws, cname)
 
         # Write the results to the collection and wait until the docs are ingested
         body = {"data": json_docs}
         write_api_endpoint = f"/v1/orgs/self/ws/{ws}/collections/{cname}/docs"
-        resp = json.loads(self._send_rs_request(
-            "POST", write_api_endpoint, body).text)
+        resp = json.loads(self._send_rs_request("POST", write_api_endpoint, body).text)
         self._wait_until_past_commit_fence(ws, cname, resp["last_offset"])
 
     def _convert_agate_data_type(self, v):
         if v is None:
             return None
         elif isinstance(v, str):
             return v
@@ -474,15 +548,15 @@
 
         # Sleep a few seconds to be extra sure that all caches are updated with the new view
         sleep(3)
 
     @available.parse(lambda *a, **k: "")
     def add_incremental_docs(self, relation, sql, unique_key):
         if unique_key and unique_key != "_id":
-            raise dbt.exceptions.NotImplementedException(
+            raise NotImplementedError(
                 "`unique_key` can only be set to `_id` with the Rockset adapter!"
             )
 
         ws = relation.schema
         cname = relation.identifier
         self._wait_until_collection_ready(ws, cname)
 
@@ -516,29 +590,27 @@
     def _execute_iis_query_and_wait_for_docs(self, relation, sql):
         query_id, num_docs_inserted = self._execute_iis_query(relation, sql)
         if num_docs_inserted > 0:
             self._wait_until_iis_query_processed(
                 relation.schema, relation.identifier, query_id
             )
         else:
-            logger.info(
-                f"Query {query_id} inserted 0 docs; no ingest to wait for.")
+            logger.info(f"Query {query_id} inserted 0 docs; no ingest to wait for.")
 
     # Execute a query not using the SQL cursor, but by hitting the REST api. This should be done
     # if you need the QueryResponse object returned
     # Returns: query_id (str), num_docs_inserted (int)
     def _execute_iis_query(self, relation, sql):
         iis_sql = f"INSERT INTO {relation} {sql}"
         logger.debug(f"Executing sql: {iis_sql}")
 
         if self._rs_vi_rrn():
-            endpoint = f"/v1/orgs/self/virtualinstances/{
-                self._rs_vi_rrn()}/queries"
+            endpoint = f"/v1/orgs/self/virtualinstances/{self._rs_vi_rrn()}/queries"
         else:
-            endpoint = '/v1/orgs/self/queries'
+            endpoint = "/v1/orgs/self/queries"
 
         body = {
             "sql": {"query": iis_sql},
         }
         if self._rs_run_async_iis():
             body["async_options"] = ASYNC_OPTIONS
 
@@ -552,28 +624,30 @@
         if json_resp["status"] == "QUEUED" or json_resp["status"] == "RUNNING":
             self._wait_until_async_query_completed(query_id)
             # Async IIS queries do not have results saved in s3 so just assume docs were inserted
             # If this behavior changes in the future, then get the results of the async IIS query
             # and get num_docs_inserted
             return query_id, 1
 
-        assert len(
-            json_resp["results"]) == 1, f"IIS queries should return only one document but got {len(json_resp['results'])}"
+        assert (
+            len(json_resp["results"]) == 1
+        ), f"IIS queries should return only one document but got {len(json_resp['results'])}"
 
         return query_id, json_resp["results"][0]["num_docs_inserted"]
 
     def _wait_until_collection_does_not_exist(self, cname, ws):
         while True:
             try:
                 self._rs_client().Collections.get(collection=cname, workspace=ws)
-                logger.debug(
-                    f"Waiting for collection {ws}.{cname} to be deleted...")
+                logger.debug(f"Waiting for collection {ws}.{cname} to be deleted...")
                 sleep(3)
             except Exception as e:
-                if hasattr(e, "status") and e.status == NOT_FOUND:  # Collection does not exist
+                if (
+                    hasattr(e, "status") and e.status == NOT_FOUND
+                ):  # Collection does not exist
                     return
                 raise e
 
     def _wait_until_view_does_not_exist(self, ws, view):
         while True:
             if self._does_view_exist(ws, view):
                 logger.debug(f"Waiting for view {ws}.{view} to be deleted")
@@ -585,34 +659,31 @@
         max_wait_time_secs = 600
         sleep_secs = 3
         total_sleep_time = 0
 
         while total_sleep_time < max_wait_time_secs:
             if not self._does_collection_exist(ws, cname):
                 logger.debug(
-                    f"Collection {ws}.{
-                        cname} does not exist. This is likely a transient consistency error."
+                    f"Collection {ws}.{cname} does not exist. This is likely a transient consistency error."
                 )
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
                 continue
 
             c = self._rs_client().Collections.get(collection=cname, workspace=ws)
             if c.data["status"] == "READY":
                 logger.debug(f"{ws}.{cname} is ready!")
                 return
             else:
-                logger.debug(
-                    f"Waiting for collection {ws}.{cname} to become ready...")
+                logger.debug(f"Waiting for collection {ws}.{cname} to become ready...")
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
 
         raise dbt.exceptions.Exception(
-            f"Waited more than {max_wait_time_secs} secs for {
-                ws}.{cname} to become ready. Something is wrong."
+            f"Waited more than {max_wait_time_secs} secs for {ws}.{cname} to become ready. Something is wrong."
         )
 
     def _rs_collection_to_relation(self, collection):
 
         if collection is None:
             return None
 
@@ -633,36 +704,51 @@
                 sleep(3)
             else:
                 break
 
     def _wait_until_collection_deleted(self, ws, cname):
         while True:
             if self._does_collection_exist(ws, cname):
-                logger.debug(
-                    f"Waiting for collection {ws}.{cname} to be deleted")
+                logger.debug(f"Waiting for collection {ws}.{cname} to be deleted")
                 sleep(3)
             else:
                 break
 
     def _delete_collection(self, ws, cname, wait_until_deleted=True):
         rs = self._rs_client()
 
         for ref_view in self._get_referencing_views(ws, cname):
             self._delete_view_recursively(ref_view[0], ref_view[1])
 
         try:
             c = rs.Collections.delete(collection=cname, workspace=ws)
 
             if wait_until_deleted:
-                self._wait_until_collection_deleted(
-                    ws, cname)
+                self._wait_until_collection_deleted(ws, cname)
         except Exception as e:
             if hasattr(e, "status") and e.status != NOT_FOUND:
                 raise e  # Unexpected error
 
+    def _delete_ql(self, ws, ql):
+        rs = self._rs_client()
+        try:
+            rs.QueryLambdas.delete_query_lambda(query_lambda=ql, workspace=ws)
+            self._wait_until_ql_deleted(ws, ql)
+        except Exception as e:
+            if hasattr(e, "status") and e.status != NOT_FOUND:
+                raise e  # Unexpected error
+
+    def _wait_until_ql_deleted(self, ws, ql):
+        while True:
+            if self._query_lambda_exists(ws, ql):
+                logger.debug(f"Waiting for ql {ws}.{ql} to be deleted")
+                sleep(3)
+            else:
+                break
+
     def _delete_alias(self, ws, alias):
         rs = self._rs_client()
 
         for ref_view in self._get_referencing_views(ws, alias):
             self._delete_view_recursively(ref_view[0], ref_view[1])
 
         try:
@@ -670,52 +756,49 @@
             self._wait_until_alias_deleted(ws, alias)
         except Exception as e:
             if hasattr(e, "status") and e.status != NOT_FOUND:
                 raise e  # Unexpected error
 
     def _wait_until_past_commit_fence(self, ws, cname, fence):
         endpoint = (
-            f"/v1/orgs/self/ws/{ws}/collections/{
-                cname}/offsets/commit?fence={fence}"
+            f"/v1/orgs/self/ws/{ws}/collections/{cname}/offsets/commit?fence={fence}"
         )
         while True:
             resp = self._send_rs_request("GET", endpoint)
             resp_json = json.loads(resp.text)
             passed = resp_json["data"]["passed"]
             commit_offset = resp_json["offsets"]["commit"]
             if passed:
                 logger.debug(
-                    f"Commit offset {
-                        commit_offset} is past given fence {fence}"
+                    f"Commit offset {commit_offset} is past given fence {fence}"
                 )
                 break
             else:
                 logger.debug(
-                    f"Waiting for commit offset to pass fence {
-                        fence}; it is currently {commit_offset}"
+                    f"Waiting for commit offset to pass fence {fence}; it is currently {commit_offset}"
                 )
                 sleep(3)
 
     def _wait_until_async_query_completed(self, query_id):
         endpoint = f"/v1/orgs/self/queries/{query_id}"
         while True:
             query_resp = self._send_rs_request("GET", endpoint)
             query_data = json.loads(query_resp.text)
 
-            status = query_data.get("data").get(
-                "status") if "data" in query_data else None
+            status = (
+                query_data.get("data").get("status") if "data" in query_data else None
+            )
             if status == "COMPLETED":
                 return
             elif status == "ERROR" or status == "CANCELLED":
                 raise Exception(
-                    f"IIS query did not complete successfully. Query data: {query_resp.text}")
-            else:
-                logger.debug(
-                    f"Insert Into Query not completed yet"
+                    f"IIS query did not complete successfully. Query data: {query_resp.text}"
                 )
+            else:
+                logger.debug(f"Insert Into Query not completed yet")
                 sleep(3)
 
     def _wait_until_iis_fully_ingested(self, ws, cname, query_id):
         endpoint = f"/v1/orgs/self/queries/{query_id}"
         while True:
             query_resp = self._send_rs_request("GET", endpoint)
             query_data = json.loads(query_resp.text)
@@ -731,17 +814,19 @@
 
     def _wait_until_iis_query_processed(self, ws, cname, query_id):
         last_offset = self._wait_until_iis_fully_ingested(ws, cname, query_id)
         self._wait_until_past_commit_fence(ws, cname, last_offset)
 
     def _send_rs_request(self, type, endpoint, body=None, check_success=True):
         url = self._rs_api_server() + endpoint
-        version = 'dbt/' + rs_version
-        headers = {"authorization": f"apikey {
-            self._rs_api_key()}", "user-agent": version}
+        version = "dbt/" + rs_version
+        headers = {
+            "authorization": f"apikey {self._rs_api_key()}",
+            "user-agent": version,
+        }
 
         if type == "GET":
             resp = requests.get(url, headers=headers)
         elif type == "POST":
             resp = requests.post(url, headers=headers, json=body)
         elif type == "DELETE":
             resp = requests.delete(url, headers=headers)
@@ -766,16 +851,15 @@
         response = self._send_rs_request("GET", endpoint, check_success=False)
         if response.status_code == NOT_FOUND:
             return False
         elif response.status_code == OK:
             return True
         else:
             raise Exception(
-                f"throwing from 332 with status_code {
-                    response.status_code} and text {response.text}"
+                f"throwing from 332 with status_code {response.status_code} and text {response.text}"
             )
 
     def _does_alias_exist(self, ws, alias):
         rs = self._rs_client()
         try:
             rs.Aliases.get(alias=alias, workspace=ws)
             return True
@@ -816,16 +900,15 @@
 
         endpoint = f"{self._views_endpoint(ws)}/{view}"
         del_resp = self._send_rs_request("DELETE", endpoint)
         if del_resp.status_code == NOT_FOUND:
             return
         elif del_resp.status_code != OK:
             raise Exception(
-                f"throwing from 395 with code {
-                    del_resp.status_code} and text {del_resp.text}"
+                f"throwing from 395 with code {del_resp.status_code} and text {del_resp.text}"
             )
 
         self._wait_until_view_does_not_exist(ws, view)
 
     def _get_referencing_views(self, ws, view):
         view_path = f"{ws}.{view}"
 
@@ -850,38 +933,34 @@
         sleep_secs = 3
         total_sleep_time = 0
 
         endpoint = f"{self._views_endpoint(ws)}/{view}"
         while total_sleep_time < max_wait_time_secs:
             if not self._does_view_exist(ws, view):
                 logger.debug(
-                    f"View {ws}.{
-                        view} does not exist. This is likely a transient consistency error."
+                    f"View {ws}.{view} does not exist. This is likely a transient consistency error."
                 )
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
                 continue
 
             resp = self._send_rs_request("GET", endpoint)
             view_json = json.loads(resp.text)["data"]
             state = view_json["state"]
 
             if state == "SYNCING":
-                logger.debug(
-                    f"Waiting for view {ws}.{view} to be fully synced")
+                logger.debug(f"Waiting for view {ws}.{view} to be fully synced")
                 sleep(sleep_secs)
                 total_sleep_time += sleep_secs
             else:
-                logger.debug(
-                    f"View {ws}.{view} is synced and ready to be queried")
+                logger.debug(f"View {ws}.{view} is synced and ready to be queried")
                 return
 
         raise dbt.exceptions.Exception(
-            f"Waited more than {max_wait_time_secs} secs for view {
-                ws}.{view} to become synced. Something is wrong."
+            f"Waited more than {max_wait_time_secs} secs for view {ws}.{view} to become synced. Something is wrong."
         )
 
     def run_sql_for_tests(self, sql, fetch, conn):
         cursor = conn.handle.cursor()
         try:
             cursor.execute(sql)
             if fetch == "one":
@@ -889,15 +968,15 @@
             elif fetch == "all":
                 return cursor.fetchall()
         except BaseException as e:
             logger.error(sql)
             logger.error(e)
             raise
         finally:
-            conn.state = 'close'
+            conn.state = "close"
 
     # Overridden because Rockset generates columns not added during testing.
     def get_rows_different_sql(
         self,
         relation_a: RocksetRelation,
         relation_b: RocksetRelation,
         column_names: Optional[List[str]] = None,
@@ -906,21 +985,19 @@
 
         names: List[str]
         # columns generated by Rockset
         skip_cmp_columns: Set[str] = {"_event_time", "_id", "_meta"}
         if column_names is None:
             columns = self.get_columns_in_relation(relation_a)
             names = sorted(
-                (self.quote(c.name)
-                 for c in columns if c.name not in skip_cmp_columns)
+                (self.quote(c.name) for c in columns if c.name not in skip_cmp_columns)
             )
         else:
             names = sorted(
-                (self.quote(n)
-                 for n in column_names if n not in skip_cmp_columns)
+                (self.quote(n) for n in column_names if n not in skip_cmp_columns)
             )
         columns_csv = ", ".join(names)
 
         sql = COLUMNS_EQUAL_SQL.format(
             columns=columns_csv,
             relation_a=str(relation_a),
             relation_b=str(relation_b),
```

### Comparing `dbt-rockset-1.7.1/dbt/adapters/rockset/relation.py` & `dbt_rockset-1.7.3/dbt/adapters/rockset/relation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass, field
 from dbt.adapters.base.relation import BaseRelation, Policy
-from dbt.contracts.relation import (
-    RelationType)
+from dbt.contracts.relation import RelationType
 
 import traceback
 from typing import List, Optional, Type
 
 
 @dataclass
 class RocksetQuotePolicy(Policy):
@@ -20,17 +19,19 @@
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class RocksetRelation(BaseRelation):
     quote_policy: RocksetQuotePolicy = field(
-        default_factory=lambda: RocksetQuotePolicy())
+        default_factory=lambda: RocksetQuotePolicy()
+    )
     include_policy: RocksetIncludePolicy = field(
-        default_factory=lambda: RocksetIncludePolicy())
+        default_factory=lambda: RocksetIncludePolicy()
+    )
 
     # We override this function with a very simple implementation. Database is not a concept
     # in Rockset, so we do not make such a comparison
     def matches(
         self,
         database: Optional[str] = None,
         schema: Optional[str] = None,
```

### Comparing `dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/incremental.sql` & `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/seed.sql` & `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/table.sql` & `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-1.7.1/dbt/include/rockset/macros/materializations/view.sql` & `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-rockset-1.7.1/dbt_rockset.egg-info/SOURCES.txt` & `dbt_rockset-1.7.3/dbt_rockset.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 dbt/include/rockset/__init__.py
 dbt/include/rockset/dbt_project.yml
 dbt/include/rockset/profile_template.yml
 dbt/include/rockset/macros/catalog.sql
 dbt/include/rockset/macros/current_ts.sql
 dbt/include/rockset/macros/macros.sql
 dbt/include/rockset/macros/materializations/incremental.sql
+dbt/include/rockset/macros/materializations/query_lambda.sql
 dbt/include/rockset/macros/materializations/seed.sql
 dbt/include/rockset/macros/materializations/table.sql
 dbt/include/rockset/macros/materializations/view.sql
 dbt_rockset.egg-info/PKG-INFO
 dbt_rockset.egg-info/SOURCES.txt
 dbt_rockset.egg-info/dependency_links.txt
 dbt_rockset.egg-info/requires.txt
```

