# Comparing `tmp/aura-cli-0.5.2.tar.gz` & `tmp/aura-cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura-cli-0.5.2.tar", last modified: Sun Sep 17 10:12:11 2023, max compression
+gzip compressed data, was "aura-cli-0.6.0.tar", last modified: Tue Apr 23 11:13:20 2024, max compression
```

## Comparing `aura-cli-0.5.2.tar` & `aura-cli-0.6.0.tar`

### file list

```diff
@@ -1,62 +1,73 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10935 2023-09-10 11:07:07.000000 aura-cli-0.5.2/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2023-09-17 10:12:11.240092 aura-cli-0.5.2/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5417 2023-09-11 15:24:43.000000 aura-cli-0.5.2/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       37 2023-08-21 13:27:27.000000 aura-cli-0.5.2/aura/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3472 2023-09-17 09:52:55.000000 aura-cli-0.5.2/aura/api_command.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6236 2023-09-12 10:19:34.000000 aura-cli-0.5.2/aura/api_repository.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1232 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/aura.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura/config/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      834 2023-09-12 10:19:34.000000 aura-cli-0.5.2/aura/config/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1342 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/config/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1114 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/config/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1616 2023-09-12 10:19:34.000000 aura-cli-0.5.2/aura/config/set.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1140 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/config/unset.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      298 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/config/valid_options.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8406 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/config_repository.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura/credentials/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      668 2023-08-20 21:13:57.000000 aura-cli-0.5.2/aura/credentials/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1438 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/credentials/add.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1166 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/credentials/current.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      862 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/credentials/delete.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1437 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/credentials/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      860 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/credentials/use.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      239 2023-07-15 15:45:24.000000 aura-cli-0.5.2/aura/decorators.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5887 2023-09-12 10:02:00.000000 aura-cli-0.5.2/aura/error_handler.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1612 2023-09-03 12:59:48.000000 aura-cli-0.5.2/aura/format.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura/instances/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      684 2023-08-20 20:45:09.000000 aura-cli-0.5.2/aura/instances/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1961 2023-09-11 15:24:43.000000 aura-cli-0.5.2/aura/instances/create.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      919 2023-08-20 21:19:15.000000 aura-cli-0.5.2/aura/instances/delete.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      621 2023-08-20 20:30:34.000000 aura-cli-0.5.2/aura/instances/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      826 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/instances/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1438 2023-09-11 15:24:43.000000 aura-cli-0.5.2/aura/instances/overwrite.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      897 2023-09-11 15:24:43.000000 aura-cli-0.5.2/aura/instances/pause.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      909 2023-09-11 15:24:43.000000 aura-cli-0.5.2/aura/instances/resume.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1319 2023-09-11 15:24:43.000000 aura-cli-0.5.2/aura/instances/update.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      948 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/logger.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura/snapshots/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      380 2023-08-20 20:56:15.000000 aura-cli-0.5.2/aura/snapshots/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      965 2023-09-11 15:24:43.000000 aura-cli-0.5.2/aura/snapshots/create.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      793 2023-08-20 21:09:15.000000 aura-cli-0.5.2/aura/snapshots/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      894 2023-08-20 21:36:10.000000 aura-cli-0.5.2/aura/snapshots/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1131 2023-09-11 15:24:43.000000 aura-cli-0.5.2/aura/snapshots/restore.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura/tenants/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      208 2023-08-20 20:59:18.000000 aura-cli-0.5.2/aura/tenants/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      809 2023-09-11 11:01:09.000000 aura-cli-0.5.2/aura/tenants/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      335 2023-08-20 21:09:15.000000 aura-cli-0.5.2/aura/tenants/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1184 2023-08-19 18:37:36.000000 aura-cli-0.5.2/aura/token_repository.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura/util/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-08-28 12:55:18.000000 aura-cli-0.5.2/aura/util/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1172 2023-09-03 12:59:48.000000 aura-cli-0.5.2/aura/util/get_instance_id.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2023-09-17 10:10:42.000000 aura-cli-0.5.2/aura/version.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-09-17 10:12:11.240092 aura-cli-0.5.2/aura_cli.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2023-09-17 10:12:11.000000 aura-cli-0.5.2/aura_cli.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1184 2023-09-17 10:12:11.000000 aura-cli-0.5.2/aura_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-09-17 10:12:11.000000 aura-cli-0.5.2/aura_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       39 2023-09-17 10:12:11.000000 aura-cli-0.5.2/aura_cli.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       50 2023-09-17 10:12:11.000000 aura-cli-0.5.2/aura_cli.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        5 2023-09-17 10:12:11.000000 aura-cli-0.5.2/aura_cli.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-09-17 10:12:11.240092 aura-cli-0.5.2/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      588 2023-08-21 13:55:41.000000 aura-cli-0.5.2/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.991334 aura-cli-0.6.0/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10935 2023-09-10 11:07:07.000000 aura-cli-0.6.0/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2024-04-23 11:13:20.991334 aura-cli-0.6.0/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5535 2024-04-23 10:42:38.000000 aura-cli-0.6.0/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.983334 aura-cli-0.6.0/aura/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       37 2023-08-21 13:27:27.000000 aura-cli-0.6.0/aura/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3546 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/api_command.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7811 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/api_repository.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1392 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/aura.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.983334 aura-cli-0.6.0/aura/config/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      559 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/config/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1367 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/config/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1138 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/config/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1703 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/config/set.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1165 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/config/unset.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      298 2023-09-11 11:01:09.000000 aura-cli-0.6.0/aura/config/valid_options.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9137 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/config_repository.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.987334 aura-cli-0.6.0/aura/credentials/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      668 2023-08-20 21:13:57.000000 aura-cli-0.6.0/aura/credentials/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1463 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/credentials/add.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1191 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/credentials/current.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      887 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/credentials/delete.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1462 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/credentials/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      885 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/credentials/use.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.987334 aura-cli-0.6.0/aura/data_apis/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      452 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2606 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/create.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1000 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/delete.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      684 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      528 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3074 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/update.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.987334 aura-cli-0.6.0/aura/data_apis/util/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/util/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      446 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/data_apis/util/type_definitions.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      239 2023-07-15 15:45:24.000000 aura-cli-0.6.0/aura/decorators.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6074 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/error_handler.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1612 2023-09-03 12:59:48.000000 aura-cli-0.6.0/aura/format.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.987334 aura-cli-0.6.0/aura/instances/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      684 2023-08-20 20:45:09.000000 aura-cli-0.6.0/aura/instances/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1948 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/instances/create.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      919 2023-08-20 21:19:15.000000 aura-cli-0.6.0/aura/instances/delete.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      621 2023-08-20 20:30:34.000000 aura-cli-0.6.0/aura/instances/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      826 2023-09-11 11:01:09.000000 aura-cli-0.6.0/aura/instances/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1425 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/instances/overwrite.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      884 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/instances/pause.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      896 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/instances/resume.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1306 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/instances/update.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      935 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/logger.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.987334 aura-cli-0.6.0/aura/snapshots/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      380 2023-08-20 20:56:15.000000 aura-cli-0.6.0/aura/snapshots/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      952 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/snapshots/create.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      793 2023-08-20 21:09:15.000000 aura-cli-0.6.0/aura/snapshots/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      894 2023-08-20 21:36:10.000000 aura-cli-0.6.0/aura/snapshots/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1118 2023-10-04 14:40:35.000000 aura-cli-0.6.0/aura/snapshots/restore.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.987334 aura-cli-0.6.0/aura/tenants/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      344 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/tenants/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      809 2023-09-11 11:01:09.000000 aura-cli-0.6.0/aura/tenants/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      833 2024-04-23 10:42:38.000000 aura-cli-0.6.0/aura/tenants/get_metrics_integration.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      335 2023-08-20 21:09:15.000000 aura-cli-0.6.0/aura/tenants/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1184 2023-08-19 18:37:36.000000 aura-cli-0.6.0/aura/token_repository.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.987334 aura-cli-0.6.0/aura/util/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-08-28 12:55:18.000000 aura-cli-0.6.0/aura/util/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1172 2023-09-03 12:59:48.000000 aura-cli-0.6.0/aura/util/get_instance_id.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-23 10:42:56.000000 aura-cli-0.6.0/aura/version.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 11:13:20.991334 aura-cli-0.6.0/aura_cli.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2024-04-23 11:13:20.000000 aura-cli-0.6.0/aura_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1443 2024-04-23 11:13:20.000000 aura-cli-0.6.0/aura_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-23 11:13:20.000000 aura-cli-0.6.0/aura_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       39 2024-04-23 11:13:20.000000 aura-cli-0.6.0/aura_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       70 2024-04-23 11:13:20.000000 aura-cli-0.6.0/aura_cli.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        5 2024-04-23 11:13:20.000000 aura-cli-0.6.0/aura_cli.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-23 11:13:20.991334 aura-cli-0.6.0/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      589 2023-09-17 10:54:54.000000 aura-cli-0.6.0/setup.py
```

### Comparing `aura-cli-0.5.2/LICENSE` & `aura-cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/README.md` & `aura-cli-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,21 +98,23 @@
 ### Logs
 
 The CLI will generate logs which can be printed using the `--verbose` flag. By default these logs are not saved, but setting the `AURA_CLI_SAVE_LOGS` environment variable or the `save_logs` config option to `true` or `yes` will write the logs to a file.
 The default location of the log file is `~/.aura/auracli.log`, but this can be changed by setting the `AURA_CLI_LOG_FILE_PATH` environment variable or the `log_file_path` config option.
 
 ## Development
 
