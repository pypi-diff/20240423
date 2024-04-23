# Comparing `tmp/datalake-scripts-2.7.2.tar.gz` & `tmp/datalake-scripts-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalake-scripts-2.7.2.tar", last modified: Tue Jan 16 10:06:43 2024, max compression
+gzip compressed data, was "datalake-scripts-2.7.3.tar", last modified: Tue Apr 23 14:50:14 2024, max compression
```

## Comparing `datalake-scripts-2.7.2.tar` & `datalake-scripts-2.7.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.974719 datalake-scripts-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-01-16 10:06:43.974719 datalake-scripts-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.962719 datalake-scripts-2.7.2/datalake/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.962719 datalake-scripts-2.7.2/datalake/api_objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/api_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/api_objects/bulk_search_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.962719 datalake-scripts-2.7.2/datalake/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/atom_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/throttler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/common/warn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/datalake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.962719 datalake-scripts-2.7.2/datalake/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/bulk_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/filtered_tag_subcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/sightings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    20320 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/endpoints/threats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.966719 datalake-scripts-2.7.2/datalake/miscellaneous/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/miscellaneous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake/miscellaneous/search_watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.966719 datalake-scripts-2.7.2/datalake_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.966719 datalake-scripts-2.7.2/datalake_scripts/common/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/common/base_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/common/base_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/common/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.966719 datalake-scripts-2.7.2/datalake_scripts/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/engines/get_engine.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6136 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/engines/post_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.966719 datalake-scripts-2.7.2/datalake_scripts/helper_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/helper_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/helper_scripts/output_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/helper_scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.970719 datalake-scripts-2.7.2/datalake_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/add_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/add_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/add_threats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/advanced_search.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8317 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/bulk_lookup_threats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/edit_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/get_atom_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/get_filtered_tag_subcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/get_query_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/get_threats_by_hashkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/get_threats_from_query_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/lookup_threats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3569 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/datalake_scripts/scripts/search_watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.974719 datalake-scripts-2.7.2/datalake_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-01-16 10:06:43.000000 datalake-scripts-2.7.2/datalake_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-16 10:06:43.000000 datalake-scripts-2.7.2/datalake_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 10:06:43.000000 datalake-scripts-2.7.2/datalake_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-16 10:06:43.000000 datalake-scripts-2.7.2/datalake_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-16 10:06:43.000000 datalake-scripts-2.7.2/datalake_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-16 10:06:43.000000 datalake-scripts-2.7.2/datalake_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-16 10:06:43.974719 datalake-scripts-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.970719 datalake-scripts-2.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.970719 datalake-scripts-2.7.2/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/common/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/common/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/common/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.970719 datalake-scripts-2.7.2/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_atom_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_auth_via_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_bulk_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_filtered_tag_subcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10402 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_search_watch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_sightings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    27933 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/lib/test_threats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:43.974719 datalake-scripts-2.7.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/scripts/test_add_new_threats.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/scripts/test_base_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/scripts/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/scripts/test_csv_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-16 10:06:33.000000 datalake-scripts-2.7.2/tests/scripts/test_endpoint_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.618767 datalake-scripts-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-23 14:50:14.618767 datalake-scripts-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.606768 datalake-scripts-2.7.3/datalake/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.606768 datalake-scripts-2.7.3/datalake/api_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/api_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/api_objects/bulk_search_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.606768 datalake-scripts-2.7.3/datalake/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/atom_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/throttler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/common/warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/datalake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.606768 datalake-scripts-2.7.3/datalake/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/bulk_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/filtered_tag_subcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/sightings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20320 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/endpoints/threats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.606768 datalake-scripts-2.7.3/datalake/miscellaneous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/miscellaneous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake/miscellaneous/search_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.610767 datalake-scripts-2.7.3/datalake_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.610767 datalake-scripts-2.7.3/datalake_scripts/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/common/base_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/common/base_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/common/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.610767 datalake-scripts-2.7.3/datalake_scripts/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/engines/get_engine.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6136 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/engines/post_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.610767 datalake-scripts-2.7.3/datalake_scripts/helper_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/helper_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/helper_scripts/output_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/helper_scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.610767 datalake-scripts-2.7.3/datalake_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/add_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/add_threats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/advanced_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8317 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/bulk_lookup_threats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/edit_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/get_atom_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/get_filtered_tag_subcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/get_query_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/get_threats_by_hashkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/get_threats_from_query_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/lookup_threats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3569 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/datalake_scripts/scripts/search_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.614767 datalake-scripts-2.7.3/datalake_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-23 14:50:14.000000 datalake-scripts-2.7.3/datalake_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-23 14:50:14.000000 datalake-scripts-2.7.3/datalake_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:50:14.000000 datalake-scripts-2.7.3/datalake_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-23 14:50:14.000000 datalake-scripts-2.7.3/datalake_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 14:50:14.000000 datalake-scripts-2.7.3/datalake_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 14:50:14.000000 datalake-scripts-2.7.3/datalake_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 14:50:14.618767 datalake-scripts-2.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.610767 datalake-scripts-2.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.614767 datalake-scripts-2.7.3/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/common/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/common/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/common/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.614767 datalake-scripts-2.7.3/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_atom_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_auth_via_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_bulk_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_filtered_tag_subcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10402 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_search_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_sightings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27933 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/lib/test_threats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:14.614767 datalake-scripts-2.7.3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/scripts/test_add_new_threats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/scripts/test_base_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/scripts/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/scripts/test_csv_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-23 14:50:00.000000 datalake-scripts-2.7.3/tests/scripts/test_endpoint_config.py
```

### Comparing `datalake-scripts-2.7.2/PKG-INFO` & `datalake-scripts-2.7.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: datalake-scripts
-Version: 2.7.2
-Summary: A collection of scripts to easily use the API of OCD Datalake
-Home-page: https://github.com/cert-orangecyberdefense/datalake/
-Author: OCD
-Author-email: cert-contact.ocd@orange.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Environment :: Console
-Classifier: Topic :: Security
-Classifier: Natural Language :: English
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 
      ____        _        _       _          ____            _       _ 
     |  _ \  __ _| |_ __ _| | __ _| | _____  / ___|  ___ _ __(_)_ __ | |_ ___
     | | | |/ _` | __/ _` | |/ _` | |/ / _ \ \___ \ / __| '__| | '_ \| __/ __|
     | |_| | (_| | || (_| | | (_| |   <  __/  ___) | (__| |  | | |_) | |_\__ \
     |____/ \__,_|\__\__,_|_|\__,_|_|\_\___| |____/ \___|_|  |_| .__/ \__|___/
                                                               |_|
@@ -53,18 +33,28 @@
 You can also use a script directly by using the following command: `<script_name> <script_options>`.
 
 > /!\ Make sure to use utf-8 **without BOM** when providing a file (-i option)
 
 ## Environment variables
 
 #### Authentication
-In case you don't want to enter credential for each commands and you are on a secured terminal, set those variables:  
+
+There are two methods of authentication:
+- The first one is the use of the username and password. Every request to the API, will then use fresh tokens periodically created with these credentials.
+- The second one is the use of a long term token. You can create long term token through the GUI, it can have more restricted permissions than your account. You can create several long term tokens for one account. 
+
+In case you don't want to enter credentials for each commands and you are on a secured terminal, set those variables:  
+* `OCD_DTL_LONGTERM_TOKEN` a long term token associated to your Datalake account.
+Please note that if this variable is set, then the long term token will be used for every request to the Datalake API, even if you set the username and passsword environment variables below. This is important because some endpoints / requests do not accept long term tokens but need fresh tokens (ie a Datalake instance with username and password). Check for the need of fresh tokens in each endpoint description [here](https://datalake.cert.orangecyberdefense.com/api/v2/docs/)
+
+or
+
 * `OCD_DTL_USERNAME` email address used to login on Datalake API/GUI.   
 * `OCD_DTL_PASSWORD` password used to login on Datalake API/GUI.
-> They are independent and one can be used without the other if you wish.
+> These last two are independent and one can be used without the other if you wish.
 
 #### Throttling
 For throttling the request, those two environment variable can be used:  
 * `OCD_DTL_QUOTA_TIME` define, in seconds, the time before resetting the requests limit, *default is 1 second*.   
 * `OCD_DTL_REQUESTS_PER_QUOTA_TIME` define the number of request to do at maximum for the given time,  *default is 5 queries*.
 
 > Please don't exceed the quota marked [here](https://datalake.cert.orangecyberdefense.com/api/v2/docs/) for each endpoint
@@ -78,9 +68,8 @@
 > -q will quiet the verbosity of the program (but still show errors / warnings)  
 
 For information about each command and more, please check [the documentation directory](https://github.com/cert-orangecyberdefense/datalake/tree/master/docs)
 
 
 ### Contributing
 
-To develop on this repository, please refer to [this file](https://github.com/cert-orangecyberdefense/datalake/tree/master/CONTRIBUTING.md) 
-
+To develop on this repository, please refer to [this file](https://github.com/cert-orangecyberdefense/datalake/tree/master/CONTRIBUTING.md)
```

