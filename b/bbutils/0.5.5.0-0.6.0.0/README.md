# Comparing `tmp/bbutils-0.5.5.0.tar.gz` & `tmp/bbutils-0.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbutils-0.5.5.0.tar", last modified: Fri Sep  1 11:11:18 2023, max compression
+gzip compressed data, was "bbutils-0.6.0.0.tar", last modified: Mon Sep 18 14:40:28 2023, max compression
```

## Comparing `bbutils-0.5.5.0.tar` & `bbutils-0.6.0.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.526099 bbutils-0.5.5.0/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    11357 2021-10-19 14:00:40.000000 bbutils-0.5.5.0/LICENSE
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     8032 2023-09-01 11:11:18.526099 bbutils-0.5.5.0/PKG-INFO
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     7455 2023-08-21 14:41:04.000000 bbutils-0.5.5.0/README.md
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2248 2023-09-01 11:09:45.000000 bbutils-0.5.5.0/bbutil/__init__.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/app/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      978 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/bbutil/app/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4745 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/bbutil/app/config.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3438 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/bbutil/app/console.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1942 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/bbutil/app/manager.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2720 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/bbutil/app/module.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5141 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/data.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/database/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1077 2023-08-31 09:58:48.000000 bbutils-0.5.5.0/bbutil/database/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2315 2023-09-01 10:57:20.000000 bbutils-0.5.5.0/bbutil/database/database.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/database/sqlite/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    14223 2023-08-31 15:44:14.000000 bbutils-0.5.5.0/bbutil/database/sqlite/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4275 2023-08-31 15:41:38.000000 bbutils-0.5.5.0/bbutil/database/sqlite/manager.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      967 2023-08-31 10:01:55.000000 bbutils-0.5.5.0/bbutil/database/sqlite/types.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     7204 2023-09-01 10:54:19.000000 bbutils-0.5.5.0/bbutil/database/table.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2263 2023-08-21 14:41:04.000000 bbutils-0.5.5.0/bbutil/database/types.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4047 2023-08-23 11:09:07.000000 bbutils-0.5.5.0/bbutil/execute.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3541 2023-08-22 11:52:18.000000 bbutils-0.5.5.0/bbutil/file.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/lang/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2965 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/lang/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1988 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/lang/domain.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/lang/parser/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    11805 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/lang/parser/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1371 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/lang/parser/domain.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1209 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/lang/parser/language.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3173 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/lang/parser/pyfile.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/logging/
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     7885 2021-12-10 15:08:49.000000 bbutils-0.5.5.0/bbutil/logging/__init__.py
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     4378 2021-10-19 14:00:40.000000 bbutils-0.5.5.0/bbutil/logging/types.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/logging/writer/
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)      748 2023-08-23 13:09:30.000000 bbutils-0.5.5.0/bbutil/logging/writer/__init__.py
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     7374 2021-12-10 15:08:49.000000 bbutils-0.5.5.0/bbutil/logging/writer/console.py
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     4532 2021-10-19 14:00:40.000000 bbutils-0.5.5.0/bbutil/logging/writer/file.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5509 2023-08-23 13:09:30.000000 bbutils-0.5.5.0/bbutil/logging/writer/qt.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4359 2023-08-23 13:09:30.000000 bbutils-0.5.5.0/bbutil/logging/writer/tkinter.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2182 2023-08-23 12:11:06.000000 bbutils-0.5.5.0/bbutil/setup.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5961 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/bbutil/utils.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutil/worker/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3660 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/bbutil/worker/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2289 2023-08-22 13:48:09.000000 bbutils-0.5.5.0/bbutil/worker/callback.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.522099 bbutils-0.5.5.0/bbutils.egg-info/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     8032 2023-09-01 11:11:18.000000 bbutils-0.5.5.0/bbutils.egg-info/PKG-INFO
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1513 2023-09-01 11:11:18.000000 bbutils-0.5.5.0/bbutils.egg-info/SOURCES.txt
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)        1 2023-09-01 11:11:18.000000 bbutils-0.5.5.0/bbutils.egg-info/dependency_links.txt
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)        9 2023-09-01 11:11:18.000000 bbutils-0.5.5.0/bbutils.egg-info/requires.txt
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)       13 2023-09-01 11:11:18.000000 bbutils-0.5.5.0/bbutils.egg-info/top_level.txt
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     1769 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/make-lang.py
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)    13993 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/run-tests.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)       38 2023-09-01 11:11:18.530099 bbutils-0.5.5.0/setup.cfg
--rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     1669 2021-11-03 11:12:22.000000 bbutils-0.5.5.0/setup.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.518099 bbutils-0.5.5.0/tests/
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.526099 bbutils-0.5.5.0/tests/app/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      739 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/app/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     9773 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/app/config.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4178 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/app/console.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1951 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/app/manager.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3785 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/app/module.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.526099 bbutils-0.5.5.0/tests/database/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      710 2023-08-21 14:41:04.000000 bbutils-0.5.5.0/tests/database/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4946 2023-09-01 11:00:50.000000 bbutils-0.5.5.0/tests/database/database.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     9299 2023-09-01 10:25:45.000000 bbutils-0.5.5.0/tests/database/manager.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    25794 2023-09-01 10:22:04.000000 bbutils-0.5.5.0/tests/database/sqlite.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    13190 2023-09-01 10:54:59.000000 bbutils-0.5.5.0/tests/database/table.py
-drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-01 11:11:18.526099 bbutils-0.5.5.0/tests/helper/
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2832 2023-08-31 14:05:26.000000 bbutils-0.5.5.0/tests/helper/__init__.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2798 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/helper/config.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2184 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/helper/console.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2270 2023-09-01 11:01:32.000000 bbutils-0.5.5.0/tests/helper/database.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3080 2023-08-23 11:09:07.000000 bbutils-0.5.5.0/tests/helper/execute.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      965 2023-08-22 11:52:18.000000 bbutils-0.5.5.0/tests/helper/file.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1905 2023-09-01 11:08:09.000000 bbutils-0.5.5.0/tests/helper/setup.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5271 2023-08-31 14:13:46.000000 bbutils-0.5.5.0/tests/helper/sqlite.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2788 2023-08-22 11:52:18.000000 bbutils-0.5.5.0/tests/helper/table.py
--rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3432 2023-08-24 14:30:20.000000 bbutils-0.5.5.0/tests/helper/worker.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.816542 bbutils-0.6.0.0/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    11357 2021-10-19 14:00:40.000000 bbutils-0.6.0.0/LICENSE
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     8032 2023-09-18 14:40:28.816542 bbutils-0.6.0.0/PKG-INFO
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     7455 2023-08-21 14:41:04.000000 bbutils-0.6.0.0/README.md
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.808543 bbutils-0.6.0.0/bbutil/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2248 2023-09-18 14:39:27.000000 bbutils-0.6.0.0/bbutil/__init__.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.808543 bbutils-0.6.0.0/bbutil/app/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      978 2023-08-24 14:30:20.000000 bbutils-0.6.0.0/bbutil/app/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4745 2023-08-24 14:30:20.000000 bbutils-0.6.0.0/bbutil/app/config.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3409 2023-09-18 13:57:23.000000 bbutils-0.6.0.0/bbutil/app/console.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1498 2023-09-18 14:24:07.000000 bbutils-0.6.0.0/bbutil/app/manager.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2523 2023-09-18 14:28:34.000000 bbutils-0.6.0.0/bbutil/app/module.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5141 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/data.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.808543 bbutils-0.6.0.0/bbutil/database/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1077 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/bbutil/database/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2315 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/bbutil/database/database.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/bbutil/database/sqlite/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    14223 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/bbutil/database/sqlite/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4275 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/bbutil/database/sqlite/manager.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      967 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/bbutil/database/sqlite/types.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     7204 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/bbutil/database/table.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2263 2023-08-21 14:41:04.000000 bbutils-0.6.0.0/bbutil/database/types.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4047 2023-08-23 11:09:07.000000 bbutils-0.6.0.0/bbutil/execute.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3541 2023-08-22 11:52:18.000000 bbutils-0.6.0.0/bbutil/file.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/bbutil/lang/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2965 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/lang/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1988 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/lang/domain.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/bbutil/lang/parser/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    11805 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/lang/parser/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1371 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/lang/parser/domain.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1209 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/lang/parser/language.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3173 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/lang/parser/pyfile.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/bbutil/logging/
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     7885 2021-12-10 15:08:49.000000 bbutils-0.6.0.0/bbutil/logging/__init__.py
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     4378 2021-10-19 14:00:40.000000 bbutils-0.6.0.0/bbutil/logging/types.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/bbutil/logging/writer/
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)      748 2023-08-23 13:09:30.000000 bbutils-0.6.0.0/bbutil/logging/writer/__init__.py
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     7374 2021-12-10 15:08:49.000000 bbutils-0.6.0.0/bbutil/logging/writer/console.py
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     4532 2021-10-19 14:00:40.000000 bbutils-0.6.0.0/bbutil/logging/writer/file.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5509 2023-08-23 13:09:30.000000 bbutils-0.6.0.0/bbutil/logging/writer/qt.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4359 2023-08-23 13:09:30.000000 bbutils-0.6.0.0/bbutil/logging/writer/tkinter.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2182 2023-08-23 12:11:06.000000 bbutils-0.6.0.0/bbutil/setup.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5961 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/bbutil/utils.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/bbutil/worker/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3660 2023-08-24 14:30:20.000000 bbutils-0.6.0.0/bbutil/worker/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2289 2023-08-22 13:48:09.000000 bbutils-0.6.0.0/bbutil/worker/callback.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/bbutils.egg-info/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     8032 2023-09-18 14:40:28.000000 bbutils-0.6.0.0/bbutils.egg-info/PKG-INFO
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1536 2023-09-18 14:40:28.000000 bbutils-0.6.0.0/bbutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)        1 2023-09-18 14:40:28.000000 bbutils-0.6.0.0/bbutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)        9 2023-09-18 14:40:28.000000 bbutils-0.6.0.0/bbutils.egg-info/requires.txt
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)       13 2023-09-18 14:40:28.000000 bbutils-0.6.0.0/bbutils.egg-info/top_level.txt
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     1769 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/make-lang.py
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)    13993 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/run-tests.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)       38 2023-09-18 14:40:28.816542 bbutils-0.6.0.0/setup.cfg
+-rwxrwxr-x   0 raphahk   (1000) raphahk   (1000)     1669 2021-11-03 11:12:22.000000 bbutils-0.6.0.0/setup.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.808543 bbutils-0.6.0.0/tests/
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/tests/app/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      739 2023-08-24 14:30:20.000000 bbutils-0.6.0.0/tests/app/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     9773 2023-08-24 14:30:20.000000 bbutils-0.6.0.0/tests/app/config.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4334 2023-09-18 14:30:33.000000 bbutils-0.6.0.0/tests/app/console.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1795 2023-09-18 14:31:15.000000 bbutils-0.6.0.0/tests/app/manager.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1832 2023-09-18 13:32:40.000000 bbutils-0.6.0.0/tests/app/module.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.812543 bbutils-0.6.0.0/tests/database/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      710 2023-08-21 14:41:04.000000 bbutils-0.6.0.0/tests/database/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     4946 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/tests/database/database.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     9299 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/tests/database/manager.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    25794 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/tests/database/sqlite.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)    13190 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/tests/database/table.py
+drwxrwxr-x   0 raphahk   (1000) raphahk   (1000)        0 2023-09-18 14:40:28.816542 bbutils-0.6.0.0/tests/helper/
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3755 2023-09-18 14:37:49.000000 bbutils-0.6.0.0/tests/helper/__init__.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2798 2023-08-24 14:30:20.000000 bbutils-0.6.0.0/tests/helper/config.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2133 2023-09-18 13:56:38.000000 bbutils-0.6.0.0/tests/helper/console.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2270 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/tests/helper/database.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3080 2023-08-23 11:09:07.000000 bbutils-0.6.0.0/tests/helper/execute.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)      965 2023-08-22 11:52:18.000000 bbutils-0.6.0.0/tests/helper/file.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3076 2023-09-18 14:30:10.000000 bbutils-0.6.0.0/tests/helper/module.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     1905 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/tests/helper/setup.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     5271 2023-09-01 11:26:26.000000 bbutils-0.6.0.0/tests/helper/sqlite.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     2788 2023-08-22 11:52:18.000000 bbutils-0.6.0.0/tests/helper/table.py
+-rw-rw-r--   0 raphahk   (1000) raphahk   (1000)     3432 2023-08-24 14:30:20.000000 bbutils-0.6.0.0/tests/helper/worker.py
```

### Comparing `bbutils-0.5.5.0/LICENSE` & `bbutils-0.6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/PKG-INFO` & `bbutils-0.6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbutils
-Version: 0.5.5.0
+Version: 0.6.0.0
 Summary: Small collection of stuff for all my other python projects (including logging).
 Home-page: https://github.com/TheUncleKai/bbutils
 Author: Kai Raphahn
 Author-email: kai.raphahn@laburec.de
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `bbutils-0.5.5.0/README.md` & `bbutils-0.6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/__init__.py` & `bbutils-0.6.0.0/bbutil/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,18 @@
 #: package credits
 __credits__ = [__author__]
 
 #: version milestone
 __milestone__ = 0
 
 #: version major
-__major__ = 5
+__major__ = 6
 
 #: version minor
-__minor__ = 5
+__minor__ = 0
 
 #: version patch
 __patch__ = 0
 
 #: package version
 __version__ = "{0:d}.{1:d}.{2:d}.{3:d}".format(__milestone__, __major__, __minor__, __patch__)
```

