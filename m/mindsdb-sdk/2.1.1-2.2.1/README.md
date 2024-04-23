# Comparing `tmp/mindsdb_sdk-2.1.1.tar.gz` & `tmp/mindsdb_sdk-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mindsdb_sdk-2.1.1.tar", last modified: Fri Jan 19 11:50:26 2024, max compression
+gzip compressed data, was "dist/mindsdb_sdk-2.2.1.tar", last modified: Tue Apr 23 18:25:28 2024, max compression
```

## Comparing `mindsdb_sdk-2.1.1.tar` & `mindsdb_sdk-2.2.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/
--rwxr-xr-x   0 runner    (1001) docker     (127)      407 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/connectors/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/ml_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18669 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/utils/objects_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/utils/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/mindsdb_sdk/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 11:50:26.000000 mindsdb_sdk-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-19 11:50:17.000000 mindsdb_sdk-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      407 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connectors/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/knowledge_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/ml_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/skills.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/objects_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/setup.py
```

### Comparing `mindsdb_sdk-2.1.1/PKG-INFO` & `mindsdb_sdk-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsdb_sdk
-Version: 2.1.1
+Version: 2.2.1
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
```

### Comparing `mindsdb_sdk-2.1.1/README.md` & `mindsdb_sdk-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/connect.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/connect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from mindsdb_sdk.server import Server
 
 from mindsdb_sdk.connectors.rest_api import RestAPI
 
+DEFAULT_LOCAL_API_URL = 'http://127.0.0.1:47334'
+DEFAULT_CLOUD_API_URL = 'https://cloud.mindsdb.com'
 
-def connect(url: str = None, login: str = None, password: str = None, is_managed: bool = False) -> Server:
+
+def connect(url: str = None, login: str = None, password: str = None, is_managed: bool = False, headers=None) -> Server:
     """
     Create connection to mindsdb server
 
     :param url: url to mindsdb server
     :param login: user login, for cloud version it contents email
     :param password: user password to login (for cloud version)
     :param is_managed: whether or not the URL points to a managed instance
+    :param headers: addtional headers to send with the connection, optional
     :return: Server object
 
     Examples
     --------
 
     >>> import mindsdb_sdk
 
@@ -32,15 +36,15 @@
 
     >>> con = mindsdb_sdk.connect('http://<YOUR_INSTANCE_IP>', login='a@b.com', password='-', is_managed=True)
 
     """
     if url is None:
         if login is not None:
             # default is cloud
-            url = 'https://cloud.mindsdb.com'
+            url = DEFAULT_CLOUD_API_URL
         else:
             # is local
-            url = 'http://127.0.0.1:47334'
+            url = DEFAULT_LOCAL_API_URL
 
-    api = RestAPI(url, login, password, is_managed)
+    api = RestAPI(url, login, password, is_managed, headers=headers)
 
-    return Server(api)
+    return Server(api)
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/databases.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/databases.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/handlers.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/jobs.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,20 +51,15 @@
 
 
 class Jobs(CollectionBase):
     def __init__(self, project, api):
         self.project = project
         self.api = api
 
-    def list(self, name: str = None) -> List[Job]:
-        """
-        Show list of jobs in project
-
-        :return: list of Job objects
-        """
+    def _list(self, name: str = None) -> List[Job]:
 
         ast_query = Select(targets=[Star()], from_table=Identifier('jobs'))
 
         if name is not None:
             ast_query.where = dict_to_binary_op({'name': name})
 
         df = self.api.sql_query(ast_query.to_string(), database=self.project.name)
@@ -74,70 +69,90 @@
         df = df.rename(columns=cols_map)
 
         return [
             Job(self.project, item)
             for item in df.to_dict('records')
         ]
 
+    def list(self) -> List[Job]:
+        """
+        Show list of jobs in project
+
+        :return: list of Job objects
+        """
+
+        return self._list()
+
     def get(self, name: str) -> Job:
         """
         Get job by name from project
 
         :param name: name of the job
         :return: Job object
         """
 
-        jobs = self.list(name)
+        jobs = self._list(name)
         if len(jobs) == 1:
             return jobs[0]
         elif len(jobs) == 0:
             raise AttributeError("Job doesn't exist")
         else:
             raise RuntimeError("Several jobs with the same name")
 
-    def create(self, name: str, query_str: str,
-                   start_at: dt.datetime = None, end_at: dt.datetime = None,
-                   repeat_str: str = None) -> Union[Job, None]:
+    def create(
+            self,
+            name: str,
+            query_str: str,
+            start_at: dt.datetime = None,
+            end_at: dt.datetime = None,
+            repeat_str: str = None,
+            repeat_min: int = None,
+        ) -> Union[Job, None]:
         """
         Create new job in project and return it.
 
         If it is not possible (job executed and not accessible anymore):
            return None
 
         More info: https://docs.mindsdb.com/sql/create/jobs
 
         :param name: name of the job
         :param query_str: str, job's query (or list of queries with ';' delimiter) which job have to execute
         :param start_at: datetime, first start of job,
         :param end_at: datetime, when job have to be stopped,
         :param repeat_str: str, optional, how to repeat job (e.g. '1 hour', '2 weeks', '3 min')
+        :param repeat_min: int, optional, period to repeat the job in minutes
         :return: Job object or None
         """
 
         if start_at is not None:
             start_str = start_at.strftime("%Y-%m-%d %H:%M:%S")
         else:
             start_str = None
 
         if end_at is not None:
             end_str = end_at.strftime("%Y-%m-%d %H:%M:%S")
         else:
             end_str = None