### Comparing `datalake-scripts-2.7.2/datalake/__init__.py` & `datalake-scripts-2.7.3/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/api_objects/bulk_search_task.py` & `datalake-scripts-2.7.3/datalake/api_objects/bulk_search_task.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/common/atom.py` & `datalake-scripts-2.7.3/datalake/common/atom.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/common/atom_type.py` & `datalake-scripts-2.7.3/datalake/common/atom_type.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/common/output.py` & `datalake-scripts-2.7.3/datalake/common/output.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/common/throttler.py` & `datalake-scripts-2.7.3/datalake/common/throttler.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/common/utils.py` & `datalake-scripts-2.7.3/datalake/common/utils.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/datalake.py` & `datalake-scripts-2.7.3/datalake/datalake.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,38 @@
 
 
 class Datalake:
     """Entrypoint to the Datalake library
 
     Usage:
     >>> dtl = Datalake(username='some username', password='some password')
+    or
+    >>> dtl = Datalake(longterm_token='some longterm token')
+    then
     >>> dtl.Threats.lookup(atom_value='mayoclinic.org', atom_type=AtomType.DOMAIN, hashkey_only=False)
+
     """
 
     def __init__(
         self,
         username: str = None,
         password: str = None,
+        longterm_token: str = None,
         env="prod",
         log_level=logging.WARNING,
     ):
         configure_logging(log_level)
         endpoint_config = Config().load_config()
         try:
             token_manager = TokenManager(
-                endpoint_config, environment=env, username=username, password=password
+                endpoint_config,
+                environment=env,
+                username=username,
+                password=password,
+                longterm_token=longterm_token,
             )
         except Exception as e:
             if "Failed to resolve" in str(e) or "Failed to establish" in str(e):
                 raise ConnectionError(
                     "Unable to access Datalake. Please check your network settings/connection"
                 )
             else:
