# Comparing `tmp/yellowdog_python_examples-7.8.7.tar.gz` & `tmp/yellowdog_python_examples-7.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog_python_examples-7.8.7.tar", last modified: Fri Apr 19 15:16:35 2024, max compression
+gzip compressed data, was "yellowdog_python_examples-7.8.8.tar", last modified: Tue Apr 23 10:28:15 2024, max compression
```

## Comparing `yellowdog_python_examples-7.8.7.tar` & `yellowdog_python_examples-7.8.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-19 15:16:35.022674 yellowdog_python_examples-7.8.7/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog_python_examples-7.8.7/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-19 15:16:35.022606 yellowdog_python_examples-7.8.7/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1442 2023-08-28 09:06:52.000000 yellowdog_python_examples-7.8.7/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   145815 2024-04-19 12:38:03.000000 yellowdog_python_examples-7.8.7/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     2140 2024-03-22 08:21:55.000000 yellowdog_python_examples-7.8.7/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)      242 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2024-04-19 15:16:35.022996 yellowdog_python_examples-7.8.7/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog_python_examples-7.8.7/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-19 15:16:34.995311 yellowdog_python_examples-7.8.7/tests/
--rw-r--r--   0 pwt        (501) staff       (20)     2092 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.7/tests/test_create_remove.py
--rw-r--r--   0 pwt        (501) staff       (20)     2636 2024-04-10 07:24:12.000000 yellowdog_python_examples-7.8.7/tests/test_demos.py
--rw-r--r--   0 pwt        (501) staff       (20)     6489 2024-04-10 07:24:12.000000 yellowdog_python_examples-7.8.7/tests/test_dryruns.py
--rw-r--r--   0 pwt        (501) staff       (20)     1656 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/tests/test_entrypoints.py
--rw-r--r--   0 pwt        (501) staff       (20)      604 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/tests/test_gui.py
--rw-r--r--   0 pwt        (501) staff       (20)     1705 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.7/tests/test_list.py
--rw-r--r--   0 pwt        (501) staff       (20)      857 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/tests/test_objects.py
--rw-r--r--   0 pwt        (501) staff       (20)     1683 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/tests/test_variable_processing.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-19 15:16:35.014699 yellowdog_python_examples-7.8.7/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2024-04-19 15:13:44.000000 yellowdog_python_examples-7.8.7/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4179 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.7/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2024-04-12 12:29:26.000000 yellowdog_python_examples-7.8.7/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    45683 2024-04-19 15:13:44.000000 yellowdog_python_examples-7.8.7/yd_commands/args.py
--rw-r--r--   0 pwt        (501) staff       (20)     1012 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/yd_commands/boost.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7489 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.7/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      607 2023-11-15 10:24:00.000000 yellowdog_python_examples-7.8.7/yd_commands/check_imports.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2502 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/yd_commands/cloudwizard.py
--rw-r--r--   0 pwt        (501) staff       (20)    38132 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_aws.py
--rw-r--r--   0 pwt        (501) staff       (20)      481 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_aws_types.py
--rw-r--r--   0 pwt        (501) staff       (20)    31534 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_azure.py
--rw-r--r--   0 pwt        (501) staff       (20)    13236 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_common.py
--rw-r--r--   0 pwt        (501) staff       (20)    12227 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_gcp.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2023-09-02 10:35:56.000000 yellowdog_python_examples-7.8.7/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)     3529 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.7/yd_commands/config_types.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    29810 2024-04-19 12:18:28.000000 yellowdog_python_examples-7.8.7/yd_commands/create.py
--rw-r--r--   0 pwt        (501) staff       (20)    14169 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.7/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2479 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4715 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.7/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      329 2023-09-04 08:20:55.000000 yellowdog_python_examples-7.8.7/yd_commands/follow.py
--rw-r--r--   0 pwt        (501) staff       (20)     3526 2024-02-26 11:02:40.000000 yellowdog_python_examples-7.8.7/yd_commands/follow_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1494 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/yd_commands/format_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      290 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.7/yd_commands/hold.py
--rw-r--r--   0 pwt        (501) staff       (20)      842 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/yd_commands/id_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    12170 2024-03-06 17:14:28.000000 yellowdog_python_examples-7.8.7/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     5247 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.7/yd_commands/interactive.py
--rw-r--r--   0 pwt        (501) staff       (20)     1007 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.7/yd_commands/items.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-09-02 10:35:56.000000 yellowdog_python_examples-7.8.7/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18484 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.7/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)    16141 2024-04-19 12:38:03.000000 yellowdog_python_examples-7.8.7/yd_commands/load_config.py
--rw-r--r--   0 pwt        (501) staff       (20)     3861 2024-03-22 10:21:47.000000 yellowdog_python_examples-7.8.7/yd_commands/load_resources.py
--rw-r--r--   0 pwt        (501) staff       (20)     8703 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.7/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)    32130 2024-04-17 11:01:34.000000 yellowdog_python_examples-7.8.7/yd_commands/printing.py
--rw-r--r--   0 pwt        (501) staff       (20)     5782 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.7/yd_commands/property_names.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17214 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.7/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     4748 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    14478 2024-04-19 12:38:03.000000 yellowdog_python_examples-7.8.7/yd_commands/remove.py
--rw-r--r--   0 pwt        (501) staff       (20)     5169 2023-09-04 08:20:55.000000 yellowdog_python_examples-7.8.7/yd_commands/resize.py
--rw-r--r--   0 pwt        (501) staff       (20)     3320 2024-04-19 12:18:28.000000 yellowdog_python_examples-7.8.7/yd_commands/settings.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4811 2024-02-27 14:55:53.000000 yellowdog_python_examples-7.8.7/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      298 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.7/yd_commands/start.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5072 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.7/yd_commands/start_hold_common.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    52170 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.7/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)    10015 2024-04-17 10:46:51.000000 yellowdog_python_examples-7.8.7/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4797 2024-02-27 14:55:53.000000 yellowdog_python_examples-7.8.7/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2023-11-24 13:35:57.000000 yellowdog_python_examples-7.8.7/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     5352 2023-11-18 08:50:59.000000 yellowdog_python_examples-7.8.7/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3615 2024-04-19 12:38:03.000000 yellowdog_python_examples-7.8.7/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     7279 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.7/yd_commands/utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2486 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.7/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    18416 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.7/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2024-02-26 11:02:40.000000 yellowdog_python_examples-7.8.7/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     3747 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.7/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-19 15:16:35.022233 yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-19 15:16:34.000000 yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1934 2024-04-19 15:16:34.000000 yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2024-04-19 15:16:34.000000 yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      860 2024-04-19 15:16:34.000000 yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)      253 2024-04-19 15:16:34.000000 yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2024-04-19 15:16:34.000000 yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-23 10:28:15.156833 yellowdog_python_examples-7.8.8/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog_python_examples-7.8.8/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-23 10:28:15.156746 yellowdog_python_examples-7.8.8/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1442 2023-08-28 09:06:52.000000 yellowdog_python_examples-7.8.8/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   145815 2024-04-19 12:38:03.000000 yellowdog_python_examples-7.8.8/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     2140 2024-03-22 08:21:55.000000 yellowdog_python_examples-7.8.8/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)      242 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2024-04-23 10:28:15.157153 yellowdog_python_examples-7.8.8/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog_python_examples-7.8.8/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-23 10:28:15.132102 yellowdog_python_examples-7.8.8/tests/
+-rw-r--r--   0 pwt        (501) staff       (20)     2092 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.8/tests/test_create_remove.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2636 2024-04-10 07:24:12.000000 yellowdog_python_examples-7.8.8/tests/test_demos.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6489 2024-04-10 07:24:12.000000 yellowdog_python_examples-7.8.8/tests/test_dryruns.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1656 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/tests/test_entrypoints.py
+-rw-r--r--   0 pwt        (501) staff       (20)      604 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/tests/test_gui.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1705 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.8/tests/test_list.py
+-rw-r--r--   0 pwt        (501) staff       (20)      857 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/tests/test_objects.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1683 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/tests/test_variable_processing.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-23 10:28:15.148643 yellowdog_python_examples-7.8.8/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2024-04-23 10:27:40.000000 yellowdog_python_examples-7.8.8/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4179 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.8/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2024-04-12 12:29:26.000000 yellowdog_python_examples-7.8.8/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    46055 2024-04-23 10:27:40.000000 yellowdog_python_examples-7.8.8/yd_commands/args.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1012 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/yd_commands/boost.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7489 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.8/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      607 2023-11-15 10:24:00.000000 yellowdog_python_examples-7.8.8/yd_commands/check_imports.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2502 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/yd_commands/cloudwizard.py
+-rw-r--r--   0 pwt        (501) staff       (20)    38132 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_aws.py
+-rw-r--r--   0 pwt        (501) staff       (20)      481 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_aws_types.py
+-rw-r--r--   0 pwt        (501) staff       (20)    31534 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_azure.py
+-rw-r--r--   0 pwt        (501) staff       (20)    13236 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_common.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12227 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_gcp.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2023-09-02 10:35:56.000000 yellowdog_python_examples-7.8.8/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3529 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.8/yd_commands/config_types.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    30081 2024-04-23 10:27:40.000000 yellowdog_python_examples-7.8.8/yd_commands/create.py
+-rw-r--r--   0 pwt        (501) staff       (20)    14169 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.8/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2479 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4715 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.8/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      329 2023-09-04 08:20:55.000000 yellowdog_python_examples-7.8.8/yd_commands/follow.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3526 2024-02-26 11:02:40.000000 yellowdog_python_examples-7.8.8/yd_commands/follow_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1494 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/yd_commands/format_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      290 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.8/yd_commands/hold.py
+-rw-r--r--   0 pwt        (501) staff       (20)      842 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/yd_commands/id_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    12170 2024-03-06 17:14:28.000000 yellowdog_python_examples-7.8.8/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5247 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.8/yd_commands/interactive.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1007 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.8/yd_commands/items.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-09-02 10:35:56.000000 yellowdog_python_examples-7.8.8/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18794 2024-04-23 10:27:40.000000 yellowdog_python_examples-7.8.8/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)    16141 2024-04-19 12:38:03.000000 yellowdog_python_examples-7.8.8/yd_commands/load_config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3861 2024-03-22 10:21:47.000000 yellowdog_python_examples-7.8.8/yd_commands/load_resources.py
+-rw-r--r--   0 pwt        (501) staff       (20)     8703 2024-03-26 08:47:18.000000 yellowdog_python_examples-7.8.8/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)    32130 2024-04-17 11:01:34.000000 yellowdog_python_examples-7.8.8/yd_commands/printing.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5782 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.8/yd_commands/property_names.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17214 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.8/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     4748 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    14580 2024-04-23 10:27:40.000000 yellowdog_python_examples-7.8.8/yd_commands/remove.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5169 2023-09-04 08:20:55.000000 yellowdog_python_examples-7.8.8/yd_commands/resize.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3320 2024-04-19 12:18:28.000000 yellowdog_python_examples-7.8.8/yd_commands/settings.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4811 2024-02-27 14:55:53.000000 yellowdog_python_examples-7.8.8/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      298 2024-02-12 09:16:25.000000 yellowdog_python_examples-7.8.8/yd_commands/start.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5072 2024-04-02 09:31:11.000000 yellowdog_python_examples-7.8.8/yd_commands/start_hold_common.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    52170 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.8/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)    10015 2024-04-17 10:46:51.000000 yellowdog_python_examples-7.8.8/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4797 2024-02-27 14:55:53.000000 yellowdog_python_examples-7.8.8/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2023-11-24 13:35:57.000000 yellowdog_python_examples-7.8.8/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5352 2023-11-18 08:50:59.000000 yellowdog_python_examples-7.8.8/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3615 2024-04-19 12:38:03.000000 yellowdog_python_examples-7.8.8/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     7279 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.8/yd_commands/utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2486 2024-03-18 08:22:49.000000 yellowdog_python_examples-7.8.8/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18416 2024-04-17 08:27:55.000000 yellowdog_python_examples-7.8.8/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2024-02-26 11:02:40.000000 yellowdog_python_examples-7.8.8/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3747 2024-02-08 14:04:26.000000 yellowdog_python_examples-7.8.8/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-23 10:28:15.156301 yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-23 10:28:15.000000 yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1934 2024-04-23 10:28:15.000000 yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2024-04-23 10:28:15.000000 yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      860 2024-04-23 10:28:15.000000 yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      253 2024-04-23 10:28:15.000000 yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2024-04-23 10:28:15.000000 yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog_python_examples-7.8.7/LICENSE` & `yellowdog_python_examples-7.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/PKG-INFO` & `yellowdog_python_examples-7.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 7.8.7
+Version: 7.8.8
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog_python_examples-7.8.7/PYPI_README.md` & `yellowdog_python_examples-7.8.8/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/README.md` & `yellowdog_python_examples-7.8.8/README.md`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/pyproject.toml` & `yellowdog_python_examples-7.8.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/setup.cfg` & `yellowdog_python_examples-7.8.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_create_remove.py` & `yellowdog_python_examples-7.8.8/tests/test_create_remove.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_demos.py` & `yellowdog_python_examples-7.8.8/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_dryruns.py` & `yellowdog_python_examples-7.8.8/tests/test_dryruns.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_entrypoints.py` & `yellowdog_python_examples-7.8.8/tests/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_gui.py` & `yellowdog_python_examples-7.8.8/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_list.py` & `yellowdog_python_examples-7.8.8/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_objects.py` & `yellowdog_python_examples-7.8.8/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/tests/test_variable_processing.py` & `yellowdog_python_examples-7.8.8/tests/test_variable_processing.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/abort.py` & `yellowdog_python_examples-7.8.8/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/admin.py` & `yellowdog_python_examples-7.8.8/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/args.py` & `yellowdog_python_examples-7.8.8/yd_commands/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,14 +513,20 @@
                 "--instances",
                 "-i",
                 action="store_true",
                 required=False,
                 help="list compute instances",
             )
             parser.add_argument(
+                "--public-ips-only",
+                action="store_true",
+                required=False,
+                help="when used with '--instances', lists public IP addresses only",
+            )
+            parser.add_argument(
                 "--allowances",
                 "-A",
                 action="store_true",
                 required=False,
                 help="list allowances",
             )
 
@@ -1415,14 +1421,19 @@
         return self.args.no_resequence
 
     @property
     @allow_missing_attribute
     def match_allowances_by_description(self) -> Optional[bool]:
         return self.args.match_allowances_by_description
 
+    @property
+    @allow_missing_attribute
+    def public_ips_only(self) -> Optional[bool]:
+        return self.args.public_ips_only
+
 
 def lookup_module_description(module_name: str) -> Optional[str]:
     """
     Descriptive string for the module's purpose.
     """
     prefix = "YellowDog command line utility for "
     suffix = None
```

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/boost.py` & `yellowdog_python_examples-7.8.8/yd_commands/boost.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/cancel.py` & `yellowdog_python_examples-7.8.8/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/check_imports.py` & `yellowdog_python_examples-7.8.8/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/cloudwizard.py` & `yellowdog_python_examples-7.8.8/yd_commands/cloudwizard.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_aws.py` & `yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_aws.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_azure.py` & `yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_azure.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_common.py` & `yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_common.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/cloudwizard_gcp.py` & `yellowdog_python_examples-7.8.8/yd_commands/cloudwizard_gcp.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/compact_json.py` & `yellowdog_python_examples-7.8.8/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/config_types.py` & `yellowdog_python_examples-7.8.8/yd_commands/config_types.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/create.py` & `yellowdog_python_examples-7.8.8/yd_commands/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -581,25 +581,32 @@
             worker_pool.name == name
             and worker_pool.type.split(".")[-1] == "ConfiguredWorkerPool"
             and worker_pool.status
             not in [WorkerPoolStatus.SHUTDOWN, WorkerPoolStatus.TERMINATED]
         ):
             print_log(
                 f"Existing Configured Worker Pool '{name}' ({worker_pool.status}) found"
-                " ... creation aborted"
+                " ... creation cancelled"
             )
             return
 
     try:
         cwp_request = _get_model_object("AddConfiguredWorkerPoolRequest", resource)
         cwp_response: AddConfiguredWorkerPoolResponse = (
             CLIENT.worker_pool_client.add_configured_worker_pool(cwp_request)
         )
         print_log(
-            f"Created Configured Worker Pool '{name}': Token = {cwp_response.token}"
+            f"Created Configured Worker Pool '{name}' ({cwp_response.workerPool.id})"
+        )
+        print_log(
+            f"                   Worker Pool Token = '{cwp_response.token.secret}'"
+        )
+        print_log(
+            "                   Worker Pool Expiry Time = "
+            f"{str(cwp_response.token.expiryTime).split('.')[0]}"
         )
         if ARGS_PARSER.quiet:
             print(cwp_response.workerPool.id)
     except Exception as e:
         print_error(f"Unable to created Configured Worker Pool '{name}': {e}")
