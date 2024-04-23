# Comparing `tmp/great_expectations_cloud-20240420.0.dev0.tar.gz` & `tmp/great_expectations_cloud-20240423.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240420.0.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240423.0.dev0.tar", max compression
```

## Comparing `great_expectations_cloud-20240420.0.dev0.tar` & `great_expectations_cloud-20240423.0.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-04-22 20:28:49.196834 great_expectations_cloud-20240420.0.dev0/LICENSE
--rw-r--r--   0        0        0     9486 2024-04-22 20:28:49.196834 great_expectations_cloud-20240420.0.dev0/README.md
--rw-r--r--   0        0        0      150 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      733 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    16465 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0     1951 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0      362 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/warnings.py
--rw-r--r--   0        0        0     1762 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     3130 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9421 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/pyproject.toml
--rw-r--r--   0        0        0    10820 1970-01-01 00:00:00.000000 great_expectations_cloud-20240420.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-23 16:11:50.759573 great_expectations_cloud-20240423.0.dev0/LICENSE
+-rw-r--r--   0        0        0     9486 2024-04-23 16:11:50.759573 great_expectations_cloud-20240423.0.dev0/README.md
+-rw-r--r--   0        0        0      150 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      733 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    16465 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0     2851 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0      362 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/warnings.py
+-rw-r--r--   0        0        0     1762 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5395 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9462 2024-04-23 16:11:50.799573 great_expectations_cloud-20240423.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    10820 1970-01-01 00:00:00.000000 great_expectations_cloud-20240423.0.dev0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240420.0.dev0/LICENSE` & `great_expectations_cloud-20240423.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/README.md` & `great_expectations_cloud-20240423.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
 
 import argparse
 import dataclasses as dc
+import json
 import logging
 import pathlib
+import sys
+from typing import Any
 
-from great_expectations_cloud.logging.logging_cfg import LogLevel, configure_logger
+from great_expectations_cloud.logging.logging_cfg import LogLevel, LogSettings, configure_logger
 
 LOGGER = logging.getLogger(__name__)
 
 
 @dc.dataclass(frozen=True)
 class Arguments:
     log_level: LogLevel
     skip_log_file: bool
+    json_log: bool
     log_cfg_file: pathlib.Path | None
     version: bool
+    custom_log_tags: str
 
 
 def _parse_args() -> Arguments:
     """
     Parse arguments from the command line and return them as a type aware
     `Arguments` dataclass.
     """
@@ -33,33 +38,60 @@
     parser.add_argument(
         "--skip-log-file",
         help="Skip writing debug logs to a file. Defaults to False. Does not affect logging to stdout/stderr.",
         default=False,
         type=pathlib.Path,
     )
     parser.add_argument(
+        "--json-log",
+        help="Output logs in JSON format. Defaults to False.",
+        default=False,
+        action="store_true",
+    )
+    parser.add_argument(
         "--log-cfg-file",
-        help="Path to a logging configuration json file. Supersedes --log-level and --skip-log-file.",
+        help="Path to a logging configuration file in JSON format. Supersedes --log-level and --skip-log-file.",
         type=pathlib.Path,
     )
+    parser.add_argument(
+        "--custom-log-tags",
+        help="Additional tags for logs in form of key-value pairs",
+        type=str,
+        default="{}",
+    )
     parser.add_argument("--version", help="Show the gx agent version.", action="store_true")
     args = parser.parse_args()
     return Arguments(
         log_level=args.log_level,
         skip_log_file=args.skip_log_file,
         log_cfg_file=args.log_cfg_file,
         version=args.version,
+        json_log=args.json_log,
+        custom_log_tags=args.custom_log_tags,
     )
 
 
 def main() -> None:
     # lazy imports ensure our cli is fast and responsive
     args: Arguments = _parse_args()
+    custom_tags: dict[str, Any] = {}
+    try:
+        custom_tags = json.loads(args.custom_log_tags)
+    except json.JSONDecodeError as e:
+        print(f"Failed to parse custom tags {args.custom_log_tags} due to {e}")
+        sys.exit(1)
+
     configure_logger(
-        log_level=args.log_level, skip_log_file=args.skip_log_file, log_cfg_file=args.log_cfg_file
+        LogSettings(
+            log_level=args.log_level,
+            skip_log_file=args.skip_log_file,
+            log_cfg_file=args.log_cfg_file,
+            json_log=args.json_log,
+            custom_tags=custom_tags,
+        )
     )
 
     if args.version:
         from great_expectations_cloud.agent import get_version
 
         print(f"GX Agent version: {get_version()}")
         return
```

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240420.0.dev0/pyproject.toml` & `great_expectations_cloud-20240423.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240420.0.dev0"
+version = "20240423.0.dev0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
@@ -40,17 +40,19 @@
 snowflake-sqlalchemy = ">=1.5.0"
 snowflake-connector-python = ">=3.3.1"
 # TODO: Remove the python constraint once this PR is merged - https://github.com/sqlalchemy-redshift/sqlalchemy-redshift/pull/288
 sqlalchemy-redshift = { version = "^0.8.8", python = "<3.11" }
 psycopg2-binary = "^2.9.9"
 
 [tool.poetry.group.dev.dependencies]
+freezegun = "^1.4.0"
 invoke = "^2.2.0"
 mypy = "1.9"
 pre-commit = "^3.3.3"
+pyfakefs = "^5.4.1"
 pytest = ">=7.4,<9.0"
 pytest-cov = ">=4.1,<6.0"
 pytest-icdiff = "*"
 pytest-mock = "*"
 responses = "^0.23.1"
 ruff = "0.3.7"
 tenacity = "^8.2.3"
```

### Comparing `great_expectations_cloud-20240420.0.dev0/PKG-INFO` & `great_expectations_cloud-20240423.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240420.0.dev0
+Version: 20240423.0.dev0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
```