### Comparing `bbutils-0.5.5.0/bbutil/app/__init__.py` & `bbutils-0.6.0.0/bbutil/app/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/app/config.py` & `bbutils-0.6.0.0/bbutil/app/config.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/app/console.py` & `bbutils-0.6.0.0/bbutil/app/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 # Copyright (C) 2020, Siemens Healthcare Diagnostics Products GmbH
 # Licensed under the Siemens Inner Source License 1.2, see LICENSE.md.
 
 import abc
 import sys
 
-from dataclasses import dataclass
-from typing import Optional
+from dataclasses import dataclass, field
+from typing import Optional, List
 from abc import ABCMeta
 
 import bbutil
 
 from bbutil.logging import Logging
 from bbutil.app.manager import ModuleManager
 from bbutil.app.config import Config
@@ -24,15 +24,15 @@
 
 
 @dataclass
 class Console(metaclass=ABCMeta):
 
     command_id: str = ""
     module: Optional[Module] = None
-    module_path: str = ""
+    module_config: List[dict] = field(default_factory=list)
 
     def __post_init__(self):
         self.init()
         return
 
     def _set_command(self) -> bool:
         if bbutil.config is None:
@@ -76,23 +76,21 @@
         pass
 
     @abc.abstractmethod
     def stop(self) -> bool:
         pass
 
     def _setup_module(self) -> bool:
-        if self.module_path == "":
-            bbutil.log.error("Module path for console it missing!")
+        if len(self.module_config) == 0:
+            bbutil.log.error("No modules!")
             return False
 
-        _modules = ModuleManager(self.module_path)
+        _modules = ModuleManager()
 
-        check = _modules.init()
-        if check is False:
-            return False
+        _modules.init(self.module_config)
 
         bbutil.set_module(_modules)
         return True
 
     def _setup_config(self) -> bool:
         _config = self.create_config()
```

### Comparing `bbutils-0.5.5.0/bbutil/app/manager.py` & `bbutils-0.6.0.0/bbutil/app/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,47 +12,34 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 #    Copyright (C) 2017, Kai Raphahn <kai.raphahn@laburec.de>
 #
 
-from dataclasses import dataclass, field
 from typing import List, Optional
 
-import bbutil
 from bbutil.app.module import Module
-from bbutil.utils import get_attribute
 
 __all__ = [
     "ModuleManager"
 ]
 
 
-@dataclass
 class ModuleManager(object):
 
-    module_path: str = ""
-    modules: List[Module] = field(default_factory=list)
-    commands: List[str] = field(default_factory=list)
-
-    def init(self) -> bool:
-
-        try:
-            _commands = get_attribute(self.module_path, "__all__")
-        except ImportError as e:
-            bbutil.log.error("Unable to find commands: {0:s}".format(self.module_path))
-            return False
-
-        for _name in _commands:
-            _module = Module()
-
-            check = _module.init(self.module_path, _name)
-            if check is False:
-                continue
+    def __init__(self):
+        self.modules: List[Module] = []
+        self.commands: List[str] = []
+        return
+
+    def init(self, config: list) -> bool:
+
+        for _config in config:
+            _module = Module(**_config)
 
             self.commands.append(_module.command)
             self.modules.append(_module)
         return True
 
     def has_command(self, command: str) -> bool:
         if command in self.commands:
