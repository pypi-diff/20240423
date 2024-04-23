# Comparing `tmp/hashboard_cli-1.0.8.tar.gz` & `tmp/hashboard_cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashboard_cli-1.0.8.tar", last modified: Tue Apr 16 14:51:46 2024, max compression
+gzip compressed data, was "hashboard_cli-1.0.9.tar", last modified: Tue Apr 23 15:13:56 2024, max compression
```

## Comparing `hashboard_cli-1.0.8.tar` & `hashboard_cli-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.738848 hashboard_cli-1.0.8/
--rw-r--r--   0 elagulsen   (501) staff       (20)    11357 2023-08-14 18:27:21.000000 hashboard_cli-1.0.8/LICENSE
--rw-r--r--   0 elagulsen   (501) staff       (20)      859 2024-04-16 14:51:46.738788 hashboard_cli-1.0.8/PKG-INFO
--rw-r--r--   0 elagulsen   (501) staff       (20)      141 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/README.md
--rw-r--r--   0 elagulsen   (501) staff       (20)      104 2023-08-15 19:32:06.000000 hashboard_cli-1.0.8/pyproject.toml
--rw-r--r--   0 elagulsen   (501) staff       (20)      837 2024-04-16 14:51:46.739091 hashboard_cli-1.0.8/setup.cfg
--rw-r--r--   0 elagulsen   (501) staff       (20)       38 2023-08-14 18:27:21.000000 hashboard_cli-1.0.8/setup.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.732293 hashboard_cli-1.0.8/src/
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.734675 hashboard_cli-1.0.8/src/hashboard/
--rw-r--r--   0 elagulsen   (501) staff       (20)       18 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/__init__.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.734942 hashboard_cli-1.0.8/src/hashboard/api/
--rw-r--r--   0 elagulsen   (501) staff       (20)    13660 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/api/__init__.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.735592 hashboard_cli-1.0.8/src/hashboard/api/access_keys/
--rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/__init__.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     4227 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/browser_auth.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     4409 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/existing_user.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     2143 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/utils.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.736025 hashboard_cli-1.0.8/src/hashboard/api/analytics/
--rw-r--r--   0 elagulsen   (501) staff       (20)      900 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/analytics/__init__.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     4003 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/analytics/cli_with_tracking.py
--rw-r--r--   0 elagulsen   (501) staff       (20)       20 2024-04-12 14:43:11.000000 hashboard_cli-1.0.8/src/hashboard/api/analytics/events.py
--rw-r--r--   0 elagulsen   (501) staff       (20)    38904 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/cli.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      346 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/constants.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1744 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/credentials.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     3843 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/filesystem.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      597 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/session.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.737039 hashboard_cli-1.0.8/src/hashboard/utils/
--rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/__init__.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      665 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/cli.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1977 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/utils/config.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      230 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/env.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     2922 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/utils/grn.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      941 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/input_validation.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1468 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/resource.py
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.738501 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/
--rw-r--r--   0 elagulsen   (501) staff       (20)      859 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/PKG-INFO
--rw-r--r--   0 elagulsen   (501) staff       (20)     1098 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)        1 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)       42 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/entry_points.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)      103 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/requires.txt
--rw-r--r--   0 elagulsen   (501) staff       (20)       10 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/top_level.txt
-drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.738310 hashboard_cli-1.0.8/tests/
--rw-r--r--   0 elagulsen   (501) staff       (20)      310 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/tests/test_cli.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     1534 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/tests/test_credentials.py
--rw-r--r--   0 elagulsen   (501) staff       (20)     3890 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/tests/test_filesystem.py
--rw-r--r--   0 elagulsen   (501) staff       (20)      668 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/tests/test_hashboard_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.975898 hashboard_cli-1.0.9/
+-rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 hashboard_cli-1.0.9/LICENSE
+-rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-23 15:13:56.975823 hashboard_cli-1.0.9/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      141 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/README.md
+-rw-r--r--   0 anixon     (501) staff       (20)      104 2023-08-30 15:47:31.000000 hashboard_cli-1.0.9/pyproject.toml
+-rw-r--r--   0 anixon     (501) staff       (20)      878 2024-04-23 15:13:56.976189 hashboard_cli-1.0.9/setup.cfg
+-rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 hashboard_cli-1.0.9/setup.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.965875 hashboard_cli-1.0.9/src/
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.968841 hashboard_cli-1.0.9/src/hashboard/
+-rw-r--r--   0 anixon     (501) staff       (20)       18 2024-04-23 15:12:51.000000 hashboard_cli-1.0.9/src/hashboard/__init__.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.969251 hashboard_cli-1.0.9/src/hashboard/api/
+-rw-r--r--   0 anixon     (501) staff       (20)    14525 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/__init__.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.970374 hashboard_cli-1.0.9/src/hashboard/api/access_keys/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4227 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/browser_auth.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4409 2024-03-18 20:02:56.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/existing_user.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2143 2024-03-18 20:02:56.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/utils.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.971419 hashboard_cli-1.0.9/src/hashboard/api/analytics/
+-rw-r--r--   0 anixon     (501) staff       (20)      900 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/src/hashboard/api/analytics/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4003 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/src/hashboard/api/analytics/cli_with_tracking.py
+-rw-r--r--   0 anixon     (501) staff       (20)       20 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/src/hashboard/api/analytics/events.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.972227 hashboard_cli-1.0.9/src/hashboard/api/datasource/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/datasource/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)    11030 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/datasource/datasource_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2950 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/datasource/utils.py
+-rw-r--r--   0 anixon     (501) staff       (20)    38873 2024-04-23 14:57:44.000000 hashboard_cli-1.0.9/src/hashboard/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)      346 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/constants.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1744 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     3843 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/src/hashboard/filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      597 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/src/hashboard/session.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.973860 hashboard_cli-1.0.9/src/hashboard/utils/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)      665 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1977 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/src/hashboard/utils/config.py
+-rw-r--r--   0 anixon     (501) staff       (20)      230 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/env.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2922 2023-11-06 18:51:09.000000 hashboard_cli-1.0.9/src/hashboard/utils/grn.py
+-rw-r--r--   0 anixon     (501) staff       (20)      941 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/input_validation.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1468 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/resource.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.975391 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/
+-rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)     1224 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        1 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       42 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anixon     (501) staff       (20)      138 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/requires.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       10 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.975180 hashboard_cli-1.0.9/tests/
+-rw-r--r--   0 anixon     (501) staff       (20)      310 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/tests/test_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1534 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/tests/test_credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     3890 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/tests/test_filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      668 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/tests/test_hashboard_api.py
```

### Comparing `hashboard_cli-1.0.8/LICENSE` & `hashboard_cli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/PKG-INFO` & `hashboard_cli-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 License-File: LICENSE
 Requires-Dist: Click>=8.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: requests>=2.0
 Requires-Dist: ruamel.yaml>=0.17
 Requires-Dist: yaspin>=2.1.0
 Requires-Dist: semver>=3.0.1