-To installing the CLI for developement, do the following:
+To install the CLI and its dependencies for development, do the following:
 
-In the root directory run `. venv/bin/activate` to active the virtual environment.
+In the root of the repository, run `python3 -m venv .venv` to create a virtual environment.
 
-Next, run `pip install --editable .` to install the dependencies. Then you can run the cli `aura --help`.
+Next, run `. .venv/bin/activate` to activate the virtual environment.
 
-When finished, run `deactivate` to deactivate the venv.
+Next, run `pip install --editable .` to install the dependencies. Then you can run the CLI using `aura --help`.
+
+When finished, run `deactivate` to deactivate the virtual environment.
 
 To run the unit tests, run `pytest tests/unit`.
 
 For development you will need the following Python libraries installed:
 
 - `pytest`
 - `black`
```

### Comparing `aura-cli-0.5.2/aura/api_command.py` & `aura-cli-0.6.0/aura/api_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         @click.option(
             "--verbose",
             is_flag=True,
             default=False,
             help="Print verbose output",
         )
         @wraps(func)
+        # pylint: disable=unused-argument
         def wrapper(output: str, include: bool, raw: bool, verbose: bool, *args, **kwargs):
             ctx = click.get_current_context()
             config: CLIConfig = ctx.obj
             logger = get_logger()
 
             try:
                 api_response = func(*args, **kwargs)