```

### Comparing `bbutils-0.5.5.0/bbutil/data.py` & `bbutils-0.6.0.0/bbutil/data.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/database/__init__.py` & `bbutils-0.6.0.0/bbutil/database/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/database/database.py` & `bbutils-0.6.0.0/bbutil/database/database.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/database/sqlite/__init__.py` & `bbutils-0.6.0.0/bbutil/database/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/database/sqlite/manager.py` & `bbutils-0.6.0.0/bbutil/database/sqlite/manager.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/database/sqlite/types.py` & `bbutils-0.6.0.0/bbutil/database/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/database/table.py` & `bbutils-0.6.0.0/bbutil/database/table.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/database/types.py` & `bbutils-0.6.0.0/bbutil/database/types.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/execute.py` & `bbutils-0.6.0.0/bbutil/execute.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/file.py` & `bbutils-0.6.0.0/bbutil/file.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/lang/__init__.py` & `bbutils-0.6.0.0/bbutil/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/lang/domain.py` & `bbutils-0.6.0.0/bbutil/lang/domain.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/lang/parser/__init__.py` & `bbutils-0.6.0.0/bbutil/lang/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/lang/parser/domain.py` & `bbutils-0.6.0.0/bbutil/lang/parser/domain.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/lang/parser/language.py` & `bbutils-0.6.0.0/bbutil/lang/parser/language.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/lang/parser/pyfile.py` & `bbutils-0.6.0.0/bbutil/lang/parser/pyfile.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/logging/__init__.py` & `bbutils-0.6.0.0/bbutil/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/logging/types.py` & `bbutils-0.6.0.0/bbutil/logging/types.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/logging/writer/__init__.py` & `bbutils-0.6.0.0/bbutil/logging/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/logging/writer/console.py` & `bbutils-0.6.0.0/bbutil/logging/writer/console.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/logging/writer/file.py` & `bbutils-0.6.0.0/bbutil/logging/writer/file.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/logging/writer/qt.py` & `bbutils-0.6.0.0/bbutil/logging/writer/qt.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/logging/writer/tkinter.py` & `bbutils-0.6.0.0/bbutil/logging/writer/tkinter.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/setup.py` & `bbutils-0.6.0.0/bbutil/setup.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/utils.py` & `bbutils-0.6.0.0/bbutil/utils.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/worker/__init__.py` & `bbutils-0.6.0.0/bbutil/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutil/worker/callback.py` & `bbutils-0.6.0.0/bbutil/worker/callback.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/bbutils.egg-info/PKG-INFO` & `bbutils-0.6.0.0/bbutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbutils
-Version: 0.5.5.0
+Version: 0.6.0.0
 Summary: Small collection of stuff for all my other python projects (including logging).
 Home-page: https://github.com/TheUncleKai/bbutils
 Author: Kai Raphahn
 Author-email: kai.raphahn@laburec.de
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `bbutils-0.5.5.0/bbutils.egg-info/SOURCES.txt` & `bbutils-0.6.0.0/bbutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,11 +53,12 @@
 tests/database/table.py
 tests/helper/__init__.py
 tests/helper/config.py
 tests/helper/console.py
 tests/helper/database.py
 tests/helper/execute.py
 tests/helper/file.py
+tests/helper/module.py
 tests/helper/setup.py
 tests/helper/sqlite.py
 tests/helper/table.py
 tests/helper/worker.py
```