+Requires-Dist: prettytable>=3.7.0
+Requires-Dist: wcwidth>=0.2.13
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: cram; extra == "test"
 
 # hashboard-cli
 
 [Command-line tools](https://docs.hashboard.com/docs/data-ops/cli) for interacting with [Hashboard](https://hashboard.com).
```

### Comparing `hashboard_cli-1.0.8/setup.cfg` & `hashboard_cli-1.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 install_requires = 
 	Click >= 8.0
 	pyyaml >= 6.0
 	requests >= 2.0
 	ruamel.yaml >= 0.17
 	yaspin >= 2.1.0
 	semver >= 3.0.1
+	prettytable >= 3.7.0
+	wcwidth >= 0.2.13
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	hb = hashboard.cli:main
```

### Comparing `hashboard_cli-1.0.8/src/hashboard/api/__init__.py` & `hashboard_cli-1.0.9/src/hashboard/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,18 @@
 
     build_func = _create_async_build if async_build else _create_build
     return build_func(
         session, project_id, build_spec, deploy, allow_dangerous_empty_build
     )
 
 
-def get_datasources(s: Session, project_id: str) -> dict:
+def get_datasources(s: Session, project_id: str) -> list:
     """Queries and formats datasources"""
     query = _get_data_connections(s, project_id)
-    data_sources = {d["name"]: d["id"] for d in query["data"]["dataConnections"]}
+    data_sources = [[d['name'], d['subType'], d['id']] for d in query["data"]["dataConnections"]]
     return data_sources
 
 
 def clear_model_cache(s: Session, model_id: str) -> str:
     """Clears the cache for the specified model"""
     return _graphql_query(
         s,
@@ -272,15 +272,16 @@
 def _get_data_connections(session: Session, project_id: str) -> dict:
     query = _graphql_query(
         session,
         """
         query dataConnections($projectId: String!){
             dataConnections(projectId: $projectId){
                 id,
-                name
+                name,
+                subType
             }
         }
         """,
         {"projectId": project_id},
     )
     return query
 
@@ -296,14 +297,38 @@
             }
         }
         """,
         {"datasourceId": datasource_id},
     )
     return query
 
+def create_data_source(session: Session, datasource: dict) -> dict:
+    # Assumes that error handling occurs a level up
+    return _graphql_query(
+        session,
+        """
+        mutation AddDatasource($datasource: DatasourceInput!) {
+          addDatasource(datasource: $datasource) {
+            id
+          }
+        }
+        """,
+        {"datasource": datasource},
+    )["data"]["addDatasource"]["id"]
+
+def test_data_source(session: Session, datasource_name: str, project_id: str) -> bool:
+    return _graphql_query(
+        session,
+        """
+        query TestDatasourceByName($name: String!, $projectId: String!) {
+            testDatasourceByName(name: $name, projectId: $projectId) 
+        }
+        """,
+        {"name": datasource_name, "projectId": project_id},
+    )["data"]["testDatasourceByName"]
 
 def get_tables(s: Session, datasource_id: str) -> Dict[str, Dict[str, str]]:
     """Queries and formats table from datasource"""
     query = _get_table_data(s, datasource_id)
     tables = _parse_table_data(query)
     return tables
 
@@ -409,7 +434,8 @@
         HASHBOARD_BASE_URI + f"/export/{endpoint}",
         data=json.dumps(data),
         headers={"Glean-CLI-Version": VERSION, **additional_headers},
     )
     if r.status_code != 200:
         raise ClickException("Unexpected error received from the Hashboard server.")
     return r.text
+
```

### Comparing `hashboard_cli-1.0.8/src/hashboard/api/access_keys/browser_auth.py` & `hashboard_cli-1.0.9/src/hashboard/api/access_keys/browser_auth.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/api/access_keys/existing_user.py` & `hashboard_cli-1.0.9/src/hashboard/api/access_keys/existing_user.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/api/access_keys/utils.py` & `hashboard_cli-1.0.9/src/hashboard/api/access_keys/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/api/analytics/__init__.py` & `hashboard_cli-1.0.9/src/hashboard/api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/api/analytics/cli_with_tracking.py` & `hashboard_cli-1.0.9/src/hashboard/api/analytics/cli_with_tracking.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/cli.py` & `hashboard_cli-1.0.9/src/hashboard/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 from contextlib import suppress
 from itertools import count
 import logging
 import os
 import sys
 from pathlib import Path, PurePath, PurePosixPath
 import time
-from requests import Session
+from hashboard.api.datasource.datasource_cli import datasource
 import string
 import subprocess
 from typing import Optional, List
 from uuid import UUID, uuid3
+from prettytable import PrettyTable
 
 import click
 from hashboard.session import get_current_session
 from ruamel.yaml import YAML
 
-from hashboard.api.analytics import track
 from hashboard.api.analytics.cli_with_tracking import (
     CommandWithTracking,
     GroupWithTracking,
     set_raw_command,
 )
 from hashboard.utils.env import env_with_fallback
-from hashboard.utils.input_validation import prompt_and_validate_value_length
 
 from hashboard import VERSION
 from hashboard.api import (
     apply_preview_build,
     build_details_uri,
     clear_model_cache,
     create_build_from_git_revision,
     create_build_from_local_files,
     fetch_build,
     fetch_build_status,
-    upload_files_to_hashboard,
     login,
     get_datasources,
     get_tables,
     pull_resource,
 )
 from hashboard.api.access_keys.existing_user import create_access_key
-from hashboard.constants import DEFAULT_CREDENTIALS_FILEPATH, HASHBOARD_BASE_URI, HASHBOARD_DEBUG
+from hashboard.constants import (
+    DEFAULT_CREDENTIALS_FILEPATH,
+    HASHBOARD_BASE_URI,
+    HASHBOARD_DEBUG,
+)
 from hashboard.credentials import get_credentials
 from hashboard.filesystem import local_resources
 from hashboard.utils.cli import cli_error_boundary, getenv_bool
 from hashboard.utils.grn import GRN_TYPE_KEY_MODEL, GRNComponents, parse_grn
 from hashboard.utils.resource import Resource
 
 
@@ -142,16 +144,20 @@
     ctx.obj["credentials_filepath"] = os.path.expanduser(credentials_filepath)
 
 
 @cli.command(cls=CommandWithTracking)
 @click.pass_context
 def signup(ctx: click.Context):
     """Sign up for a new Hashboard account."""
-    click.echo(f"👋 Welcome! Follow this link to get started with Hashboard and create a new project: {HASHBOARD_BASE_URI}/getAccess")
-    click.echo("After creating your project, we recommend you to run `hb token` to create an access key.")
+    click.echo(
+        f"👋 Welcome! Follow this link to get started with Hashboard and create a new project: {HASHBOARD_BASE_URI}/getAccess"
+    )
+    click.echo(
+        "After creating your project, we recommend you to run `hb token` to create an access key."
+    )
 
 
 @cli.command(cls=CommandWithTracking)
 @click.option(
     "--project-id",
     type=str,
     required=False,
@@ -163,45 +169,14 @@
 
     If `--credentials-filepath` is passed, will save the access key in that location.
     """
     create_access_key(ctx.obj["credentials_filepath"], project_id)
 
 
 @cli.command(
-    "upload",
-    cls=CommandWithTracking,
-    context_settings=dict(),
-)
-@click.argument(
-    "filepaths",
-    nargs=-1,
-    required=True,
-    type=click.Path(exists=True, dir_okay=False, allow_dash=True),
-)
-@click.pass_context
-def upload(ctx, filepaths):
-    """
-    Upload file(s) to Hashboard that can be queried using duckdb and
-    used as the basis for a data model.
-    """
-
-    s = get_current_session()
-    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
-    project_id = login(s, ctx.obj["credentials"])
-
-    files_noun = f"{len(filepaths)} file{'' if len(filepaths) == 1 else 's'}"
-    click.echo(f"📄 Uploading {files_noun} to Hashboard...")
-    for filepath in filepaths:
-        fp = os.path.expanduser(filepath)
-        uploaded_name = upload_files_to_hashboard(s, project_id, fp)
-        click.echo(f'   Uploaded "{uploaded_name}"')
-    click.echo(f"✅ Successfully uploaded {files_noun}.")
-
-
-@cli.command(
     "preview",
     cls=CommandWithTracking,
     context_settings=dict(
         ignore_unknown_options=True,
     ),
 )
 @git_revision_option