```

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/csv_data.py` & `yellowdog_python_examples-7.8.8/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/delete.py` & `yellowdog_python_examples-7.8.8/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/download.py` & `yellowdog_python_examples-7.8.8/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/follow_utils.py` & `yellowdog_python_examples-7.8.8/yd_commands/follow_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/format_json.py` & `yellowdog_python_examples-7.8.8/yd_commands/format_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/id_utils.py` & `yellowdog_python_examples-7.8.8/yd_commands/id_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/instantiate.py` & `yellowdog_python_examples-7.8.8/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/interactive.py` & `yellowdog_python_examples-7.8.8/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/items.py` & `yellowdog_python_examples-7.8.8/yd_commands/items.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/jsonnet2json.py` & `yellowdog_python_examples-7.8.8/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/list.py` & `yellowdog_python_examples-7.8.8/yd_commands/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,14 +339,25 @@
     search_client: SearchClient = CLIENT.compute_client.get_instances(
         instance_search=instance_search
     )
     instances: List[Instance] = search_client.list_all()
     if len(instances) == 0:
         print_log("No instances to list")
         return
+
+    if ARGS_PARSER.public_ips_only:
+        print_log("Listing public IP addresses only:")
+        for instance in instances:
+            try:
+                if instance.publicIpAddress is not None:
+                    print(instance.publicIpAddress)
+            except:
+                pass
+        return
+
     if ARGS_PARSER.details:
         for instance in select(CLIENT, search_client.list_all()):
             print_yd_object(instance)
     else:
         print_numbered_object_list(CLIENT, search_client.list_all())
```

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/load_config.py` & `yellowdog_python_examples-7.8.8/yd_commands/load_config.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/load_resources.py` & `yellowdog_python_examples-7.8.8/yd_commands/load_resources.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/object_utilities.py` & `yellowdog_python_examples-7.8.8/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/printing.py` & `yellowdog_python_examples-7.8.8/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/property_names.py` & `yellowdog_python_examples-7.8.8/yd_commands/property_names.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/provision.py` & `yellowdog_python_examples-7.8.8/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/provision_utils.py` & `yellowdog_python_examples-7.8.8/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/remove.py` & `yellowdog_python_examples-7.8.8/yd_commands/remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,42 +290,46 @@
         print_error(f"Expected property to be defined ({e})")
         return
 
     worker_pools: List[WorkerPoolSummary] = (
         CLIENT.worker_pool_client.find_all_worker_pools()
     )
 
