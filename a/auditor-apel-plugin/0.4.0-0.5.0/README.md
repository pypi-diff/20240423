# Comparing `tmp/auditor_apel_plugin-0.4.0.tar.gz` & `tmp/auditor_apel_plugin-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auditor_apel_plugin-0.4.0.tar", last modified: Mon Feb  5 14:26:41 2024, max compression
+gzip compressed data, was "auditor_apel_plugin-0.5.0.tar", last modified: Tue Apr 23 14:01:58 2024, max compression
```

## Comparing `auditor_apel_plugin-0.4.0.tar` & `auditor_apel_plugin-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.721397 auditor_apel_plugin-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-05 14:26:41.721397 auditor_apel_plugin-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 14:26:41.721397 auditor_apel_plugin-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.717397 auditor_apel_plugin-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.717397 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/republish.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.721397 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-05 14:26:41.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-05 14:26:41.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 14:26:41.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-05 14:26:41.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-05 14:26:41.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-05 14:26:41.000000 auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:26:41.721397 auditor_apel_plugin-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    42356 2024-02-05 14:26:26.000000 auditor_apel_plugin-0.4.0/tests/test_auditor_apel_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:01:58.276623 auditor_apel_plugin-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-23 14:01:58.276623 auditor_apel_plugin-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:01:58.276623 auditor_apel_plugin-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:01:58.272623 auditor_apel_plugin-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:01:58.272623 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22976 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/republish.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:01:58.272623 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-23 14:01:58.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-23 14:01:58.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:01:58.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 14:01:58.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 14:01:58.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 14:01:58.000000 auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:01:58.272623 auditor_apel_plugin-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40202 2024-04-23 14:01:46.000000 auditor_apel_plugin-0.5.0/tests/test_auditor_apel_plugin.py
```

### Comparing `auditor_apel_plugin-0.4.0/LICENSE` & `auditor_apel_plugin-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auditor_apel_plugin-0.4.0/PKG-INFO` & `auditor_apel_plugin-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: auditor_apel_plugin
-Version: 0.4.0
+Version: 0.5.0
 Summary: AUDITOR plugin for sending accounting data to APEL
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-auditor==0.4.0
+Requires-Dist: python-auditor==0.5.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: cryptography==42.0.2
+Requires-Dist: cryptography==42.0.5
+Requires-Dist: pyyaml==6.0.1
 Provides-Extra: style
 Requires-Dist: black; extra == "style"
 Requires-Dist: flake8; extra == "style"
 Provides-Extra: tests
-Requires-Dist: pytest==8.0.0; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
 Provides-Extra: build
-Requires-Dist: build==1.0.3; extra == "build"
-Requires-Dist: setuptools==69.0.3; extra == "build"
+Requires-Dist: build==1.2.1; extra == "build"
+Requires-Dist: setuptools==69.2.0; extra == "build"
 
 # AUDITOR-APEL-plugin
 
 Plugin for AUDITOR to report job records to APEL
 
 ## License