```

### Comparing `datalake-scripts-2.7.2/datalake/endpoints/advanced_search.py` & `datalake-scripts-2.7.3/datalake/endpoints/advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/endpoints/bulk_search.py` & `datalake-scripts-2.7.3/datalake/endpoints/bulk_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/endpoints/endpoint.py` & `datalake-scripts-2.7.3/datalake/endpoints/endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,27 +61,29 @@
     ) -> Response:
         """
         Use it to request the API
         """
         tries_left = self.SET_MAX_RETRY
 
         while tries_left > 0:
-            headers["Authorization"] = self.token_manager.access_token
+            headers["Authorization"] = (
+                self.token_manager.access_token or self.token_manager.longterm_token
+            )
             logger.debug(self._pretty_debug_request(url, method, post_body, headers))
 
             response = self._send_request(
                 url, method, headers, post_body, stream=stream
             )
 
             if logger.isEnabledFor(logging.DEBUG):
                 # Don't compute response.text var if not needed, especially for streaming response
                 logger.debug("API response:\n%s", response.text)
             if response.status_code == 401:
                 logger.warning(
-                    "Token expired or Missing authorization header. Updating token"
+                    "Missing authorization header or Token Error. Updating token"
                 )
                 self.token_manager.process_auth_error(response.json())
             elif response.status_code == 422:
                 json_resp = response.json()
                 try:
                     error_msg = get_error_message(json_resp)
                 except ValueError:
