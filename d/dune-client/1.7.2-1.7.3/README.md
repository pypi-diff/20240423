# Comparing `tmp/dune_client-1.7.2.tar.gz` & `tmp/dune_client-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_client-1.7.2.tar", last modified: Mon Apr  8 08:31:45 2024, max compression
+gzip compressed data, was "dune_client-1.7.3.tar", last modified: Tue Apr 23 08:00:08 2024, max compression
```

## Comparing `dune_client-1.7.2.tar` & `dune_client-1.7.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.957249 dune_client-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 08:31:37.000000 dune_client-1.7.2/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.945249 dune_client-1.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.949249 dune_client-1.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 08:31:37.000000 dune_client-1.7.2/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 08:31:37.000000 dune_client-1.7.2/.github/workflows/py-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 08:31:37.000000 dune_client-1.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 08:31:37.000000 dune_client-1.7.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 08:31:37.000000 dune_client-1.7.2/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 08:31:37.000000 dune_client-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 08:31:37.000000 dune_client-1.7.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-08 08:31:45.957249 dune_client-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-08 08:31:37.000000 dune_client-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.949249 dune_client-1.7.2/dune_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.953249 dune_client-1.7.2/dune_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/api/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/api/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/api/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/client_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.953249 dune_client-1.7.2/dune_client/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/file/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/file/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.953249 dune_client-1.7.2/dune_client/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-08 08:31:37.000000 dune_client-1.7.2/dune_client/viz/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.957249 dune_client-1.7.2/dune_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-08 08:31:45.000000 dune_client-1.7.2/dune_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-08 08:31:45.000000 dune_client-1.7.2/dune_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:31:45.000000 dune_client-1.7.2/dune_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:31:45.000000 dune_client-1.7.2/dune_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 08:31:45.000000 dune_client-1.7.2/dune_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 08:31:45.000000 dune_client-1.7.2/dune_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 08:31:37.000000 dune_client-1.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.953249 dune_client-1.7.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 08:31:37.000000 dune_client-1.7.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 08:31:37.000000 dune_client-1.7.2/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-08 08:31:45.957249 dune_client-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 08:31:37.000000 dune_client-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.945249 dune_client-1.7.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.953249 dune_client-1.7.2/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/e2e/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/e2e/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.953249 dune_client-1.7.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/fixtures/sample_table_insert.csv
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/fixtures/sample_table_insert.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:31:45.957249 dune_client-1.7.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/unit/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-08 08:31:37.000000 dune_client-1.7.2/tests/unit/test_viz_sankey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.057742 dune_client-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 08:00:00.000000 dune_client-1.7.3/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.049742 dune_client-1.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.049742 dune_client-1.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-23 08:00:00.000000 dune_client-1.7.3/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-23 08:00:00.000000 dune_client-1.7.3/.github/workflows/py-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 08:00:00.000000 dune_client-1.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 08:00:00.000000 dune_client-1.7.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 08:00:00.000000 dune_client-1.7.3/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 08:00:00.000000 dune_client-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-23 08:00:00.000000 dune_client-1.7.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-23 08:00:08.057742 dune_client-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-23 08:00:00.000000 dune_client-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.053743 dune_client-1.7.3/dune_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.053743 dune_client-1.7.3/dune_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/api/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/api/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/api/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/client_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.053743 dune_client-1.7.3/dune_client/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/file/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.053743 dune_client-1.7.3/dune_client/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 08:00:00.000000 dune_client-1.7.3/dune_client/viz/graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.057742 dune_client-1.7.3/dune_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-23 08:00:08.000000 dune_client-1.7.3/dune_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-23 08:00:08.000000 dune_client-1.7.3/dune_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:00:08.000000 dune_client-1.7.3/dune_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:00:08.000000 dune_client-1.7.3/dune_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 08:00:08.000000 dune_client-1.7.3/dune_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 08:00:08.000000 dune_client-1.7.3/dune_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 08:00:00.000000 dune_client-1.7.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.057742 dune_client-1.7.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 08:00:00.000000 dune_client-1.7.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 08:00:00.000000 dune_client-1.7.3/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-23 08:00:08.057742 dune_client-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 08:00:00.000000 dune_client-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.049742 dune_client-1.7.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.057742 dune_client-1.7.3/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/e2e/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/e2e/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.057742 dune_client-1.7.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/fixtures/sample_table_insert.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/fixtures/sample_table_insert.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:00:08.057742 dune_client-1.7.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/unit/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-23 08:00:00.000000 dune_client-1.7.3/tests/unit/test_viz_sankey.py
```

### Comparing `dune_client-1.7.2/.github/workflows/pull-request.yaml` & `dune_client-1.7.3/.github/workflows/pull-request.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   push:
     branches: [ main ]
 jobs:
   lint-format-types-unit:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.11"]
