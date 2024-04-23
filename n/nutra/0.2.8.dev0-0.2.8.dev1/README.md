# Comparing `tmp/nutra-0.2.8.dev0.tar.gz` & `tmp/nutra-0.2.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutra-0.2.8.dev0.tar", last modified: Tue Feb 27 00:42:47 2024, max compression
+gzip compressed data, was "nutra-0.2.8.dev1.tar", last modified: Tue Apr 23 18:42:50 2024, max compression
```

## Comparing `nutra-0.2.8.dev0.tar` & `nutra-0.2.8.dev1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.761365 nutra-0.2.8.dev0/
--rw-rw-r--   0 shane     (1000) shane     (1000)    35149 2022-07-04 05:47:34.000000 nutra-0.2.8.dev0/LICENSE
--rw-rw-r--   0 shane     (1000) shane     (1000)      258 2023-03-27 01:46:26.000000 nutra-0.2.8.dev0/MANIFEST.in
--rw-rw-r--   0 shane     (1000) shane     (1000)     8686 2024-02-27 00:42:47.761365 nutra-0.2.8.dev0/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     7187 2023-05-01 21:44:01.000000 nutra-0.2.8.dev0/README.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.729365 nutra-0.2.8.dev0/ntclient/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3100 2024-02-25 22:25:26.000000 nutra-0.2.8.dev0/ntclient/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4123 2024-02-14 20:23:58.000000 nutra-0.2.8.dev0/ntclient/__main__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.733365 nutra-0.2.8.dev0/ntclient/argparser/
--rw-rw-r--   0 shane     (1000) shane     (1000)    11864 2024-02-25 21:27:02.000000 nutra-0.2.8.dev0/ntclient/argparser/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    11755 2024-02-25 22:31:44.000000 nutra-0.2.8.dev0/ntclient/argparser/funcs.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      622 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/argparser/types.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.733365 nutra-0.2.8.dev0/ntclient/core/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-04-14 05:51:30.000000 nutra-0.2.8.dev0/ntclient/core/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1172 2024-02-23 19:53:51.000000 nutra-0.2.8.dev0/ntclient/core/nnest.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      190 2024-02-26 03:32:10.000000 nutra-0.2.8.dev0/ntclient/core/nnr2.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     5029 2024-02-26 03:03:29.000000 nutra-0.2.8.dev0/ntclient/core/nutprogbar.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.733365 nutra-0.2.8.dev0/ntclient/models/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1767 2024-02-13 15:01:08.000000 nutra-0.2.8.dev0/ntclient/models/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.733365 nutra-0.2.8.dev0/ntclient/ntsqlite/
--rw-rw-r--   0 shane     (1000) shane     (1000)      137 2024-02-25 22:25:52.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.737365 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/
--rwxrwxr-x   0 shane     (1000) shane     (1000)     1849 2024-02-25 22:25:52.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      157 2024-02-25 22:25:52.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/__main__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.741365 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/data/
--rw-rw-r--   0 shane     (1000) shane     (1000)       31 2024-02-13 14:59:30.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/data/bf_eq.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)       74 2024-02-13 14:59:30.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/data/bmr_eq.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      102 2024-02-13 14:59:30.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/data/meal_name.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      761 2024-02-13 14:59:30.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/data/rda.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      365 2024-02-25 22:25:53.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/data/version.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      690 2024-02-25 22:25:52.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/functions.sql
--rw-rw-r--   0 shane     (1000) shane     (1000)     6582 2024-02-25 22:25:53.000000 nutra-0.2.8.dev0/ntclient/ntsqlite/sql/tables.sql
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.741365 nutra-0.2.8.dev0/ntclient/persistence/
--rw-rw-r--   0 shane     (1000) shane     (1000)      707 2024-02-26 03:35:10.000000 nutra-0.2.8.dev0/ntclient/persistence/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.741365 nutra-0.2.8.dev0/ntclient/persistence/sql/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3321 2024-02-25 00:36:51.000000 nutra-0.2.8.dev0/ntclient/persistence/sql/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.741365 nutra-0.2.8.dev0/ntclient/persistence/sql/nt/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3131 2024-02-26 03:34:26.000000 nutra-0.2.8.dev0/ntclient/persistence/sql/nt/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      302 2024-02-25 00:36:51.000000 nutra-0.2.8.dev0/ntclient/persistence/sql/nt/funcs.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.741365 nutra-0.2.8.dev0/ntclient/persistence/sql/usda/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5110 2024-02-25 21:12:58.000000 nutra-0.2.8.dev0/ntclient/persistence/sql/usda/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3858 2023-03-19 02:09:32.000000 nutra-0.2.8.dev0/ntclient/persistence/sql/usda/funcs.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.725365 nutra-0.2.8.dev0/ntclient/resources/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.725365 nutra-0.2.8.dev0/ntclient/resources/recipe/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.745365 nutra-0.2.8.dev0/ntclient/resources/recipe/dinner/
--rw-rw-r--   0 shane     (1000) shane     (1000)      607 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/dinner/burrito-bowl.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      463 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/dinner/grass-fed-burger.csv
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.745365 nutra-0.2.8.dev0/ntclient/resources/recipe/snack/
--rw-rw-r--   0 shane     (1000) shane     (1000)      219 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/snack/baked-potato-wedges.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      642 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/snack/buckwheat-pancake.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      503 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/snack/fruit-smoothie.csv
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.749365 nutra-0.2.8.dev0/ntclient/resources/recipe/tmp/
--rw-rw-r--   0 shane     (1000) shane     (1000)      947 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/tmp/food_amounts.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)      142 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/tmp/names.csv
--rw-rw-r--   0 shane     (1000) shane     (1000)       34 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/resources/recipe/tmp/servings.csv
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.749365 nutra-0.2.8.dev0/ntclient/services/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1296 2024-02-25 00:36:51.000000 nutra-0.2.8.dev0/ntclient/services/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     9879 2024-02-26 03:14:06.000000 nutra-0.2.8.dev0/ntclient/services/analyze.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.753365 nutra-0.2.8.dev0/ntclient/services/api/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1846 2024-02-26 19:02:31.000000 nutra-0.2.8.dev0/ntclient/services/api/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3049 2024-02-26 03:30:20.000000 nutra-0.2.8.dev0/ntclient/services/bugs.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    14443 2024-02-13 15:01:08.000000 nutra-0.2.8.dev0/ntclient/services/calculate.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.753365 nutra-0.2.8.dev0/ntclient/services/recipe/
--rw-rw-r--   0 shane     (1000) shane     (1000)      293 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/services/recipe/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      946 2023-03-19 02:09:32.000000 nutra-0.2.8.dev0/ntclient/services/recipe/csv_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2228 2022-07-28 09:01:39.000000 nutra-0.2.8.dev0/ntclient/services/recipe/utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8159 2024-02-26 03:14:03.000000 nutra-0.2.8.dev0/ntclient/services/usda.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.757365 nutra-0.2.8.dev0/ntclient/utils/
--rw-rw-r--   0 shane     (1000) shane     (1000)     4578 2024-02-13 19:15:45.000000 nutra-0.2.8.dev0/ntclient/utils/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      808 2023-04-01 20:27:55.000000 nutra-0.2.8.dev0/ntclient/utils/colors.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      574 2022-07-04 05:47:34.000000 nutra-0.2.8.dev0/ntclient/utils/exceptions.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      464 2024-02-13 19:44:47.000000 nutra-0.2.8.dev0/ntclient/utils/sql.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3292 2024-02-25 20:27:32.000000 nutra-0.2.8.dev0/ntclient/utils/tree.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.761365 nutra-0.2.8.dev0/nutra.egg-info/
--rw-rw-r--   0 shane     (1000) shane     (1000)     8686 2024-02-27 00:42:47.000000 nutra-0.2.8.dev0/nutra.egg-info/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     1974 2024-02-27 00:42:47.000000 nutra-0.2.8.dev0/nutra.egg-info/SOURCES.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2024-02-27 00:42:47.000000 nutra-0.2.8.dev0/nutra.egg-info/dependency_links.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)       50 2024-02-27 00:42:47.000000 nutra-0.2.8.dev0/nutra.egg-info/entry_points.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2024-02-27 00:42:47.000000 nutra-0.2.8.dev0/nutra.egg-info/not-zip-safe
--rw-rw-r--   0 shane     (1000) shane     (1000)      148 2024-02-27 00:42:47.000000 nutra-0.2.8.dev0/nutra.egg-info/requires.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        9 2024-02-27 00:42:47.000000 nutra-0.2.8.dev0/nutra.egg-info/top_level.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)      164 2023-05-01 21:44:01.000000 nutra-0.2.8.dev0/requirements-old.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)       27 2023-03-27 01:46:26.000000 nutra-0.2.8.dev0/requirements-optional.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)      111 2024-02-14 02:07:20.000000 nutra-0.2.8.dev0/requirements.txt
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-02-27 00:42:47.761365 nutra-0.2.8.dev0/scripts/
--rwxrwxr-x   0 shane     (1000) shane     (1000)      286 2023-03-27 01:46:26.000000 nutra-0.2.8.dev0/scripts/n
--rw-rw-r--   0 shane     (1000) shane     (1000)     1024 2024-02-27 00:42:47.761365 nutra-0.2.8.dev0/setup.cfg
--rw-rw-r--   0 shane     (1000) shane     (1000)     2588 2023-04-01 20:27:55.000000 nutra-0.2.8.dev0/setup.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.407807 nutra-0.2.8.dev1/
+-rw-rw-r--   0 shane     (1000) shane     (1000)    35149 2022-07-04 05:47:34.000000 nutra-0.2.8.dev1/LICENSE
+-rw-rw-r--   0 shane     (1000) shane     (1000)      258 2023-03-27 01:46:26.000000 nutra-0.2.8.dev1/MANIFEST.in
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8688 2024-04-23 18:42:50.407807 nutra-0.2.8.dev1/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     7189 2024-04-23 18:40:28.000000 nutra-0.2.8.dev1/README.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.395808 nutra-0.2.8.dev1/ntclient/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3345 2024-04-23 18:42:36.000000 nutra-0.2.8.dev1/ntclient/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4123 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/__main__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.395808 nutra-0.2.8.dev1/ntclient/argparser/
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11920 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/argparser/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11044 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/argparser/funcs.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      622 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/argparser/types.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.395808 nutra-0.2.8.dev1/ntclient/core/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-04-14 05:51:30.000000 nutra-0.2.8.dev1/ntclient/core/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1172 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/core/nnest.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      190 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/core/nnr2.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5140 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/core/nutprogbar.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.395808 nutra-0.2.8.dev1/ntclient/models/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2074 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/models/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.395808 nutra-0.2.8.dev1/ntclient/ntsqlite/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      137 2024-02-25 22:25:52.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.395808 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/
+-rwxrwxr-x   0 shane     (1000) shane     (1000)     1889 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      157 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/__main__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.399808 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/data/
+-rw-rw-r--   0 shane     (1000) shane     (1000)       31 2024-02-13 14:59:30.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/data/bf_eq.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)       74 2024-02-13 14:59:30.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/data/bmr_eq.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      102 2024-02-13 14:59:30.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/data/meal_name.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      761 2024-02-13 14:59:30.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/data/rda.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      365 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/data/version.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      690 2024-02-25 22:25:52.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/functions.sql
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6582 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/ntsqlite/sql/tables.sql
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.399808 nutra-0.2.8.dev1/ntclient/persistence/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      621 2024-04-20 16:14:30.000000 nutra-0.2.8.dev1/ntclient/persistence/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.399808 nutra-0.2.8.dev1/ntclient/persistence/sql/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3123 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/persistence/sql/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.399808 nutra-0.2.8.dev1/ntclient/persistence/sql/nt/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2912 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/persistence/sql/nt/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      361 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/persistence/sql/nt/funcs.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.399808 nutra-0.2.8.dev1/ntclient/persistence/sql/usda/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4409 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/persistence/sql/usda/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4258 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/persistence/sql/usda/funcs.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.391808 nutra-0.2.8.dev1/ntclient/resources/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.391808 nutra-0.2.8.dev1/ntclient/resources/recipe/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.399808 nutra-0.2.8.dev1/ntclient/resources/recipe/dinner/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      607 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/dinner/burrito-bowl.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      463 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/dinner/grass-fed-burger.csv
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.403807 nutra-0.2.8.dev1/ntclient/resources/recipe/snack/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      219 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/snack/baked-potato-wedges.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      642 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/snack/buckwheat-pancake.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      503 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/snack/fruit-smoothie.csv
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.403807 nutra-0.2.8.dev1/ntclient/resources/recipe/tmp/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      947 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/tmp/food_amounts.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)      142 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/tmp/names.csv
+-rw-rw-r--   0 shane     (1000) shane     (1000)       34 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/resources/recipe/tmp/servings.csv
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.403807 nutra-0.2.8.dev1/ntclient/services/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1393 2024-04-20 16:16:18.000000 nutra-0.2.8.dev1/ntclient/services/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     9952 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/services/analyze.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.403807 nutra-0.2.8.dev1/ntclient/services/api/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1810 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/services/api/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4490 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/services/bugs.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    14443 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/services/calculate.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.403807 nutra-0.2.8.dev1/ntclient/services/recipe/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      293 2022-07-28 09:01:39.000000 nutra-0.2.8.dev1/ntclient/services/recipe/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      946 2023-03-19 02:09:32.000000 nutra-0.2.8.dev1/ntclient/services/recipe/csv_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2249 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/services/recipe/recipe.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8135 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/services/usda.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.407807 nutra-0.2.8.dev1/ntclient/utils/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4555 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/utils/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      808 2023-04-01 20:27:55.000000 nutra-0.2.8.dev1/ntclient/utils/colors.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      574 2022-07-04 05:47:34.000000 nutra-0.2.8.dev1/ntclient/utils/exceptions.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      441 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/utils/sql.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3352 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/ntclient/utils/tree.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.407807 nutra-0.2.8.dev1/nutra.egg-info/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8688 2024-04-23 18:42:50.000000 nutra-0.2.8.dev1/nutra.egg-info/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1975 2024-04-23 18:42:50.000000 nutra-0.2.8.dev1/nutra.egg-info/SOURCES.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2024-04-23 18:42:50.000000 nutra-0.2.8.dev1/nutra.egg-info/dependency_links.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)       50 2024-04-23 18:42:50.000000 nutra-0.2.8.dev1/nutra.egg-info/entry_points.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2024-04-23 18:42:50.000000 nutra-0.2.8.dev1/nutra.egg-info/not-zip-safe
+-rw-rw-r--   0 shane     (1000) shane     (1000)      148 2024-04-23 18:42:50.000000 nutra-0.2.8.dev1/nutra.egg-info/requires.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        9 2024-04-23 18:42:50.000000 nutra-0.2.8.dev1/nutra.egg-info/top_level.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)      164 2023-05-01 21:44:01.000000 nutra-0.2.8.dev1/requirements-old.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)       27 2023-03-27 01:46:26.000000 nutra-0.2.8.dev1/requirements-optional.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)      111 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/requirements.txt
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2024-04-23 18:42:50.407807 nutra-0.2.8.dev1/scripts/
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      346 2024-04-19 19:40:49.000000 nutra-0.2.8.dev1/scripts/n
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1024 2024-04-23 18:42:50.407807 nutra-0.2.8.dev1/setup.cfg
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2588 2023-04-01 20:27:55.000000 nutra-0.2.8.dev1/setup.py
```

### Comparing `nutra-0.2.8.dev0/LICENSE` & `nutra-0.2.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/PKG-INFO` & `nutra-0.2.8.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutra
-Version: 0.2.8.dev0
+Version: 0.2.8.dev1
 Summary: Home and office nutrient tracking software
 Home-page: https://github.com/nutratech/cli
 Author: Shane Jaroch
 Author-email: chown_tee@proton.me
 License: GPL v3
 Platform: linux
 Platform: darwin