@@ -144,14 +146,15 @@
             + "DEBUG - datalake_requests:\n"
             + f" - url: \n{url}\n"
             + f" - method: \n{method}\n"
             + f" - headers: \n{headers}\n"
             + f" - data: \n{data}\n"
             + f" - token: \n{self.token_manager.access_token}\n"
             + f" - refresh_token: \n{self.token_manager.refresh_token}\n"
+            + f" - longterm_token: \n{self.token_manager.longterm_token}\n"
             + "-" * self.terminal_size
         )
         return debug
 
     def _build_url_for_endpoint(self, endpoint_name):
         base_url = urljoin(
             self.endpoint_config["main"][self.environment],
```

### Comparing `datalake-scripts-2.7.2/datalake/endpoints/filtered_tag_subcategory.py` & `datalake-scripts-2.7.3/datalake/endpoints/filtered_tag_subcategory.py`

 * *Files 17% similar despite different names*

```diff
@@ -69,12 +69,23 @@
                 )
             limit_match = re.search(
                 r"Must be greater than or equal to 0 and less than or equal to 5000",
                 error_message,
             )
             if limit_match:
                 print("The 'limit' parameter must be >= 0 and <= 5000.")
-            if not tag_category_match and not ordering_match and not limit_match:
+            token_match = re.search(
+                r"token",
+                error_message,
+            )
+            if token_match:
+                raise ve
+            if (
+                not tag_category_match
+                and not ordering_match
+                and not limit_match
+                and not token_match
+            ):
                 print(
                     "An error occurred, but no specific pattern was matched in the 422 HTTP error message."
                 )
             sys.exit(1)
```

### Comparing `datalake-scripts-2.7.2/datalake/endpoints/sightings.py` & `datalake-scripts-2.7.3/datalake/endpoints/sightings.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/endpoints/tags.py` & `datalake-scripts-2.7.3/datalake/endpoints/tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/endpoints/threats.py` & `datalake-scripts-2.7.3/datalake/endpoints/threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake/miscellaneous/search_watch.py` & `datalake-scripts-2.7.3/datalake/miscellaneous/search_watch.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/cli.py` & `datalake-scripts-2.7.3/datalake_scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     get_filtered_tag_subcategory,
     search_watch,
 )
 
 
 class Cli:
     CLI_NAME = "ocd-dtl"
-    VERSION = "2.7.2"
+    VERSION = "2.7.3"
 
     def __init__(self):
         parser = argparse.ArgumentParser(
             description="Cli to interact with OCD's Datalake",
             usage=f"{self.CLI_NAME} <command> [<args>]",
         )
         parser.add_argument(
```

### Comparing `datalake-scripts-2.7.2/datalake_scripts/common/__init__.py` & `datalake-scripts-2.7.3/datalake_scripts/common/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/common/base_engine.py` & `datalake-scripts-2.7.3/datalake_scripts/common/base_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,16 @@
         self, url: str, method: str, headers: dict, post_body: dict = None
     ):
         """
         Wrapper around the new datalake_requests to keep compatibility with old scrips
         """
         try:
             response = self.endpoint.datalake_requests(url, method, headers, post_body)