+
+        if repeat_min is not None:
+            repeat_str = f'{repeat_min} minutes'
+
         ast_query = CreateJob(
             name=Identifier(name),
             query_str=query_str,
             start_str=start_str,
             end_str=end_str,
             repeat_str=repeat_str
         )
 
         self.api.sql_query(ast_query.to_string(), database=self.project.name)
 
         # job can be executed and remove it is not repeatable
-        jobs = self.list(name)
+        jobs = self._list(name)
         if len(jobs) == 1:
             return jobs[0]
 
     def drop(self, name: str):
         """
         Drop job from project
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/ml_engines.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/ml_engines.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/models.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,22 +26,22 @@
     List model versions
 
     >>> model.list_versions()
 
 
     Get info
 
-    >>> print(model.status)
+    >>> print(model.get_status())
     >>> print(model.data)
 
     Update model data from server
 
     >>> model.refresh()
 
-Usng model
+    **Usng model**
 
     Dataframe on input
 
     >>> result_df = model.predict(df_rental)
     >>> result_df = model.predict(df_rental, params={'a': 'q'})
 
     Dict on input
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/projects.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/projects.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from typing import  List
 
 from mindsdb_sql.parser.dialects.mindsdb import CreateDatabase
 from mindsdb_sql.parser.ast import DropDatabase
-from mindsdb_sql.parser.ast import  Identifier, Delete
+from mindsdb_sql.parser.ast import Identifier, Delete
 
 from mindsdb_sdk.utils.sql import dict_to_binary_op
 
+from mindsdb_sdk.agents import Agents
+from mindsdb_sdk.databases import Databases
+from mindsdb_sdk.skills import Skills
 from mindsdb_sdk.utils.objects_collection import CollectionBase
 
 from .models import Models
 from .query import Query
 from .views import Views
 from .jobs import Jobs
+from .knowledge_bases import KnowledgeBases
 
 
 class Project:
     """
     Allows to work with project: to manage models and views inside of it or call raw queries inside of project
 
     Server instance allows to manipulate project and databases (integration) on mindsdb server