@@ -134,15 +134,15 @@
     # Need to add hook, too
     # See: https://direnv.net/docs/hook.html
     DEFAULT_SHELL=$(basename $SHELL)
     SHELL_RC_FILE=~/.${DEFAULT_SHELL}rc
     HOOK='eval "$(direnv hook '$DEFAULT_SHELL')"'
 
     # Install the hook, if not already
-    grep "$HOOK" $SHELL_RC_FILE || echo "$HOOK" >>$SHELL_RC_FILE
+    grep ^"$HOOK"$ $SHELL_RC_FILE || echo "$HOOK" >>$SHELL_RC_FILE
     source $SHELL_RC_FILE
 
 This is what the ``.envrc`` file is for. It automatically activates ``venv``.
 
 
 
 Notes
```

### Comparing `nutra-0.2.8.dev0/README.rst` & `nutra-0.2.8.dev1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     # Need to add hook, too
     # See: https://direnv.net/docs/hook.html
     DEFAULT_SHELL=$(basename $SHELL)
     SHELL_RC_FILE=~/.${DEFAULT_SHELL}rc
     HOOK='eval "$(direnv hook '$DEFAULT_SHELL')"'
 
     # Install the hook, if not already
-    grep "$HOOK" $SHELL_RC_FILE || echo "$HOOK" >>$SHELL_RC_FILE
+    grep ^"$HOOK"$ $SHELL_RC_FILE || echo "$HOOK" >>$SHELL_RC_FILE
     source $SHELL_RC_FILE
 
 This is what the ``.envrc`` file is for. It automatically activates ``venv``.
 
 
 
 Notes