+        python-version: ["3.8", "3.12"]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `dune_client-1.7.2/.github/workflows/py-publish.yaml` & `dune_client-1.7.3/.github/workflows/py-publish.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/LICENSE` & `dune_client-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/PKG-INFO` & `dune_client-1.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.7.2
+Version: 1.7.3
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/duneanalytics/dune-client
 Author: Benjamin H. Smith & Dune Analytics
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/duneanalytics/dune-client/issues
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Build](https://github.com/duneanalytics/dune-client/actions/workflows/pull-request.yaml/badge.svg)](https://github.com/duneanalytics/dune-client/actions/workflows/pull-request.yaml)
 
 # Dune Client
 
 A python framework for interacting with Dune Analytics' [officially supported API
-service](https://duneanalytics.notion.site/API-Documentation-1b93d16e0fa941398e15047f643e003a).
+service](https://docs.dune.com/api-reference/overview/introduction).
 
 ## Installation
 
 Import as a project dependency
 
 ```shell
 pip install dune-client
```

### Comparing `dune_client-1.7.2/README.md` & `dune_client-1.7.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Build](https://github.com/duneanalytics/dune-client/actions/workflows/pull-request.yaml/badge.svg)](https://github.com/duneanalytics/dune-client/actions/workflows/pull-request.yaml)
 
 # Dune Client
 
 A python framework for interacting with Dune Analytics' [officially supported API
-service](https://duneanalytics.notion.site/API-Documentation-1b93d16e0fa941398e15047f643e003a).
+service](https://docs.dune.com/api-reference/overview/introduction).
 
 ## Installation
 
 Import as a project dependency
 
 ```shell
 pip install dune-client
```

### Comparing `dune_client-1.7.2/dune_client/api/base.py` & `dune_client-1.7.3/dune_client/api/base.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/api/execution.py` & `dune_client-1.7.3/dune_client/api/execution.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/api/extensions.py` & `dune_client-1.7.3/dune_client/api/extensions.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/api/query.py` & `dune_client-1.7.3/dune_client/api/query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/api/table.py` & `dune_client-1.7.3/dune_client/api/table.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/client.py` & `dune_client-1.7.3/dune_client/client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/client_async.py` & `dune_client-1.7.3/dune_client/client_async.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/file/base.py` & `dune_client-1.7.3/dune_client/file/base.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/file/interface.py` & `dune_client-1.7.3/dune_client/file/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/interface.py` & `dune_client-1.7.3/dune_client/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/models.py` & `dune_client-1.7.3/dune_client/models.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/query.py` & `dune_client-1.7.3/dune_client/query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/types.py` & `dune_client-1.7.3/dune_client/types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client/util.py` & `dune_client-1.7.3/dune_client/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Utility methods for package."""
 
 from datetime import datetime, timezone
+import importlib
 from typing import Optional
 
-import pkg_resources
-
 DUNE_DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def postgres_date(date_str: str) -> datetime:
     """Parse a postgres compatible date string into datetime object"""
     return datetime.strptime(date_str, DUNE_DATE_FORMAT)
 
 
 def get_package_version(package_name: str) -> Optional[str]:
     """
-    Returns the package version by `package_name`
+    Returns the package version by `package_name` using the importlib.metadata module
+    which is available in Python 3.8 and later.
     """
     try:
-        return pkg_resources.get_distribution(package_name).version
-    except pkg_resources.DistributionNotFound:
+        return importlib.metadata.version(package_name)
+    except importlib.metadata.PackageNotFoundError:
         return None
 
 
 def age_in_hours(timestamp: datetime) -> float:
     """
     Returns the time (in hours) between now and `timestamp`
     """
```

### Comparing `dune_client-1.7.2/dune_client/viz/graphs.py` & `dune_client-1.7.3/dune_client/viz/graphs.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/dune_client.egg-info/PKG-INFO` & `dune_client-1.7.3/dune_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.7.2
+Version: 1.7.3
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/duneanalytics/dune-client
 Author: Benjamin H. Smith & Dune Analytics
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/duneanalytics/dune-client/issues
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Build](https://github.com/duneanalytics/dune-client/actions/workflows/pull-request.yaml/badge.svg)](https://github.com/duneanalytics/dune-client/actions/workflows/pull-request.yaml)
 
 # Dune Client
 
 A python framework for interacting with Dune Analytics' [officially supported API
-service](https://duneanalytics.notion.site/API-Documentation-1b93d16e0fa941398e15047f643e003a).
+service](https://docs.dune.com/api-reference/overview/introduction).
 
 ## Installation
 
 Import as a project dependency
 
 ```shell
 pip install dune-client
```

### Comparing `dune_client-1.7.2/dune_client.egg-info/SOURCES.txt` & `dune_client-1.7.3/dune_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/setup.cfg` & `dune_client-1.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/e2e/test_async_client.py` & `dune_client-1.7.3/tests/e2e/test_async_client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/e2e/test_client.py` & `dune_client-1.7.3/tests/e2e/test_client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/unit/test_file.py` & `dune_client-1.7.3/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/unit/test_models.py` & `dune_client-1.7.3/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/unit/test_query.py` & `dune_client-1.7.3/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/unit/test_types.py` & `dune_client-1.7.3/tests/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/unit/test_utils.py` & `dune_client-1.7.3/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.7.2/tests/unit/test_viz_sankey.py` & `dune_client-1.7.3/tests/unit/test_viz_sankey.py`

 * *Files identical despite different names*