-        except ValueError:
+        except ValueError as ve:
+            logger.error(f"Error while attempting to request datalake : {ve}")
             logger.error("Request failed: Will return nothing for this request")
             return {}
         if (
             "Content-Type" in response.headers
             and "text/csv" in response.headers["Content-Type"]
         ):
             return response.text
```

### Comparing `datalake-scripts-2.7.2/datalake_scripts/common/base_script.py` & `datalake-scripts-2.7.3/datalake_scripts/common/base_script.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/common/mixins.py` & `datalake-scripts-2.7.3/datalake_scripts/common/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,18 @@
             spinner.start()
 
         start_time = time()
         back_off_time = 1
 
         json_response = None
         while not json_response:
-            headers = {"Authorization": self.token_manager.access_token}
+            headers = {
+                "Authorization": self.token_manager.access_token
+                or self.token_manager.longterm_token
+            }
             response = requests.get(
                 url=retrieve_bulk_result_url,
                 headers=headers,
                 verify=self.requests_ssl_verify,
             )
             if response.status_code == 200:
                 potential_json_response = response.json()
```

### Comparing `datalake-scripts-2.7.2/datalake_scripts/engines/get_engine.py` & `datalake-scripts-2.7.3/datalake_scripts/engines/get_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/engines/post_engine.py` & `datalake-scripts-2.7.3/datalake_scripts/engines/post_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/helper_scripts/output_builder.py` & `datalake-scripts-2.7.3/datalake_scripts/helper_scripts/output_builder.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/helper_scripts/utils.py` & `datalake-scripts-2.7.3/datalake_scripts/helper_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/add_comments.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/add_comments.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/add_tags.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/add_tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/add_threats.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/add_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/advanced_search.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/bulk_lookup_threats.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/bulk_lookup_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/edit_score.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/edit_score.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/get_atom_values.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/get_atom_values.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/get_filtered_tag_subcategory.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/get_filtered_tag_subcategory.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/get_query_hash.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/get_query_hash.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/get_threats_by_hashkey.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/get_threats_by_hashkey.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/get_threats_from_query_hash.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/get_threats_from_query_hash.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/lookup_threats.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/lookup_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts/scripts/search_watch.py` & `datalake-scripts-2.7.3/datalake_scripts/scripts/search_watch.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/datalake_scripts.egg-info/SOURCES.txt` & `datalake-scripts-2.7.3/datalake_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/setup.py` & `datalake-scripts-2.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/common/fixture.py` & `datalake-scripts-2.7.3/tests/common/fixture.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,7 +45,13 @@
 def datalake():
     url = "https://datalake.cert.orangecyberdefense.com/api/v2/auth/token/"
 
     auth_response = {"access_token": "12345", "refresh_token": "123456"}
 
     responses.add(responses.POST, url, json=auth_response, status=200)
     return Datalake(username="username", password="password")
+
+
+@pytest.fixture
+@responses.activate
+def datalake_longterm_token():
+    return Datalake(longterm_token="longterm_token1234")
```

### Comparing `datalake-scripts-2.7.2/tests/common/test_output.py` & `datalake-scripts-2.7.3/tests/common/test_output.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/common/test_utils.py` & `datalake-scripts-2.7.3/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_advanced_search.py` & `datalake-scripts-2.7.3/tests/lib/test_advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_atom_type.py` & `datalake-scripts-2.7.3/tests/lib/test_atom_type.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_auth_via_tokens.py` & `datalake-scripts-2.7.3/datalake/common/token_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,181 +1,147 @@
+"""
+Token manager will manage tokens for the scripts.
+"""
 import json