```

### Comparing `nutra-0.2.8.dev0/ntclient/__init__.py` & `nutra-0.2.8.dev1/ntclient/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,47 +12,58 @@
 import shutil
 import sys
 
 from ntclient.ntsqlite.sql import NT_DB_NAME
 
 # Package info
 __title__ = "nutra"
-__version__ = "0.2.8.dev0"
+__version__ = "0.2.8.dev1"
 __author__ = "Shane Jaroch"
 __email__ = "chown_tee@proton.me"
 __license__ = "GPL v3"
 __copyright__ = "Copyright 2018-2022 Shane Jaroch"
 __url__ = "https://github.com/nutratech/cli"
 
 # Sqlite target versions
 # TODO: should this be via versions.csv file?  Don't update in two places?
 __db_target_nt__ = "0.0.7"
-__db_target_usda__ = "0.0.9"
+__db_target_usda__ = "0.0.10"
 USDA_XZ_SHA256 = "25dba8428ced42d646bec704981d3a95dc7943240254e884aad37d59eee9616a"
 
 # Global variables
 PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
 NUTRA_HOME = os.getenv("NUTRA_HOME", os.path.join(os.path.expanduser("~"), ".nutra"))
-USDA_DB_NAME = "usda.sqlite"
+USDA_DB_NAME = "usda.sqlite3"
 # NOTE: NT_DB_NAME = "nt.sqlite3" is defined in ntclient.ntsqlite.sql
 
 NTSQLITE_BUILDPATH = os.path.join(PROJECT_ROOT, "ntsqlite", "sql", NT_DB_NAME)
 NTSQLITE_DESTINATION = os.path.join(NUTRA_HOME, NT_DB_NAME)
 
-# Check Python version
+
+def version_check() -> None:
+    """Check Python version"""
+    # pylint: disable=global-statement
+    global PY_SYS_VER, PY_SYS_STR
+    PY_SYS_VER = sys.version_info[0:3]
+    PY_SYS_STR = ".".join(str(x) for x in PY_SYS_VER)
+
+    if PY_SYS_VER < PY_MIN_VER:
+        # TODO: make this testable with: `class CliConfig`?
+        raise RuntimeError(
+            "ERROR: %s requires Python %s or later to run" % (__title__, PY_MIN_STR),
+            "HINT:  You're running Python %s" % PY_SYS_STR,
+        )
+
+
 PY_MIN_VER = (3, 4, 3)
 PY_SYS_VER = sys.version_info[0:3]
 PY_MIN_STR = ".".join(str(x) for x in PY_MIN_VER)
 PY_SYS_STR = ".".join(str(x) for x in PY_SYS_VER)
-if PY_SYS_VER < PY_MIN_VER:
-    # TODO: make this testable with: `class CliConfig`?
-    raise RuntimeError(  # pragma: no cover
-        "ERROR: %s requires Python %s or later to run" % (__title__, PY_MIN_STR),
-        "HINT:  You're running Python %s" % PY_SYS_STR,
-    )
+# Run the check
+version_check()
 
 # Console size, don't print more than it
 BUFFER_WD = shutil.get_terminal_size()[0]
 BUFFER_HT = shutil.get_terminal_size()[1]
 
 DEFAULT_RESULT_LIMIT = BUFFER_HT - 4
```

### Comparing `nutra-0.2.8.dev0/ntclient/__main__.py` & `nutra-0.2.8.dev1/ntclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/argparser/__init__.py` & `nutra-0.2.8.dev1/ntclient/argparser/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 from ntclient.argparser import types
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
 def build_subcommands(subparsers: argparse._SubParsersAction) -> None:
     """Attaches subcommands to main parser"""
 