@@ -74,23 +75,23 @@
                     print(json.dumps(response_data))
                     return click.get_current_context().exit(code=0)
 
                 output_format = fixed_cmd_output or output or config.env["output"]
 
                 if data is None:
                     print("Operation successful")
-                elif output_format == "json":
+                elif output_format.lower() == "json":
                     print(json.dumps(data, indent=2))
-                elif output_format == "table":
+                elif output_format.lower() == "table":
                     out = format_table_output(data)
                     print(out)
-                elif output_format == "text":
+                elif output_format.lower() == "text":
                     out = format_text_output(data)
                     print(out)
-                elif output_format == "yaml":
+                elif output_format.lower() == "yaml":
                     print(yaml.dump(data))
                 else:
                     raise UnsupportedOutputFormat(output_format)
 
                 logger.debug("CLI command completed successfully.")
                 return click.get_current_context().exit(code=0)
```

### Comparing `aura-cli-0.5.2/aura/api_repository.py` & `aura-cli-0.6.0/aura/api_repository.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module defines methods for making HTTP request to the Aura API"""
+
 import os
 import json
-import click
 import time
+import click
 from requests.auth import HTTPBasicAuth
 import requests
 
 from aura.config_repository import CLIConfig
 from aura.version import __version__
 from aura.logger import get_logger
 from aura.error_handler import (
@@ -24,30 +25,38 @@
 def _get_credentials():
     logger = get_logger()
 
     client_id = os.environ.get("AURA_CLI_CLIENT_ID")
     client_secret = os.environ.get("AURA_CLI_CLIENT_SECRET")
 
     if client_id:
-        logger.debug("Reading API client id from environment variable AURA_CLI_CLIENT_ID.")
+        logger.debug(
+            "Reading API client id from environment variable AURA_CLI_CLIENT_ID."
+        )
     if client_secret:
-        logger.debug("Reading API client secret from environment variable AURA_CLI_CLIENT_SECRET.")
+        logger.debug(
+            "Reading API client secret from environment variable AURA_CLI_CLIENT_SECRET."
+        )
 
     if not client_id or not client_secret:
         ctx = click.get_current_context()
         config = ctx.obj
         cred_name, current_credentials = config.current_credentials()
 
         if current_credentials is None:
             raise NoCredentialsConfigured()
 
         if not client_id:
-            logger.debug(f"Reading API client id from configured credentials {cred_name}.")
+            logger.debug(
+                f"Reading API client id from configured credentials {cred_name}."
+            )
         if not client_secret:
-            logger.debug(f"Reading API client secret from configured credentials {cred_name}.")
+            logger.debug(
+                f"Reading API client secret from configured credentials {cred_name}."
+            )
 
         client_id = client_id or current_credentials["CLIENT_ID"]
         client_secret = client_secret or current_credentials["CLIENT_SECRET"]
 
     if not client_id or not client_secret:
         logger.warning("No API credentials were configured.")
         raise NoCredentialsConfigured()
@@ -85,17 +94,17 @@
         headers=headers,
         data=data,
         auth=HTTPBasicAuth(client_id, client_secret),
         timeout=10,
     )
     try:
         response.raise_for_status()
-    except Exception as e:
+    except Exception as exception:
         logger.warning("Authentication request was not succesful.")
-        raise e
+        raise exception
 
     logger.debug("Authentication request successful. Using new auth token.")
 
     token, expires_in = (
         response.json()["access_token"],
         response.json()["expires_in"],
     )
@@ -125,19 +134,29 @@
 
     headers = get_headers()
 
     # Get url by priority: First by env var, then by config setting, then by default url
     base_url = config.env["base_url"]
     full_url = base_url + path
 
-    logger.debug(f"Initializing connection to Aura Cloud Platform API endpoint: {base_url}")
-    data_string = " with data: " + json.dumps(kwargs["data"]) if "data" in kwargs else ""
+    logger.debug(
+        f"Initializing connection to Aura Cloud Platform API endpoint: {base_url}"
+    )
+    data_string = (
+        " with data: " + json.dumps(kwargs["data"]) if "data" in kwargs else ""
+    )
     logger.debug(f"Sending {method} request to {full_url}{data_string}")
 
-    response = requests.request(method, full_url, headers=headers, timeout=10, **kwargs)
+    timeout = 10
+    if config.env.get("data_apis", False):
+        timeout = 30
+
+    response = requests.request(
+        method, full_url, headers=headers, timeout=timeout, **kwargs
+    )
     # If authentication failed, delete the token file to avoid using same token again
     if response.status_code in [401, 403]:
         logger.warning("API authentication failed.")
         delete_token_file()
 
     return response
 
@@ -164,16 +183,16 @@
         data = res.json()["data"]
         status = data["status"]
 
         logger.debug(f'Polling instance. Status is "{status}".')
 
         if status == desired_status:
             return res
-        else:
-            time.sleep(30)
+
+        time.sleep(30)
 
     raise InstanceOperationTimeoutError(instance_id, desired_status)
 
 
 def make_api_call_and_wait_for_snapshot_completed(
     method: str, path: str, instance_id: str, **kwargs
 ):
@@ -195,11 +214,52 @@
         data = res.json()["data"]
         status = data["status"]
 
         logger.debug(f'Polling snapshot. Status is "{status}".')
 
         if status == "Completed":
             return res
-        else:
-            time.sleep(30)
+
+        time.sleep(30)
 
     raise SnapshotOperationTimeoutError(snapshot_id, "Completed")
+
+
+def make_api_call_and_wait_for_data_api_status(
+    method: str, path: str, desired_status: str, **kwargs
+):
+    logger = get_logger()
+
+    main_response = make_api_call(method, path, **kwargs)
+    main_response.raise_for_status()
+
+    data = main_response.json()["data"]
+    data_api_id = data["id"]
+    instance_id = data["aura_instance"]["id"]
+    status = data.get("status")
+
+    if "api_key" in data:
+        api_key = data["api_key"]
+        print(f'Data API with ID "{data_api_id}" has been created.')
+        print(
+            f'The API key is "{api_key}". Please securely save this and use it to authenticate with the Data API once it is ready.'
+        )
+        print("Beginning polling for ready state of the Data API.")
+
+    logger.debug(f"Data API has status {status}.")
+    logger.debug(f"Waiting for data API to have status {desired_status}.")
+
+    # Poll every 30 seconds, 40 times. Max total wait = 20 min
+    for _ in range(40):
+        res = make_api_call("GET", f"/instances/{instance_id}/data-apis/{data_api_id}")
+        res.raise_for_status()
+        data = res.json()["data"]
+        status = data["status"]
+
+        logger.debug(f'Polling instance. Status is "{status}".')
+
+        if status == desired_status:
+            return res
+
+        time.sleep(30)
+
+    raise InstanceOperationTimeoutError(instance_id, desired_status)
```

### Comparing `aura-cli-0.5.2/aura/aura.py` & `aura-cli-0.6.0/aura/aura.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from functools import wraps
 import click
-import sys
 from aura.config_repository import CLIConfig
 from aura.instances import instances
 from aura.credentials import credentials
 from aura.logger import get_logger
 from aura.snapshots import snapshots
 from aura.tenants import tenants
 from aura.config import config
+from aura.data_apis import data_apis
 from aura.version import __version__
 
 CLI_VERSION_MESSAGE = f"Aura CLI: version {__version__}, Aura API: version v1"
 
+cli_config = CLIConfig()
+
 
 @click.group()
 @click.version_option(
     message=CLI_VERSION_MESSAGE,
     package_name="aura-cli",
 )
 @click.pass_context
-@click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
-def cli(ctx, verbose):
-    ctx.obj = CLIConfig()
+@click.option(
+    "--verbose", "-v", is_flag=True, default=False, help="Print verbose output"
+)
+# pylint: disable=unused-argument
+def cli(ctx, verbose: bool):
+    ctx.obj = cli_config
 
 
 cli.add_command(credentials)
 cli.add_command(instances)
 cli.add_command(snapshots)
 cli.add_command(tenants)
 cli.add_command(config)
+if cli_config.env["data_apis"]:
+    cli.add_command(data_apis)
 
 
 def log_usage_errors(func):
     @wraps(func)
     def log_decorator(*args, **kwargs):
         logger = get_logger()
         logger.debug("Error: " + str(args[0]))
```

### Comparing `aura-cli-0.5.2/aura/config/__init__.py` & `aura-cli-0.6.0/aura/config/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import click
-from .set import set_option
+from .set import set_option, VALID_OPTIONS_HELP_TEXT
 from .unset import unset_option
 from .get import get_option
 from .list import list_options
 
-HELP_TEXT = """
+HELP_TEXT = f"""
 Manage configurations and set default values
 
-Valid config options:\n
-    • default_tenant\tSet a default tenant\n
-    • output\t\tSet a default output format\n
-    • auth_url\t\tChange the auth url\n
-    • base_url\t\tChange the api base url\n
-    • save_logs\t\tFlag if CLI logs are saved to a file\n
-    • log_file_path\tPath to file where logs are saved to
+{VALID_OPTIONS_HELP_TEXT}
 
 Example usage:\n
 aura config set default_tenant <my-tenant-id>\n
 aura config unset output\n
 aura config set save_logs true
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aura-cli-0.5.2/aura/config/get.py` & `aura-cli-0.6.0/aura/config/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 """
 
 
 @click.argument("name")
 @click.command(name="get", help=HELP_TEXT)
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @pass_config
+# pylint: disable=unused-argument
 def get_option(config: CLIConfig, name: str, verbose: bool):
     """
     Print a config option
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         if name not in VALID_OPTIONS:
             raise InvalidConfigOption(name)
 
         value = config.get_option(name)
     except Exception as exception:
```

### Comparing `aura-cli-0.5.2/aura/config/list.py` & `aura-cli-0.6.0/aura/config/list.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 aura config list
 """
 
 
 @click.command(name="list", help=HELP_TEXT)
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @pass_config
+# pylint: disable=unused-argument
 def list_options(config: CLIConfig, verbose: bool):
     """
     List all configured config options
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         values = config.list_options()
     except Exception as exception:
         handle_error(exception)
 
     if values is None or len(values) == 0:
-        logger.info(f"No config options set.")
+        logger.info("No config options set.")
         if not config.env["verbose"]:
             print("No config options set.")
     else:
         logger.info(f"Config options: {values}")
         if not config.env["verbose"]:
             out = format_text_output(values)
             print(out)
```

### Comparing `aura-cli-0.5.2/aura/config/set.py` & `aura-cli-0.6.0/aura/config/set.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,42 +5,47 @@
 from aura.error_handler import (
     InvalidConfigOption,
     InvalidConfigOptionValue,
     handle_error,
 )
 from aura.logger import get_logger
 
-HELP_TEXT = """
-Set a config option to a new value
-
+VALID_OPTIONS_HELP_TEXT = """
 Valid config options:\n
     • default_tenant\tSet a default tenant\n
     • output\t\tSet a default output format\n
     • auth_url\t\tChange the auth url\n
     • base_url\t\tChange the api base url\n
     • save_logs\t\tFlag if CLI logs are saved to a file\n
     • log_file_path\tPath to file where logs are saved to
+"""
+
+HELP_TEXT = f"""
+Set a config option to a new value
+
+{VALID_OPTIONS_HELP_TEXT}
 
 
 Example usage:\n
 aura config set default_tenant my-tenant-id\n
 aura config set output table
 """
 
 
 @click.command(name="set", help=HELP_TEXT)
 @click.argument("name")
 @click.argument("value")
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @pass_config
+# pylint: disable=unused-argument
 def set_option(config: CLIConfig, name: str, value: str, verbose: bool):
     """
     Set a config option to specified value
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         if name not in VALID_OPTIONS:
             raise InvalidConfigOption(name)
         if value is None:
             raise InvalidConfigOptionValue(name)
```

### Comparing `aura-cli-0.5.2/aura/config/unset.py` & `aura-cli-0.6.0/aura/config/unset.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 """
 
 
 @click.argument("name")
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @click.command(name="unset", help=HELP_TEXT)
 @pass_config