-    # Shut down all matching Configured Worker Pools in appropriate states.
+    # Shut down a matching Configured Worker Pool if in an appropriate state
     for worker_pool in worker_pools:
         if (
             worker_pool.name == name
             and worker_pool.type.split(".")[-1] == "ConfiguredWorkerPool"
         ):
             if worker_pool.status not in [
                 WorkerPoolStatus.SHUTDOWN,
                 WorkerPoolStatus.TERMINATED,
             ]:
                 if not confirmed(
                     f"Shut down Configured Worker Pool '{worker_pool.name}'"
                     f" ({worker_pool.id})?"
                 ):
-                    continue
+                    break
                 try:
                     CLIENT.worker_pool_client.shutdown_worker_pool_by_id(worker_pool.id)
                     print_log(
                         f"Shutting down [{worker_pool.status}] Configured Worker Pool"
                         f" '{name}' ({worker_pool.id})"
                     )
+                    return
                 except Exception as e:
                     print_error(f"Failed to shut down Configured Worker Pool: {e}")
             else:
                 print_log(
                     f"Not shutting down [{worker_pool.status}] Configured Worker Pool"
                     f" '{name}' ({worker_pool.id})"
                 )
+                return
+
+    print_log("No Configured Worker Pool shut down")
 
 
 def remove_allowance(resource: Dict):
     """
     Remove an allowance, matching on the 'description' property.
     """
     description = resource.get("description", None)