@@ -414,17 +389,28 @@
         )
         _echo_async_build_creation(build_results, False)
         build_id = build_results["data"]["createAsyncBuild"]
         build_results = _poll_for_build_status(build_id)
         _echo_async_build_results(build_results)
         if not click.confirm("Continue with deploy?"):
             ctx.exit(1)
-        deploy_build = _deploy_preview_build(build_id)
-        deploy_build_results = deploy_build["data"]["applyPreviewBuild"]
-        _echo_async_build_results(deploy_build_results, deploy=True)
+        deploy_results = _create_build_using_options(
+            ctx,
+            filepath,
+            git_revision=git_revision,
+            git_path=git_path,
+            deploy=True,
+            dbt_manifest_path=dbt_manifest_path,
+            allow_dangerous_empty_build=allow_dangerous_empty_build,
+            async_build=True,
+        )
+        _echo_async_build_creation(deploy_results, True)
+        deploy_id = deploy_results["data"]["createAsyncBuild"]
+        deploy_completed = _poll_for_build_status(deploy_id)
+        _echo_async_build_results(deploy_completed)
 
     click.echo("")
     click.echo(click.style("✅ Deploy complete.", fg="bright_green"))
 
 
 def _poll_for_build_status(build_id):
     s = get_current_session()
@@ -441,28 +427,14 @@
             return build
         time.sleep(10)
     click.echo("Error fetching build, max attempt.", fg="red")
     click.get_current_context().exit(1)
 
 
 @cli.command(cls=CommandWithTracking)