+# pylint: disable=unused-argument
 def unset_option(config: CLIConfig, name: str, verbose: bool):
     """
     Delete a config value
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         if name not in VALID_OPTIONS:
             raise InvalidConfigOption(name)
 
         config.unset_option(name)
     except Exception as exception:
```

### Comparing `aura-cli-0.5.2/aura/config_repository.py` & `aura-cli-0.6.0/aura/config_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 from aura.error_handler import (
     CredentialsAlreadyExist,
     CredentialsNotFound,
     InvalidConfigFile,
     UnsupportedConfigFileVersion,
     handle_error,
 )
-from aura.logger import get_logger, setup_logger
+from aura.logger import setup_logger
 from aura.token_repository import delete_token_file
 from aura.version import __version__
 
 
 class CLIConfig:
     """
     Class which handles configurations of the CLI.
     The CLI's configuration is saved locally as a json file.
-    This class handles loading, validatinf and updating this config.
+    This class handles loading, validating and updating this config.
     """
 
     DEFAULT_AURA_CONFIG_PATH = "~/.aura/config.json"
     DEFAULT_LOG_FILE_PATH = "~/.aura/auracli.log"
     DEFAULT_CONFIG = {
         "VERSION": __version__,
         "AUTH": {"CREDENTIALS": {}, "ACTIVE": None},
         "OPTIONS": {},
     }
     DEFAULT_BASE_URL = "https://api.neo4j.io/v1"
     DEFAULT_AUTH_URL = "https://api.neo4j.io/oauth/token"
 
     def __init__(self):
         self.logger = None
-        self.config_path = os.environ.get("AURA_CLI_CONFIG_PATH", None) or os.path.expanduser(
-            self.DEFAULT_AURA_CONFIG_PATH
-        )
+        self.config_path = os.environ.get(
+            "AURA_CLI_CONFIG_PATH", None
+        ) or os.path.expanduser(self.DEFAULT_AURA_CONFIG_PATH)
         self.config = self.load_config()
         self.env = self.load_env()
 
         self.logger = setup_logger(
             self.env["verbose"], self.env["save_logs"], self.env["log_file_path"]
         )
         self.logger.debug(f"CLI initiated. Version {__version__}")
@@ -54,56 +54,82 @@
             or self.DEFAULT_BASE_URL
         )
         env["auth_url"] = (
             os.environ.get("AURA_CLI_AUTH_URL")
             or self.get_option("auth_url")
             or self.DEFAULT_AUTH_URL
         )
-        env["output"] = os.environ.get("AURA_CLI_OUTPUT") or self.get_option("output") or "json"
+        env["output"] = (
+            os.environ.get("AURA_CLI_OUTPUT") or self.get_option("output") or "json"
+        )
         env["default_tenant"] = (
-            os.environ.get("AURA_CLI_DEFAULT_TENANT") or self.get_option("default_tenant") or None
+            os.environ.get("AURA_CLI_DEFAULT_TENANT")
+            or self.get_option("default_tenant")
+            or None
         )
         env["config_path"] = self.config_path
 
         if os.environ.get("AURA_CLI_SAVE_LOGS") is not None:
             env["save_logs"] = os.environ.get("AURA_CLI_SAVE_LOGS", "").lower() in {
                 "yes",
                 "y",
                 "true",
                 "1",
             }
         elif self.get_option("save_logs") is not None:
-            env["save_logs"] = self.get_option("save_logs").lower() in {"yes", "y", "true", "1"}
+            env["save_logs"] = self.get_option("save_logs").lower() in {
+                "yes",
+                "y",
+                "true",
+                "1",
+            }
         else:
             env["save_logs"] = False
 
         env["log_file_path"] = (
             os.environ.get("AURA_CLI_LOG_FILE_PATH")
             or self.get_option("log_file_path")
             or os.path.expanduser(self.DEFAULT_LOG_FILE_PATH)
         )
         # The verbose flag is supposed to be global but click does not allow checking
         # all nested subcommands and options at this level. So we manually check if the
         # flag was set at any level.
         env["verbose"] = "--verbose" in sys.argv
 
+        if os.environ.get("DATA_APIS") is not None:
+            env["data_apis"] = os.environ.get("DATA_APIS", "").lower() in {
+                "yes",
+                "y",
+                "true",
+                "1",
+            }
+        elif self.get_option("data_apis") is not None:
+            env["data_apis"] = self.get_option("data_apis").lower() in {
+                "yes",
+                "y",
+                "true",
+                "1",
+            }
+        else:
+            env["data_apis"] = False
+
         return env
 
     def load_config(self) -> dict:
         try:
             with open(self.config_path, "r", encoding="utf-8") as configfile:
                 config = json.load(configfile)
         except (FileNotFoundError, json.JSONDecodeError):
             config = self.write_config(self.DEFAULT_CONFIG)
             return config
 
         try:
             self.validate_config(config)
-        except Exception as e:
-            handle_error(e)
+        except Exception as exception:
+            handle_error(exception)
 
         return config
 
     def write_config(self, config: dict):
         if self.logger:
             self.logger.debug("Updating user configuration at " + self.config_path)
 
@@ -112,15 +138,18 @@
         with open(self.config_path, "w", encoding="utf-8") as configfile:
             json.dump(config, configfile)
 
         return config
 
     def list_credentials(self):
         credentials = self.config["AUTH"].get("CREDENTIALS")
-        return [{"Name": c, "ClientId": credentials[c]["CLIENT_ID"]} for c in credentials.keys()]
+        return [
+            {"Name": c, "ClientId": credentials[c]["CLIENT_ID"]}
+            for c in credentials.keys()
+        ]
 
     def add_credentials(self, name: str, client_id: str, client_secret: str, use: bool):
         if self.config["AUTH"]["CREDENTIALS"].get(name, None) is not None:
             raise CredentialsAlreadyExist(name)
 
         self.config["AUTH"]["CREDENTIALS"][name] = {
             "CLIENT_ID": client_id,
@@ -189,19 +218,23 @@
         for _, cred in credentials.items():
             if not isinstance(cred, dict):
                 raise InvalidConfigFile()
 
             if "CLIENT_ID" not in cred or not isinstance(cred["CLIENT_ID"], str):
                 raise InvalidConfigFile()
 
-            if "CLIENT_SECRET" not in cred or not isinstance(cred["CLIENT_SECRET"], str):
+            if "CLIENT_SECRET" not in cred or not isinstance(
+                cred["CLIENT_SECRET"], str
+            ):
                 raise InvalidConfigFile()
 
         active = auth.get("ACTIVE")
-        if active is not None and (not isinstance(active, str) or active not in credentials):
+        if active is not None and (
+            not isinstance(active, str) or active not in credentials
+        ):
             raise InvalidConfigFile()
 
         # Validate Defaults section
         defaults = config.get("OPTIONS")
         if defaults is None:
             self.config["OPTIONS"] = {}
             self.write_config(self.config)
```

### Comparing `aura-cli-0.5.2/aura/credentials/__init__.py` & `aura-cli-0.6.0/aura/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/credentials/add.py` & `aura-cli-0.6.0/aura/credentials/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 @click.option("--name", "-n", help="Name for the credentials")
 @click.option("--client-id", "-id", help="The client ID")
 @click.option("--client-secret", "-s", help="The client secret")
 @click.option("--use", "-u", is_flag=True, default=False, help="Use the credentials")
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @click.command(name="add", help="Add new OAuth client credentials")
 @pass_config
+# pylint: disable=unused-argument
 def add_credentials(
     config: CLIConfig, name: str, client_id: str, client_secret: str, use: bool, verbose: bool
 ):
     """
     Add a new set of credentials
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     if not name:
         name = click.prompt("Credentials Name")
     if not client_id:
         client_id = click.prompt("Client ID")
     if not client_secret:
         client_secret = click.prompt("Client Secret")