-    build_init_subcommand(subparsers)
-    build_nt_subcommand(subparsers)
-    build_search_subcommand(subparsers)
-    build_sort_subcommand(subparsers)
-    build_analyze_subcommand(subparsers)
-    build_day_subcommand(subparsers)
-    build_recipe_subcommand(subparsers)
-    build_calc_subcommand(subparsers)
+    build_subcommand_init(subparsers)
+    build_subcommand_nt(subparsers)
+    build_subcommand_search(subparsers)
+    build_subcommand_sort(subparsers)
+    build_subcommand_analyze(subparsers)
+    build_subcommand_day(subparsers)
+    build_subcommand_recipe(subparsers)
+    build_subcommand_calc(subparsers)
     build_subcommand_bug(subparsers)
 
 
 ################################################################################
 # Methods to build subparsers, and attach back to main arg_parser
 ################################################################################
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_init_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_init(subparsers: argparse._SubParsersAction) -> None:
     """Self running init command"""
 
     init_parser = subparsers.add_parser(
         "init", help="setup profiles, USDA and NT database"
     )
     init_parser.add_argument(
         "-y",
@@ -42,25 +42,25 @@
         action="store_true",
         help="automatically agree to (potentially slow) USDA download",
     )
     init_parser.set_defaults(func=parser_funcs.init)
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_nt_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_nt(subparsers: argparse._SubParsersAction) -> None:
     """Lists out nutrients details with computed totals and averages"""
 
     nutrient_parser = subparsers.add_parser(
         "nt", help="list out nutrients and their info"
     )
     nutrient_parser.set_defaults(func=parser_funcs.nutrients)
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_search_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_search(subparsers: argparse._SubParsersAction) -> None:
     """Search: terms [terms ... ]"""
 
     search_parser = subparsers.add_parser(
         "search", help="search foods by name, list overview info"
     )
     search_parser.add_argument(
         "terms",
@@ -80,15 +80,15 @@
         type=int,
         help="filter by a specific food group ID",
     )
     search_parser.set_defaults(func=parser_funcs.search)
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_sort_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_sort(subparsers: argparse._SubParsersAction) -> None:
     """Sort foods ranked by nutr_id, per 100g or 200kcal"""
 
     sort_parser = subparsers.add_parser("sort", help="sort foods by nutrient ID")
 
     sort_parser.add_argument(
         "-c",
         dest="kcal",
@@ -103,15 +103,15 @@
         help="show top N results (defaults to console height)",
     )
     sort_parser.add_argument("nutr_id", type=int)
     sort_parser.set_defaults(func=parser_funcs.sort)
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_analyze_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_analyze(subparsers: argparse._SubParsersAction) -> None:
     """Analyzes (foods only for now)"""
 
     analyze_parser = subparsers.add_parser(
         "anl", help="analyze food(s), recipe(s), or day(s)"
     )
 
     analyze_parser.add_argument(
@@ -121,15 +121,15 @@
         help="scale to custom number of grams (default is 100g)",
     )
     analyze_parser.add_argument("food_id", type=int, nargs="+")
     analyze_parser.set_defaults(func=parser_funcs.analyze)
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_day_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_day(subparsers: argparse._SubParsersAction) -> None:
     """Analyzes a DAY.csv, uses new colored progress bar spec"""
 
     day_parser = subparsers.add_parser(
         "day", help="analyze a DAY.csv file, RDAs optional"
     )
     day_parser.add_argument(
         "food_log",
@@ -145,15 +145,15 @@
         type=types.file_path,
         help="provide a custom RDA file in csv format",
     )
     day_parser.set_defaults(func=parser_funcs.day)
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_recipe_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_recipe(subparsers: argparse._SubParsersAction) -> None:
     """View, add, edit, delete recipes"""
 
     recipe_parser = subparsers.add_parser("recipe", help="list and analyze recipes")
     recipe_parser.set_defaults(func=parser_funcs.recipes)
 
     recipe_subparsers = recipe_parser.add_subparsers(title="recipe subcommands")
 
@@ -182,15 +182,15 @@
     recipe_anl_parser.add_argument(
         "path", type=str, help="view (and analyze) recipe by file path"
     )
     recipe_anl_parser.set_defaults(func=parser_funcs.recipe)
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
-def build_calc_subcommand(subparsers: argparse._SubParsersAction) -> None:
+def build_subcommand_calc(subparsers: argparse._SubParsersAction) -> None:
     """BMR, 1 rep-max, and other calculators"""
 
     calc_parser = subparsers.add_parser(
         "calc", help="calculate 1-rep max, body fat, BMR, etc."
     )
 
     calc_subparsers = calc_parser.add_subparsers(title="calc subcommands")
@@ -318,14 +318,15 @@
     )
     calc_lbl_parser.add_argument(
         "ankle", type=float, nargs="?", help="ankle (cm) [casey_butt]"
     )
     calc_lbl_parser.set_defaults(func=parser_funcs.calc_lbm_limits)
 
 