-@click.pass_context
-def databases(ctx):
-    """See your available database connections.
-
-    A database connection can be added in the Settings tab on hashboard.com."""
-    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
-    s = get_current_session()
-    project_id = login(s, ctx.obj["credentials"])
-
-    datasources = get_datasources(s, project_id)
-    _echo_datasources(datasources)
-
-
-@cli.command(cls=CommandWithTracking)
 @click.argument("database")
 @click.pass_context
 def tables(ctx, database):
     """Specify a database connection and see its available tables."""
     ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     s = get_current_session()
     project_id = login(s, ctx.obj["credentials"])
@@ -764,14 +736,17 @@
         )
 
     click.echo()
     click.echo(f"✅ Using manifest file at {manifest_path}\n")
     return manifest_path
 
 
+cli.add_command(datasource)
+
+
 def _create_build_using_options(
     ctx: click.Context,
     filepath: str,
     dbt_manifest_path: Optional[PurePath] = None,
     git_revision: Optional[str] = None,
     git_path: Optional[str] = None,
     deploy: bool = False,
@@ -820,20 +795,26 @@
     click.echo("")
     click.secho(f"❗{table} was not found in {datasource}'s tables.", fg="red")
     click.echo("")
     _echo_tables(list(tables.keys()), datasource)
     click.echo("")
 
 
-def _echo_datasources(datasources: dict) -> None:
-    click.secho("🗒  Available Database Connections ", fg="bright_green")
-    _echo_list(list(datasources.keys()))
+def _echo_datasources(datasources: list) -> None:
+    click.secho("🗒  Available data connections ", fg="bright_green")
+    columns = ["Data connection name", "Data connection type", "ID"]
+    table = PrettyTable(columns)
+    for col in columns:
+        table.align[col] = "l"
+    for ds in datasources:
+        table.add_row(ds)
+    click.echo(table)
 
 
-def _echo_datasource_not_found(datasource: str, datasources: dict) -> None:
+def _echo_datasource_not_found(datasource: str, datasources: list) -> None:
     """If datasource not found, output warning and available datasources."""
     click.echo("")
     click.secho(f"❗{datasource} was not found in your database connections.", fg="red")
     click.echo("")
     _echo_datasources(datasources)
     click.echo("")
     click.echo(
@@ -929,15 +910,17 @@
         + click.style(created_build_results["id"], bold=True)
         + click.style(" completed successfully.", fg="bright_green")
     )
 
     click.echo()
 
     _echo_build_resources(
-        _convert_to_resource_update_list(build_results["changeSet"]["resourceChanges"]),
+        _convert_to_resource_update_list(
+            created_build_results["changeSet"]["resourceChanges"]
+        ),
         deploy,
     )
 
     if created_build_results["warnings"]:
         _echo_build_warnings(created_build_results["warnings"])
 
     click.echo("")
@@ -999,14 +982,27 @@
         errors = ["Something went wrong, please contact Hashboard for support."]
     _echo_list(errors, color="red")
     click.echo("")
     click.secho("Build failed.", fg="red")
     click.get_current_context().exit(1)
 
 
+def _echo_datasource_creation_errors_and_exit(errors: List[str]):
+    click.echo("")
+    click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――–––", fg="red")
+    click.echo("❗ Errors encountered when creating your datasource")
+    click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――–––", fg="red")
+    if not errors:
+        errors = ["Something went wrong, please contact Hashboard for support."]
+    _echo_list(errors, color="red")
+    click.echo("")
+    click.secho("Datasource creation failed.", fg="red")
+    click.get_current_context().exit(1)
+
+
 def _echo_build_warnings(warnings: List[str]):
     click.echo("")
     click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="yellow")
     click.echo(" ⚠️  Warnings encountered when creating your build")
     click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="yellow")
     if not warnings:
         warnings = ["Warning message missing, please contact Hashboard for support."]
