# Comparing `tmp/dsms_sdk-1.4.0rc7.tar.gz` & `tmp/dsms_sdk-1.4.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsms_sdk-1.4.0rc7.tar", last modified: Fri Apr 19 01:23:47 2024, max compression
+gzip compressed data, was "dsms_sdk-1.4.0rc8.tar", last modified: Tue Apr 23 00:32:22 2024, max compression
```

## Comparing `dsms_sdk-1.4.0rc7.tar` & `dsms_sdk-1.4.0rc8.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.859026 dsms_sdk-1.4.0rc7/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 01:23:47.859026 dsms_sdk-1.4.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.847026 dsms_sdk-1.4.0rc7/dsms/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.847026 dsms_sdk-1.4.0rc7/dsms/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/apps/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.851026 dsms_sdk-1.4.0rc7/dsms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/core/dsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.851026 dsms_sdk-1.4.0rc7/dsms/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16352 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/ktype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.851026 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/affiliations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.851026 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/custom_datatype/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/custom_datatype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/custom_datatype/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/linked_kitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/properties/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.851026 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.851026 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.855026 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/sparql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.855026 dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/sparql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/dsms/knowledge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.855026 dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 01:23:47.000000 dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-19 01:23:47.000000 dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:23:47.000000 dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 01:23:47.000000 dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 01:23:47.000000 dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-19 01:23:47.859026 dsms_sdk-1.4.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:47.855026 dsms_sdk-1.4.0rc7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/tests/test_kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-19 01:23:44.000000 dsms_sdk-1.4.0rc7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.572747 dsms_sdk-1.4.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-23 00:32:22.572747 dsms_sdk-1.4.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.560747 dsms_sdk-1.4.0rc8/dsms/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.560747 dsms_sdk-1.4.0rc8/dsms/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/apps/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.560747 dsms_sdk-1.4.0rc8/dsms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/dsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/ktype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/linked_kitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/sparql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17151 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-23 00:32:22.572747 dsms_sdk-1.4.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/test_kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/test_utils.py
```

### Comparing `dsms_sdk-1.4.0rc7/LICENSE` & `dsms_sdk-1.4.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/PKG-INFO` & `dsms_sdk-1.4.0rc8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc7
+Version: 1.4.0rc8
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click<9,>=8
 Requires-Dist: html5lib<2,>=1
 Requires-Dist: lru-cache<1
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic>=2
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: rdflib<7,>=6
```

### Comparing `dsms_sdk-1.4.0rc7/README.md` & `dsms_sdk-1.4.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/apps/apps.py` & `dsms_sdk-1.4.0rc8/dsms/apps/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/apps/utils.py` & `dsms_sdk-1.4.0rc8/dsms/apps/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/core/configuration.py` & `dsms_sdk-1.4.0rc8/dsms/core/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,28 @@
     )
 
     datetime_format: str = Field(
         "%Y-%m-%dT%H:%M:%S.%f",
         description="Datetime format used in the DSMS instance.",
     )
 