### Comparing `bbutils-0.5.5.0/make-lang.py` & `bbutils-0.6.0.0/make-lang.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/run-tests.py` & `bbutils-0.6.0.0/run-tests.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/setup.py` & `bbutils-0.6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/app/__init__.py` & `bbutils-0.6.0.0/tests/app/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/app/config.py` & `bbutils-0.6.0.0/tests/app/config.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/app/console.py` & `bbutils-0.6.0.0/tests/app/console.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import unittest
 
 from unittest.mock import patch, Mock
 
 import bbutil
 from tests.helper.console import AppConsole
+from tests.helper.module import config_modules, config_modules_2
 
 
 __all__ = [
     "TestConsole"
 ]
 
 oserror = OSError("Something strange did happen!")
@@ -36,46 +37,38 @@
 class TestConsole(unittest.TestCase):
     """Testing class for locking module."""
 
     def setUp(self):
         return
 
     def test_setup_01(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
 
         _check = _console.setup()
         self.assertTrue(_check)
         return
 
     def test_setup_02(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=[])
         _console.module_path = "testdata.app.xcommands"
 
         _check = _console.setup()
         self.assertFalse(_check)
         return
 
     def test_setup_03(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
         _console.filename = "fuhhhhhhh"
 
         _check = _console.setup()
         self.assertFalse(_check)
         return
 
-    def test_setup_04(self):
-        _console = AppConsole()
-        _console.module_path = ""
-
-        _check = _console.setup()
-        self.assertFalse(_check)
-        return
-
     def test_execute_01(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
 
         _argv = [
             "run-tests.py",
             "test01"
         ]
 
         _check1 = _console.setup()
@@ -84,29 +77,29 @@
             _ret = _console.execute()
 
         self.assertTrue(_check1)
         self.assertEqual(_ret, 0)
         return
 
     def test_execute_02(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
 
         _check1 = _console.setup()
 
         # noinspection PyTypeChecker
         bbutil.set_config(None)
 
         _ret = _console.execute()
 
         self.assertTrue(_check1)
         self.assertEqual(_ret, -1)
         return
 
     def test_execute_03(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
 
         _argv = [
             "run-tests.py",
             "xxxxtest01"
         ]
 
         _check1 = _console.setup()
@@ -115,32 +108,32 @@
             _ret = _console.execute()
 
         self.assertTrue(_check1)
         self.assertEqual(_ret, -1)
         return
 
     def test_execute_04(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules_2)
 
         _argv = [
             "run-tests.py",
-            "test02"
+            "test01"
         ]
 
         _check1 = _console.setup()
 
         with patch("sys.argv", _argv):
             _ret = _console.execute()
 
         self.assertTrue(_check1)
         self.assertEqual(_ret, 2)
         return
 
     def test_execute_05(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
 
         _argv = [
             "run-tests.py",
             "test01"
         ]
 
         _check1 = _console.setup()
@@ -150,15 +143,15 @@
             _ret = _console.execute()
 
         self.assertTrue(_check1)
         self.assertEqual(_ret, 1)
         return
 
     def test_execute_06(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
 
         _argv = [
             "run-tests.py",
             "test01"
         ]
 
         _check1 = _console.setup()
@@ -168,19 +161,19 @@
             _ret = _console.execute()
 
         self.assertTrue(_check1)
         self.assertEqual(_ret, 4)
         return
 
     def test_execute_07(self):
-        _console = AppConsole()
+        _console = AppConsole(module_config=config_modules)
 
         _argv = [
             "run-tests.py",
-            "test06"
+            "test03"
         ]
 
         _check1 = _console.setup()
 
         with patch("sys.argv", _argv):
             _ret = _console.execute()
```

### Comparing `bbutils-0.5.5.0/tests/app/manager.py` & `bbutils-0.6.0.0/tests/app/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import unittest
 
 import unittest.mock as mock
 
 from bbutil.app.manager import ModuleManager
 
 from tests.helper import set_log, reset_module
+from tests.helper.module import config_modules
 
 
 __all__ = [
     "TestManager"
 ]
 
 oserror = OSError("Something strange did happen!")
@@ -39,30 +40,23 @@
 
     def setUp(self):
         set_log()
         reset_module()
         return
 
     def test_init_01(self):
-        _module = ModuleManager(module_path="testdata.app.commands")
-        _check1 = _module.init()
+        _module = ModuleManager()
+        _check1 = _module.init(config_modules)
 
         _command1 = _module.get_command("test01")
         _command2 = _module.get_command("test01xx")
         _check2 = _module.has_command("test01")
         _check3 = _module.has_command("test01xx")
 
         self.assertTrue(_check1)
         self.assertTrue(_check2)
         self.assertFalse(_check3)
         self.assertIsNotNone(_command1)
         self.assertIsNone(_command2)
-        self.assertEqual(len(_module.commands), 4)
-        self.assertEqual(len(_module.modules), 4)
-        return
-
-    def test_init_02(self):
-        _module = ModuleManager(module_path="testdata.app.xcommands")
-        _check1 = _module.init()
-
-        self.assertFalse(_check1)
+        self.assertEqual(len(_module.commands), 3)
+        self.assertEqual(len(_module.modules), 3)
         return
```

### Comparing `bbutils-0.5.5.0/tests/database/__init__.py` & `bbutils-0.6.0.0/tests/database/__init__.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/database/database.py` & `bbutils-0.6.0.0/tests/database/database.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/database/manager.py` & `bbutils-0.6.0.0/tests/database/manager.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/database/sqlite.py` & `bbutils-0.6.0.0/tests/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/database/table.py` & `bbutils-0.6.0.0/tests/database/table.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/__init__.py` & `bbutils-0.6.0.0/tests/helper/console.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,101 +14,60 @@
 #    limitations under the License.
 #
 #    Copyright (C) 2017, Kai Raphahn <kai.raphahn@laburec.de>
 #
 
 import os
 
-from shutil import copyfile
+from dataclasses import dataclass
 
-import bbutil
-from bbutil.logging import Logging
-from bbutil.app.manager import ModuleManager
-from bbutil.database import SQLite
 from bbutil.utils import full_path
+from bbutil.logging import Logging
+from bbutil.app import Console, Config
+
+from testdata.app.config import AppConfig
 
 __all__ = [
-    "config",
-    "console",
-    "database",
-    "execute",
-    "file",
-    "setup",
-    "sqlite",
-    "table",
-    "worker",
-
-    "get_sqlite",
-    "copy_sqlite",
-    "set_log",
-    "set_module",
-    "reset_module"
+    "AppConsole"
 ]
 
 _index = {
     0: ["INFORM", "WARN", "ERROR", "EXCEPTION", "TIMER", "PROGRESS"],
     1: ["INFORM", "DEBUG1", "WARN", "ERROR", "EXCEPTION", "TIMER", "PROGRESS"],
     2: ["INFORM", "DEBUG1", "DEBUG2", "WARN", "ERROR", "EXCEPTION", "TIMER", "PROGRESS"],
     3: ["INFORM", "DEBUG1", "DEBUG2", "DEBUG3", "WARN", "ERROR", "EXCEPTION", "TIMER", "PROGRESS"]
 }
 
 
-def get_sqlite(filename: str, path: str = os.getcwd(), clean: bool = False) -> SQLite:
-    _testfile = full_path("{0:s}/{1:s}".format(path, filename))
-    _name = "Test"
-
-    if (os.path.exists(_testfile) is True) and (clean is True):
-        os.remove(_testfile)
-
-    _sqlite = SQLite(filename=_testfile, name="Test")
-    return _sqlite
-
+@dataclass
+class AppConsole(Console):
 
-def copy_sqlite(filename: str, path: str = os.getcwd(), clean: bool = False) -> SQLite:
-    _sourcefile = full_path("{0:s}/{1:s}".format(path, filename))
-    _name = "Test"
-    _testfile = "{0:s}/{1:s}".format(os.getcwd(), filename)
+    filename: str = ""
+    return_start: bool = True
+    return_stop: bool = True
+
+    def create_logging(self) -> Logging:
+        _log = Logging()
+        _log.setup(app="Test", level=2, index=_index)
+
+        console = _log.get_writer("console")
+        _log.register(console)
+        _log.open()
+        return _log
+
+    def create_config(self) -> Config:
+        _work = "{0:s}/test".format(os.getcwd())
+        if os.path.exists(_work) is False:
+            os.mkdir(_work)
 
-    if os.path.exists(_testfile):
-        os.remove(_testfile)
+        _config = AppConfig(use_config=True, config_filename=self.filename)
+        return _config
 
-    copyfile(_sourcefile, _testfile)
-
-    _sqlite = SQLite(filename=_testfile, name="Test")
-    return _sqlite
-
-
-def set_log():
-    if bbutil.log is not None:
+    def init(self):
+        self.filename = full_path("{0:s}/testdata/config01.json".format(os.getcwd()))
         return
 
-    _log = Logging()
-    _log.setup(app="Test", level=2, index=_index)
-
-    console = _log.get_writer("console")
-    _log.register(console)
-    _log.open()
-
-    bbutil.set_log(_log)
-    return
-
-
-def set_module():
-    if bbutil.module is not None:
-        return
-
-    _module = ModuleManager(module_path="testdata.app.commands")
-    _check = _module.init()
-
-    if _check is False:
-        return
-
-    bbutil.set_module(_module)
-    return
-
-
-def reset_module():
-    if bbutil.module is None:
-        return
+    def start(self) -> bool:
+        return self.return_start
 
-    bbutil.set_module(None)
-    return
+    def stop(self) -> bool:
+        return self.return_stop
```

### Comparing `bbutils-0.5.5.0/tests/helper/config.py` & `bbutils-0.6.0.0/tests/helper/config.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/database.py` & `bbutils-0.6.0.0/tests/helper/database.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/execute.py` & `bbutils-0.6.0.0/tests/helper/execute.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/file.py` & `bbutils-0.6.0.0/tests/helper/file.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/setup.py` & `bbutils-0.6.0.0/tests/helper/setup.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/sqlite.py` & `bbutils-0.6.0.0/tests/helper/sqlite.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/table.py` & `bbutils-0.6.0.0/tests/helper/table.py`

 * *Files identical despite different names*

### Comparing `bbutils-0.5.5.0/tests/helper/worker.py` & `bbutils-0.6.0.0/tests/helper/worker.py`

 * *Files identical despite different names*