+# noinspection PyUnresolvedReferences,PyProtectedMember
 def build_subcommand_bug(subparsers: argparse._SubParsersAction) -> None:
     """List and report bugs"""
 
     bug_parser = subparsers.add_parser("bug", help="report bugs")
     bug_subparser = bug_parser.add_subparsers(title="bug subcommands")
     bug_parser.add_argument(
         "--show", action="store_true", help="show list of unsubmitted bugs"
```

### Comparing `nutra-0.2.8.dev0/ntclient/argparser/funcs.py` & `nutra-0.2.8.dev1/ntclient/argparser/funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 import traceback
 
 from tabulate import tabulate
 
 import ntclient.services.analyze
 import ntclient.services.bugs
-import ntclient.services.recipe.utils
+import ntclient.services.recipe.recipe
 import ntclient.services.usda
 from ntclient.services import calculate as calc
 from ntclient.utils import CLI_CONFIG, Gender, activity_factor_from_index
 
 
 def init(args: argparse.Namespace) -> tuple:
     """Wrapper init method for persistence stuff"""
@@ -77,31 +77,31 @@
 ##############################################################################
 # Recipes
 ##############################################################################
 def recipes_init(args: argparse.Namespace) -> tuple:
     """Copy example/stock data into RECIPE_HOME"""
     _force = args.force
 
-    return ntclient.services.recipe.utils.recipes_init(_force=_force)
+    return ntclient.services.recipe.recipe.recipes_init(_force=_force)
 
 
 def recipes() -> tuple:
     """Show all, in tree or detail view"""
-    return ntclient.services.recipe.utils.recipes_overview()
+    return ntclient.services.recipe.recipe.recipes_overview()
 
 
 def recipe(args: argparse.Namespace) -> tuple:
     """
     View and analyze a single (or a range)
     @todo: argcomplete based on RECIPE_HOME folder
     @todo: use as default command? Currently this is reached by `nutra recipe anl`
     """
     recipe_path = args.path
 
-    return ntclient.services.recipe.utils.recipe_overview(recipe_path=recipe_path)
+    return ntclient.services.recipe.recipe.recipe_overview(recipe_path=recipe_path)
 
 
 ##############################################################################
 # Calculators
 ##############################################################################
 def calc_1rm(args: argparse.Namespace) -> tuple:
     """Perform 1-rep max calculations"""
@@ -337,46 +337,26 @@
 
     return 0, result
 
 
 ##############################################################################
 # Bug
 ##############################################################################
-# TODO: these all require args parameter due to parent parser defining a `--show` arg
+# TODO: these all require args parameter (due to parent parser defining a `--show` arg)
 
 
 # pylint: disable=unused-argument
 def bug_simulate(args: argparse.Namespace) -> tuple:
     """Simulate a bug report"""
     raise NotImplementedError("This service intentionally raises an error, for testing")
 
 
 def bugs_list(args: argparse.Namespace) -> tuple:
     """List bug reports that have been saved"""
-    _bugs_list = ntclient.services.bugs.list_bugs()
-    n_bugs_total = len(_bugs_list)
-    n_bugs_unsubmitted = len([x for x in _bugs_list if not bool(x[-1])])
-
-    print(f"You have: {n_bugs_total} total bugs amassed in your journey.")
-    print(f"Of these, {n_bugs_unsubmitted} require submission/reporting.")
-    print()
-
-    for bug in _bugs_list:
-        if not args.show:
-            continue
-        # Skip submitted bugs by default
-        if bool(bug[-1]) and not args.debug:
-            continue
-        # Print all bug properties (except noisy stacktrace)
-        print(", ".join(str(x) for x in bug if "\n" not in str(x)))
-
-    if n_bugs_unsubmitted > 0:
-        print("NOTE: You have bugs awaiting submission.  Please run the report command")
-
-    return 0, _bugs_list
+    return ntclient.services.bugs.list_bugs(show_all=args.show)
 
 
 # pylint: disable=unused-argument
 def bugs_report(args: argparse.Namespace) -> tuple:
     """Report bugs"""
     n_submissions = ntclient.services.bugs.submit_bugs()
     return 0, n_submissions
```

### Comparing `nutra-0.2.8.dev0/ntclient/argparser/types.py` & `nutra-0.2.8.dev1/ntclient/argparser/types.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/core/nnest.py` & `nutra-0.2.8.dev1/ntclient/core/nnest.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/core/nutprogbar.py` & `nutra-0.2.8.dev1/ntclient/core/nutprogbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
     # Tally the nutrient totals
     nut_amts = {}
     for food_id in _food_amts.keys():
         analysis = food_analyses_dict[food_id]
         for nutrient_id, amt in analysis.items():
             if nutrient_id not in nut_amts:
                 nut_amts[int(nutrient_id)] = amt
-            else:
-                nut_amts[int(nutrient_id)] += amt
+            else:  # pragma: no cover
+                # nut_amts[int(nutrient_id)] += amt
+                raise ValueError("Not implemented yet, need to sum up nutrient amounts")
 
     print_bars()
     return nut_amts
 
 
 def print_nutrient_bar(
     _n_id: int, _amount: float, _nutrients: Mapping[int, tuple]
```

### Comparing `nutra-0.2.8.dev0/ntclient/models/__init__.py` & `nutra-0.2.8.dev1/ntclient/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,35 +23,42 @@
         self.headers = tuple()  # type: ignore
         self.rows = tuple()  # type: ignore
 
         self.uuid = str()
 
         self.food_data = {}  # type: ignore
 
+    def _aggregate_rows(self) -> tuple:
+        """Aggregate rows into a tuple"""
+        print("Processing recipe file: %s" % self.file_path)
+        with open(self.file_path, "r", encoding="utf-8") as _file:
+            self.csv_reader = csv.DictReader(_file)
+            return tuple(list(self.csv_reader))
+
     def process_data(self) -> None:
         """
         Parses out the raw CSV input read in during self.__init__()
         TODO: test this with an empty CSV file, one with missing or corrupt values
-              (e.g. empty or non-numeric grams or food_id)
+              (e.g. empty or non-numeric grams or food_id).
+        TODO: test with a CSV file that has duplicate recipe_id/uuid values.
+        TODO: how is the recipe home directory determined here?
         """
 
         # Read into memory
-        print("Processing recipe file: %s" % self.file_path)
-        with open(self.file_path, "r", encoding="utf-8") as _file:
-            self.csv_reader = csv.DictReader(_file)
-            self.rows = tuple(self.csv_reader)
+        self.rows = self._aggregate_rows()
 
         # Validate data
         uuids = {x["recipe_id"] for x in self.rows}
         if len(uuids) != 1:
-            print("Found %s keys: %s" % (len(uuids), uuids))
+            print("ERROR: Found %s keys: %s" % (len(uuids), uuids))
             raise KeyError("FATAL: must have exactly 1 uuid per recipe CSV file!")
         self.uuid = list(uuids)[0]
 
         # exc: ValueError (could not cast int / float)
         self.food_data = {int(x["food_id"]): float(x["grams"]) for x in self.rows}
 
         if CLI_CONFIG.debug:
             print("Finished with recipe.")
 
     def print_analysis(self) -> None:
         """Run analysis on a single recipe"""
+        # TODO: implement this
```

### Comparing `nutra-0.2.8.dev0/ntclient/ntsqlite/sql/__init__.py` & `nutra-0.2.8.dev1/ntclient/ntsqlite/sql/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Builds and inserts stock data into nt.sqlite3"""
     # cd into this script's directory
     os.chdir(SCRIPT_DIR)
 
     if verbose:
         print("Cleanup...")
     if os.path.isfile(NT_DB_NAME):
-        os.remove(NT_DB_NAME)
+        os.remove(NT_DB_NAME)  # pragma: no cover
 
     if verbose:
         # pylint: disable=consider-using-f-string
         print("\nPack %s" % NT_DB_NAME)
     con = sqlite3.connect(NT_DB_NAME)
     cur = con.cursor()
 
@@ -58,8 +58,8 @@
     con.close()
     if verbose:
         print("\nDone!")
     return True
 
 
 if __name__ == "__main__":
-    build_ntsqlite(verbose=True)
+    build_ntsqlite(verbose=True)  # pragma: no cover
```

### Comparing `nutra-0.2.8.dev0/ntclient/ntsqlite/sql/data/rda.csv` & `nutra-0.2.8.dev1/ntclient/ntsqlite/sql/data/rda.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/ntsqlite/sql/functions.sql` & `nutra-0.2.8.dev1/ntclient/ntsqlite/sql/functions.sql`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/ntsqlite/sql/tables.sql` & `nutra-0.2.8.dev1/ntclient/ntsqlite/sql/tables.sql`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/persistence/__init__.py` & `nutra-0.2.8.dev1/ntclient/persistence/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 @author: shane
 """
 import configparser
 import os
 
 from ntclient import NUTRA_HOME
 
-# TODO: create and maintain prefs.json file?  See if there's a library for that, lol
-
 PREFS_FILE = os.path.join(NUTRA_HOME, "prefs.ini")
 
 os.makedirs(NUTRA_HOME, 0o755, exist_ok=True)
 
 if not os.path.isfile(PREFS_FILE):  # pragma: no cover
     print("INFO: Generating prefs.ini file")
     config = configparser.ConfigParser()
```

### Comparing `nutra-0.2.8.dev0/ntclient/persistence/sql/__init__.py` & `nutra-0.2.8.dev1/ntclient/persistence/sql/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 from ntclient.utils import CLI_CONFIG
 
 # ------------------------------------------------
 # Entry fetching methods
 # ------------------------------------------------
 
 
-def sql_entries(sql_result: sqlite3.Cursor) -> list:
-    """Formats and returns a `sql_result()` for console digestion and output"""
-    # TODO: return object: metadata, command, status, errors, etc?
-
-    rows = sql_result.fetchall()
-    return rows
+def sql_entries(sql_result: sqlite3.Cursor) -> tuple:
+    """
+    Formats and returns a `sql_result()` for console digestion and output
+    FIXME: the IDs are not necessarily integers, but are unique.
 
+    TODO: return object: metadata, command, status, errors, etc?
+    """
 
-def sql_entries_headers(sql_result: sqlite3.Cursor) -> tuple:
-    """Formats and returns a `sql_result()` for console digestion and output"""
     rows = sql_result.fetchall()
-    headers = [x[0] for x in sql_result.description]
+    headers = [x[0] for x in (sql_result.description if sql_result.description else [])]
 
-    return headers, rows
+    return (
+        rows,
+        headers,
+        sql_result.rowcount,
+        sql_result.lastrowid,
+    )
 
 
 # ------------------------------------------------
 # Supporting methods
 # ------------------------------------------------
 def version(con: sqlite3.Connection) -> str:
     """Gets the latest entry from version table"""
@@ -73,49 +76,36 @@
         if values:
             # TODO: better debug logging, more "control-findable",
             #  distinguish from most prints()
             print(values)
 
     # TODO: separate `entry` & `entries` entity for single vs. bulk insert?
     if values:
-        if isinstance(values, list):
-            cur.executemany(query, values)
-        else:  # tuple
+        if isinstance(values, tuple):
             cur.execute(query, values)
+        # elif isinstance(values, list):
+        #     cur.executemany(query, values)
+        else:
+            raise TypeError("'values' must be a list or tuple!")
+
     else:
         cur.execute(query)
 
     return cur
 
 
 def _sql(
     con: sqlite3.Connection,
     query: str,
     db_name: str,
     values: Sequence = (),
-) -> list:
+) -> tuple:
     """@param values: tuple | list"""
 
     cur = _prep_query(con, query, db_name, values)
 
     # TODO: print "<number> SELECTED", or other info
     #  BASED ON command SELECT/INSERT/DELETE/UPDATE
     result = sql_entries(cur)
 
     close_con_and_cur(con, cur)
     return result
-
-
-def _sql_headers(
-    con: sqlite3.Connection,
-    query: str,
-    db_name: str,
-    values: Sequence = (),
-) -> tuple:
-    """@param values: tuple | list"""
-
-    cur = _prep_query(con, query, db_name, values)
-
-    result = sql_entries_headers(cur)
-
-    close_con_and_cur(con, cur)
-    return result
```

### Comparing `nutra-0.2.8.dev0/ntclient/persistence/sql/nt/__init__.py` & `nutra-0.2.8.dev1/ntclient/persistence/sql/nt/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ntclient import (
     NT_DB_NAME,
     NTSQLITE_BUILDPATH,
     NTSQLITE_DESTINATION,
     NUTRA_HOME,
     __db_target_nt__,
 )
-from ntclient.persistence.sql import _sql, _sql_headers, version
+from ntclient.persistence.sql import _sql, version
 from ntclient.utils.exceptions import SqlConnectError, SqlInvalidVersionError
 
 
 def nt_ver() -> str:
     """Gets version string for nt.sqlite3 database"""
 
     con = nt_sqlite_connect(version_check=False)
@@ -76,19 +76,12 @@
             )
         return con
 
     # Else it's not on disk
     raise SqlConnectError("ERROR: nt database doesn't exist, please run `nutra init`")
 
 