```

### Comparing `hashboard_cli-1.0.8/src/hashboard/credentials.py` & `hashboard_cli-1.0.9/src/hashboard/credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/filesystem.py` & `hashboard_cli-1.0.9/src/hashboard/filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/session.py` & `hashboard_cli-1.0.9/src/hashboard/session.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/utils/cli.py` & `hashboard_cli-1.0.9/src/hashboard/utils/cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/utils/config.py` & `hashboard_cli-1.0.9/src/hashboard/utils/config.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/utils/grn.py` & `hashboard_cli-1.0.9/src/hashboard/utils/grn.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/utils/input_validation.py` & `hashboard_cli-1.0.9/src/hashboard/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard/utils/resource.py` & `hashboard_cli-1.0.9/src/hashboard/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/src/hashboard_cli.egg-info/PKG-INFO` & `hashboard_cli-1.0.9/src/hashboard_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 License-File: LICENSE
 Requires-Dist: Click>=8.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: requests>=2.0
 Requires-Dist: ruamel.yaml>=0.17
 Requires-Dist: yaspin>=2.1.0
 Requires-Dist: semver>=3.0.1
+Requires-Dist: prettytable>=3.7.0
+Requires-Dist: wcwidth>=0.2.13
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: cram; extra == "test"
 
 # hashboard-cli
 
 [Command-line tools](https://docs.hashboard.com/docs/data-ops/cli) for interacting with [Hashboard](https://hashboard.com).
```

### Comparing `hashboard_cli-1.0.8/src/hashboard_cli.egg-info/SOURCES.txt` & `hashboard_cli-1.0.9/src/hashboard_cli.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 src/hashboard/api/access_keys/__init__.py
 src/hashboard/api/access_keys/browser_auth.py
 src/hashboard/api/access_keys/existing_user.py
 src/hashboard/api/access_keys/utils.py
 src/hashboard/api/analytics/__init__.py
 src/hashboard/api/analytics/cli_with_tracking.py
 src/hashboard/api/analytics/events.py
+src/hashboard/api/datasource/__init__.py
+src/hashboard/api/datasource/datasource_cli.py
+src/hashboard/api/datasource/utils.py
 src/hashboard/utils/__init__.py
 src/hashboard/utils/cli.py
 src/hashboard/utils/config.py
 src/hashboard/utils/env.py
 src/hashboard/utils/grn.py
 src/hashboard/utils/input_validation.py
 src/hashboard/utils/resource.py
```

### Comparing `hashboard_cli-1.0.8/tests/test_credentials.py` & `hashboard_cli-1.0.9/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/tests/test_filesystem.py` & `hashboard_cli-1.0.9/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.8/tests/test_hashboard_api.py` & `hashboard_cli-1.0.9/tests/test_hashboard_api.py`

 * *Files identical despite different names*