```

### Comparing `auditor_apel_plugin-0.4.0/pyproject.toml` & `auditor_apel_plugin-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [build-system]
-requires = ["setuptools==69.0.3"]
+requires = ["setuptools==69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "auditor_apel_plugin"
-version = "0.4.0"
+version = "0.5.0"
 requires-python = ">=3.8"
 dependencies = [
-	     "python-auditor==0.4.0",
+	     "python-auditor==0.5.0",
 	     "requests==2.31.0",
-	     "cryptography==42.0.2",
+	     "cryptography==42.0.5",
+	     "pyyaml==6.0.1",
 ]
 description = "AUDITOR plugin for sending accounting data to APEL"
 readme = "README.md"
 
 [project.optional-dependencies]
 style = [
       "black",
       "flake8",
 ]
 tests = [
-      "pytest==8.0.0",
-      "pytest-cov==4.1.0",
+      "pytest==8.1.1",
+      "pytest-cov==5.0.0",
 ]
 build = [
-      "build==1.0.3",
-      "setuptools==69.0.3",
+      "build==1.2.1",
+      "setuptools==69.2.0",
 ]
 
 [project.scripts]
 auditor-apel-publish = "auditor_apel_plugin.publish:main"
 auditor-apel-republish = "auditor_apel_plugin.republish:main"
 
 [tool.setuptools.packages.find]
```

### Comparing `auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/core.py` & `auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 # SPDX-FileCopyrightText: © 2022 Dirk Sammel <dirk.sammel@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause-Patent
 
 import logging
-from pathlib import Path
 import sqlite3
 from sqlite3 import Error
 from datetime import datetime, timedelta, time, timezone
 from time import sleep
 import json
 import sys
 import requests
@@ -16,16 +15,16 @@
 from cryptography import x509
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.serialization import pkcs7
 from pyauditor import Value, Operator, MetaOperator, MetaQuery, QueryBuilder
 
 
 def get_records(config, client, start_time, delay_time, site=None, end_time=None):
-    sites_to_report = json.loads(config["site"].get("sites_to_report"))
-    meta_key_site = config["auditor"].get("meta_key_site")
+    sites_to_report = config["site"]["sites_to_report"]
+    meta_key_site = config["auditor"]["meta_key_site"]
 
     site_ids = []
 
     if site is not None:
         site_ids = sites_to_report[site]
         logging.info(f"Getting records for site {site} with site_ids: {site_ids}")
     else:
@@ -80,152 +79,119 @@
     first_previous_month = previous_month.replace(day=1)
     begin_previous_month = datetime.combine(first_previous_month, time())
     begin_previous_month_utc = begin_previous_month.replace(tzinfo=timezone.utc)
 
     return begin_previous_month_utc
 
 
-def get_time_db(config):
-    time_db_path = config["paths"].get("time_db_path")
-    publish_since = config["site"].get("publish_since")
-
-    if Path(time_db_path).is_file():
-        conn = sqlite3.connect(
-            time_db_path,
-            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
-        )
-    else:
-        conn = create_time_db(publish_since, time_db_path)
+def get_begin_current_month(current_time):
+    first_current_month = current_time.replace(day=1)
+    begin_current_month = datetime.combine(first_current_month, time())
+    begin_current_month_utc = begin_current_month.replace(tzinfo=timezone.utc)
 
-    return conn
+    return begin_current_month_utc
 
 
-def create_time_db(publish_since, time_db_path):
-    create_table_sql = """
-                       CREATE TABLE IF NOT EXISTS times(
-                           last_end_time INTEGER NOT NULL,
-                           last_report_time timestamp NOT NULL
-                       )
-                       """
+def get_time_json(config):
+    time_json_path = config["time_json_path"]
+
+    try:
+        with open(time_json_path, "r", encoding="utf-8") as f:
+            time_dict = json.load(f)
+    except FileNotFoundError:
+        logging.warning(f"Path {time_json_path} not found, creating new time json")
+        time_dict = create_time_json(time_json_path)
+
+    return time_dict
 
-    insert_sql = """
-                 INSERT INTO times(
-                     last_end_time,
-                     last_report_time
-                 )
-                 VALUES(
-                     ?, ?
-                 )
-                 """
 
+def create_time_json(time_json_path):
     initial_report_time = datetime(1970, 1, 1, 0, 0, 0)
-    publish_since_datetime = datetime.strptime(publish_since, "%Y-%m-%d %H:%M:%S%z")
-    data_tuple = (
-        publish_since_datetime.replace(tzinfo=timezone.utc).timestamp(),
-        initial_report_time,
-    )
+    time_dict = {
+        "last_report_time": initial_report_time.isoformat(),
+        "site_end_times": {},
+    }
 
     try:
-        conn = sqlite3.connect(
-            time_db_path,
-            detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
-        )
-        cur = conn.cursor()
-        cur.execute(create_table_sql)
-        cur.execute(insert_sql, data_tuple)
-        conn.commit()
-        cur.close()
-        return conn
-    except Error as e:
-        logging.critical(e)
+        with open(time_json_path, "w", encoding="utf-8") as f:
+            json.dump(time_dict, f)
+    except FileNotFoundError:
+        logging.critical(f"Path {time_json_path} not found, could not create time json")
         raise
 
+    return time_dict
 
-def get_start_time(conn):
+
+def get_start_time(config, time_dict, site):
     try:
-        cur = conn.cursor()
-        cur.row_factory = lambda cursor, row: row[0]
-        cur.execute("SELECT last_end_time FROM times")
-        start_time_row = cur.fetchall()
-        start_time = datetime.fromtimestamp(start_time_row[0], tz=timezone.utc)
-        cur.close()
-        return start_time
-    except Error as e:
-        logging.critical(e)
-        raise
+        start_time = datetime.fromisoformat(time_dict["site_end_times"][site])
+    except KeyError:
+        start_time = config["site"]["publish_since"]
 
+    return start_time
 
-def get_report_time(conn):
-    try:
-        cur = conn.cursor()
-        cur.row_factory = lambda cursor, row: row[0]
-        cur.execute("SELECT last_report_time FROM times")
-        report_time_row = cur.fetchall()
-        report_time = report_time_row[0]
-        cur.close()
-        return report_time
-    except Error as e:
-        logging.critical(e)
-        raise
 
+def get_report_time(time_dict):
+    report_time = datetime.fromisoformat(time_dict["last_report_time"])
+
+    return report_time
+
+
+def update_time_json(config, time_dict, site, stop_time, report_time):
+    time_json_path = config["time_json_path"]
+
+    time_dict["last_report_time"] = report_time.isoformat()
+    time_dict["site_end_times"][site] = stop_time.isoformat()
 
-def update_time_db(conn, stop_time, report_time):
-    update_sql = """
-                 UPDATE times
-                 SET last_end_time = ?,
-                     last_report_time = ?
-                 """
     try:
-        cur = conn.cursor()
-        cur.execute(update_sql, (stop_time, report_time))
-        conn.commit()
-        cur.close()
-    except Error as e:
-        logging.critical(e)
+        with open(time_json_path, "w", encoding="utf-8") as f:
+            json.dump(time_dict, f)
+    except FileNotFoundError:
+        logging.critical(f"Path {time_json_path} not found, could not update time json")
         raise
 
 
 def replace_record_string(string):
     updated_string = urllib.parse.unquote(string)
 
     return updated_string
 
 
 def get_site_id(config, record):
-    meta_key_site = config["auditor"].get("meta_key_site")
+    meta_key_site = config["auditor"]["meta_key_site"]
 
     try:
         site_id = record.meta.get(meta_key_site)[0]
         return site_id
     except AttributeError:
         logging.critical(f"No meta data found in {record.record_id}, aborting")
         raise
     except TypeError:
         logging.critical(f"No site name found in {record.record_id}, aborting")
         raise
 
 
 def get_submit_host(config, record):
-    meta_key_submithost = config["auditor"].get("meta_key_submithost")
-    default_submit_host = config["site"].get("default_submit_host")
+    meta_key_submithost = config["auditor"]["meta_key_submithost"]
+    default_submit_host = config["site"]["default_submit_host"]
 
     try:
         submit_host = replace_record_string(record.meta.get(meta_key_submithost)[0])
     except TypeError:
         logging.warning(
             f"No {meta_key_submithost} found in record {record.record_id}, "
             f"sending default SubmitHost {default_submit_host}"
         )
         submit_host = default_submit_host
 
     return submit_host
 
 
 def get_voms_info(config, record):
-    meta_key_voms = config["auditor"].get("meta_key_voms")
+    meta_key_voms = config["auditor"]["meta_key_voms"]
     voms_dict = {}
 
     try:
         voms_string = replace_record_string(record.meta.get(meta_key_voms)[0])
     except TypeError:
         logging.warning(
             f"No VOMS information found in {record.record_id}, "
@@ -336,22 +302,22 @@
         conn = sqlite3.connect(":memory:")
         cur = conn.cursor()
         cur.execute(create_table_sql)
     except Error as e:
         logging.critical(e)
         raise
 
-    sites_to_report = json.loads(config["site"].get("sites_to_report"))
-    infrastructure = config["site"].get("infrastructure_type")
-    benchmark_type = config["site"].get("benchmark_type")
-    benchmark_name = config["auditor"].get("benchmark_name")
-    cores_name = config["auditor"].get("cores_name")
-    cpu_time_name = config["auditor"].get("cpu_time_name")
-    nnodes_name = config["auditor"].get("nnodes_name")
-    meta_key_username = config["auditor"].get("meta_key_username")
+    sites_to_report = config["site"]["sites_to_report"]
+    infrastructure = config["site"]["infrastructure_type"]
+    benchmark_type = config["site"]["benchmark_type"]
+    benchmark_name = config["auditor"]["benchmark_name"]
+    cores_name = config["auditor"]["cores_name"]
+    cpu_time_name = config["auditor"]["cpu_time_name"]
+    nnodes_name = config["auditor"]["nnodes_name"]
+    meta_key_username = config["auditor"]["meta_key_username"]
 
     for r in records:
         site_id = get_site_id(config, r)
 
         for k, v in sites_to_report.items():
             if site_id in v:
                 site_name = k
@@ -475,15 +441,15 @@
         conn = sqlite3.connect(":memory:")
         cur = conn.cursor()
         cur.execute(create_table_sql)
     except Error as e:
         logging.critical(e)
         raise
 
-    sites_to_report = json.loads(config["site"].get("sites_to_report"))
+    sites_to_report = config["site"]["sites_to_report"]
 
     for r in records:
         site_id = get_site_id(config, r)
 
         for k, v in sites_to_report.items():
             if site_id in v:
                 site_name = k
@@ -653,32 +619,32 @@
         sync += f"NumberOfJobs: {entry['jobcount']}\n"
         sync += "%%\n"
 
     return sync
 
 
 def get_token(config):
-    auth_url = config["authentication"].get("auth_url")
-    client_cert = config["authentication"].get("client_cert")
-    client_key = config["authentication"].get("client_key")
-    verify_ca = config["authentication"].getboolean("verify_ca")
+    auth_url = config["authentication"]["auth_url"]
+    client_cert = config["authentication"]["client_cert"]
+    client_key = config["authentication"]["client_key"]
+    verify_ca = config["authentication"]["verify_ca"]
     if verify_ca:
-        ca_path = config["authentication"].get("ca_path")
+        ca_path = config["authentication"]["ca_path"]
     else:
         ca_path = False
 
     response = requests.get(auth_url, cert=(client_cert, client_key), verify=ca_path)
     token = response.json()["token"]
 
     return token
 
 
 def sign_msg(config, msg):
-    client_cert = config["authentication"].get("client_cert")
-    client_key = config["authentication"].get("client_key")
+    client_cert = config["authentication"]["client_cert"]
+    client_key = config["authentication"]["client_key"]
 
     with open(client_cert, "rb") as cc:
         cert = x509.load_pem_x509_certificate(cc.read())
 
     with open(client_key, "rb") as ck:
         key = serialization.load_pem_private_key(ck.read(), None)
 
@@ -691,28 +657,28 @@
         .sign(serialization.Encoding.SMIME, options)
     )
 
     return signed_msg
 
 
 def build_payload(msg):
-    current_time = datetime.utcnow().strftime("%Y%m%d%H%M%S")
+    current_time = datetime.now(timezone.utc).strftime("%Y%m%d%H%M%S")
     empaid = f"{current_time[:8]}/{current_time}"
 
     payload = {"messages": [{"attributes": {"empaid": empaid}, "data": msg}]}
 
     return payload
 
 
 def send_payload(config, token, payload):
-    ams_url = config["authentication"].get("ams_url")
-    verify_ca = config["authentication"].getboolean("verify_ca")
+    ams_url = config["authentication"]["ams_url"]
+    verify_ca = config["authentication"]["verify_ca"]
 
     if verify_ca:
-        ca_path = config["authentication"].get("ca_path")
+        ca_path = config["authentication"]["ca_path"]
     else:
         ca_path = False
 
     logging.debug(f"{ams_url}{token}")
     post = requests.post(
         f"{ams_url}{token}",
         json=payload,
@@ -720,31 +686,31 @@
         verify=ca_path,
     )
 
     return post
 
 
 def convert_to_seconds(config, cpu_time):
-    cpu_time_name = config["auditor"].get("cpu_time_name")
-    cpu_time_unit = config["auditor"].get("cpu_time_unit")
+    cpu_time_name = config["auditor"]["cpu_time_name"]
+    cpu_time_unit = config["auditor"]["cpu_time_unit"]
 
     if cpu_time_unit == "seconds":
         return cpu_time
     elif cpu_time_unit == "milliseconds":
         return round(cpu_time / 1000)
     else:
         logging.critical(
             f"Unknown unit for {cpu_time_name}: {cpu_time_unit}. "
             "Possible values are seconds or milliseconds."
         )
         raise ValueError
 
 
 def check_sites_in_records(config, records):
-    sites_to_report = json.loads(config["site"].get("sites_to_report"))
+    sites_to_report = config["site"]["sites_to_report"]
 
     logging.debug(f"Sites to report from config: {list(sites_to_report.keys())}")
 
     sites_in_records = {get_site_id(config, r) for r in records}
     sites = []
 
     for site_id in sites_in_records:
```

### Comparing `auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/publish.py` & `auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/publish.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,142 +2,141 @@
 
 # SPDX-FileCopyrightText: © 2022 Dirk Sammel <dirk.sammel@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause-Patent
 
 import logging
 from pyauditor import AuditorClientBuilder
 from datetime import datetime, timedelta, timezone
-import configparser
+import yaml
 import argparse
 import base64
 from time import sleep
 from auditor_apel_plugin.core import (
     get_token,
-    get_time_db,
+    get_time_json,
     get_report_time,
-    get_start_time,
+    # get_start_time,
     create_summary_db,
     group_summary_db,
     create_summary,
     sign_msg,
     build_payload,
     send_payload,
-    update_time_db,
+    update_time_json,
     get_begin_previous_month,
+    get_begin_current_month,
     create_sync_db,
     group_sync_db,
     create_sync,
     get_records,
-    check_sites_in_records,
 )
 
 
 def run(config, client):
-    report_interval = config["intervals"].getint("report_interval")
+    report_interval = config["report_interval"]
+    sites_to_report = config["site"]["sites_to_report"]
+
     token = get_token(config)
     logging.debug(token)
 
     while True:
-        time_db_conn = get_time_db(config)
-        last_report_time = get_report_time(time_db_conn)
+        time_dict = get_time_json(config)
+        last_report_time = get_report_time(time_dict)
         current_time = datetime.now()
         time_since_report = (current_time - last_report_time).total_seconds()
 
         if time_since_report < report_interval:
             logging.info("Not enough time since last report")
-            time_db_conn.close()
             sleep(report_interval - time_since_report)
             continue
         else:
             logging.info("Enough time since last report, create new report")
 
-        start_time = get_start_time(time_db_conn)
-        logging.info(f"Getting records since {start_time}")
-
-        records_summary = get_records(config, client, start_time, 30)
-
-        if len(records_summary) == 0:
-            logging.info("No new records, do nothing for now")
-            time_db_conn.close()
-            logging.info(
-                "Next report scheduled for "
-                f"{datetime.now() + timedelta(seconds=report_interval)}"
-            )
-            sleep(report_interval)
-            continue
-
-        sites_to_report = check_sites_in_records(config, records_summary)
-        logging.info(f"Create reports for {sites_to_report}")
+        if current_time.day < last_report_time.day:
+            begin_month = get_begin_previous_month(current_time)
+        else:
+            begin_month = get_begin_current_month(current_time)
 
-        latest_stop_time = records_summary[-1].stop_time.replace(tzinfo=timezone.utc)
+        for site in sites_to_report.keys():
+            logging.info(f"Getting records for {site}")
 
-        logging.debug(f"Latest stop time is {latest_stop_time}")
-        summary_db = create_summary_db(config, records_summary)
-        grouped_summary_list = group_summary_db(summary_db)
-        summary = create_summary(config, grouped_summary_list)
-        logging.debug(summary)
-        signed_summary = sign_msg(config, summary)
-        logging.debug(signed_summary)
-        encoded_summary = base64.b64encode(signed_summary).decode("utf-8")
-        logging.debug(encoded_summary)
-        payload_summary = build_payload(encoded_summary)
-        logging.debug(payload_summary)
-        post_summary = send_payload(config, token, payload_summary)
-        logging.debug(post_summary.status_code)
-
-        begin_previous_month = get_begin_previous_month(current_time)
-        records_sync = get_records(config, client, begin_previous_month, 30)
-        sync_db = create_sync_db(config, records_sync)
-        grouped_sync_list = group_sync_db(sync_db)
-        sync = create_sync(grouped_sync_list)
-        logging.debug(sync)
-        signed_sync = sign_msg(config, sync)
-        logging.debug(signed_sync)
-        encoded_sync = base64.b64encode(signed_sync).decode("utf-8")
-        logging.debug(encoded_sync)
-        payload_sync = build_payload(encoded_sync)
-        logging.debug(payload_sync)
-        post_sync = send_payload(config, token, payload_sync)
-        logging.debug(post_sync.status_code)
+            # start_time = get_start_time(config, time_dict, site)
+            # logging.info(f"Getting records since {start_time}")
 
-        latest_report_time = datetime.now()
-        update_time_db(time_db_conn, latest_stop_time.timestamp(), latest_report_time)
+            records = get_records(config, client, begin_month, 30, site=site)
+
+            if len(records) == 0:
+                logging.info(f"No new records for {site}")
+                continue
+
+            latest_stop_time = records[-1].stop_time.replace(tzinfo=timezone.utc)
+            logging.debug(f"Latest stop time is {latest_stop_time}")
+
+            summary_db = create_summary_db(config, records)
+            grouped_summary_list = group_summary_db(summary_db)
+            summary = create_summary(config, grouped_summary_list)
+            logging.debug(summary)
+            signed_summary = sign_msg(config, summary)
+            logging.debug(signed_summary)
+            encoded_summary = base64.b64encode(signed_summary).decode("utf-8")
+            logging.debug(encoded_summary)
+            payload_summary = build_payload(encoded_summary)
+            logging.debug(payload_summary)
+            post_summary = send_payload(config, token, payload_summary)
+            logging.debug(post_summary.status_code)
+
+            sync_db = create_sync_db(config, records)
+            grouped_sync_list = group_sync_db(sync_db)
+            sync = create_sync(grouped_sync_list)
+            logging.debug(sync)
+            signed_sync = sign_msg(config, sync)
+            logging.debug(signed_sync)
+            encoded_sync = base64.b64encode(signed_sync).decode("utf-8")
+            logging.debug(encoded_sync)
+            payload_sync = build_payload(encoded_sync)
+            logging.debug(payload_sync)
+            post_sync = send_payload(config, token, payload_sync)
+            logging.debug(post_sync.status_code)
+
+            latest_report_time = datetime.now()
+            update_time_json(
+                config, time_dict, site, latest_stop_time, latest_report_time
+            )
 
-        time_db_conn.close()
         logging.info(
             "Next report scheduled for "
             f"{datetime.now() + timedelta(seconds=report_interval)}"
         )
         sleep(report_interval)
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-c", "--config", required=True, help="Path to the config file")
     args = parser.parse_args()
 
-    config = configparser.ConfigParser()
-    config.read(args.config)
+    with open(args.config) as f:
+        config = yaml.safe_load(f)
 
-    log_level = config["logging"].get("log_level")
+    log_level = config["log_level"]
     log_format = (
         "[%(asctime)s] %(levelname)-8s %(message)s (%(pathname)s at line %(lineno)d)"
     )
     logging.basicConfig(
         # filename="apel_plugin.log",
         level=log_level,
         format=log_format,
         datefmt="%Y-%m-%d %H:%M:%S",
     )
     logging.getLogger("aiosqlite").setLevel("WARNING")
     logging.getLogger("urllib3").setLevel("WARNING")
 
-    auditor_ip = config["auditor"].get("auditor_ip")
-    auditor_port = config["auditor"].getint("auditor_port")
-    auditor_timeout = config["auditor"].getint("auditor_timeout")
+    auditor_ip = config["auditor"]["auditor_ip"]
+    auditor_port = config["auditor"]["auditor_port"]
+    auditor_timeout = config["auditor"]["auditor_timeout"]
 
     builder = AuditorClientBuilder()
     builder = builder.address(auditor_ip, auditor_port).timeout(auditor_timeout)
     client = builder.build_blocking()
 
     try:
         run(config, client)
```

### Comparing `auditor_apel_plugin-0.4.0/src/auditor_apel_plugin/republish.py` & `auditor_apel_plugin-0.5.0/src/auditor_apel_plugin/republish.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 
 # SPDX-FileCopyrightText: © 2022 Dirk Sammel <dirk.sammel@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause-Patent
 
 import logging
 from pyauditor import AuditorClientBuilder
-import configparser
 import argparse
 from datetime import datetime, timezone
+import yaml
 import base64
 import sys
 from auditor_apel_plugin.core import (
     get_token,
     create_summary_db,
     group_summary_db,
     create_summary,
@@ -23,19 +23,19 @@
 
 
 def run(config, client, args):
     month = args.month
     year = args.year
     site = args.site
 
-    begin_month = datetime(year, month, 1).replace(tzinfo=timezone.utc)
+    begin_month = datetime(year, month, 1, tzinfo=timezone.utc)
     if month == 12:
-        end_month = datetime(year + 1, 1, 1).replace(tzinfo=timezone.utc)
+        end_month = datetime(year + 1, 1, 1, tzinfo=timezone.utc)
     else:
-        end_month = datetime(year, month + 1, 1).replace(tzinfo=timezone.utc)
+        end_month = datetime(year, month + 1, 1, tzinfo=timezone.utc)
 
     records = get_records(config, client, begin_month, 30, site, end_month)
 
     if len(records) == 0:
         logging.critical("No records found!")
         sys.exit(1)
 
@@ -66,30 +66,30 @@
     )
     parser.add_argument(
         "-s", "--site", required=True, help="Site (GOCDB): UNI-FREIBURG, ..."
     )
     parser.add_argument("-c", "--config", required=True, help="Path to the config file")
     args = parser.parse_args()
 
-    config = configparser.ConfigParser()
-    config.read(args.config)
+    with open(args.config) as f:
+        config = yaml.safe_load(f)
 
-    log_level = config["logging"].get("log_level")
+    log_level = config["log_level"]
     log_format = "[%(asctime)s] %(levelname)-8s %(message)s"
     logging.basicConfig(
         level=log_level,
         format=log_format,
         datefmt="%Y-%m-%d %H:%M:%S",
     )
     logging.getLogger("aiosqlite").setLevel("WARNING")
     logging.getLogger("urllib3").setLevel("WARNING")
 
-    auditor_ip = config["auditor"].get("auditor_ip")
-    auditor_port = config["auditor"].getint("auditor_port")
-    auditor_timeout = config["auditor"].getint("auditor_timeout")
+    auditor_ip = config["auditor"]["auditor_ip"]
+    auditor_port = config["auditor"]["auditor_port"]
+    auditor_timeout = config["auditor"]["auditor_timeout"]
 
     builder = AuditorClientBuilder()
     builder = builder.address(auditor_ip, auditor_port).timeout(auditor_timeout)
     client = builder.build_blocking()
 
     try:
         run(config, client, args)
```

### Comparing `auditor_apel_plugin-0.4.0/src/auditor_apel_plugin.egg-info/PKG-INFO` & `auditor_apel_plugin-0.5.0/src/auditor_apel_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: auditor_apel_plugin
-Version: 0.4.0
+Version: 0.5.0
 Summary: AUDITOR plugin for sending accounting data to APEL
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python-auditor==0.4.0
+Requires-Dist: python-auditor==0.5.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: cryptography==42.0.2
+Requires-Dist: cryptography==42.0.5
+Requires-Dist: pyyaml==6.0.1
 Provides-Extra: style
 Requires-Dist: black; extra == "style"
 Requires-Dist: flake8; extra == "style"
 Provides-Extra: tests
-Requires-Dist: pytest==8.0.0; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
 Provides-Extra: build
-Requires-Dist: build==1.0.3; extra == "build"
-Requires-Dist: setuptools==69.0.3; extra == "build"
+Requires-Dist: build==1.2.1; extra == "build"
+Requires-Dist: setuptools==69.2.0; extra == "build"
 
 # AUDITOR-APEL-plugin
 
 Plugin for AUDITOR to report job records to APEL
 
 ## License
```

### Comparing `auditor_apel_plugin-0.4.0/tests/test_auditor_apel_plugin.py` & `auditor_apel_plugin-0.5.0/tests/test_auditor_apel_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import pytest
 from auditor_apel_plugin.core import (
     get_begin_previous_month,
-    create_time_db,
-    get_time_db,
+    get_begin_current_month,
+    create_time_json,
+    get_time_json,
     sign_msg,
     get_start_time,
     get_report_time,
-    update_time_db,
+    update_time_json,
     create_summary_db,
     get_submit_host,
     get_voms_info,
     replace_record_string,
     get_records,
     get_site_id,
     convert_to_seconds,
     check_sites_in_records,
 )
 from datetime import datetime, timezone
-import sqlite3
 import os
+import json
 import subprocess
-import configparser
 import pyauditor
 from unittest.mock import patch, PropertyMock
-import ast
 from pathlib import Path, PurePath
 
 test_dir = PurePath(__file__).parent
 
 
 class FakeAuditorClient:
     def __init__(self, test_case=""):
@@ -92,92 +91,68 @@
 
         result = get_begin_previous_month(time_a)
         assert result == datetime(2022, 9, 1, 00, 00, 00, tzinfo=timezone.utc)
 
         result = get_begin_previous_month(time_b)
         assert result == datetime(1969, 12, 1, 00, 00, 00, tzinfo=timezone.utc)
 
-    def test_create_time_db(self):
-        path = ":memory:"
-        publish_since_list = [
-            "1970-01-01 00:00:00+00:00",
-            "2020-01-01 17:23:00+00:00",
-            "2022-12-17 20:20:20+01:00",
-        ]
+    def test_get_begin_current_month(self):
+        time_a = datetime(2022, 10, 23, 12, 23, 55)
+        time_b = datetime(1970, 1, 1, 00, 00, 00)
 
-        for publish_since in publish_since_list:
-            time_db = create_time_db(publish_since, path)
-            cur = time_db.cursor()
-            cur.execute("SELECT * FROM times")
-            result = cur.fetchall()
-            cur.close()
-            time_db.close()
-            time_dt = datetime.strptime(publish_since, "%Y-%m-%d %H:%M:%S%z")
-            time_stamp = time_dt.replace(tzinfo=timezone.utc).timestamp()
+        result = get_begin_current_month(time_a)
+        assert result == datetime(2022, 10, 1, 00, 00, 00, tzinfo=timezone.utc)
 
-            assert result == [(time_stamp, datetime(1970, 1, 1, 0, 0, 0))]
+        result = get_begin_current_month(time_b)
+        assert result == datetime(1970, 1, 1, 00, 00, 00, tzinfo=timezone.utc)
 
-    def test_create_time_db_fail(self):
-        path = "/home/nonexistent/55/abc/time.db"
-        publish_since = "1970-01-01 00:00:00+00:00"
+    def test_create_time_json(self):
+        path = "/tmp/test.json"
 
-        with pytest.raises(Exception) as pytest_error:
-            create_time_db(publish_since, path)
-        assert pytest_error.type == sqlite3.OperationalError
+        result = create_time_json(path)
 
-        publish_since = "1970-01-01"
+        assert result["site_end_times"] == {}
+        assert result["last_report_time"] == "1970-01-01T00:00:00"
+
+        with open("/tmp/test.json", "r", encoding="utf-8") as f:
+            result = json.load(f)
+
+        os.remove(path)
+
+        assert result["site_end_times"] == {}
+        assert result["last_report_time"] == "1970-01-01T00:00:00"
+
+    def test_create_time_json_fail(self):
+        path = "/home/nonexistent/55/abc/time.db"
 
         with pytest.raises(Exception) as pytest_error:
-            create_time_db(publish_since, path)
-        assert pytest_error.type == ValueError
+            create_time_json(path)
+
+        assert pytest_error.type == FileNotFoundError
 
-    def test_get_time_db(self):
+    def test_get_time_json(self):
         path = "/tmp/nonexistent_55_abc_time.db"
-        publish_since_list = [
-            "1970-01-01 00:00:00+00:00",
-            "2020-01-01 17:23:00+00:00",
-            "2022-12-17 20:20:20+01:00",
-        ]
 
-        conf = configparser.ConfigParser()
-        conf["paths"] = {"time_db_path": path}
-        conf["site"] = {}
+        conf = {"time_json_path": path}
 
-        for publish_since in publish_since_list:
-            conf["site"]["publish_since"] = publish_since
-            time_db = get_time_db(conf)
-            cur = time_db.cursor()
-            cur.execute("SELECT * FROM times")
-            result = cur.fetchall()
-            cur.close()
-            time_db.close()
-            time_dt = datetime.strptime(publish_since, "%Y-%m-%d %H:%M:%S%z")
-            time_stamp = time_dt.replace(tzinfo=timezone.utc).timestamp()
-            os.remove(path)
+        result = get_time_json(conf)
+        os.remove(path)
 
-            assert result == [(time_stamp, datetime(1970, 1, 1, 0, 0, 0))]
+        assert result["site_end_times"] == {}
+        assert result["last_report_time"] == "1970-01-01T00:00:00"
 
-        for publish_since in publish_since_list:
-            conf["site"]["publish_since"] = publish_since
-            time_db = create_time_db(publish_since, path)
-            time_db.close()
-            time_db = get_time_db(conf)
-            cur = time_db.cursor()
-            cur.execute("SELECT * FROM times")
-            result = cur.fetchall()
-            cur.close()
-            time_db.close()
-            time_dt = datetime.strptime(publish_since, "%Y-%m-%d %H:%M:%S%z")
-            time_stamp = time_dt.replace(tzinfo=timezone.utc).timestamp()
-            os.remove(path)
+        create_time_json(path)
+        result = get_time_json(conf)
+        os.remove(path)
 
-            assert result == [(time_stamp, datetime(1970, 1, 1, 0, 0, 0))]
+        assert result["site_end_times"] == {}
+        assert result["last_report_time"] == "1970-01-01T00:00:00"
 
     def test_sign_msg(self):
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["authentication"] = {
             "client_cert": Path.joinpath(test_dir, "test_cert.cert"),
             "client_key": Path.joinpath(test_dir, "test_key.key"),
         }
 
         result = sign_msg(conf, "test")
 
@@ -189,15 +164,15 @@
             bashCommand.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         process.communicate()
 
         assert process.returncode == 0
 
     def test_sign_msg_fail(self):
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["authentication"] = {
             "client_cert": "tests/nodir/test_cert.cert",
             "client_key": "tests/no/dir/test_key.key",
         }
 
         with pytest.raises(Exception) as pytest_error:
             sign_msg(conf, "test")
@@ -221,163 +196,162 @@
             bashCommand.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         process.communicate()
 
         assert process.returncode == 4
 
     def test_get_start_time(self):
-        path = ":memory:"
+        path = "/tmp/test.json"
+
+        conf = {}
+        conf["site"] = {}
+        conf["time_json_path"] = path
+
         publish_since_list = [
             "1970-01-01 00:00:00+00:00",
             "2020-01-01 17:23:00+00:00",
-            "2022-12-17 20:20:20+01:00",
         ]
 
+        time_dict = create_time_json(path)
+
         for publish_since in publish_since_list:
-            time_db = create_time_db(publish_since, path)
-            result = get_start_time(time_db)
-            time_db.close()
-            time_dt = datetime.strptime(publish_since, "%Y-%m-%d %H:%M:%S%z")
-            time_dt_utc = time_dt.replace(tzinfo=timezone.utc)
-
-            assert result == time_dt_utc
-
-    def test_get_start_time_fail(self):
-        path = ":memory:"
-        publish_since = "1970-01-01 00:00:00+00:00"
-
-        time_db = create_time_db(publish_since, path)
-        drop_column = "ALTER TABLE times DROP last_end_time"
-
-        cur = time_db.cursor()
-        cur.execute(drop_column)
-        time_db.commit()
-        cur.close()
-        with pytest.raises(Exception) as pytest_error:
-            get_start_time(time_db)
-        time_db.close()
+            conf["site"]["publish_since"] = datetime.fromisoformat(publish_since)
+            result = get_start_time(conf, time_dict, "TEST")
+            time_dt = datetime.fromisoformat(publish_since)
+
+            assert result == time_dt
+
+        stop_time = datetime(1984, 3, 3, 0, 0, 0, tzinfo=timezone.utc)
+        update_time_json(
+            conf,
+            time_dict,
+            "TEST",
+            stop_time,
+            datetime(1970, 1, 1, 0, 0, 0),
+        )
+        result = get_start_time(conf, time_dict, "TEST")
+
+        assert result == stop_time
+
+        stop_time = datetime(2002, 12, 3, 0, 45, 0, tzinfo=timezone.utc)
+        update_time_json(
+            conf,
+            time_dict,
+            "TEST-2",
+            stop_time,
+            datetime(1970, 1, 1, 0, 0, 0),
+        )
+        result = get_start_time(conf, time_dict, "TEST-2")
+
+        os.remove(path)
 
-        assert pytest_error.type == sqlite3.OperationalError
+        assert result == stop_time
 
     def test_get_report_time(self):
-        path = ":memory:"
-        publish_since = "1970-01-01 00:00:00+00:00"
+        path = "/tmp/test.json"
 
-        time_db = create_time_db(publish_since, path)
-        result = get_report_time(time_db)
-        time_db.close()
+        conf = {"time_json_path": path}
+
+        time_dict = create_time_json(path)
+
+        result = get_report_time(time_dict)
 
         initial_report_time = datetime(1970, 1, 1, 0, 0, 0)
 
         assert result == initial_report_time
 
-    def test_get_report_time_fail(self):
-        path = ":memory:"
-        publish_since = "1970-01-01 00:00:00+00:00"
-
-        time_db = create_time_db(publish_since, path)
-        drop_column = "ALTER TABLE times DROP last_report_time"
-
-        cur = time_db.cursor()
-        cur.execute(drop_column)
-        time_db.commit()
-        cur.close()
-        with pytest.raises(Exception) as pytest_error:
-            get_report_time(time_db)
-        time_db.close()
+        new_report_time = datetime(2023, 2, 10, 11, 13, 45)
+        stop_time = datetime(2002, 12, 3, 0, 45, 0, tzinfo=timezone.utc)
 
-        assert pytest_error.type == sqlite3.OperationalError
+        update_time_json(
+            conf,
+            time_dict,
+            "TEST-2",
+            stop_time,
+            new_report_time,
+        )
 
-    def test_update_time_db(self):
-        path = ":memory:"
-        publish_since = "1970-01-01 00:00:00+00:00"
-
-        time_db = create_time_db(publish_since, path)
-        cur = time_db.cursor()
-        cur.row_factory = lambda cursor, row: row[0]
+        result = get_report_time(time_dict)
+        os.remove(path)
+        assert result == new_report_time
+
+    def test_update_time_json(self):
+        path = "/tmp/test.json"
+
+        conf = {"time_json_path": path}
+
+        time_dict = create_time_json(path)
 
         stop_time_list = [
             datetime(1984, 3, 3, 0, 0, 0),
             datetime(2022, 12, 23, 12, 44, 23),
             datetime(1999, 10, 1, 23, 17, 45),
         ]
         report_time_list = [
             datetime(1993, 4, 4, 0, 0, 0),
             datetime(2100, 8, 19, 14, 16, 11),
             datetime(1887, 2, 27, 0, 11, 31),
         ]
+        site_list = ["SITE_A", "SITE_B"]
 
         for stop_time in stop_time_list:
             for report_time in report_time_list:
-                update_time_db(time_db, stop_time, report_time)
-
-                cur.execute("SELECT last_end_time FROM times")
-                last_end_time_row = cur.fetchall()
-                last_end_time = last_end_time_row[0]
+                for site in site_list:
+                    update_time_json(conf, time_dict, site, stop_time, report_time)
 
-                assert last_end_time == stop_time.strftime("%Y-%m-%d %H:%M:%S")
+                    with open(path, "r", encoding="utf-8") as f:
+                        time_dict_test = json.load(f)
+                        last_end_time = time_dict_test["site_end_times"][site]
+                        last_report_time = time_dict_test["last_report_time"]
 
-                cur.execute("SELECT last_report_time FROM times")
-                last_report_time_row = cur.fetchall()
-                last_report_time = last_report_time_row[0]
+                    assert last_end_time == stop_time.isoformat()
+                    assert last_report_time == report_time.isoformat()
 
-                assert last_report_time == report_time
-
-                update_time_db(time_db, stop_time.timestamp(), report_time)
-
-                cur.execute("SELECT last_end_time FROM times")
-                last_end_time_row = cur.fetchall()
-                last_end_time = last_end_time_row[0]
-
-                assert last_end_time == stop_time.timestamp()
-
-        cur.close()
-        time_db.close()
+        os.remove(path)
 
     def test_update_time_db_fail(self):
-        path = ":memory:"
-        publish_since = "1970-01-01 00:00:00+00:00"
+        path = "/tmp/test.json"
 
-        time_db = create_time_db(publish_since, path)
-        cur = time_db.cursor()
-        cur.row_factory = lambda cursor, row: row[0]
+        conf = {"time_json_path": path}
+
+        time_dict = create_time_json(path)
 
         stop_time = datetime(1984, 3, 3, 0, 0, 0)
-        report_time = datetime(2032, 11, 5, 12, 12, 15)
+        report_time = datetime(1993, 4, 4, 0, 0, 0)
+        site = "SITE_A"
 
-        drop_column = "ALTER TABLE times DROP last_report_time"
-        cur.execute(drop_column)
-        time_db.commit()
+        os.remove(path)
 
-        with pytest.raises(Exception) as pytest_error:
-            update_time_db(time_db, stop_time, report_time)
+        path_new = "/dfghdfh/test.json"
+        conf["time_json_path"] = path_new
 
-        assert pytest_error.type == sqlite3.OperationalError
+        with pytest.raises(Exception) as pytest_error:
+            update_time_json(conf, time_dict, site, stop_time, report_time)
 
-        cur.close()
-        time_db.close()
+        assert pytest_error.type == FileNotFoundError
 
     def test_create_summary_db(self):
-        sites_to_report = (
-            '{"TEST_SITE_1": ["test-site-1"], "TEST_SITE_2": ["test-site-2"]}'
-        )
+        sites_to_report = {
+            "TEST_SITE_1": ["test-site-1"],
+            "TEST_SITE_2": ["test-site-2"],
+        }
         default_submit_host = "https://default.submit_host.de:1234/xxx"
         infrastructure_type = "grid"
         benchmark_name = "hepscore"
         cores_name = "Cores"
         cpu_time_name = "TotalCPU"
         cpu_time_unit = "seconds"
         nnodes_name = "NNodes"
         meta_key_site = "site_id"
         meta_key_submithost = "headnode"
         meta_key_voms = "voms"
         meta_key_username = "subject"
         benchmark_type = "hepscore23"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "sites_to_report": sites_to_report,
             "default_submit_host": default_submit_host,
             "infrastructure_type": infrastructure_type,
             "benchmark_type": benchmark_type,
         }
         conf["auditor"] = {
@@ -441,17 +415,15 @@
         cur.execute("SELECT * FROM records")
         content = cur.fetchall()
 
         cur.close()
         result.close()
 
         for idx, rec_values in enumerate(rec_value_list):
-            assert (
-                content[idx][0] == list(ast.literal_eval(sites_to_report).keys())[idx]
-            )
+            assert content[idx][0] == list(sites_to_report.keys())[idx]
             assert content[idx][1] == replace_record_string(rec_values["submit_host"])
             assert (
                 content[idx][2]
                 == replace_record_string(rec_values["voms"]).split("/")[1]
             )
             assert content[idx][3] == replace_record_string(rec_values["voms"])
             assert content[idx][4] is None
@@ -496,31 +468,32 @@
 
         assert content[0][17] is None
 
         cur.close()
         result.close()
 
     def test_create_summary_db_fail(self):
-        sites_to_report = (
-            '{"TEST_SITE_1": ["test-site-1"], "TEST_SITE_2": ["test-site-2"]}'
-        )
+        sites_to_report = {
+            "TEST_SITE_1": ["test-site-1"],
+            "TEST_SITE_2": ["test-site-2"],
+        }
         default_submit_host = "https://default.submit_host.de:1234/xxx"
         infrastructure_type = "grid"
         benchmark_name = "hepscore"
         cores_name = "Cores"
         cpu_time_name = "TotalCPU"
         cpu_time_unit = "seconds"
         nnodes_name = "NNodes"
         meta_key_site = "site_id"
         meta_key_submithost = "headnode"
         meta_key_voms = "voms"
         meta_key_username = "subject"
         benchmark_type = "hepscore23"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "sites_to_report": sites_to_report,
             "default_submit_host": default_submit_host,
             "infrastructure_type": infrastructure_type,
             "benchmark_type": benchmark_type,
         }
         conf["auditor"] = {
@@ -612,15 +585,15 @@
         cpu_time_name = "TotalCPU"
         nnodes_name = "NNodes"
         meta_key_site = "site_id"
         meta_key_submithost = "headnode"
         meta_key_voms = "voms"
         meta_key_username = "subject"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "default_submit_host": default_submit_host,
         }
         conf["auditor"] = {
             "benchmark_name": benchmark_name,
             "cores_name": cores_name,
             "cpu_time_name": cpu_time_name,
@@ -704,15 +677,15 @@
         cpu_time_name = "TotalCPU"
         nnodes_name = "NNodes"
         meta_key_site = "site_id"
         meta_key_submithost = "headnode"
         meta_key_voms = "voms"
         meta_key_username = "subject"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "default_submit_host": default_submit_host,
         }
         conf["auditor"] = {
             "benchmark_name": benchmark_name,
             "cores_name": cores_name,
             "cpu_time_name": cpu_time_name,
@@ -875,49 +848,45 @@
 
         result = replace_record_string(test_str_3)
         assert result == "El Niño"
 
     def test_get_records(self):
         client = FakeAuditorClient("pass")
 
-        sites_to_report = '{"TEST_SITE_1": ["test-site-1"]}'
+        sites_to_report = {"TEST_SITE_1": ["test-site-1"]}
         meta_key_site = "site_id"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "sites_to_report": sites_to_report,
         }
         conf["auditor"] = {
             "meta_key_site": meta_key_site,
         }
 
         start_time_str = "2022-12-17 20:20:20+01:00"