+    display_units: bool = Field(
+        False,
+        description="""Whether the custom properties or the hdf5 columns shall
+        directly reveal their unit when printed. WARNING: This might lead to performance issues.""",
+    )
+
+    autocomplete_units: bool = Field(
+        True,
+        description="""When a unit is fetched but does not hold a symbol
+        next to its URI, it shall be fetched from the respective ontology
+        (which is general side effect from the `units_sparq_object`.)
+        WARNING: This might lead to performance issues.""",
+    )
+
     kitem_repo: str = Field(
         DEFAULT_REPO,
         description="Repository of the triplestore for KItems in the DSMS",
     )
 
     qudt_units: AnyUrl = Field(
         "http://qudt.org/2.1/vocab/unit",
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/core/context.py` & `dsms_sdk-1.4.0rc8/dsms/core/context.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/core/dsms.py` & `dsms_sdk-1.4.0rc8/dsms/core/dsms.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/core/utils.py` & `dsms_sdk-1.4.0rc8/dsms/core/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/kitem.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/kitem.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             self.dsms = DSMS()
 
         # initialize the kitem
         super().__init__(**kwargs)
 
         # add kitem to buffer
         if (
-            not _kitem_exists(self)
+            _slug_is_available(self._get_ktype_as_str(), self.slug)
             and self.id not in self.context.buffers.created
         ):
             self.context.buffers.created.update({self.id: self})
             self.context.buffers.updated.update({self.id: self})
 
         self._set_kitem_for_properties()
 
@@ -224,23 +224,23 @@
     def __repr__(self) -> str:
         """Pretty print the kitem Fields"""
         return str(self)
 
     def __hash__(self) -> int:
         return hash(str(self))
 
-    @field_validator("affiliations")
+    @field_validator("affiliations", mode="after")
     @classmethod
     def validate_affiliation(
         cls, value: List[Affiliation]
     ) -> AffiliationsProperty:
         """Validate affiliations Field"""
         return AffiliationsProperty(value)
 
-    @field_validator("annotations")
+    @field_validator("annotations", mode="after")
     @classmethod
     def validate_annotations(
         cls, value: List[Annotation]
     ) -> AnnotationsProperty:
         """Validate annotations Field"""
         return AnnotationsProperty(value)
 
@@ -261,15 +261,15 @@
     @classmethod
     def validate_attachments_after(
         cls, value: List[Attachment]
     ) -> AttachmentsProperty:
         """Validate attachments Field"""
         return AttachmentsProperty(value)
 
-    @field_validator("kitem_apps")
+    @field_validator("kitem_apps", mode="after")
     @classmethod
     def validate_apps(cls, value: List[App]) -> AppsProperty:
         """Validate apps Field"""
         return AppsProperty(value)
 
     @field_validator("authors")
     @classmethod
@@ -278,32 +278,32 @@
         return AuthorsProperty(
             [
                 Author(user_id=author) if isinstance(author, str) else author
                 for author in value
             ]
         )
 
-    @field_validator("contacts")
+    @field_validator("contacts", mode="after")
     @classmethod
     def validate_contacts(cls, value: List[ContactInfo]) -> ContactsProperty:
         """Validate contacts Field"""
         return ContactsProperty(value)
 
-    @field_validator("external_links")
+    @field_validator("external_links", mode="after")
     @classmethod
     def validate_external_links(
         cls, value: List[ExternalLink]
     ) -> ExternalLinksProperty:
         """Validate external links Field"""
         return ExternalLinksProperty(value)
 
     @field_validator("linked_kitems", mode="before")
     @classmethod
     def validate_linked_kitems_list(
-        cls, value: "List[Union[Dict, KItem, Any]]", info: ValidationInfo
+        cls, value: "List[Union[Dict, KItem, Any]]"
     ) -> List[LinkedKItem]:
         """Validate each single kitem to be linked"""
         linked_kitems = []
         for item in value:
             if isinstance(item, dict):
                 dest_id = item.get("id")
                 if not dest_id:
@@ -313,29 +313,27 @@
             else:
                 try:
                     dest_id = getattr(item, "id")
                 except AttributeError as error:
                     raise AttributeError(
                         f"Linked KItem `{item}` has no attribute `id`."
                     ) from error
-            linked_kitems.append(
-                LinkedKItem(id=dest_id, source_id=info.data["id"])
-            )
+            linked_kitems.append(LinkedKItem(id=dest_id))
         return linked_kitems
 
     @field_validator("linked_kitems", mode="after")
     @classmethod
     def validate_linked_kitems(
         cls,
         value: List[LinkedKItem],
     ) -> LinkedKItemsProperty:
         """Validate the list out of linked KItems"""
         return LinkedKItemsProperty(value)
 
-    @field_validator("user_groups")
+    @field_validator("user_groups", mode="after")
     @classmethod
     def validate_user_groups(
         cls, value: List[UserGroup]
     ) -> UserGroupsProperty:
         """Validate user groups Field"""
         return UserGroupsProperty(value)
 
@@ -381,20 +379,20 @@
         from dsms import Context
 
         ktype_id = info.data["ktype_id"]
         name = info.data.get("name")
         kitem_id = info.data.get("id")
         if not value:
             value = _slugify(name)
-            if Context.dsms.config.individual_slugs:
-                value += f"-{str(kitem_id).split('-', maxsplit=1)[0]}"
             if len(value) < 4:
                 raise ValueError(
                     "Slug length must have a minimum length of 4."
                 )
+            if Context.dsms.config.individual_slugs:
+                value += f"-{str(kitem_id).split('-', maxsplit=1)[0]}"
         if not _kitem_exists(kitem_id) and not _slug_is_available(
             ktype_id.value, value
         ):
             raise ValueError(f"Slug for `{value}` is already taken.")
         return value
 
     @field_validator("summary")
@@ -496,9 +494,19 @@
 
         return Context
 
     @property
     def url(cls) -> str:
         """URL of the KItem"""
         return urljoin(
-            str(cls.context.dsms.config.host_url), f"{cls.ktype_id}/{cls.slug}"
+            str(cls.context.dsms.config.host_url),
+            f"knowledge/{cls._get_ktype_as_str()}/{cls.slug}",
         )
+
+    def _get_ktype_as_str(self) -> str:
+        if isinstance(self.ktype_id, str):
+            ktype = self.ktype_id
+        elif isinstance(self.ktype_id, Enum):
+            ktype = self.ktype_id.value  # pylint: disable=no-member
+        else:
+            raise TypeError(f"Datatype for KType is unknown: {type(ktype)}")
+        return ktype
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/ktype.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/ktype.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/properties/__init__.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/properties/annotations.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/annotations.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,26 +22,7 @@
     """KProperty for annotations"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         """Annotation data model"""
         return Annotation
-
-    # OVERRIDE
-    def _add(self, item: Annotation) -> Annotation:
-        """Side effect when an Annotation is added to the KProperty"""
-        return item
-
-    # OVERRIDE
-    def _update(self, item: Annotation) -> Annotation:
-        """Side effect when an Annotation is updated at the KProperty"""
-        return item
-
-    # OVERRIDE
-    def _delete(self, item: Annotation) -> None:
-        """Side effect when deleting the Annotation of a KItem"""
-
-    # OVERRIDE
-    def _get(self, item: Annotation) -> Annotation:
-        """Side effect when getting the Annotation for a specfic kitem"""
-        return item
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/properties/apps.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/apps.py`

 * *Files 23% similar despite different names*

```diff
@@ -63,26 +63,7 @@
     """KProperty for apps"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         """App data model"""
         return App
-
-    # OVERRIDE
-    def _add(self, item: App) -> App:
-        """Side effect when an App is added to the KProperty"""
-        return item
-
-    # OVERRIDE
-    def _update(self, item: App) -> App:
-        """Side effect when an App is updated at the KProperty"""
-        return item
-
-    # OVERRIDE
-    def _delete(self, item: App) -> None:
-        """Side effect when deleting the App of a KItem"""
-
-    # OVERRIDE
-    def _get(self, item: App) -> App:
-        """Side effect when getting the App for a specfic kitem"""
-        return item
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/properties/base.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     ConfigDict,
     Field,
     PrivateAttr,
     model_serializer,
 )
 
 from dsms.core.utils import _snake_to_camel  # isort:skip
-from dsms.knowledge.utils import _get_kitem  # isort:skip
 
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Dict, Iterable, List, Set, Union
 
     from dsms import Context, KItem
 
@@ -50,33 +49,46 @@
 
     def __repr__(self) -> str:
         """Pretty print the KProperty"""
         return str(self)
 
     def __setattr__(self, index: int, item: "Any") -> None:
         """Add KItem to updated buffer."""
-        if self._kitem and self.id not in self.context.buffers.updated:
-            self.context.buffers.updated.update({self.id: self._kitem})
+        if self.kitem and self.kitem.id not in self.context.buffers.updated:
+            self.context.buffers.updated.update({self.id: self.kitem})
         super().__setattr__(index, item)
 
     def __hash__(self) -> int:
         return hash(str(self))
 
     @property
     def kitem(cls) -> "KItem":
         """KItem related to the KPropertyItem"""
-        if not cls.id:
-            raise ValueError("KItem not defined yet for KProperty")
-        return _get_kitem(cls.id)
+        return cls._kitem
+
+    @kitem.setter
+    def kitem(cls, item: "KItem") -> None:
+        """Set KItem related to the KPropertyItem"""
+        cls._kitem = item
+        cls.id = item.id
 
     @property
     def exclude(cls) -> "Optional[Set[str]]":
         """Fields to be excluded from the JSON-schema"""
         return cls.model_config.get("exclude")
 
+    @property
+    def context(cls) -> "Context":
+        """Getter for Context"""
+        from dsms import (  # isort:skip
+            Context,
+        )
+
+        return Context
+
     @model_serializer
     def serialize(self):
         """Serialize KPropertItem"""
         return {
             key: value for key, value in self.__dict__.items() if key != "id"
         }
 
@@ -89,30 +101,14 @@
         self.extend(args)
 
     @property
     @abstractmethod
     def k_property_item(cls) -> "Callable":
         """Return the KPropertyItem-class for the KProperty"""
 
-    @abstractmethod
-    def _add(self, item: KPropertyItem) -> KPropertyItem:
-        """Side effect when an KPropertyItem is added to the KProperty"""
-
-    @abstractmethod
-    def _update(self, item: KPropertyItem) -> KPropertyItem:
-        """Side effect when an KPropertyItem is updated in the KProperty"""
-
-    @abstractmethod
-    def _get(self, item: KPropertyItem) -> KPropertyItem:
-        """Side effect when an KPropertyItem is retrieved from the KProperty"""
-
-    @abstractmethod
-    def _delete(self, item: KPropertyItem) -> None:
-        """Side effect when an KPropertyItem is deleted from the KProperty"""
-
     def __str__(self) -> str:
         """Pretty print the KProperty"""
         values = ", \n".join(["\t\t" + repr(value) for value in self])
         if values:
             values = f"\n{values}\n\t"
         return f"[{values}]"
 
@@ -125,94 +121,85 @@
 
     def __setitem__(
         self, index: int, item: "Union[Dict, KPropertyItem]"
     ) -> None:
         """Add or Update KPropertyItem and add it to the updated-buffer."""
 
         self._mark_as_updated()
-        item = self._check_k_property_item(item)
-        if self.kitem:
-            item.id = self.kitem.id
-        try:
-            if self[index] != item:
-                item = self._update(item)
-        except IndexError:
-            item = self._add(item)
+        item = self._check_item(item)
         super().__setitem__(index, item)
 
     def __delitem__(self, index: int) -> None:
         """Delete the KPropertyItem from the KProperty"""
 
         self._mark_as_updated()
-        item = super().__delitem__(index)
-        self._delete(item)
-
-    def __getitem__(self, index: int) -> KPropertyItem:
-        """Get the KPropertyItem from the KProperty"""
-
-        item = super().__getitem__(index)
-        return self._get(item)
+        super().__delitem__(index)
 
     def __imul__(self, index: int) -> None:
         """Imul the KPropertyItem"""
         self._mark_as_updated()
         super().__imul__(index)
 
     def extend(self, iterable: "Iterable") -> None:
         """Extend KProperty with list of KPropertyItem"""
         from dsms import KItem
 
         to_extend = []
         for item in iterable:
             if isinstance(item, (list, tuple)):
                 for subitem in item:
-                    item = self._check_and_add_item(subitem)
-                    to_extend.append(item)
+                    item = self._check_item(subitem)
+                    if not item in self:
+                        to_extend.append(item)
             elif isinstance(item, (dict, KPropertyItem, KItem)):
-                item = self._check_and_add_item(item)
-                to_extend.append(item)
+                item = self._check_item(item)
+                if not item in self:
+                    to_extend.append(item)
             else:
-                to_extend.append(item)
-        self._mark_as_updated()
-        super().extend(to_extend)
+                if not item in self:
+                    to_extend.append(item)
+        if to_extend:
+            self._mark_as_updated()
+            super().extend(to_extend)
 
     def append(self, item: "Union[Dict, Any]") -> None:
         """Append KPropertyItem to KProperty"""
 
-        item = self._check_and_add_item(item)
-        self._mark_as_updated()
-        super().append(item)
+        item = self._check_item(item)
+
+        if not item in self:
+            self._mark_as_updated()
+            super().append(item)
 
     def insert(self, index: int, item: "Union[Dict, Any]") -> None:
         """Insert KPropertyItem at KProperty at certain index"""
 
-        item = self._check_and_add_item(item)
-        self._mark_as_updated()
-        super().insert(index, item)
+        item = self._check_item(item)
+        if not item in self:
+            self._mark_as_updated()
+            super().insert(index, item)
 
     def pop(self, index=-1) -> KPropertyItem:
         """Pop KPropertyItem from KProperty"""
 
         item = super().pop(index)
         self._mark_as_updated()
-        self._delete(item)
         return item
 
     def remove(self, item: "Union[Dict, Any]") -> None:
         """Remove KPropertyItem from KProperty"""
 
         self._mark_as_updated()
-        self._delete(item)
         super().remove(item)
 
-    def _check_and_add_item(self, item: "Union[Dict, Any]") -> KPropertyItem:
+    def _check_item(self, item: "Union[Dict, Any]") -> KPropertyItem:
         item = self._check_k_property_item(item)
         if self.kitem:
-            item.id = self.kitem.id
-        return self._add(item)
+            item.kitem = self.kitem
+        return item
 
     def _check_k_property_item(
         self, item: "Union[Dict, Any]"
     ) -> KPropertyItem:
         """Check the type of the processsed KPropertyItem"""
         from dsms import KItem
 
@@ -245,13 +232,13 @@
         return cls._kitem
 
     @kitem.setter
     def kitem(cls, value: "KItem") -> None:
         """KItem setter"""
         cls._kitem = value
         for item in cls:
-            item.id = cls.kitem.id
+            item.kitem = cls.kitem
 
     @property
     def values(cls) -> "List[Dict[str, Any]]":
         """Values of the KProperty"""
         return list(cls)
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/properties/custom_datatype/numerical.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/numerical.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,50 @@
 """Module for custom numerical data type"""
 
+import logging
 from typing import TYPE_CHECKING
 
 from dsms.knowledge.semantics.units.utils import (
     get_conversion_factor,
     get_property_unit,
 )
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Optional
 
     from dsms import KItem
 
 
+logger = logging.Logger(__name__)
+
+
 class NumericalDataType(float):
     """Custom Base data type for custom properties"""
 
     def __init__(self, value) -> None:  # pylint: disable=unused-argument
         self._kitem: "Optional[KItem]" = None
         self._name: "Optional[str]" = None
 
+    def __str__(self) -> str:
+        """Pretty print the numerical datatype"""
+        if self.kitem.dsms.config.display_units:
+            try:
+                string = f"{self.__float__()} {self.get_unit().get('symbol')}"
+            except Exception as error:
+                logger.debug(
+                    "Could not fetch unit from `%i`: %i", self.name, error.args
+                )
+                string = str(self.__float__())
+        else:
+            string = str(self.__float__())
+        return string
+
+    def __repr__(self) -> str:
+        return str(self)
+
     @property
     def kitem(cls) -> "Optional[KItem]":
         """Context of the current kitem for this property"""
         return cls._kitem
 
     @kitem.setter
     def kitem(cls, value: "Optional[KItem]") -> None:
@@ -38,15 +59,20 @@
     @name.setter
     def name(cls, value: str) -> None:
         """Setter for the name of the property"""
         cls._name = value
 
     def get_unit(self) -> "Dict[str, Any]":
         """Get unit for the property"""
-        return get_property_unit(self.kitem.id, self.name)
+        return get_property_unit(
+            self.kitem.id,
+            self.name,
+            is_hdf5_column=True,
+            autocomplete_symbol=self.kitem.dsms.config.autocomplete_units,
+        )
 
     def convert_to(
         self,
         unit_symbol_or_iri: str,
         decimals: "Optional[int]" = None,
         use_input_iri: bool = True,
     ) -> float:
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/properties/hdf5.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/hdf5.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """HDF5 Properties of a KItem"""
+import logging
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from pydantic import Field
 
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
 from dsms.knowledge.utils import _get_hdf5_column
 
 from dsms.knowledge.semantics.units import (  # isort:skip
     get_conversion_factor,
     get_property_unit,
 )
 
+logger = logging.Logger(__name__)
+
 if TYPE_CHECKING:
     from typing import Any, Callable, Dict, List, Optional
 
 
 class Column(KPropertyItem):
     """
     Column of an HDF5 data frame.
@@ -28,14 +31,30 @@
 
     column_id: int = Field(..., description="Column ID in the data frame")
 
     name: str = Field(
         ..., description="Name of the column in the data series."
     )
 
+    def __repr__(self) -> str:
+        """Pretty print the numerical datatype"""
+        if self.kitem.dsms.config.display_units:
+            try:
+                unit = f"\tunit={self.get_unit().get('symbol')}\n\t\t"
+                string = str(self)
+                string = string[:-1] + unit + string[-1:]
+            except Exception as error:
+                logger.debug(
+                    "Could not fetch unit from `%i`: %i", self.name, error.args
+                )
+                string = str(self)
+        else:
+            string = str(self)
+        return string
+
     def get(self) -> "List[Any]":
         """
         Download the data for the column in a time series.
 
         Returns:
             List[Any]: List of data for the column.
         """
@@ -44,15 +63,20 @@
     def get_unit(self) -> "Dict[str, Any]":
         """
         Retrieve the unit of the column.
 
         Returns:
             Dict[str, Any]: Dictionary containing unit information.
         """
-        return get_property_unit(self.id, self.name, is_hdf5_column=True)
+        return get_property_unit(
+            self.id,
+            self.name,
+            is_hdf5_column=True,
+            autocomplete_symbol=self.kitem.dsms.config.autocomplete_units,
+        )
 
     def convert_to(
         self,
         unit_symbol_or_iri: str,
         decimals: "Optional[int]" = None,
         use_input_iri: bool = True,
     ) -> "List[Any]":
@@ -83,33 +107,14 @@
     """HDF5 container of a data frame related to a KItem"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         return Column
 
-    # OVERRIDE
-    def _add(self, item: Column) -> Column:
-        """Side effect when an Column is added to the KProperty"""
-        return item
-
-    # OVERRIDE
-    def _update(self, item: Column) -> Column:
-        """Side effect when an Column is updated at the KProperty"""
-        return item
-
-    # OVERRIDE
-    def _delete(self, item: Column) -> None:
-        """Side effect when deleting the Column of a KItem"""
-
-    # OVERRIDE
-    def _get(self, item: Column) -> Column:
-        """Side effect when getting the Column for a specfic kitem"""
-        return item
-
     def to_df(self) -> pd.DataFrame:
         """Return hdf5 as pandas DataFrame"""
         data = {column.name: column.get() for column in self}
         return pd.DataFrame.from_dict(data)
 
     def get(self, name: str) -> "Optional[Column]":
         """Get a column with a certain name."""
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/properties/summary.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/summary.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/queries/base.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,19 +49,28 @@
     @property
     @abstractmethod
     def query(cls) -> str:
         """
         Define sparql query by using the kwargs defined during initialization.
         """
 
+    @abstractmethod
+    def postprocess_result(cls, row: "Dict[str, Any]") -> "Dict[str, Any]":
+        """
+        Define a function that postprocesses the result of the indivudal row in the
+        sparql result. This might e.g. be some string operations etc.
+        """
+
     def execute(self) -> None:
         """Execute sparql query and bind results."""
         result = self.dsms.sparql_interface.query(self.query)
         self._results = []
         for row in JSONResult(result).bindings:
             row_converted = {str(key): value for key, value in row.items()}
             self._results.append(
-                {
-                    name: func(row_converted.get(name))
-                    for name, func in self.result_mappings.items()
-                }
+                self.postprocess_result(
+                    {
+                        name: func(row_converted.get(name))
+                        for name, func in self.result_mappings.items()
+                    }
+                )
             )
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/base.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,19 +17,21 @@
     """
 
     def __init__(
         self,
         kitem_id: "Union[str, UUID]",
         property_name: str,
         is_hdf5_column: bool = False,
+        autocomplete_symbol: bool = True,
     ) -> None:
         super().__init__(
             kitem_id=kitem_id,
             property_name=property_name,
             is_hdf5_column=is_hdf5_column,
+            autocomplete_symbol=autocomplete_symbol,
         )
 
     # OVERRIDE
     @property
     def result_mappings(cls) -> "Dict[str, Any]":
         """Define mappings for the results of the units sparql queries"""
         return {"symbol": str, "iri": str}
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/conversion.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/conversion.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,23 @@
     SELECT DISTINCT ?factor
         WHERE {{
             <{uri}> a qudt:Unit ;
                     qudt:conversionMultiplier ?factor .
         }}"""
 
 
+def _sparql_symbol_from_iri(uri: str) -> str:
+    return f"""PREFIX qudt: <http://qudt.org/schema/qudt/>
+    SELECT DISTINCT ?symbol
+        WHERE {{
+            <{uri}> a qudt:Unit ;
+                    qudt:ucumCode ?symbol .
+        }}"""
+
+
 def _qudt_sparql_quantity(original_uri: str, target_uri: str) -> str:
     return f"""PREFIX qudt: <http://qudt.org/schema/qudt/>
     SELECT DISTINCT ?kind
         WHERE {{
             ?kind a qudt:QuantityKind ;
                   qudt:applicableUnit <{original_uri}> , <{target_uri}> .
         }}"""
@@ -77,14 +86,28 @@
         raise ValueError(
             f"More than one QUDT Mapping found for unit with symbol `{symbol}`."
         )
     return match.pop()
 
 
 @lru_cache
+def _get_symbol_from_uri(uri: str) -> str:
+    graph = _get_qudt_graph("qudt_units")
+    query = _sparql_symbol_from_iri(uri)
+    symbol = [str(row["symbol"]) for row in graph.query(query)]
+    if len(symbol) == 0:
+        raise ValueError(f"No symbol found for unit with uri `{uri}`.")
+    if len(symbol) > 1:
+        raise ValueError(
+            f"More than one symbol factor for unit with uri `{uri}`."
+        )
+    return symbol.pop()
+
+
+@lru_cache
 def _get_factor_from_uri(uri: str) -> int:
     graph = _get_qudt_graph("qudt_units")
     query = _qudt_sparql_factor(uri)
     factor = [float(row["factor"]) for row in graph.query(query)]
     if len(factor) == 0:
         raise ValueError(f"No conversion factor for unit with uri `{uri}`.")
     if len(factor) > 1:
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/semantics/units/utils.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,24 +65,28 @@
     return factor
 
 
 def get_property_unit(
     kitem_id: "Union[str, UUID]",
     property_name: str,
     is_hdf5_column: bool = False,
+    autocomplete_symbol: bool = True,
 ) -> "Dict[str, Any]":
     """
     Retrieve the unit associated with a given property of a KIitem.
 
     Args:
         kitem (KItem): The identifier of the KItem.
         property_name (str): The name of the property of the KItem  for which
             the unit is to be retrieved.
         is_hdf5_column (bool, optional): Indicates whether the property is an HDF5
             column or a custom property. Defaults to False.
+        autocomplete_symbol (bool, optional): Whether the symbol of a unit shall be
+            fetched automatically from the ontology when it is not given next to the
+            URI.
 
     Returns:
         Dict[str, Any]: A dictionary with the symbol and iri of the unit associated
             with the specified property.
 
     Raises:
         ValueError: If unable to retrieve the unit for the property due to any errors or if
@@ -92,15 +96,20 @@
 
     units_sparql_object = Context.dsms.config.units_sparql_object
     if not issubclass(units_sparql_object, BaseUnitSparqlQuery):
         raise TypeError(
             f"´{units_sparql_object}´ must be a subclass of `{BaseUnitSparqlQuery}`"
         )
     try:
-        query = units_sparql_object(kitem_id, property_name, is_hdf5_column)
+        query = units_sparql_object(
+            kitem_id=kitem_id,
+            property_name=property_name,
+            is_hdf5_column=is_hdf5_column,
+            autocomplete_symbol=autocomplete_symbol,
+        )
     except Exception as error:
         raise ValueError(
             f"Something went wrong catching the unit for property `{property_name}`."
         ) from error
     if len(query.results) == 0:
         raise ValueError(
             f"""Property `{property_name}` does not own any
```

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/sparql_interface.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/sparql_interface.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/subgraph.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/subgraph.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/sparql_interface/utils.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/dsms/knowledge/utils.py` & `dsms_sdk-1.4.0rc8/dsms/knowledge/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -350,16 +350,24 @@
         )
     return response.text
 
 
 def _get_attachment_diffs(kitem_old: "KItem", kitem_new: "KItem"):
     """Check which attachments should be removed and which should be added."""
     return {
-        "remove": set(kitem_old.attachments) - set(kitem_new.attachments),
-        "add": set(kitem_new.attachments) - set(kitem_old.attachments),
+        "remove": [
+            attachment
+            for name, attachment in kitem_old.attachments.by_name.items()
+            if name not in kitem_new.attachments.by_name
+        ],
+        "add": [
+            attachment
+            for name, attachment in kitem_new.attachments.by_name.items()
+            if name not in kitem_old.attachments.by_name
+        ],
     }
 
 
 def _get_kitems_diffs(kitem_old: "KItem", kitem_new: "KItem"):
     """Get the differences in the attributes between two kitems"""
     differences = {}
     attributes = [
@@ -371,19 +379,21 @@
     for name, terms in attributes:
         to_add_name = terms[0] + "_to_" + terms[1]
         to_remove_name = terms[0] + "_to_" + terms[2]
         old_attr = getattr(kitem_old, name)
         new_attr = getattr(kitem_new, name)
         differences[to_add_name] = [
             json.loads(attr.model_dump_json())
-            for attr in set(new_attr) - set(old_attr)
+            for attr in new_attr
+            if new_attr not in old_attr
         ]
         differences[to_remove_name] = [
             json.loads(attr.model_dump_json())
-            for attr in set(old_attr) - set(new_attr)
+            for attr in old_attr
+            if old_attr not in new_attr
         ]
     return differences
 
 
 def _commit(buffers: "Buffers") -> None:
     """Commit the buffers for the
     created, updated and deleted buffers"""
@@ -431,15 +441,15 @@
 ) -> "List[SearchResult]":
     """Search for KItems in the remote backend"""
     from dsms import KItem  # isort:skip
 
     payload = {
         "search_term": query or "",
         "ktypes": [ktype.value for ktype in ktypes],
-        "kitem_annotations": annotations,
+        "annotations": annotations,
         "limit": limit,
     }
     response = _perform_request(
         "api/knowledge/kitems/search",
         "post",
         json=payload,
         params={"allow_fuzzy": allow_fuzzy},
```

### Comparing `dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/PKG-INFO` & `dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc7
+Version: 1.4.0rc8
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click<9,>=8
 Requires-Dist: html5lib<2,>=1
 Requires-Dist: lru-cache<1
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic>=2
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: rdflib<7,>=6
```

### Comparing `dsms_sdk-1.4.0rc7/dsms_sdk.egg-info/SOURCES.txt` & `dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 dsms/apps/utils.py
 dsms/core/__init__.py
 dsms/core/configuration.py
 dsms/core/context.py
 dsms/core/dsms.py
 dsms/core/utils.py
 dsms/knowledge/__init__.py
+dsms/knowledge/cli.py
 dsms/knowledge/kitem.py
 dsms/knowledge/ktype.py
 dsms/knowledge/search.py
 dsms/knowledge/utils.py
 dsms/knowledge/properties/__init__.py
 dsms/knowledge/properties/affiliations.py
 dsms/knowledge/properties/annotations.py
@@ -42,13 +43,14 @@
 dsms/knowledge/sparql_interface/__init__.py
 dsms/knowledge/sparql_interface/sparql_interface.py
 dsms/knowledge/sparql_interface/subgraph.py
 dsms/knowledge/sparql_interface/utils.py
 dsms_sdk.egg-info/PKG-INFO
 dsms_sdk.egg-info/SOURCES.txt
 dsms_sdk.egg-info/dependency_links.txt
+dsms_sdk.egg-info/entry_points.txt
 dsms_sdk.egg-info/requires.txt
 dsms_sdk.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_kitem.py
 tests/test_utils.py
```

### Comparing `dsms_sdk-1.4.0rc7/setup.cfg` & `dsms_sdk-1.4.0rc8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsms_sdk
-version = v1.4.0rc7
+version = v1.4.0rc8
 description = Python SDK core-package for working with the Dataspace Management System (DSMS).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 author = Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 license = BSD-3-Clause
@@ -15,25 +15,30 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
+	click>=8,<9
 	html5lib>=1,<2
 	lru-cache<1
 	pandas>=2,<3
 	pydantic>=2
 	pydantic-settings
 	python-dotenv
 	rdflib>=6,<7
 	requests
 python_requires = >=3.8
 include_package_data = True
 
+[options.entry_points]
+console_scripts = 
+	kitem = dsms.knowledge.cli:lookup_kitem
+
 [options.extras_require]
 dev = 
 	bumpver==2021.1114
 	dunamai==1.7.0
 pre_commit = 
 	pre-commit==3.3.2
 	pylint
```

### Comparing `dsms_sdk-1.4.0rc7/tests/conftest.py` & `dsms_sdk-1.4.0rc8/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,16 +26,24 @@
             "name": "foo789",
             "id": "a00af336-e714-499a-9dbf-298651939e62",
         },
         "698acdc5-dd97-4217-906e-2c0b44248c17": {
             "name": "bar123",
             "id": "698acdc5-dd97-4217-906e-2c0b44248c17",
         },
+        "cc834fb6-d4cd-43c1-b4b8-4c720ac6f038": {
+            "name": "bar456",
+            "id": "cc834fb6-d4cd-43c1-b4b8-4c720ac6f038",
+        },
     }
 
+    slugs = [
+        value.get("name") + "-" + key[:8] for key, value in kitems.items()
+    ]
+
     hdf5 = {
         "698acdc5-dd97-4217-906e-2c0b44248c17": [
             {
                 "column_id": 0,
                 "name": "bar123column",
             },
         ]
@@ -110,14 +118,22 @@
         # Your logic to generate a dynamic response based on 'item_id'
         # This is just a placeholder; you should replace it with your actual logic
         if item_id not in MockDB.hdf5:
             return 404, {}, "KItem does not exist"
         else:
             return 200, {}, json.dumps(MockDB.hdf5[item_id])
 
+    def return_slugs(request):
+        url_parts = request.url.split("/")
+        slug = url_parts[-1]
+        if slug not in MockDB.slugs:
+            return 404, {}, "Slug does not exist"
+        else:
+            return 200, {}, "Slug exists"
+
     def _get_kitems() -> "Dict[str, Any]":
         return {
             urljoin(custom_address, f"api/knowledge/kitems/{uid}"): [
                 {
                     "method": responses.GET,
                     "returns": {
                         "content_type": "application/json",
@@ -138,26 +154,43 @@
                         "callback": return_hdf5,
                     },
                 }
             ]
             for uid in MockDB.kitems
         }
 
+    def _get_slugs() -> "Dict[str, Any]":
+        return {
+            urljoin(
+                custom_address, f"api/knowledge/kitems/organization/{slug}"
+            ): [
+                {
+                    "method": responses.HEAD,
+                    "returns": {
+                        "content_type": "application/json",
+                        "callback": return_slugs,
+                    },
+                }
+            ]
+            for slug in MockDB.slugs
+        }
+
     return {
         ktypes: [
             {
                 "method": responses.GET,
                 "returns": {
                     "content_type": "application/json",
                     "callback": return_ktypes,
                 },
             }
         ],
         **_get_kitems(),
         **_get_hdf5(),
+        **_get_slugs(),
     }
 
 
 @pytest.fixture(autouse=True, scope="function")
 def register_mocks(
     mock_responses, mock_callbacks, passthru, custom_address
 ) -> str:
```

### Comparing `dsms_sdk-1.4.0rc7/tests/test_kitem.py` & `dsms_sdk-1.4.0rc8/tests/test_kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc7/tests/test_utils.py` & `dsms_sdk-1.4.0rc8/tests/test_utils.py`

 * *Files identical despite different names*