-def sql(query: str, values: Sequence = ()) -> list:
+def sql(query: str, values: Sequence = ()) -> tuple:
     """Executes a SQL command to nt.sqlite3"""
 
     con = nt_sqlite_connect()
     return _sql(con, query, db_name="nt", values=values)
-
-
-def sql_headers(query: str, values: Sequence = ()) -> tuple:
-    """Executes a SQL command to nt.sqlite3"""
-
-    con = nt_sqlite_connect()
-    return _sql_headers(con, query, db_name="nt", values=values)
```

### Comparing `nutra-0.2.8.dev0/ntclient/persistence/sql/usda/__init__.py` & `nutra-0.2.8.dev1/ntclient/persistence/sql/usda/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sqlite3
 import tarfile
 import urllib.request
 from collections.abc import Sequence
 
 from ntclient import NUTRA_HOME, USDA_DB_NAME, __db_target_usda__
-from ntclient.persistence.sql import _sql, _sql_headers, version
+from ntclient.persistence.sql import _sql, version
 from ntclient.utils.exceptions import SqlConnectError, SqlInvalidVersionError
 
 
 def usda_init(yes: bool = False) -> None:
     """On-boarding function. Downloads tarball and unpacks usda.sqlite3 file"""
 
     def input_agree() -> str:
@@ -94,15 +94,15 @@
 def usda_ver() -> str:
     """Gets version string for usda.sqlite3 database"""
 
     con = usda_sqlite_connect(version_check=False)
     return version(con)
 
 
-def sql(query: str, values: Sequence = (), version_check: bool = True) -> list:
+def sql(query: str, values: Sequence = (), version_check: bool = True) -> tuple:
     """
     Executes a SQL command to usda.sqlite3
 
     @param query: Input SQL query
     @param values: Union[tuple, list] Leave as empty tuple for no values,
         e.g. bare query. Populate a tuple for a single insert. And use a list for
         cur.executemany()
@@ -110,25 +110,7 @@
     @return: List of selected SQL items
     """
 
     con = usda_sqlite_connect(version_check=version_check)
 
     # TODO: support argument: _sql(..., params=params, ...)
     return _sql(con, query, db_name="usda", values=values)
-
-
-def sql_headers(query: str, values: Sequence = (), version_check: bool = True) -> tuple:
-    """
-    Executes a SQL command to usda.sqlite3 [WITH HEADERS]
-
-    @param query: Input SQL query
-    @param values: Union[tuple, list] Leave as empty tuple for no values,
-        e.g. bare query. Populate a tuple for a single insert. And use a list for
-        cur.executemany()
-    @param version_check: Ignore mismatch version, useful for "meta" commands
-    @return: List of selected SQL items
-    """
-
-    con = usda_sqlite_connect(version_check=version_check)
-
-    # TODO: support argument: _sql(..., params=params, ...)
-    return _sql_headers(con, query, db_name="usda", values=values)
```

### Comparing `nutra-0.2.8.dev0/ntclient/persistence/sql/usda/funcs.py` & `nutra-0.2.8.dev1/ntclient/persistence/sql/usda/funcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """usda.sqlite functions module"""
 
 from ntclient import NUTR_ID_KCAL
-from ntclient.persistence.sql.usda import sql, sql_headers
+from ntclient.persistence.sql.usda import sql
 
 
 ################################################################################
 # Basic functions
 ################################################################################
 def sql_fdgrp() -> dict:
     """Shows food groups"""
 
     query = "SELECT * FROM fdgrp;"
-    result = sql(query)
-    return {x[0]: x for x in result}
+    rows, _, _, _ = sql(query)
+    return {x[0]: x for x in rows}
 
 
 def sql_food_details(_food_ids: set = None) -> list:  # type: ignore
     """Readable human details for foods"""
 
     if not _food_ids:
         query = "SELECT * FROM food_des;"
     else:
         # TODO: does sqlite3 driver support this? cursor.executemany() ?
         query = "SELECT * FROM food_des WHERE id IN (%s);"
         food_ids = ",".join(str(x) for x in set(_food_ids))
         query = query % food_ids
 
-    return sql(query)
+    rows, _, _, _ = sql(query)
+    return list(rows)
 
 
 def sql_nutrients_overview() -> dict:
     """Shows nutrients overview"""
 
     query = "SELECT * FROM nutrients_overview;"
-    result = sql(query)
-    return {x[0]: x for x in result}
+    rows, _, _, _ = sql(query)
+    return {x[0]: x for x in rows}
 
 
 def sql_nutrients_details() -> tuple:
     """Shows nutrients 'details'"""
 
     query = "SELECT * FROM nutrients_overview;"
-    return sql_headers(query)
+    rows, headers, _, _ = sql(query)
+    return rows, headers
 
 
 def sql_servings(_food_ids: set) -> list:
     """Food servings"""
     # TODO: apply connective logic from `sort_foods()` IS ('None') ?
     query = """
 SELECT
@@ -57,15 +59,16 @@
   serving serv
   LEFT JOIN serv_desc ON serv.msre_id = serv_desc.id
 WHERE
   serv.food_id IN (%s);
 """
     # FIXME: support this kind of thing by library code & parameterized queries
     food_ids = ",".join(str(x) for x in set(_food_ids))
-    return sql(query % food_ids)
+    rows, _, _, _ = sql(query % food_ids)
+    return list(rows)
 
 
 def sql_analyze_foods(food_ids: set) -> list:
     """Nutrient analysis for foods"""
     query = """
 SELECT
   id,
@@ -75,15 +78,16 @@
   food_des
   INNER JOIN nut_data ON food_des.id = nut_data.food_id
 WHERE
   food_des.id IN (%s);
 """
     # TODO: parameterized queries
     food_ids_concat = ",".join(str(x) for x in set(food_ids))