-        start_time = datetime.strptime(start_time_str, "%Y-%m-%d %H:%M:%S%z").replace(
-            tzinfo=timezone.utc
-        )
+        start_time = datetime.fromisoformat(start_time_str).replace(tzinfo=timezone.utc)
 
         result = get_records(conf, client, start_time, 1)
         assert "".join(result) == "good"
 
     def test_get_records_fail(self):
-        sites_to_report = '{"TEST_SITE_1": ["test-site-1"]}'
+        sites_to_report = {"TEST_SITE_1": ["test-site-1"]}
         meta_key_site = "site_id"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "sites_to_report": sites_to_report,
         }
         conf["auditor"] = {
             "meta_key_site": meta_key_site,
         }
 
         start_time_str = "2022-12-17 20:20:20+01:00"
-        start_time = datetime.strptime(start_time_str, "%Y-%m-%d %H:%M:%S%z").replace(
-            tzinfo=timezone.utc
-        )
+        start_time = datetime.fromisoformat(start_time_str).replace(tzinfo=timezone.utc)
 
         client = FakeAuditorClient("fail_timeout")
 
         with pytest.raises(SystemExit) as pytest_error:
             get_records(conf, client, start_time, 1)
         assert pytest_error.type == SystemExit
 
@@ -938,15 +907,15 @@
         cpu_time_name = "TotalCPU"
         nnodes_name = "NNodes"
         meta_key_site = "site_id"
         meta_key_submithost = "headnode"
         meta_key_voms = "voms"
         meta_key_username = "subject"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "sites_to_report": sites_to_report,
             "default_submit_host": default_submit_host,
             "infrastructure_type": infrastructure_type,
         }
         conf["auditor"] = {
             "benchmark_name": benchmark_name,
@@ -1007,15 +976,15 @@
         cpu_time_name = "TotalCPU"
         nnodes_name = "NNodes"
         meta_key_site = "site_id"
         meta_key_submithost = "headnode"
         meta_key_voms = "voms"
         meta_key_username = "subject"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "sites_to_report": sites_to_report,
             "default_submit_host": default_submit_host,
             "infrastructure_type": infrastructure_type,
         }
         conf["auditor"] = {
             "benchmark_name": benchmark_name,
@@ -1067,15 +1036,15 @@
             get_site_id(conf, rec_2)
         assert pytest_error.type == AttributeError
 
     def test_convert_to_seconds(self):
         cpu_time_name = "TotalCPU"
         cpu_time_unit = "seconds"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["auditor"] = {
             "cpu_time_name": cpu_time_name,
             "cpu_time_unit": cpu_time_unit,
         }
 
         result = convert_to_seconds(conf, 1100)
         assert result == 1100
@@ -1091,38 +1060,39 @@
         result = convert_to_seconds(conf, 1500)
         assert result == 2
 
     def test_convert_to_seconds_fail(self):
         cpu_time_name = "TotalCPU"
         cpu_time_unit = "hours"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["auditor"] = {
             "cpu_time_name": cpu_time_name,
             "cpu_time_unit": cpu_time_unit,
         }
 
         with pytest.raises(Exception) as pytest_error:
             convert_to_seconds(conf, 1100)
         assert pytest_error.type == ValueError
 
     def test_check_sites_in_records(self):
-        sites_to_report = (
-            '{"TEST_SITE_1": ["test-site-1"], "TEST_SITE_2": ["test-site-2"]}'
-        )
+        sites_to_report = {
+            "TEST_SITE_1": ["test-site-1"],
+            "TEST_SITE_2": ["test-site-2"],
+        }
         benchmark_name = "hepscore"
         cores_name = "Cores"
         cpu_time_name = "TotalCPU"
         nnodes_name = "NNodes"
         meta_key_site = "site_id"
         meta_key_submithost = "headnode"
         meta_key_voms = "voms"
         meta_key_username = "subject"
 
-        conf = configparser.ConfigParser()
+        conf = {}
         conf["site"] = {
             "sites_to_report": sites_to_report,
         }
         conf["auditor"] = {
             "benchmark_name": benchmark_name,
             "cores_name": cores_name,
             "cpu_time_name": cpu_time_name,
@@ -1174,16 +1144,16 @@
             for r_values in rec_value_list:
                 rec = create_rec(r_values, conf["auditor"])
                 records.append(rec)
 
             result = check_sites_in_records(conf, records)
             assert len(result) == 2
 
-            conf["site"]["sites_to_report"] = '{"TEST_SITE_1": ["test-site-1"]}'
+            conf["site"]["sites_to_report"] = {"TEST_SITE_1": ["test-site-1"]}
 
             result = check_sites_in_records(conf, records)
             assert len(result) == 1
 
-            conf["site"]["sites_to_report"] = '{"TEST_SITE_3": ["test-site-3"]}'
+            conf["site"]["sites_to_report"] = {"TEST_SITE_3": ["test-site-3"]}
 
             result = check_sites_in_records(conf, records)
             assert len(result) == 0
```