-import logging
-from functools import partial
-
-import pytest
-import responses
-
-from datalake import Datalake, AtomType
-from tests.common.fixture import datalake  # noqa needed fixture import
-
-
-@responses.activate
-def test_token_auth(datalake):
-    expected_tokens = {
-        "access_token": "12345",
-        "refresh_token": "123456",
-    }
-
-    token_manager = datalake.Threats.token_manager
-
-    assert token_manager.access_token == f"Token {expected_tokens['access_token']}"
-    assert token_manager.refresh_token == f"Token {expected_tokens['refresh_token']}"
-
-
-@responses.activate
-def test_invalid_credentials(caplog):
-    url = "https://datalake.cert.orangecyberdefense.com/api/v2/auth/token/"
-
-    api_error_msg = "Wrong credentials provided"
-    api_response = {"message": api_error_msg}
-    responses.add(responses.POST, url, json=api_response, status=401)
-    with caplog.at_level(logging.ERROR):
-        with pytest.raises(ValueError) as ve:
-            Datalake(username="username@wow.com", password="password")
-    assert str(ve.value) == f'Could not login: {{"message": "{api_error_msg}"}}'
-    assert caplog.messages == [
-        f"An error occurred while retrieving an access token, for URL: {url}\n"
-        f'response of the API: {{"message": "{api_error_msg}"}}'
-    ]
-
-
-def lookup_callback(
-    request,
-    expired_token,
-    valid_token,
-    response_on_valid_token,
-    response_on_expired_token=None,
-):
-    headers = {}
-    if not response_on_expired_token:
-        response_on_expired_token = {"msg": "Token has expired"}  # Default value
-    if request.headers["Authorization"] == f"Token {expired_token}":
-        return 401, headers, json.dumps(response_on_expired_token)
-    elif request.headers["Authorization"] == f"Token {valid_token}":
-        return 200, headers, json.dumps(response_on_valid_token)
-    else:
-        raise Exception()
-
-
-@responses.activate
-def test_access_token_expired(datalake, caplog):
-    caplog.set_level(level=logging.INFO, logger="OCD_DTL")
-    expected_json = {"wow.com": "bad"}
-
-    responses.add_callback(
-        responses.GET,
-        "https://datalake.cert.orangecyberdefense.com/api/v2/mrti/threats/lookup/",
-        callback=partial(
-            lookup_callback,
-            expired_token="12345",
-            valid_token="refreshed_token",
-            response_on_valid_token=expected_json,
-        ),
-        content_type="application/json",
-    )
-
-    def refresh_token_callback(request):
-        headers = {}
-        assert (
-            request.headers["Authorization"] == "Token 123456"
-        ), "token passed is not the refresh token"
-        return 200, headers, json.dumps({"access_token": "refreshed_token"})
-
-    responses.add_callback(
-        responses.POST,
-        "https://datalake.cert.orangecyberdefense.com/api/v2/auth/refresh-token/",
-        callback=refresh_token_callback,
-        content_type="application/json",
-    )
-
-    assert (
-        datalake.Threats.lookup(atom_value="wow.com", atom_type=AtomType.DOMAIN)
-        == expected_json
-    )
-    assert caplog.messages == [
-        "Token expired or Missing authorization header. Updating token"
-    ]
-
-
-@responses.activate
-def test_refresh_token_expired(datalake, caplog):
-    caplog.set_level(level=logging.INFO, logger="OCD_DTL")
-    expected_json = {"wow.com": "bad"}
-
-    responses.add_callback(
-        responses.GET,
-        "https://datalake.cert.orangecyberdefense.com/api/v2/mrti/threats/lookup/",
-        callback=partial(
-            lookup_callback,
-            expired_token="12345",
-            valid_token="new_token",
-            response_on_valid_token=expected_json,
-        ),
-        content_type="application/json",
-    )
-
-    def refresh_token_callback(request):
-        headers = {}
-        assert (
-            request.headers["Authorization"] == "Token 123456"
-        ), "token passed is not the refresh token"
-        return 401, headers, json.dumps({"msg": "Token has expired"})
-
-    responses.add_callback(
-        responses.POST,
-        "https://datalake.cert.orangecyberdefense.com/api/v2/auth/refresh-token/",
-        callback=refresh_token_callback,
-        content_type="application/json",
-    )
-    responses.post(
-        url="https://datalake.cert.orangecyberdefense.com/api/v2/auth/token/",
-        json={"access_token": "new_token", "refresh_token": ""},
-        status=200,
-    )
-
-    assert (
-        datalake.Threats.lookup(atom_value="wow.com", atom_type=AtomType.DOMAIN)
-        == expected_json
-    )
-    assert caplog.messages == [
-        "Token expired or Missing authorization header. Updating token",
-        "Refreshing the refresh token",
-    ]
-
-
-@responses.activate
-def test_invalid_token(datalake, caplog):
-    expected_json = {"wow.com": "bad"}
-    invalid_access_token = "not-valid-token"
-    valid_access_token = "valid_token"
-
-    responses.add_callback(
-        responses.GET,
-        "https://datalake.cert.orangecyberdefense.com/api/v2/mrti/threats/lookup/",
-        callback=partial(
-            lookup_callback,
-            expired_token=invalid_access_token,
-            valid_token=valid_access_token,
-            response_on_valid_token=expected_json,
-            response_on_expired_token={
-                "msg": "Missing 'Token' type in 'Authorization' header. Expected 'Authorization: Token <JWT>'"
-            },
-        ),
-        content_type="application/json",
-    )
-
-    responses.post(
-        "https://datalake.cert.orangecyberdefense.com/api/v2/auth/token/",
-        json={"access_token": valid_access_token, "refresh_token": ""},
-        content_type="application/json",
-    )
-
-    datalake.Threats.token_manager.access_token = f"Token {invalid_access_token}"
-
-    assert (
-        datalake.Threats.lookup(atom_value="wow.com", atom_type=AtomType.DOMAIN)
-        == expected_json
-    )
-    assert caplog.messages == [
-        "Token expired or Missing authorization header. Updating token"
-    ]
+import os
+from getpass import getpass
+from urllib.parse import urljoin
+
+import requests
+
+from datalake.common.logger import logger
+from datalake.common.utils import get_error_message
+
+
+class TokenManager:
+    """
+    Use it to generate token access to the API
+    """
+
+    def __init__(
+        self,
+        endpoint_config: dict,
+        *,
+        environment: str,
+        username=None,
+        password=None,
+        longterm_token=None,
+    ):
+        """environment can be either prod or preprod"""
+        base_url = urljoin(
+            endpoint_config["main"][environment], endpoint_config["api_version"]
+        )
+        endpoints = endpoint_config["endpoints"]
+
+        self.url_token = urljoin(base_url, endpoints["token"], allow_fragments=True)
+        self.url_refresh = urljoin(
+            base_url, endpoints["refresh_token"], allow_fragments=True
+        )
+
+        self.username = username
+        self.password = password
+        self.longterm_token = longterm_token
+        self.access_token = None
+        self.refresh_token = None
+        self.get_token()
+
+    def get_token(self):
+        """
+        Generate token from user input
+         by default, we use the values given as args,
+         then in second choice, we try the environment variables,
+         and finally we ask for user input
+         Priority is given to the long term token if it is provided at the same place (args, environment variable or prompt) than the username/password )
+        """
+        if self.username is None and self.password is None:
+            """We do not ignore the values username and password in favor of long term token if the two credentials are given explicitly when instancing Datalake"""
+            self.longterm_token = self.longterm_token or os.getenv(
+                "OCD_DTL_LONGTERM_TOKEN"
+            )
+
+        self.username = self.username or os.getenv("OCD_DTL_USERNAME")
+        self.password = self.password or os.getenv("OCD_DTL_PASSWORD")
+
+        if self.longterm_token is None and (
+            self.username is None or self.password is None
+        ):
+            """I only ask in prompt if no other choice"""
+            self.username = self.username or input("Email: ")
+            self.password = self.password or getpass()
+            self.longterm_token = self.longterm_token or input(
+                "Long term token (Default : None): "
+            )
+            print()
+
+        if self.longterm_token:
+            self.longterm_token = f"Token {self.longterm_token}"
+            if self.username or self.password:
+                logger.warning(
+                    f"Using provided Long Term Token for Authentication to the Datalake API. Ignoring username and/or password."
+                )
+        else:
+            data = {"email": self.username, "password": self.password}
+
+            response = requests.post(url=self.url_token, json=data)
+            json_response = json.loads(response.text)
+            try:
+                self.access_token = f'Token {json_response["access_token"]}'
+                self.refresh_token = f'Token {json_response["refresh_token"]}'
+            except KeyError:
+                logger.error(
+                    f"An error occurred while retrieving an access token, for URL: {self.url_token}\n"
+                    f"response of the API: {response.text}"
+                )
+                raise ValueError(f"Could not login: {response.text}")
+
+    def fetch_new_token(self):
+        logger.debug("Token will be refreshed")
+        headers = {"Authorization": self.refresh_token}
+        response = requests.post(url=self.url_refresh, headers=headers)
+
+        json_response = response.json()
+        if (
+            response.status_code == 401
+            and json_response.get("msg") == "Token has expired"
+        ):
+            logger.info("Refreshing the refresh token")
+            # Refresh token is also expired, we need to restart the authentication from scratch
+            self.get_token()
+        elif "access_token" in json_response:
+            self.access_token = f'Token {json_response["access_token"]}'
+        else:  # an error occurred
+            logger.error(
+                f"An error occurred while refreshing the refresh token, for URL: {self.url_refresh}\n"
+                f"response of the API: {response.text}"
+            )
+            raise ValueError(f"Could not refresh the token: {response.text}")
+
+    def process_auth_error(self, json_resp: dict):
+        """
+        Allow to update token when API response is either Missing Authorization Header or Token has expired.
+        """
+        error_msg = get_error_message(json_resp)
+        if error_msg in (
+            "Missing Authorization Header",
+            "Bad Authorization header. Expected value 'Token <JWT>'",
+            "Missing 'Token' type in 'Authorization' header. Expected 'Authorization: Token <JWT>'",
+        ):
+            self.get_token()
+        elif error_msg == "Token has expired":
+            if self.longterm_token:
+                raise ValueError(f"Long term token has expired")
+            else:
+                self.fetch_new_token()
+        elif error_msg == "Token has been revoked":
+            raise ValueError(f"Long term token has been revoked")
+        elif error_msg == "Fresh token required":
+            raise ValueError(
+                f"You cannot use Long term token with this endpoint, please use only the credentials username and password to init the Datalake instance for this request"
+            )
+        elif (
+            error_msg
+            in ("Invalid token", "Not enough segments", "Signature verification failed")
+            and self.longterm_token
+        ):
+            raise ValueError(f"Long term token is invalid")
+        else:
+            raise ValueError(f"Unexpected msg: {error_msg}")
```

### Comparing `datalake-scripts-2.7.2/tests/lib/test_bulk_search.py` & `datalake-scripts-2.7.3/tests/lib/test_bulk_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_filtered_tag_subcategory.py` & `datalake-scripts-2.7.3/tests/lib/test_filtered_tag_subcategory.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_search_watch.py` & `datalake-scripts-2.7.3/tests/lib/test_search_watch.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_sightings.py` & `datalake-scripts-2.7.3/tests/lib/test_sightings.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_tags.py` & `datalake-scripts-2.7.3/tests/lib/test_tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/lib/test_threats.py` & `datalake-scripts-2.7.3/tests/lib/test_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/scripts/test_add_new_threats.py` & `datalake-scripts-2.7.3/tests/scripts/test_add_new_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/scripts/test_base_engine.py` & `datalake-scripts-2.7.3/tests/scripts/test_base_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/scripts/test_cli.py` & `datalake-scripts-2.7.3/tests/scripts/test_cli.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/scripts/test_csv_builder.py` & `datalake-scripts-2.7.3/tests/scripts/test_csv_builder.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.7.2/tests/scripts/test_endpoint_config.py` & `datalake-scripts-2.7.3/tests/scripts/test_endpoint_config.py`

 * *Files identical despite different names*