-    return sql(query % food_ids_concat)
+    rows, _, _, _ = sql(query % food_ids_concat)
+    return list(rows)
 
 
 ################################################################################
 # Sort
 ################################################################################
 def sql_sort_helper1(nutrient_id: int) -> list:
     """Selects relevant bits from nut_data for sorting"""
@@ -97,18 +101,20 @@
   nut_data
 WHERE
   nutr_id = %s
   OR nutr_id = %s
 ORDER BY
   food_id;
 """
-
-    return sql(query % (NUTR_ID_KCAL, nutrient_id))
+    # TODO: parameterized queries
+    rows, _, _, _ = sql(query % (NUTR_ID_KCAL, nutrient_id))
+    return list(rows)
 
 
+# TODO: these functions are unused, replace `sql_sort_helper1` (above) with these two
 def sql_sort_foods(nutr_id: int) -> list:
     """Sort foods by nutr_id per 100 g"""
 
     query = """
 SELECT
   nut_data.food_id,
   fdgrp_id,
@@ -123,16 +129,17 @@
   LEFT JOIN nut_data kcal ON food.id = kcal.food_id
     AND kcal.nutr_id = 208
 WHERE
   nut_data.nutr_id = %s
 ORDER BY
   nut_data.nutr_val DESC;
 """
-
-    return sql(query % nutr_id)
+    # TODO: parameterized queries
+    rows, _, _, _ = sql(query % nutr_id)
+    return list(rows)
 
 
 def sql_sort_foods_by_kcal(nutr_id: int) -> list:
     """Sort foods by nutr_id per 200 kcal"""
 
     # TODO: use parameterized queries
     query = """
@@ -152,9 +159,10 @@
     AND kcal.nutr_id = 208
     AND kcal.nutr_val > 0
 WHERE
   nut_data.nutr_id = %s
 ORDER BY
   (nut_data.nutr_val / kcal.nutr_val) DESC;
 """
-
-    return sql(query % nutr_id)
+    # TODO: parameterized queries
+    rows, _, _, _ = sql(query % nutr_id)
+    return list(rows)
```

### Comparing `nutra-0.2.8.dev0/ntclient/resources/recipe/dinner/burrito-bowl.csv` & `nutra-0.2.8.dev1/ntclient/resources/recipe/dinner/burrito-bowl.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/resources/recipe/snack/buckwheat-pancake.csv` & `nutra-0.2.8.dev1/ntclient/resources/recipe/snack/buckwheat-pancake.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/resources/recipe/tmp/food_amounts.csv` & `nutra-0.2.8.dev1/ntclient/resources/recipe/tmp/food_amounts.csv`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/services/__init__.py` & `nutra-0.2.8.dev1/ntclient/services/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,27 @@
     @return: tuple[int, bool]
     """
 
     print("Nutra directory  ", end="")
     if not os.path.isdir(NUTRA_HOME):
         os.makedirs(NUTRA_HOME, 0o755)
     print("..DONE!")
+    # TODO: should creating preferences/settings file be handled in persistence module?
 
     # TODO: print off checks, return False if failed
     print("USDA db          ", end="")
     usda_init(yes=yes)
     print("..DONE!")
 
     print("Nutra db         ", end="")
     build_ntsqlite()
     nt_init()
 
-    print("\nAll checks have passed!")
+    print("\nSuccess!  All checks have passed!")
     print(
         """
-Nutrient tracker is free software. It comes with NO warranty or guarantee.
+Nutrient Tracker is free software. It comes with NO warranty or guarantee.
 You may use it as you please.
-You may make changes, as long as you disclose and publish them.
+You may make changes as long as you disclose and publish them.
     """
     )
     return 0, True
```

### Comparing `nutra-0.2.8.dev0/ntclient/services/analyze.py` & `nutra-0.2.8.dev1/ntclient/services/analyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,17 @@
 
 ##############################################################################
 # Foods
 ##############################################################################
 def foods_analyze(food_ids: set, grams: float = 100) -> tuple:
     """
     Analyze a list of food_ids against stock RDA values
-    TODO: from ntclient.utils.nutprogbar import nutprogbar
-    TODO: support -t (tabular/non-visual) output flag
+    (NOTE: only supports a single food for now... add compare foods support later)
+    TODO: support flag -t (tabular/non-visual output)
+    TODO: support flag -s (scale to 2000 kcal)
     """
 
     ##########################################################################
     # Get analysis
     ##########################################################################
     raw_analyses = sql_analyze_foods(food_ids)
     analyses = {}
@@ -100,15 +101,14 @@
             print(refuse[0])
             print("    ({0}%, by mass)".format(refuse[1]))
 
         ######################################################################
         # Nutrient colored RDA tree-view
         ######################################################################
         print_header("NUTRITION")
-        headers = ["id", "nutrient", "rda %", "amount", "units"]
         nutrient_rows = []
         # TODO: skip small values (<1% RDA), report as color bar if RDA is available
         for nutrient_id, amount in nut_val_tuples:
             # Skip zero values
             if not amount:
                 continue
 
@@ -122,28 +122,29 @@
             else:
                 rda_perc = None
             row = [nutrient_id, nutr_desc, rda_perc, round(amount, 2), unit]
 
             # Add to list
             nutrient_rows.append(row)
 
+        # Add to list of lists
+        nutrients_rows.append(nutrient_rows)
+
         # Print view
-        # TODO: nested, color-coded tree view
         # TODO: either make this function singular, or handle plural logic here
         _food_id = list(food_ids)[0]
         nutrient_progress_bars(
             {_food_id: grams},
             [(_food_id, x[0], x[1]) for x in analyses[_food_id]],
             nutrients,
         )
-        # BEGIN: deprecated code
+        # TODO: make this into the `-t` or `--tabular` branch of the function
+        # headers = ["id", "nutrient", "rda %", "amount", "units"]
         # table = tabulate(nutrient_rows, headers=headers, tablefmt="presto")
         # print(table)
-        # END: deprecated code
-        nutrients_rows.append(nutrient_rows)
 
     return 0, nutrients_rows, servings_rows
 
 
 ##############################################################################
 # Day
 ##############################################################################
```

### Comparing `nutra-0.2.8.dev0/ntclient/services/api/__init__.py` & `nutra-0.2.8.dev1/ntclient/services/api/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Feb 13 14:28:20 2024
 
 @author: shane
 """
-import sqlite3
-
 import requests
 
 REQUEST_READ_TIMEOUT = 18
 REQUEST_CONNECT_TIMEOUT = 5
 
 # TODO: try all of these; cache (save in prefs.json) the one which works first
 URLS_API = (
@@ -29,18 +26,18 @@
                 mirror,
                 timeout=(REQUEST_CONNECT_TIMEOUT, REQUEST_READ_TIMEOUT),
                 verify=mirror.startswith("https://"),
             )
 
             _res.raise_for_status()
             # TODO: save in persistence config.ini
-            print(f"INFO: mirror SUCCESS '{mirror}'")
+            print("INFO: mirror SUCCESS '%s'" % mirror)
             return mirror
-        except requests.exceptions.ConnectionError:  # pragma: no cover
-            print(f"WARN: mirror FAILURE '{mirror}'")
+        except (requests.exceptions.ConnectionError, requests.exceptions.HTTPError):
+            print("WARN: mirror FAILURE '%s'" % mirror)
 
     return str()
 
 
 class ApiClient:
     """Client for connecting to the remote server/API."""
 
@@ -48,18 +45,18 @@
         self.host = cache_mirrors()
         if not self.host:  # pragma: no cover
             raise ConnectionError("Cannot find suitable API host!")
 
     def post(self, path: str, data: dict) -> requests.Response:
         """Post data to the API."""
         _res = requests.post(
-            f"{self.host}/{path}",
+            self.host + "/" + path,
             json=data,
             timeout=(REQUEST_CONNECT_TIMEOUT, REQUEST_READ_TIMEOUT),
         )
-        # _res.raise_for_status()
+        _res.raise_for_status()
         return _res
 
     # TODO: move this outside class; support with host iteration helper method
-    def post_bug(self, bug: sqlite3.Row) -> requests.Response:
+    def post_bug(self, bug: dict) -> requests.Response:
         """Post a bug report to the developer."""
-        return self.post("bug", dict(bug))
+        return self.post("bug", bug)
```

### Comparing `nutra-0.2.8.dev0/ntclient/services/calculate.py` & `nutra-0.2.8.dev1/ntclient/services/calculate.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/services/recipe/csv_utils.py` & `nutra-0.2.8.dev1/ntclient/services/recipe/csv_utils.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/services/recipe/utils.py` & `nutra-0.2.8.dev1/ntclient/services/recipe/recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     @return: (exit_code: int, None)
     """
 
     try:
         csv_utils.csv_recipe_print_tree()
         return 0, None