```

### Comparing `aura-cli-0.5.2/aura/credentials/current.py` & `aura-cli-0.6.0/aura/credentials/current.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from aura.decorators import pass_config
 from aura.logger import get_logger
 
 
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @click.command(name="current", help="Print the currently selected credentials")
 @pass_config
+# pylint: disable=unused-argument
 def current_credentials(config: CLIConfig, verbose: bool):
     """
     Print the credentials currently in use
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         name, creds = config.current_credentials()
     except Exception as exception:
         handle_error(exception)
 
     if name is None:
```

### Comparing `aura-cli-0.5.2/aura/credentials/delete.py` & `aura-cli-0.6.0/aura/credentials/delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from aura.logger import get_logger
 
 
 @click.argument("name")
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @click.command(name="delete", help="Delete OAuth client credentials")
 @pass_config
+# pylint: disable=unused-argument
 def delete_credentials(config: CLIConfig, name: str, verbose: bool):
     """
     Deletes the specified credentials
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         config.delete_credentials(name)
     except Exception as exception:
         handle_error(exception)
 
     logger.info(f"Credentials {name} successfully deleted")
```

### Comparing `aura-cli-0.5.2/aura/credentials/list.py` & `aura-cli-0.6.0/aura/credentials/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from aura.format import format_text_output
 from aura.logger import get_logger
 
 
 @click.command(name="list", help="List all configured OAuth client credentials")
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @pass_config
+# pylint: disable=unused-argument
 def list_credentials(config: CLIConfig, verbose: bool):
     """
     List all configured credentials
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         credentials = config.list_credentials()
         current_creds, _ = config.current_credentials()
     except Exception as exception:
         handle_error(exception)
```

### Comparing `aura-cli-0.5.2/aura/credentials/use.py` & `aura-cli-0.6.0/aura/credentials/use.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from aura.logger import get_logger
 
 
 @click.argument("name")
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Print verbose output")
 @click.command(name="use", help="Select which OAuth client credentials to use for authentication")
 @pass_config
+# pylint: disable=unused-argument
 def use_credentials(config: CLIConfig, name: str, verbose: bool):
     """
     Use the speccified credentials
     """
-    logger = get_logger("auracli")
+    logger = get_logger()
 
     try:
         config.use_credentials(name)
     except Exception as exception:
         handle_error(exception)
 
     logger.info(f"Now using credentials {name}")
```

### Comparing `aura-cli-0.5.2/aura/error_handler.py` & `aura-cli-0.6.0/aura/error_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """This module defines the error_handler function and a set of custom exceptions"""
+
+from graphql import GraphQLError
 from requests.exceptions import HTTPError, Timeout, ConnectionError as ConnError
 import click
 
 from aura.logger import get_logger
 
 
 def handle_error(exception: Exception):
@@ -26,22 +28,26 @@
                 error_message = str(exception)
             # Most errors returned by the API will have a error/errors field with the error message
             elif "error" in error_data:
                 error_message = error_data["error"]
             elif "errors" in error_data:
                 error_message = "\n".join([e["message"] for e in error_data["errors"]])
         except ValueError:
-            error_message = f"Unknown error (status code {exception.response.status_code})"
+            error_message = (
+                f"Unknown error (status code {exception.response.status_code})"
+            )
 
     elif isinstance(exception, ClientError):
         error_message = exception.message
     elif isinstance(exception, Timeout):
         error_message = "Request timed out"
     elif isinstance(exception, ConnError):
         error_message = "Connection error"
+    elif isinstance(exception, GraphQLError):
+        error_message = "Could not parse as GraphQL"
     else:
         error_message = "An unexpected error occurred"
 
     ctx = click.get_current_context()
     config = ctx.obj
 
     logger.warning(f"Error: {error_message}")
@@ -68,15 +74,17 @@
         super().__init__(message)
 
 
 class InstanceIDAndNameBothProvided(ClientError):
     """Exception raised when providing both instance ID and name in a command"""
 
     def __init__(self):
-        super().__init__("Only one of the options instance-id and instance-name should be provided")
+        super().__init__(
+            "Only one of the options instance-id and instance-name should be provided"
+        )
 
 
 class InstanceIDorNameMissing(ClientError):
     """
     Exception raised when providing neither instance ID nor name
     in a command where either is required
     """
```

### Comparing `aura-cli-0.5.2/aura/format.py` & `aura-cli-0.6.0/aura/format.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/instances/__init__.py` & `aura-cli-0.6.0/aura/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/instances/create.py` & `aura-cli-0.6.0/aura/instances/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,9 +58,9 @@
         "cloud_provider": cloud_provider,
     }
 
     if wait:
         return make_api_call_and_wait_for_instance_status(
             "POST", path, "running", data=json.dumps(data)
         )
-    else:
-        return make_api_call("POST", path, data=json.dumps(data))
+
+    return make_api_call("POST", path, data=json.dumps(data))
```

### Comparing `aura-cli-0.5.2/aura/instances/delete.py` & `aura-cli-0.6.0/aura/instances/delete.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/instances/get.py` & `aura-cli-0.6.0/aura/instances/get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/instances/list.py` & `aura-cli-0.6.0/aura/instances/list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/instances/overwrite.py` & `aura-cli-0.6.0/aura/instances/overwrite.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,9 +35,9 @@
 
     path = f"/instances/{instance_id}/overwrite"
 
     if wait:
         return make_api_call_and_wait_for_instance_status(
             "POST", path, "running", data=json.dumps(data)
         )
-    else:
-        return make_api_call("POST", path, data=json.dumps(data))
+
+    return make_api_call("POST", path, data=json.dumps(data))
```

### Comparing `aura-cli-0.5.2/aura/instances/pause.py` & `aura-cli-0.6.0/aura/instances/pause.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
     instance_id = get_instance_id(instance_id, name)
 
     path = f"/instances/{instance_id}/pause"
 
     if wait:
         return make_api_call_and_wait_for_instance_status("POST", path, "paused")
-    else:
-        return make_api_call("POST", path)
+
+    return make_api_call("POST", path)
```

### Comparing `aura-cli-0.5.2/aura/instances/resume.py` & `aura-cli-0.6.0/aura/instances/resume.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
     instance_id = get_instance_id(instance_id, name)
 
     path = f"/instances/{instance_id}/resume"
 
     if wait:
         return make_api_call_and_wait_for_instance_status("POST", path, "running")
-    else:
-        return make_api_call("POST", path)
+
+    return make_api_call("POST", path)
```

### Comparing `aura-cli-0.5.2/aura/instances/update.py` & `aura-cli-0.6.0/aura/instances/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,9 +34,9 @@
         data["name"] = new_name
     path = f"/instances/{instance_id}"
 
     if wait:
         return make_api_call_and_wait_for_instance_status(
             "PATCH", path, "running", data=json.dumps(data)
         )
-    else:
-        return make_api_call("PATCH", path, data=json.dumps(data))
+
+    return make_api_call("PATCH", path, data=json.dumps(data))
```

### Comparing `aura-cli-0.5.2/aura/logger.py` & `aura-cli-0.6.0/aura/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
 
     return logger
 
 
-def get_logger(verbose=False):
+def get_logger():
     return logging.getLogger("auracli")
```

### Comparing `aura-cli-0.5.2/aura/snapshots/create.py` & `aura-cli-0.6.0/aura/snapshots/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
     instance_id = get_instance_id(instance_id, instance_name)
 
     path = f"/instances/{instance_id}/snapshots"
 
     if wait:
         return make_api_call_and_wait_for_snapshot_completed("POST", path, instance_id)
-    else:
-        return make_api_call("POST", path)
+
+    return make_api_call("POST", path)
```

### Comparing `aura-cli-0.5.2/aura/snapshots/get.py` & `aura-cli-0.6.0/aura/snapshots/get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/snapshots/list.py` & `aura-cli-0.6.0/aura/snapshots/list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/snapshots/restore.py` & `aura-cli-0.6.0/aura/snapshots/restore.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 
     instance_id = get_instance_id(instance_id, instance_name)
 
     path = f"/instances/{instance_id}/snapshots/{snapshot_id}/restore"
 
     if wait:
         return make_api_call_and_wait_for_instance_status("POST", path, "running")
-    else:
-        return make_api_call("POST", path)
+
+    return make_api_call("POST", path)
```

### Comparing `aura-cli-0.5.2/aura/tenants/get.py` & `aura-cli-0.6.0/aura/tenants/get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/token_repository.py` & `aura-cli-0.6.0/aura/token_repository.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura/util/get_instance_id.py` & `aura-cli-0.6.0/aura/util/get_instance_id.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.5.2/aura_cli.egg-info/SOURCES.txt` & `aura-cli-0.6.0/aura_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 aura/config/valid_options.py
 aura/credentials/__init__.py
 aura/credentials/add.py
 aura/credentials/current.py
 aura/credentials/delete.py
 aura/credentials/list.py
 aura/credentials/use.py
+aura/data_apis/__init__.py
+aura/data_apis/create.py
+aura/data_apis/delete.py
+aura/data_apis/get.py
+aura/data_apis/list.py
+aura/data_apis/update.py
+aura/data_apis/util/__init__.py
+aura/data_apis/util/type_definitions.py
 aura/instances/__init__.py
 aura/instances/create.py
 aura/instances/delete.py
 aura/instances/get.py
 aura/instances/list.py
 aura/instances/overwrite.py
 aura/instances/pause.py
@@ -36,14 +44,15 @@
 aura/snapshots/__init__.py
 aura/snapshots/create.py
 aura/snapshots/get.py
 aura/snapshots/list.py
 aura/snapshots/restore.py
 aura/tenants/__init__.py
 aura/tenants/get.py
+aura/tenants/get_metrics_integration.py
 aura/tenants/list.py
 aura/util/__init__.py
 aura/util/get_instance_id.py
 aura_cli.egg-info/PKG-INFO
 aura_cli.egg-info/SOURCES.txt
 aura_cli.egg-info/dependency_links.txt
 aura_cli.egg-info/entry_points.txt
```

### Comparing `aura-cli-0.5.2/setup.py` & `aura-cli-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Load the version
 version = {}
 with open("aura/version.py") as f:
     exec(f.read(), version)
 
 setup(
     name="aura-cli",
-    version=version['__version__'],
+    version=version["__version__"],
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     tests_require=test_requirements,
     entry_points="""
         [console_scripts]
         aura=aura.aura:cli
     """,
-)
+)
```