```

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/resize.py` & `yellowdog_python_examples-7.8.8/yd_commands/resize.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/settings.py` & `yellowdog_python_examples-7.8.8/yd_commands/settings.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/shutdown.py` & `yellowdog_python_examples-7.8.8/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/start_hold_common.py` & `yellowdog_python_examples-7.8.8/yd_commands/start_hold_common.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/submit.py` & `yellowdog_python_examples-7.8.8/yd_commands/submit.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/submit_utils.py` & `yellowdog_python_examples-7.8.8/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/terminate.py` & `yellowdog_python_examples-7.8.8/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/type_check.py` & `yellowdog_python_examples-7.8.8/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/upload.py` & `yellowdog_python_examples-7.8.8/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/upload_utils.py` & `yellowdog_python_examples-7.8.8/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/utils.py` & `yellowdog_python_examples-7.8.8/yd_commands/utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/validate_properties.py` & `yellowdog_python_examples-7.8.8/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/variables.py` & `yellowdog_python_examples-7.8.8/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/version.py` & `yellowdog_python_examples-7.8.8/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yd_commands/wrapper.py` & `yellowdog_python_examples-7.8.8/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 7.8.7
+Version: 7.8.8
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog_python_examples-7.8.7/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog_python_examples-7.8.8/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