-    except FileNotFoundError:
+    except FileNotFoundError:  # pragma: no covers
         print("WARN: no recipes found, create some or run: nutra recipe init")
         return 1, None
 
 
 def recipe_overview(recipe_path: str) -> tuple:
     """
     Shows single recipe overview
```

### Comparing `nutra-0.2.8.dev0/ntclient/services/usda.py` & `nutra-0.2.8.dev1/ntclient/services/usda.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 from ntclient.utils import CLI_CONFIG
 
 
 def list_nutrients() -> tuple:
     """Lists out nutrients with basic details"""
 
-    headers, nutrients = sql_nutrients_details()
+    nutrients, headers = sql_nutrients_details()
     # TODO: include in SQL table cache?
     headers.append("avg_rda")
     nutrients = [list(x) for x in nutrients]
     for nutrient in nutrients:
         rda = nutrient[1]
         val = nutrient[6]
         if rda:
@@ -57,26 +57,25 @@
 def sort_foods(
     nutrient_id: int, by_kcal: bool, limit: int = DEFAULT_RESULT_LIMIT
 ) -> tuple:
     """Sort, by nutrient, either (amount / 100 g) or (amount / 200 kcal)"""
 
     # TODO: sub shrt_desc for long if available, and support config.FOOD_NAME_TRUNC
 
-    def print_results(_results: list, _nutrient_id: int) -> list:
+    def print_results(_results: list, _nutrient_id: int) -> None:
         """Prints truncated list for sort"""
         nutrients = sql_nutrients_overview()
         nutrient = nutrients[_nutrient_id]
         unit = nutrient[2]
 
         val_header = "grams" if by_kcal else "kcal"
         headers = ["food", "fdgrp", "val (%s)" % unit, val_header, "long_desc"]
 
         table = tabulate(_results, headers=headers, tablefmt="simple")
         print(table)
-        return _results
 
     # Gets values for nutrient_id and kcal=208
     nut_data = sql_sort_helper1(nutrient_id)
 
     # Assembles duplicate tuples into single dict entry
     food_dat = {}
     for food_id, nutr_id, nutr_val in nut_data:
```

### Comparing `nutra-0.2.8.dev0/ntclient/utils/__init__.py` & `nutra-0.2.8.dev1/ntclient/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Sun Mar 26 23:07:30 2023
 
 @author: shane
 """
 import argparse
```

### Comparing `nutra-0.2.8.dev0/ntclient/utils/colors.py` & `nutra-0.2.8.dev1/ntclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/utils/exceptions.py` & `nutra-0.2.8.dev1/ntclient/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/ntclient/utils/tree.py` & `nutra-0.2.8.dev1/ntclient/utils/tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 colorize(os.readlink(path), full=True),
             ]
         )
 
     if os.path.isdir(path):
         return "".join([COLOR_DIR, file, colors.STYLE_RESET_ALL])
 
-    if os.access(path, os.X_OK):
+    if os.access(path, os.X_OK):  # pragma: no cover
         return "".join([COLOR_EXEC, file, colors.STYLE_RESET_ALL])
 
     return file
 
 
 # Tree properties - display / print
 SHOW_HIDDEN = False
@@ -64,19 +64,19 @@
 
     if not pre:
         print(COLOR_DIR + _dir + colors.STYLE_RESET_ALL)
 
     dir_len = len(os.listdir(_dir)) - 1
     for i, file in enumerate(sorted(os.listdir(_dir), key=str.lower)):
         path = os.path.join(_dir, file)
-        if file.startswith(".") and not SHOW_HIDDEN:
+        if file.startswith(".") and not SHOW_HIDDEN:  # pragma: no cover
             continue
         if os.path.isdir(path):
             print(pre + strs[2 if i == dir_len else 1] + colorize(path))
-            if os.path.islink(path):
+            if os.path.islink(path):  # pragma: no cover
                 n_dirs += 1
             else:
                 n_d, n_f, n_s = print_dir(path, pre + strs[3 if i == dir_len else 0])
                 n_dirs += n_d + 1
                 n_files += n_f
                 n_size += n_s
         else:
```

### Comparing `nutra-0.2.8.dev0/nutra.egg-info/PKG-INFO` & `nutra-0.2.8.dev1/nutra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutra
-Version: 0.2.8.dev0
+Version: 0.2.8.dev1
 Summary: Home and office nutrient tracking software
 Home-page: https://github.com/nutratech/cli
 Author: Shane Jaroch
 Author-email: chown_tee@proton.me
 License: GPL v3
 Platform: linux
 Platform: darwin
@@ -134,15 +134,15 @@
     # Need to add hook, too
     # See: https://direnv.net/docs/hook.html
     DEFAULT_SHELL=$(basename $SHELL)
     SHELL_RC_FILE=~/.${DEFAULT_SHELL}rc
     HOOK='eval "$(direnv hook '$DEFAULT_SHELL')"'
 
     # Install the hook, if not already
-    grep "$HOOK" $SHELL_RC_FILE || echo "$HOOK" >>$SHELL_RC_FILE
+    grep ^"$HOOK"$ $SHELL_RC_FILE || echo "$HOOK" >>$SHELL_RC_FILE
     source $SHELL_RC_FILE
 
 This is what the ``.envrc`` file is for. It automatically activates ``venv``.
 
 
 
 Notes
```

### Comparing `nutra-0.2.8.dev0/nutra.egg-info/SOURCES.txt` & `nutra-0.2.8.dev1/nutra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ntclient/services/analyze.py
 ntclient/services/bugs.py
 ntclient/services/calculate.py
 ntclient/services/usda.py
 ntclient/services/api/__init__.py
 ntclient/services/recipe/__init__.py
 ntclient/services/recipe/csv_utils.py
-ntclient/services/recipe/utils.py
+ntclient/services/recipe/recipe.py
 ntclient/utils/__init__.py
 ntclient/utils/colors.py
 ntclient/utils/exceptions.py
 ntclient/utils/sql.py
 ntclient/utils/tree.py
 nutra.egg-info/PKG-INFO
 nutra.egg-info/SOURCES.txt
```

### Comparing `nutra-0.2.8.dev0/setup.cfg` & `nutra-0.2.8.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nutra-0.2.8.dev0/setup.py` & `nutra-0.2.8.dev1/setup.py`

 * *Files identical despite different names*