@@ -41,15 +45,15 @@
     ...     WHERE t.saledate > LATEST AND t.type = 'house'
     ...     AND t.bedrooms=2
     ...     LIMIT 4;
     ...    ''').fetch()
 
     """
 
-    def __init__(self, api, name):
+    def __init__(self, api, name, agents: Agents = None, skills: Skills = None, knowledge_bases: KnowledgeBases = None, databases: Databases = None):
         self.name = name
         self.api = api
 
         self.models = Models(self, api)
 
         # old api
         self.get_model = self.models.get
@@ -69,14 +73,20 @@
 
         # old api
         self.get_job = self.jobs.get
         self.list_jobs = self.jobs.list
         self.create_job = self.jobs.create
         self.drop_job = self.jobs.drop
 
+        self.databases = databases or Databases(api)
+        self.knowledge_bases = knowledge_bases or KnowledgeBases(self, api)
+
+        self.skills = skills or Skills(api, name)
+        self.agents = agents or Agents(api, name, self.knowledge_bases, self.databases, self.skills)
+
     def __repr__(self):
         return f'{self.__class__.__name__}({self.name})'
 
     def query(self, sql: str) -> Query:
         """
         Execute raw query inside of project
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/query.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/server.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from .agents import Agents
 from .databases import Databases
 from .projects import Project, Projects
 from .ml_engines import MLEngines
 from .handlers import Handlers
+from .skills import Skills
 
 
 class Server(Project):
     """
     Server instance allows to manipulate project and databases (integration) on mindsdb server
 
     Attributes for accessing to different objects:
@@ -19,27 +21,28 @@
     Server is also root(mindsdb) project and has attributes of project:
         - models, see :func:`~mindsdb_sdk.models.Models`
         - views, see :func:`~mindsdb_sdk.views.Views`
         - jobs, see :func:`~mindsdb_sdk.jobs.Jobs`
 
     """
 
-    def __init__(self, api):
+    def __init__(self, api, skills: Skills = None, agents: Agents = None):
         # server is also mindsdb project
-        super().__init__(api, 'mindsdb')
+        project_name = 'mindsdb'
+        self.databases = Databases(api)
+        super().__init__(api, project_name, skills=skills, agents=agents, databases=self.databases)
 
         self.projects = Projects(api)
 
         # old api
         self.get_project = self.projects.get
         self.list_projects = self.projects.list
         self.create_project = self.projects.create
         self.drop_project = self.projects.drop
 
-        self.databases = Databases(api)
 
         # old api
         self.get_database = self.databases.get
         self.list_databases = self.databases.list
         self.create_database = self.databases.create
         self.drop_database = self.databases.drop
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/tables.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import copy
 from typing import Union
 from typing import List
 
 import pandas as pd
 
 from mindsdb_sql.parser.ast import DropTables
-from mindsdb_sql.parser.ast import Select, Star, Identifier, Constant, Delete, Insert, Update
+from mindsdb_sql.parser.ast import Select, Star, Identifier, Constant, Delete, Insert, Update, Last, BinaryOperation
 
-from mindsdb_sdk.utils.sql import dict_to_binary_op
+from mindsdb_sdk.utils.sql import dict_to_binary_op, add_condition
 from mindsdb_sdk.utils.objects_collection import CollectionBase
 
 from .query import Query
 
 
 class Table(Query):
     def __init__(self, db, name):
         super().__init__(db.api, '', db.name)
         self.name = name
         self.db = db
         self._filters = {}
         self._limit = None
+        self._track_column = None
         self._update_query()
 
     def _filters_repr(self):
         filters = ''
         if len(self._filters) > 0:
             filters = ', '.join(
                 f'{k}={v}'
@@ -41,37 +42,67 @@
     def filter(self, **kwargs):
         """
         Applies filters on table
         table.filter(a=1, b=2) adds where condition to table:
         'select * from table1 where a=1 and b=2'
 
         :param kwargs: filter
+        :return: Table object
         """
         # creates new object
         query = copy.deepcopy(self)
         query._filters.update(kwargs)
         query._update_query()
         return query
 
     def limit(self, val: int):
         """
         Applies limit condition to table query
 
         :param val: limit size
+        :return: Table object
         """
         query = copy.deepcopy(self)
         query._limit = val
         query._update_query()
         return query
 
+    def track(self, column):
+        """
+        Apply tracking column to table. ('LAST' keyword in mindsdb)
+        First call returns nothing
+        The next calls return new records since previous call (where value of track_column is greater)
+
+        Example:
+
+        >>> query = con.databases.my_db.tables.sales.filter(type='house').track('created_at')
+        >>> # first call returns no records
+        >>> df = query.fetch()
+        >>> # second call returns rows with created_at is greater since previous fetch
+        >>> df = query.fetch()
+
+        :param column: column to track new data from table.
+        :return: Table object
+        """
+        query = copy.deepcopy(self)
+        query._track_column = column
+
+        query._update_query()
+        return query
+
     def _update_query(self):
+        where = dict_to_binary_op(self._filters)
+        if self._track_column is not None:
+            condition = BinaryOperation(op='>', args=[Identifier(self._track_column), Last()])
+            where = add_condition(where, condition)
+
         ast_query = Select(
             targets=[Star()],
             from_table=Identifier(self.name),
-            where=dict_to_binary_op(self._filters)
+            where=where
         )
         if self._limit is not None:
             ast_query.limit = Constant(self._limit)
         self.sql = ast_query.to_string()
 
     def insert(self, query: Union[pd.DataFrame, Query]):
         """
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/utils/objects_collection.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/utils/objects_collection.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk/views.py` & `mindsdb_sdk-2.2.1/mindsdb_sdk/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         :param database: datasource of the view (where input sql will be executed)
         :return: View object
         """
         if isinstance(sql, Query):
             database = sql.database
             sql = sql.sql
         elif not isinstance(sql, str):
-            raise ValueError()
+            raise ValueError(sql)
 
         if database is not None:
             database = Identifier(database)
         ast_query = CreateView(
             name=Identifier(name),
             query_str=sql,
             from_table=database
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/PKG-INFO` & `mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsdb-sdk
-Version: 2.1.1
+Version: 2.2.1
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
```

### Comparing `mindsdb_sdk-2.1.1/mindsdb_sdk.egg-info/SOURCES.txt` & `mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 mindsdb_sdk/__about__.py
 mindsdb_sdk/__init__.py
+mindsdb_sdk/agents.py
 mindsdb_sdk/connect.py
 mindsdb_sdk/databases.py
 mindsdb_sdk/handlers.py
 mindsdb_sdk/jobs.py
+mindsdb_sdk/knowledge_bases.py
 mindsdb_sdk/ml_engines.py
 mindsdb_sdk/models.py
 mindsdb_sdk/projects.py
 mindsdb_sdk/query.py
 mindsdb_sdk/server.py
+mindsdb_sdk/skills.py
 mindsdb_sdk/tables.py
 mindsdb_sdk/views.py
 mindsdb_sdk.egg-info/PKG-INFO
 mindsdb_sdk.egg-info/SOURCES.txt
 mindsdb_sdk.egg-info/dependency_links.txt
 mindsdb_sdk.egg-info/requires.txt
 mindsdb_sdk.egg-info/top_level.txt
```

### Comparing `mindsdb_sdk-2.1.1/setup.py` & `mindsdb_sdk-2.2.1/setup.py`

 * *Files identical despite different names*

