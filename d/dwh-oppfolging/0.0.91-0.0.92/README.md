# Comparing `tmp/dwh_oppfolging-0.0.91.tar.gz` & `tmp/dwh_oppfolging-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwh_oppfolging-0.0.91.tar", max compression
+gzip compressed data, was "dwh_oppfolging-0.0.92.tar", max compression
```

## Comparing `dwh_oppfolging-0.0.91.tar` & `dwh_oppfolging-0.0.92.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-04-08 10:48:41.589381 dwh_oppfolging-0.0.91/LICENSE
--rw-r--r--   0        0        0      325 2024-04-08 10:48:41.589381 dwh_oppfolging-0.0.91/README.md
--rw-r--r--   0        0        0       22 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/README.md
--rw-r--r--   0        0        0        0 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/__init__.py
--rw-r--r--   0        0        0       14 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/airflow_api_v1.py
--rw-r--r--   0        0        0     8543 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1.py
--rw-r--r--   0        0        0     4051 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1_types.py
--rw-r--r--   0        0        0    17798 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v2.py
--rw-r--r--   0        0        0     2179 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/dbt_oracle_api_v1.py
--rw-r--r--   0        0        0      422 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/generic_api_v1.py
--rw-r--r--   0        0        0      741 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1.py
--rw-r--r--   0        0        0    24608 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1_types.py
--rw-r--r--   0        0        0    11838 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/oracle_api_v1.py
--rw-r--r--   0        0        0      125 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/oracle_api_v1_types.py
--rw-r--r--   0        0        0     2371 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/secrets_api_v1.py
--rw-r--r--   0        0        0     6831 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1.py
--rw-r--r--   0        0        0    11693 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1_types.py
--rw-r--r--   0        0        0        0 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/__init__.py
--rw-r--r--   0        0        0     9224 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/datatypes.py
--rw-r--r--   0        0        0     9521 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/functions.py
--rw-r--r--   0        0        0     1661 2024-04-08 10:48:41.593381 dwh_oppfolging-0.0.91/pyproject.toml
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.91/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/LICENSE
+-rw-r--r--   0        0        0      325 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/README.md
+-rw-r--r--   0        0        0       22 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/__init__.py
+-rw-r--r--   0        0        0       14 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/airflow_api_v1.py
+-rw-r--r--   0        0        0     8543 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1.py
+-rw-r--r--   0        0        0     4051 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1_types.py
+-rw-r--r--   0        0        0    17798 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v2.py
+-rw-r--r--   0        0        0     2297 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/dbt_oracle_api_v1.py
+-rw-r--r--   0        0        0      422 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/generic_api_v1.py
+-rw-r--r--   0        0        0      741 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1.py
+-rw-r--r--   0        0        0    24608 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1_types.py
+-rw-r--r--   0        0        0    11838 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/oracle_api_v1.py
+-rw-r--r--   0        0        0      125 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/oracle_api_v1_types.py
+-rw-r--r--   0        0        0     2371 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/secrets_api_v1.py
+-rw-r--r--   0        0        0     6831 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1.py
+-rw-r--r--   0        0        0    11693 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1_types.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/__init__.py
+-rw-r--r--   0        0        0     9224 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/datatypes.py
+-rw-r--r--   0        0        0     9521 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/functions.py
+-rw-r--r--   0        0        0     1661 2024-04-23 07:33:40.700167 dwh_oppfolging-0.0.92/pyproject.toml
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.92/PKG-INFO
```

### Comparing `dwh_oppfolging-0.0.91/LICENSE` & `dwh_oppfolging-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v1_types.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/brreg_api_v2.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/brreg_api_v2.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/dbt_oracle_api_v1.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/dbt_oracle_api_v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         "DBT_ENV_SECRET_HOST": creds["host"],
         "DBT_ENV_SECRET_PORT": creds["port"],
         "DBT_ENV_SECRET_SERVICE": creds["service"],
         "DBT_ENV_SECRET_DATABASE": creds["database"],
         "DBT_ENV_SECRET_SCHEMA": schema,
         "ORA_PYTHON_DRIVER_TYPE": "thin",
     }
+    for val in dbt_env_params.values():
+        assert isinstance(val, str), "All dbt env var values must be strings"
     os.environ.update(dbt_env_params)
     yield
     for key in dbt_env_params:
         os.environ.pop(key)
 
 
 def execute_dbt_project(command: str, profiles_dir: str, project_dir: str, *args):
```

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/kafka_api_v1_types.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/kafka_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/oracle_api_v1.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/oracle_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/secrets_api_v1.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/secrets_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/apis/ssb_api_v1_types.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/apis/ssb_api_v1_types.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/datatypes.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/datatypes.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/dwh_oppfolging/transforms/functions.py` & `dwh_oppfolging-0.0.92/dwh_oppfolging/transforms/functions.py`

 * *Files identical despite different names*

### Comparing `dwh_oppfolging-0.0.91/pyproject.toml` & `dwh_oppfolging-0.0.92/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dwh-oppfolging"
-version = "0.0.91"
+version = "0.0.92"
 description = "Oppfolging python package for DWH ETL"
 authors = ["Team Oppfølging"]
 packages = [{include = "dwh_oppfolging"}]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "3.11.*"       # python 3.12 mangler distutils, som ødelegger installasjon av pendulum 2.1.2
                         # derfor låser vi oss til python 3.11
 requests = "2.31.0"
 pendulum = "3.0.0"      # fjernet airflow/dataverk i dev fordi den bruker en eldgammel versjon av pendulum
 ijson = "3.2.3"
-oracledb = "2.1.0"      # versjonen her begrenses av dbt-oracle, så dbt-oracle må oppgraderes først
-dbt-oracle = "1.7.3"    # denne krever cx_Oracle 8.3, som vi ikke klarer å bygge uten gcc
+oracledb = "2.1.2"      # versjonen her begrenses av dbt-oracle, så dbt-oracle må oppgraderes først
+dbt-oracle = "1.7.4"    # denne krever cx_Oracle 8.3, som vi ikke klarer å bygge uten gcc
                         # 3.11-slim har ikke gcc, men 3.11 har det, men den er +700 MB..
 google-cloud-secret-manager = "2.19.0"
 confluent-kafka = "2.3.0"
 fastavro = "1.9.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "24.2.0"
```

### Comparing `dwh_oppfolging-0.0.91/PKG-INFO` & `dwh_oppfolging-0.0.92/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dwh-oppfolging
-Version: 0.0.91
+Version: 0.0.92
 Summary: Oppfolging python package for DWH ETL
 Author: Team Oppfølging
 Requires-Python: ==3.11.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: confluent-kafka (==2.3.0)
-Requires-Dist: dbt-oracle (==1.7.3)
+Requires-Dist: dbt-oracle (==1.7.4)
 Requires-Dist: fastavro (==1.9.4)
 Requires-Dist: google-cloud-secret-manager (==2.19.0)
 Requires-Dist: ijson (==3.2.3)
-Requires-Dist: oracledb (==2.1.0)
+Requires-Dist: oracledb (==2.1.2)
 Requires-Dist: pendulum (==3.0.0)
 Requires-Dist: requests (==2.31.0)
 Description-Content-Type: text/markdown
 
 # dwh-oppfolging
 Public repository for the development of the dwh-oppfolging python package.
```

