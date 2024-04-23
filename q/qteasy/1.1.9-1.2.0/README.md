# Comparing `tmp/qteasy-1.1.9.tar.gz` & `tmp/qteasy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-jvv8wh92/qteasy-1.1.9.tar", last modified: Mon Apr  8 15:19:43 2024, max compression
+gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-52p0dblw/qteasy-1.2.0.tar", last modified: Tue Apr 23 05:16:38 2024, max compression
```

## Comparing `qteasy-1.1.9.tar` & `qteasy-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.9/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    27754 2024-04-08 15:19:43.000000 qteasy-1.1.9/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24516 2024-04-08 15:10:08.000000 qteasy-1.1.9/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2181 2024-04-08 15:10:08.000000 qteasy-1.1.9/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8505 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.1.9/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-04-02 14:50:54.000000 qteasy-1.1.9/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.1.9/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   109762 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   386999 2024-04-08 15:18:39.000000 qteasy-1.1.9/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.1.9/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.1.9/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.1.9/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    50575 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)   180412 2024-04-03 15:51:09.000000 qteasy-1.1.9/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 14:28:39.000000 qteasy-1.1.9/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-04-02 02:35:24.000000 qteasy-1.1.9/qteasy/tsfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    75004 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-08 15:10:08.000000 qteasy-1.1.9/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    27754 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1192 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.9/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      154 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-08 15:19:43.000000 qteasy-1.1.9/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1515 2024-04-08 15:19:43.000000 qteasy-1.1.9/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.1.9/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-08 15:19:43.000000 qteasy-1.1.9/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.9/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.9/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.1.9/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   121286 2024-04-08 15:18:58.000000 qteasy-1.1.9/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.9/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.9/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.9/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.9/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-07 13:30:44.000000 qteasy-1.1.9/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.9/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.9/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43391 2024-04-03 15:51:09.000000 qteasy-1.1.9/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    44385 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-08 15:10:08.000000 qteasy-1.1.9/tests/test_trading.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.9/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.1.9/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.9/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 05:16:38.000000 qteasy-1.2.0/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.0/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    28538 2024-04-23 05:16:38.000000 qteasy-1.2.0/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    25292 2024-04-22 13:38:27.000000 qteasy-1.2.0/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2194 2024-04-22 13:38:27.000000 qteasy-1.2.0/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 05:16:38.000000 qteasy-1.2.0/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8526 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    68444 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-21 23:36:55.000000 qteasy-1.2.0/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.0/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.2.0/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   110897 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   390889 2024-04-22 01:51:11.000000 qteasy-1.2.0/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.0/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-21 23:36:55.000000 qteasy-1.2.0/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-05 14:28:39.000000 qteasy-1.2.0/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.0/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.2.0/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.2.0/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.0/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.2.0/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.2.0/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    50640 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)    98476 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    93097 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/trader_cli.py
+-rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/trader_tui.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-05 14:28:39.000000 qteasy-1.2.0/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.0/qteasy/tsfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-04-22 13:38:27.000000 qteasy-1.2.0/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.0/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 05:16:38.000000 qteasy-1.2.0/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    28538 2024-04-23 05:16:38.000000 qteasy-1.2.0/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1252 2024-04-23 05:16:38.000000 qteasy-1.2.0/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-23 05:16:38.000000 qteasy-1.2.0/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.0/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      155 2024-04-23 05:16:38.000000 qteasy-1.2.0/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-23 05:16:38.000000 qteasy-1.2.0/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1515 2024-04-23 05:16:38.000000 qteasy-1.2.0/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.0/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-23 05:16:38.000000 qteasy-1.2.0/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.2.0/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.0/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.0/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.0/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.2.0/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-04-22 13:38:27.000000 qteasy-1.2.0/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.0/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.0/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.0/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.0/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.0/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.0/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-05 14:28:39.000000 qteasy-1.2.0/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-07 13:30:44.000000 qteasy-1.2.0/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.0/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.2.0/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-04-22 13:38:27.000000 qteasy-1.2.0/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-04-22 13:38:27.000000 qteasy-1.2.0/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.0/tests/test_trading.py
+-rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-04-22 13:38:27.000000 qteasy-1.2.0/tests/test_tui.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.0/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.0/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.0/tests/test_visual.py
```

### Comparing `qteasy-1.1.9/LICENSE` & `qteasy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/PKG-INFO` & `qteasy-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.9
+Version: 1.2.0
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -37,18 +37,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.6
+Requires-Python: <3.13,>=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: talib
 Provides-Extra: database
-Provides-Extra: hdf
 Provides-Extra: feather
 License-File: LICENSE
 
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
@@ -92,15 +92,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.9`
+- Latest Version: `1.2.0`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -128,17 +128,17 @@
 ### **实盘交易模拟**
 - 读取实时市场数据，实盘运行交易策略
 - 生成交易信号，模拟交易结果
 - 跟踪记录交易日志、股票持仓、账户资金变化等信息
 - 随时查看交易过程，检查盈亏情况
 - 手动控制交易进程、调整交易参数，手动下单
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_2.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_1.png)  
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png)  
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
 
 ## 安装
 
 ```bash
 $ pip install qteasy
 ```
 
@@ -148,18 +148,36 @@
 
 
 ### python 版本
 - *`python` version >= 3.6, < 3.13* 
 
 ### 安装可选依赖包
 
-`qteasy`所有必要的依赖包都可以在pip安装的同时安装好，但如果需要使用`qteasy`的全部功能，需要安装以下依赖包：
+`qteasy`所有必要的依赖包都可以在`pip`安装的同时安装好，但某些特殊情况下，您需要在安装时指定可选依赖包，以便在安装`qteasy`时同时安装，或者手动安装依赖包：
 
-- **`ta-lib`**, 以便使用所有的内置交易策略
-- **`pymysql`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+- **`pymysql`**, 用于连接`MySQL`数据库,将本地数据存储到`MySQL`数据库（`qteasy`默认使用`csv`文件作为本地数据源，但数据量大时推荐使用`mysql`数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+`pymysql`可以在安装`qteasy`时自动安装，也可以手动安装：
+    ```bash
+    $ pip install 'qteasy[database]'  # 安装qteasy时自动安装pymysql
+    $ pip install pymysql  # 手动安装pymysql
+    ```
+- **`pyarrow`**, 用于操作`feather`文件，将本地数据存储为`feather`文件，`pyarrow`可以在安装`qteasy`时自动安装，也可以手动安装：
+    ```bash
+    $ pip install 'qteasy[feather]'  # 安装qteasy时自动安装pyarrow
+    $ pip install pyarrow  # 手动安装pyarrow
+    ```
+- **`pytables`**, 用于操作`HDF`文件，将本地数据存储到`HDF`文件，`pytables`不能自动安装，需要使用`conda`手动安装`pytables`：
+    ```bash
+    $ conda install pytables  # 安装pytables
+    ```
+- **`ta-lib`**, 以便使用所有的内置交易策略，下面的方法可以安装`ta-lib API`，但它还依赖C语言的`TA-Lib`包，安装方法请参考[FAQ](https://qteasy.readthedocs.io/zh/latest/faq.html#id2)
+    ```bash
+    $ pip install 'qteasy[talib]'  # 安装qteasy时自动安装ta-lib
+    $ pip install ta-lib  # 手动安装ta-lib
+    ```
 
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
@@ -554,44 +572,19 @@
         sell_batch_size=1,  # 卖出数量为1股的整数倍
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
 )
 
 qt.run(op)
 ```
-此时`qteasy`会启动一个`Trader Shell`命令行界面，同时交易策略会自动定时运行，运行的参数随`QT_CONFIG`而定。启动TraderShell后，所有交易相关的重要信息都会显示在console中：
-
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)   
-
-此时控制台上会显示当前交易执行状态：
-- 当前日期、时间、运行状态
-- 产生的交易信号和交易订单
-- 交易订单的成交情况
-- 账户资金变动情况
-- 账户持仓变动情况
-- 开盘和收盘时间预告等
-
-在`TraderShell`运行过程中可以随时按`Ctrl+C`进入Shell选单：
-```commandline
-Current mode interrupted, Input 1 or 2 or 3 for below options: 
-[1], Enter command mode; 
-[2], Enter dashboard mode. 
-[3], Exit and stop the trader; 
-please input your choice: 
-```
+qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
-此时按1可以进入Interactive模式（交互模式）。在交互模式下，用户可以在(QTEASY)命令行提示符后输入
-命令来控制交易策略的运行：
+为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_2.png)   
+- **`TraderShell`** 交互式命令行界面，可以在命令行中输入命令，查看交易日志、查看持仓、查看账户资金变化等信息：
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
 ![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+- **`TraderApp`** (v1.2.0新增) 交互式图形界面，可以在图形界面中查看交易日志、查看持仓、查看账户资金变化等信息
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png) 
 
-在命令行模式下可以与`TraderShell`实现交互，操作当前账户，查询交易历史、修改状态等：
-
-- `pause` / `resume`: 暂停/重新启动交易策略
-- `change`: 修改当前持仓和现金余额
-- `positions`: 查看当前持仓
-- `orders`: 查看当前订单
-- `history`: 查看历史交易记录
-- `exit`: 退出TraderShell
-- ... 更多`TraderShell`命令参见[`QTEASY`文档](https://qteasy.readthedocs.io)
-
+上面两种方式都可以在实盘运行时使用，根据qteasy的配置参数进入不同的交互界，关于更多实盘运行的介绍，请参见[`QTEASY`文档](https://qteasy.readthedocs.io)
```

### Comparing `qteasy-1.1.9/README.md` & `qteasy-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.9`
+- Latest Version: `1.2.0`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -78,17 +78,17 @@
 ### **实盘交易模拟**
 - 读取实时市场数据，实盘运行交易策略
 - 生成交易信号，模拟交易结果
 - 跟踪记录交易日志、股票持仓、账户资金变化等信息
 - 随时查看交易过程，检查盈亏情况
 - 手动控制交易进程、调整交易参数，手动下单
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_2.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_1.png)  
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png)  
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
 
 ## 安装
 
 ```bash
 $ pip install qteasy
 ```
 
@@ -98,18 +98,36 @@
 
 
 ### python 版本
 - *`python` version >= 3.6, < 3.13* 
 
 ### 安装可选依赖包
 
-`qteasy`所有必要的依赖包都可以在pip安装的同时安装好，但如果需要使用`qteasy`的全部功能，需要安装以下依赖包：
+`qteasy`所有必要的依赖包都可以在`pip`安装的同时安装好，但某些特殊情况下，您需要在安装时指定可选依赖包，以便在安装`qteasy`时同时安装，或者手动安装依赖包：
 
-- **`ta-lib`**, 以便使用所有的内置交易策略
-- **`pymysql`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+- **`pymysql`**, 用于连接`MySQL`数据库,将本地数据存储到`MySQL`数据库（`qteasy`默认使用`csv`文件作为本地数据源，但数据量大时推荐使用`mysql`数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+`pymysql`可以在安装`qteasy`时自动安装，也可以手动安装：
+    ```bash
+    $ pip install 'qteasy[database]'  # 安装qteasy时自动安装pymysql
+    $ pip install pymysql  # 手动安装pymysql
+    ```
+- **`pyarrow`**, 用于操作`feather`文件，将本地数据存储为`feather`文件，`pyarrow`可以在安装`qteasy`时自动安装，也可以手动安装：
+    ```bash
+    $ pip install 'qteasy[feather]'  # 安装qteasy时自动安装pyarrow
+    $ pip install pyarrow  # 手动安装pyarrow
+    ```
+- **`pytables`**, 用于操作`HDF`文件，将本地数据存储到`HDF`文件，`pytables`不能自动安装，需要使用`conda`手动安装`pytables`：
+    ```bash
+    $ conda install pytables  # 安装pytables
+    ```
+- **`ta-lib`**, 以便使用所有的内置交易策略，下面的方法可以安装`ta-lib API`，但它还依赖C语言的`TA-Lib`包，安装方法请参考[FAQ](https://qteasy.readthedocs.io/zh/latest/faq.html#id2)
+    ```bash
+    $ pip install 'qteasy[talib]'  # 安装qteasy时自动安装ta-lib
+    $ pip install ta-lib  # 手动安装ta-lib
+    ```
 
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
@@ -504,44 +522,19 @@
         sell_batch_size=1,  # 卖出数量为1股的整数倍
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
 )
 
 qt.run(op)
 ```
-此时`qteasy`会启动一个`Trader Shell`命令行界面，同时交易策略会自动定时运行，运行的参数随`QT_CONFIG`而定。启动TraderShell后，所有交易相关的重要信息都会显示在console中：
-
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)   
-
-此时控制台上会显示当前交易执行状态：
-- 当前日期、时间、运行状态
-- 产生的交易信号和交易订单
-- 交易订单的成交情况
-- 账户资金变动情况
-- 账户持仓变动情况
-- 开盘和收盘时间预告等
-
-在`TraderShell`运行过程中可以随时按`Ctrl+C`进入Shell选单：
-```commandline
-Current mode interrupted, Input 1 or 2 or 3 for below options: 
-[1], Enter command mode; 
-[2], Enter dashboard mode. 
-[3], Exit and stop the trader; 
-please input your choice: 
-```
+qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
-此时按1可以进入Interactive模式（交互模式）。在交互模式下，用户可以在(QTEASY)命令行提示符后输入
-命令来控制交易策略的运行：
+为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_2.png)   
+- **`TraderShell`** 交互式命令行界面，可以在命令行中输入命令，查看交易日志、查看持仓、查看账户资金变化等信息：
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
 ![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+- **`TraderApp`** (v1.2.0新增) 交互式图形界面，可以在图形界面中查看交易日志、查看持仓、查看账户资金变化等信息
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png) 
 
-在命令行模式下可以与`TraderShell`实现交互，操作当前账户，查询交易历史、修改状态等：
-
-- `pause` / `resume`: 暂停/重新启动交易策略
-- `change`: 修改当前持仓和现金余额
-- `positions`: 查看当前持仓
-- `orders`: 查看当前订单
-- `history`: 查看历史交易记录
-- `exit`: 退出TraderShell
-- ... 更多`TraderShell`命令参见[`QTEASY`文档](https://qteasy.readthedocs.io)
-
+上面两种方式都可以在实盘运行时使用，根据qteasy的配置参数进入不同的交互界，关于更多实盘运行的介绍，请参见[`QTEASY`文档](https://qteasy.readthedocs.io)
```

### Comparing `qteasy-1.1.9/pyproject.toml` & `qteasy-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,33 +14,34 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.6"
+requires-python = ">=3.6, <3.13"
 keywords = ["quantitative investment", "quantitative trading", "stock", "finance", "investment"]
 dependencies = [
     "pandas>=1.4.0",
     "numpy>=1.18.1",
     "numba>=0.47.0",
     "tushare>=1.2.89",
     "mplfinance",
     "rich>=10.0.0",
+    "textual",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: BSD License",
@@ -62,10 +63,10 @@
 
 [project.urls]
 Homepage = "https://github.com/shepherdpp/qteasy"
 Documentation = "https://qteasy.readthedocs.io/zh/latest/"
 Issues = "https://github.com/shepherdpp/qteasy/issues"
 
 [project.optional-dependencies]
+talib = ["ta-lib"]
 database = ["pymysql >= 1.0.0"]
-hdf = ["pytables >= 3.6.1"]
 feather = ["pyarrow >= 3"]
```

### Comparing `qteasy-1.1.9/qteasy/__init__.py` & `qteasy-1.2.0/qteasy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,24 @@
 from .built_in import built_ins, built_in_list, built_in_strategies, get_built_in_strategy
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
-__version__ = '1.1.9'
+# qteasy版本信息
+__version__ = '1.2.0'
 version_info = Namespace(
         major=1,
-        minor=1,
-        patch=9,
-        short=(1, 1),
-        full=(1, 1, 9),
-        string='1.1.9',
-        tuple=('1', '1', '9'),
+        minor=2,
+        patch=0,
+        short=(1, 2),
+        full=(1, 2, 0),
+        string='1.2.0',
+        tuple=('1', '2', '0'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
```

### Comparing `qteasy-1.1.9/qteasy/_arg_validators.py` & `qteasy-1.2.0/qteasy/_arg_validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         合法参数列表
     """
     vkwargs = {
         'mode':
             {'Default':   1,  # 运行模式
              'Validator': lambda value: value in (0, 1, 2, 3),
              'level':     0,
-             'text':      'qteasy 的运行模式: \n'
+             'text':      'qteasy 的运行模式，取值范围: \n'
                           '0: 实盘运行模式\n'
                           '1: 回测-评价模式\n'
                           '2: 策略优化模式\n'
                           '3: 统计预测模式\n'},
 
         'time_zone':  # this parameter is now not used
             {'Default':   'local',
@@ -83,39 +83,42 @@
                           'US/Pacific\n'
                           'Europe/London\n'
                           'Europe/Paris\n'
                           'Australia/Sydney\n'
                           'Australia/Melbourne\n'
                           'Pacific/Auckland\n'
                           'Pacific/Chatham\n'
-                          'etc.\n'},
+                          '...'},
 
         'asset_pool':
             {'Default':   '000300.SH',  #
              'Validator': lambda value: isinstance(value, (str, list))
                                         and _validate_asset_pool(value),
              'level':     0,
-             'text':      '可用投资产品池，投资组合基于池中的产品创建'},
+             'text':      '可用投资产品池，投资组合基于池中的产品创建，可以输入一个包含资产代码的列表，'
+                          '或者逗号分隔字符串，例如下面两种输入等价:\n'
+                          '["000001.SZ", "000002.SZ", "000003.SZ"]\n'
+                          '"000001.SZ, 000002.SZ, 000003.SZ"'},
 
         'asset_type':
             {'Default':   'IDX',  #
              'Validator': lambda value: isinstance(value, str)
                                         and _validate_asset_type(value),
              'level':     0,
-             'text':      '投资产品的资产类型，包括：\n'
+             'text':      '投资产品的资产类型，取值范围：\n'
                           'IDX  : 指数\n'
                           'E    : 股票\n'
                           'FT   : 期货\n'
-                          'FD   : 基金\n'},
+                          'FD   : 基金'},
 
         'live_trade_account_id':
             {'Default':   None,  # 指定account_id后，实盘交易时会直接使用该账户，除非账户不存在
              'Validator': lambda value: isinstance(value, int) or value is None,
              'level':     0,
-             'text':      '实盘交易账户ID，用于实盘交易，如果指定了该参数，则会直接\n'
+             'text':      '实盘交易账户ID，一个整数。用于实盘交易，如果指定了该参数，则会直接\n'
                           '使用该账户，除非账户不存在'},
 
         'live_trade_account':
             {'Default':   None,  # 指定account后，会查找该账户对应的account_id并使用该账户，除非账户不存在
              'Validator': lambda value: isinstance(value, str) or value is None,
              'level':     0,
              'text':      '实盘交易账户名称，用于实盘交易，如果指定了该参数，则会查找该\n'
@@ -128,15 +131,15 @@
              'text':      '实盘交易调试模式，True: 调试模式，False: 正常模式'},
 
         'live_trade_init_cash':
             {'Default':   1000000.0,
              'Validator': lambda value: isinstance(value, (int, float))
                                         and value > 0,
              'level':     1,
-             'text':      '实盘交易账户的初始资金，浮点数，例如：\n'
+             'text':      '实盘交易账户的初始资金，大于0的浮点数或整数：\n'
                           '1000000.0 : 初始资金为100万\n'
                           '1000000   : 初始资金为100万\n'},
 
         'live_trade_init_holdings':
             {'Default':   None,
              'Validator': lambda value: isinstance(value, dict) or value is None,
              'level':     1,
@@ -162,178 +165,182 @@
              'level':     1,
              'text':      '实盘交易账户的交易代理商参数，字典，例如：\n'
                           "{'host': 'localhost', 'port': 8888} : 交易代理商的主机名和端口号\n"
                           "具体的参数设置请参考交易代理商的文档\n"
                           "如果使用 'simulator' broker，且设置此参数为None，则会使用config中的\n"
                           "backtest参数"},
 
+        'live_trade_ui_type':
+            {'Default':   'cli',
+             'Validator': lambda value: isinstance(value, str) and value.lower() in ['tui', 'cli'],
+             'level':     1,
+             'text':      '实盘交易时的用户界面风格，可以设置为文本界面或图形界面\n'
+                          '默认使用文本界面'},
+
+
         'live_price_acquire_channel':
             {'Default':   'eastmoney',
              'Validator': lambda value: isinstance(value, str) and value.lower() in ['eastmoney', 'tushare', 'akshare'],
              'level':     2,
              'text':      '实盘交易时获取实时价格的方式：\n'
                           'eastmoney - 通过东方财富网获取实时价格\n'
                           'tushare  - 通过tushare获取实时价格(需要自行开通权限)\n'
-                          'akshare  - Not Implemented: 从akshare获取实时价格\n'},
+                          'akshare  - Not Implemented: 从akshare获取实时价格'},
 
         'live_price_acquire_freq':
             {'Default':   '15MIN',
              'Validator': lambda value: isinstance(value, str) and value.upper() in
                                         ['H', '30MIN', '15MIN', '5MIN', '1MIN', 'TICK'],
              'level':     2,
-             'text':      '实盘交易时获取实时价格的频率：\n'
+             'text':      '实盘交易时获取实时价格的频率，取值范围：\n'
                           'H      - 每1小时获取一次数据\n'
                           '30MIN  - 每30分钟获取一次数据\n'
                           '15MIN  - 每15分钟获取一次数据\n'
                           '5MIN   - 每5分钟获取一次数据\n'
-                          '1MIN   - 每1分钟获取一次数据\n'},
+                          '1MIN   - 每1分钟获取一次数据'},
 
         'watched_price_refresh_interval':
             {'Default':   5,
              'Validator': lambda value: isinstance(value, int) and value >= 5,
              'level':     4,
              'text':      '实盘交易时监看实时价格的刷新频率，单位为秒，默认为5秒\n'
                           '该数值不能低于5秒'},
 
         'trade_batch_size':
             {'Default':   0.0,
-             'Validator': lambda value: isinstance(value, (int, float))
-                                        and value >= 0,
+             'Validator': lambda value: isinstance(value, (int, float)) and value >= 0,
              'level':     0,
-             'text':      '投资产品的最小申购批量大小，浮点数，例如：\n'
+             'text':      '投资产品的最小申购批量大小，大于等于0的浮点数，例如：\n'
                           '0. : 可以购买任意份额的投资产品，包括小数份额\n'
                           '1. : 只能购买整数份额的投资产品\n'
                           '100: 可以购买100的整数倍份额投资产品\n'
-                          'n  : 可以购买的投资产品份额为n的整数倍，n不必为整数\n'},
+                          'n  : 可以购买的投资产品份额为n的整数倍，n不必为整数'},
 
         'sell_batch_size':
             {'Default':   0.0,
-             'Validator': lambda value: isinstance(value, (int, float))
-                                        and value >= 0,
+             'Validator': lambda value: isinstance(value, (int, float)) and value >= 0,
              'level':     0,
-             'text':      '投资产品的最小卖出或赎回批量大小，浮点数，例如：\n'
+             'text':      '投资产品的最小卖出或赎回批量大小，大于等于0的浮点数，例如：\n'
                           '0. : 可以购买任意份额的投资产品，包括小数份额\n'
                           '1. : 只能购买整数份额的投资产品\n'
                           '100: 可以购买100的整数倍份额投资产品\n'
                           'n  : 可以购买的投资产品份额为n的整数倍，n不必为整数\n'},
 
         'cash_decimal_places':
             {'Default':   2,
              'Validator': lambda value: isinstance(value, int) and value >= 0,
              'level':     2,
-             'text':      '现金的小数位数，例如：\n'
+             'text':      '现金的小数位数，大于等于0的整数，例如：\n'
                           '0: 现金只能为整数\n'
                           '2: 保留小数点后两位数字\n'},
 
         'amount_decimal_places':
             {'Default':   2,
              'Validator': lambda value: isinstance(value, int) and value >= 0,
              'level':     2,
-             'text':      '投资产品的份额的小数位数，例如：\n'
+             'text':      '投资产品的份额的小数位数，大于等于0的整数，例如：\n'
                           '0: 份额只能为整数\n'
                           '2: 保留小数点后两位数字\n'},
 
         'riskfree_ir':
             {'Default':   0.0035,
-             'Validator': lambda value: isinstance(value, float)
-                                        and 0 <= value < 1,
+             'Validator': lambda value: isinstance(value, float) and 0 <= value < 1,
              'level':     1,
-             'text':      '无风险利率，如果选择"考虑现金的时间价值"，则回测时现金按此年利率增值'},
+             'text':      '无风险利率，如果选择"考虑现金的时间价值"，则回测时现金按此年利率增值，取值范围[0, 1)'},
 
         'parallel':
             {'Default':   True,
              'Validator': lambda value: isinstance(value, bool),
              'level':     1,
              'text':      '如果True，策略参数寻优时将利用多核心CPU进行并行计算提升效率'},
 
         'hist_dnld_parallel':
             {'Default':   16,
              'Validator': lambda value: isinstance(value, int) and value >= 0,
              'level':     4,
-             'text':      '下载历史数据时启用的线程数量，为0或1时采用单线程下载，大于1时启用多线程'},
+             'text':      '下载历史数据时启用的线程数量，大于等于0的整数，为0或1时采用单线程下载，大于1时启用多线程'},
 
         'hist_dnld_delay':
             {'Default':   0.,
-             'Validator': lambda value: isinstance(value, float) and value >= 0,
+             'Validator': lambda value: isinstance(value, (int, float)) and value >= 0,
              'level':     4,
-             'text':      '为防止服务器数据压力过大，下载历史数据时下载一定数量的数据后延迟的时间长度，单位为秒'},
+             'text':      '为防止服务器数据压力过大，下载历史数据时下载一定数量的数据后延迟的时间长度，单位为秒，'
+                          '取值范围为[0, inf)，值为0时不延迟'},
 
         'hist_dnld_delay_evy':
             {'Default':   0,
              'Validator': lambda value: isinstance(value, int) and value >= 0,
              'level':     4,
              'text':      '为防止服务器数据压力过大，下载历史数据时，每下载一定数量的数据，就延迟一段时间。\n'
-                          '此参数为两次延迟之间的数据下载量'},
+                          '此参数为两次延迟之间的数据下载量，取值范围为大于等于0的整数，取值0时不延迟'},
 
         'hist_dnld_prog_bar':
             {'Default':   False,
              'Validator': lambda value: isinstance(value, bool),
              'level':     4,
              'text':      '下载历史数据时是否显示进度条'},
 
         'hist_dnld_retry_cnt':
             {'Default':   7,
-             'Validator': lambda value: isinstance(value, int) and
-                                        0 < value <= 10,
+             'Validator': lambda value: isinstance(value, int) and 0 < value <= 10,
              'level':     4,
-             'text':      '下载历史数据失败时的自动重试次数'},
+             'text':      '下载历史数据失败时的自动重试次数，取值范围为(0, 10]且必须为整数'},
 
         'hist_dnld_retry_wait':
             {'Default':   1.,
-             'Validator': lambda value: isinstance(value, (int, float)) and
-                                        0.1 <= value <= 5.0,
+             'Validator': lambda value: isinstance(value, (int, float)) and 0.1 <= value <= 5.0,
              'level':     4,
-             'text':      '下载历史数据失败时的自动重试前的延迟时间，单位为秒'},
+             'text':      '下载历史数据失败时的自动重试前的延迟时间，单位为秒，取值范围为[0.1, 5.0]'},
 
         'hist_dnld_backoff':
             {'Default':   2.,
-             'Validator': lambda value: isinstance(value, (int, float)) and
-                                        1.0 <= value <= 3.0,
+             'Validator': lambda value: isinstance(value, (int, float)) and 1.0 <= value <= 3.0,
              'level':     4,
              'text':      '下载历史数据失败时的自动重试的延迟时间倍增乘数\n'
                           '例如，设置hist_dnld_backoff = 2时，每次重试失败\n'
-                          '后延迟时间会变为前一次的2倍'},
+                          '后延迟时间会变为前一次的2倍，取值范围为[1.0, 3.0]'},
 
         'auto_dnld_hist_tables':
             {'Default':   [],
-             'Validator': lambda value: isinstance(value, list) and
-                                        all(isinstance(item, str) for item in value),
+             'Validator': lambda value: isinstance(value, list) and all(isinstance(item, str) for item in value),
              'level':     4,
              'text':      '在实盘运行时自动下载的历史数据表名列表，例如：\n'
                           '["stock_daily", "index_weekly", "stock_monthly"]\n'
                           '如果列表为空，则不自动下载任何历史数据'},
 
         'gpu':
             {'Default':   False,
              'Validator': lambda value: isinstance(value, bool),
              'level':     4,
              'text':      '如果True，策略参数寻优时使用GPU加速计算\n'
                           '<本功能目前尚未实现! NotImplemented>'},
 
         'local_data_source':
             {'Default':   'file',
-             'Validator': lambda value: isinstance(value, str) and value.lower() in ['file',
-                                                                                     'database',
-                                                                                     'db'],
+             'Validator': lambda value: isinstance(value, str)
+                                        and value.lower() in ['file',
+                                                              'database',
+                                                              'db'],
              'level':     1,
-             'text':      '确定本地历史数据存储方式：\n'
+             'text':      '确定本地历史数据存储方式，取值范围如下：\n'
                           'file     - 历史数据以本地文件的形式存储，\n'
                           '           文件格式在"local_data_file_type"属性中指定，包括csv/hdf等多种选项\n'
                           'database - 历史数据存储在一个mysql数据库中\n'
                           '           选择此选项时，需要在配置文件中配置数据库的连接信息\n'
                           'db       - 等同于"database"'},
 
         'local_data_file_type':
             {'Default':   'csv',
-             'Validator': lambda value: isinstance(value, str) and value.lower() in ['csv',
-                                                                                     'hdf',
-                                                                                     'feather',
-                                                                                     'fth'],
+             'Validator': lambda value: isinstance(value, str)
+                                        and value.lower() in ['csv',
+                                                              'hdf',
+                                                              'feather',
+                                                              'fth'],
              'level':     4,
-             'text':      '确定本地历史数据文件的存储格式：\n'
+             'text':      '确定本地历史数据文件的存储格式，取值范围如下：\n'
                           'csv - 历史数据文件以csv形式存储，速度较慢但可以用Excel打开\n'
                           'hdf - 历史数据文件以hd5形式存储，数据存储和读取速度较快\n'
                           'feather/fth - 历史数据文件以feather格式存储，数据交换速度快但不适用长期存储'},
 
         'local_data_file_path':
             {'Default':   'data/',
              'Validator': lambda value: isinstance(value, str),
@@ -355,41 +362,39 @@
         'local_db_name':
             {'Default':   'qt_db',
              'Validator': lambda value: isinstance(value, str) and
                                         (len(value) <= 255) and
                                         (all(char not in value for
                                              char in '+-/?<>{}[]()|\\!@#$%^&*=~`')),
              'level':     4,
-             'text':      '用于存储历史数据的数据库名，默认值为"qt_db"'},
+             'text':      '用于存储历史数据的数据库名，默认值为"qt_db"，数据库名称不能包含特殊字符'},
 
         'local_db_user':
             {'Default':   '',
              'Validator': lambda value: isinstance(value, str),
              'level':     4,
-             'text':      '访问数据库的用户名，该用户需具备足够的操作权限\n'
-                          '建议通过配置文件配置数据库用户名和密码'},
+             'text':      '访问数据库的用户名，该用户需具备足够的操作权限。建议通过配置文件配置数据库用户名和密码'},
 
         'local_db_password':
             {'Default':   '',
              'Validator': lambda value: isinstance(value, str),
              'level':     4,
-             'text':      '数据库的访问密码\n\n'
-                          '建议通过配置文件配置数据库用户名和密码'},
+             'text':      '数据库的访问密码。建议通过配置文件配置数据库用户名和密码'},
 
         'sys_log_file_path':
             {'Default':   'syslog/',
              'Validator': lambda value: isinstance(value, str),
              'level':     4,
-             'text':      '系统运行日志及错误日志的存储路径\n'},
+             'text':      '系统运行日志及错误日志的存储路径'},
 
         'trade_log_file_path':
             {'Default':   'tradelog/',
              'Validator': lambda value: isinstance(value, str),
              'level':     4,
-             'text':      '明细交易日志的存储路径\n'},
+             'text':      '明细交易日志的存储路径'},
 
         'trade_log':
             {'Default':   True,
              'Validator': lambda value: isinstance(value, bool),
              'level':     1,
              'text':      '是否生成明细交易清单，以pd.DataFrame形式给出明细的每日交易清单\n'
                           '包括交易信号以及每一步骤的交易结果'},
@@ -404,19 +409,19 @@
                           '绝对值意外，还需要考虑同时期的市场平均表现，只有当投资收益优于市场平均表现的，才会\n'
                           '被算作超额收益或alpha收益，这才是投资策略追求的目标'},
 
         'benchmark_asset_type':
             {'Default':   'IDX',
              'Validator': lambda value: _validate_asset_type(value),
              'level':     1,
-             'text':      '基准收益的资产类型，包括：\n'
+             'text':      '基准收益的资产类型，取值范围如下：\n'
                           'IDX  : 指数\n'
                           'E    : 股票\n'
                           'FT   : 期货\n'
-                          'FD   : 基金\n'},
+                          'FD   : 基金'},
 
         'benchmark_dtype':
             {'Default':   'close',
              'Validator': lambda value: value.lower() in ['open',
                                                           'high',
                                                           'low',
                                                           'close',
@@ -456,61 +461,61 @@
 
         'cost_fixed_buy':
             {'Default':   0.,
              'Validator': lambda value: isinstance(value, float)
                                         and value >= 0,
              'level':     2,
              'text':      '买入证券或资产时的固定成本或固定佣金，该金额不随买入金额变化\n'
-                          '默认值为10元'},
+                          '默认值为10元，取值范围为[0, inf)'},
 
         'cost_fixed_sell':
             {'Default':   0.,
              'Validator': lambda value: isinstance(value, float)
                                         and value >= 0,
              'level':     2,
              'text':      '卖出证券或资产时的固定成本或固定佣金，该金额不随卖出金额变化\n'
-                          '默认值为0'},
+                          '默认值为0，取值范围为[0, inf)'},
 
         'cost_rate_buy':
             {'Default':   0.0003,
              'Validator': lambda value: isinstance(value, float)
                                         and 0 <= value < 1,
              'level':     1,
              'text':      '买入证券或资产时的成本费率或佣金比率，以买入金额的比例计算\n'
-                          '默认值为万分之三'},
+                          '默认值为万分之，取值范围为[0, 1)'},
 
         'cost_rate_sell':
             {'Default':   0.0001,
              'Validator': lambda value: isinstance(value, float)
                                         and 0 <= value < 1,
              'level':     1,
              'text':      '卖出证券或资产时的成本费率或佣金比率，以卖出金额的比例计算\n'
-                          '默认值为万分之一'},
+                          '默认值为万分之一，取值范围为[0, 1)'},
 
         'cost_min_buy':
             {'Default':   5.0,
              'Validator': lambda value: isinstance(value, float)
                                         and value >= 0,
              'level':     2,
              'text':      '买入证券或资产时的最低成本或佣金，买入佣金只能大于或等于该最低金额\n'
-                          '默认值为5元'},
+                          '默认值为5元，取值范围为[0, inf)'},
 
         'cost_min_sell':
             {'Default':   5.0,
              'Validator': lambda value: isinstance(value, float)
                                         and value >= 0,
              'level':     2,
-             'text':      '卖出证券或资产时的最低成本或佣金，卖出佣金只能大于或等于该最低金额'},
+             'text':      '卖出证券或资产时的最低成本或佣金，卖出佣金只能大于或等于该最低金额，取值范围为[0, inf)'},
 
         'cost_slippage':
             {'Default':   0.0,
              'Validator': lambda value: isinstance(value, float)
                                         and 0 <= value < 1,
              'level':     2,
-             'text':      '交易滑点，一个预设参数，模拟由于交易延迟或交易金额过大产生的额外交易成本'},
+             'text':      '交易滑点，一个预设参数，模拟由于交易延迟或交易金额过大产生的额外交易成本，取值范围为[0, 1)'},
 
         'invest_start':
             {'Default':   '20160405',
              'Validator': lambda value: isinstance(value, str)
                                         and _is_datelike(value),
              'level':     0,
              'text':      '回测模式下的回测开始日期\n'
@@ -550,25 +555,25 @@
 
         'allow_sell_short':
             {'Default':   False,
              'Validator': lambda value: isinstance(value, bool),
              'level':     4,
              'text':      '是否允许卖空交易，：\n'
                           '- False - 默认值，不允许卖空操作，卖出数量最多仅为当前可用持仓数量\n'
-                          '- True -  允许卖空，卖出数量大于持仓量时，即持有空头仓位\n'},
+                          '- True -  允许卖空，卖出数量大于持仓量时，即持有空头仓位'},
 
         'long_position_limit':
             {'Default':   1.,
              'Validator': lambda value: isinstance(value, float) and (value > 0),
              'level':     3,
              'text':      '回测过程中允许交易信号建立的多头仓位百分比的极限值，即允许动用\n'
                           '总资产（包括现金和持有股票的总额）的多少百分比用于持有多头仓位，\n'
                           '默认值1.0，即100%\n'
                           '如果设置值大于1，则表示允许超过持有现金建仓，这种情况会产生负现金\n'
-                          '余额，表示产生了借贷\n'},
+                          '余额，表示产生了借贷'},
 
         'short_position_limit':
             {'Default':   -1.,
              'Validator': lambda value: isinstance(value, float) and (value < 0),
              'level':     3,
              'text':      '回测过程中允许交易信号建立的空头仓位百分比的极限值，即允许持有的\n'
                           '空头仓位占当前净资产总额的最高比例限额，默认值-1.0，即最多允许借入\n'
@@ -579,19 +584,19 @@
             {'Default':   'none',
              'Validator': lambda value: isinstance(value, str)
                                         and value.lower() in ['none', 'n', 'back', 'b', 'adj'],
              'level':     4,
              'text':      '回测时的复权价格处理方法：\n'
                           '股票分红除权的处理，正常来说，应该在股票分红除权时计算分红和派息对持仓\n'
                           '数量和现金的影响，但是目前这种处理方法比较复杂，暂时先采用比较简单的方\n'
-                          '法，即直接采用复权价格进行回测，目前处理方法有两种'
+                          '法，即直接采用复权价格进行回测，取值范围如下：'
                           '- none/n - 默认值，不使用复权价格，但也不处理派息，这只是临时处理，因\n'
                           '           为长期回测不考虑除权派息将会导致回测结果与实际相差巨大\n'
                           '- back/b - 使用后复权价格回测，可以弥补不考虑分红派股的不足\n'
-                          '- adj    - 使用前复权价格回测。\n'},
+                          '- adj    - 使用前复权价格回测。'},
 
         'maximize_cash_usage':
             {'Default':   True,
              'Validator': lambda value: isinstance(value, bool),
              'level':     4,
              'text':      '回测交易时是否最大化利用同一批次交易获得的现金。即优先卖出股票并将获得的现金立即\n'
                           '用于同一批次的买入交易，以便最大限度利用可用现金。当现金的交割期大于0时无效。\n'
@@ -601,40 +606,38 @@
                           '          次交易委托同时提交时，这是正常情况'},
 
         'PT_signal_timing':
             {'Default':   'lazy',
              'Validator': lambda value: value.lower() in ['aggressive', 'lazy'],
              'level':     3,
              'text':      '回测信号模式为PT（position target）时，控制检查实际持仓比例并自动生成交易\n'
-                          '信号的时机，默认normal\n'
+                          '信号的时机，默认normal，取值范围如下：\n'
                           '- aggressive: 在整个策略运行时间点上都会产生交易信号，不论此时PT信号是否发\n'
                           '              生变化，实时监控实际持仓与计划持仓之间的差异，只要二者发生偏\n'
                           '              离，就产生信号\n'
                           '- lazy:       在策略运行时间点上，只有当持仓比例发生变化时，才会产生交易\n'
                           '              信号，不实时监控实际持仓与计划持仓的差异'},
 
         'PT_buy_threshold':
             {'Default':   0.,
-             'Validator': lambda value: isinstance(value, (float, int))
-                                        and (0 <= value < 1),
+             'Validator': lambda value: isinstance(value, (float, int)) and (0 <= value < 1),
              'level':     3,
              'text':      '回测信号模式为PT（position target）时，触发买入信号的仓位差异阈值\n'
                           '在这种模式下，当持有的投资产品的仓位比目标仓位低，且差额超过阈值时，触发买入信号\n'
                           '例如当卖出阈值为0.05即5%时，若目标持仓30%，那么只有当实际持仓<=25%时，才会产生\n'
-                          '交易信号，即此时实际持仓与目标持仓之间的差值大于5%了'},
+                          '交易信号，即此时实际持仓与目标持仓之间的差值大于5%了。取值范围为[0, 1)'},
 
         'PT_sell_threshold':
             {'Default':   0.,
-             'Validator': lambda value: isinstance(value, (float, int))
-                                        and (0 <= value < 1),
+             'Validator': lambda value: isinstance(value, (float, int)) and (0 <= value < 1),
              'level':     3,
              'text':      '回测信号模式为PT（position target）时，触发卖出信号的仓位差异阈值\n'
                           '在这种模式下，当持有的投资产品的仓位比目标仓位高，且差额超过阈值时，触发卖出信号\n'
                           '例如当卖出阈值为0.05即5%时，若目标持仓30%，那么只有当实际持仓>=35%时，才会产生\n'
-                          '交易信号，即此时实际持仓与目标持仓之间的差值大于5%了'},
+                          '交易信号，即此时实际持仓与目标持仓之间的差值大于5%了。取值范围为[0, 1)'},
 
         'price_priority_OHLC':
             {'Default':   'OHLC',
              'Validator': lambda value: isinstance(value, str)
                                         and all(item.upper() in 'OHLCA'
                                                 for item in value)
                                         and all(item.upper() in value
@@ -646,16 +649,15 @@
 
         'price_priority_quote':
             {'Default':   'normal',
              'Validator': lambda value: isinstance(value, str)
                                         and (value in ['normal', 'reverse']),
              'level':     3,
              'text':      '回测时如果存在多种价格类型的交易信号，而且交易价格的类型为实时报价时，回测程序处理\n'
-                          '不同的价格信号的优先级。\n'
-                          '输入包括"normal" 以及 "reverse"两种，分别表示：\n'
+                          '不同的价格信号的优先级。取值范围如下：\n'
                           '- "normal"：  优先处理更接近成交价的报价，如卖1/买1等\n'
                           '- "reverse"： 优先处理更远离成交价的报价，如卖5/买5等'},
 
         'cash_delivery_period':
             {'Default':   0,
              'Validator': lambda value: isinstance(value, int)
                                         and value in range(5),
@@ -703,59 +705,60 @@
 
         'strategy_open_close_timing_offset':
             {'Default':   1,
              'Validator': lambda value: isinstance(value, int)
                                         and value in range(5),
              'level':     3,
              'text':      '策略信号的开盘/收盘运行时间偏移量，单位为分钟，当策略信号运行时机为开盘/收盘，需要提前/推迟\n'
-                          '一个偏移量运行，避免无法交易。'},
+                          '一个偏移量运行，避免无法交易。取值范围为[1, 5]'},
 
         'opti_start':
             {'Default':   '20160405',
              'Validator': lambda value: isinstance(value, str)
                                         and _is_datelike(value),
              'level':     0,
-             'text':      '优化模式下的策略优化区间开始日期'},
+             'text':      '优化模式下的策略优化区间开始日期，输入为"YYYYMMDD"或其他类似日期格式的字符串'},
 
         'opti_end':
             {'Default':   '20191231',
              'Validator': lambda value: isinstance(value, str)
                                         and _is_datelike(value),
              'level':     0,
-             'text':      '优化模式下的策略优化区间结束日期'},
+             'text':      '优化模式下的策略优化区间结束日期，输入为"YYYYMMDD"或其他类似日期格式的字符串'},
 
         'opti_cash_amounts':
             {'Default':   [100000.0],
              'Validator': lambda value: isinstance(value, (tuple, list))
                                         and all(isinstance(item, (float, int))
                                                 for item in value)
                                         and all(item > 1 for item in value),
              'level':     1,
-             'text':      '优化模式投资的金额，一个tuple或list，每次投入资金的金额，多个数字表示多次投入'},
+             'text':      '优化模式投资的金额，一个tuple或list，每次投入资金的金额，多个数字表示多次投入\n'
+                          '输入的数字的个数必须与cash_dates中的日期数量相'},
 
         'opti_cash_dates':
             {'Default':   None,
              'Validator': lambda value: isinstance(value, (str, list))
                                         and all(isinstance(item, str)
                                                 for item in value) or value is None,
              'level':     2,
              'text':      '策略优化区间现金投入的日期，一个str或list，多个日期表示多次现金投入。默认为None\n'
                           '当此参数为None时，现金投入日期与invest_start相同，当参数不为None时，此参数覆盖\n'
                           'invest_start\n'
                           '参数输入类型为str时，格式为"YYYYMMDD"\n'
                           '如果需要模拟现金多次定投投入，或者多次分散投入，则可以输入list类型或str类型\n'
                           '以下两种输入方式等效：\n'
-                          '"20100104,20100202,20100304"'
+                          '"20100104,20100202,20100304" == '
                           '["20100104", "20100202", "20100304"]'},
 
         'opti_type':
             {'Default':   'single',
              'Validator': lambda value: isinstance(value, str) and value in ['single', 'multiple'],
              'level':     3,
-             'text':      '优化类型。指优化数据的利用方式:\n'
+             'text':      '优化类型。指优化数据的利用方，取值范围如下:\n'
                           '"single"   - 在每一回合的优化测试中，在优化区间上进行覆盖整个区间的单次回测并评价\n'
                           '             回测结果\n'
                           '"multiple" - 在每一回合的优化测试中，将优化区间的数据划分为多个子区间，在这些子\n'
                           '             区间上分别测试，并根据所有测试的结果确定策略在整个区间上的评价结果'},
 
         'opti_sub_periods':
             {'Default':   5,
@@ -772,25 +775,23 @@
 
         'test_start':
             {'Default':   '20200106',
              'Validator': lambda value: isinstance(value, str)
                                         and _is_datelike(value),
              'level':     0,
              'text':      '优化模式下的策略测试区间开始日期'
-                          '格式为"YYYYMMDD"'
-                          '字符串类型输入'},
+                          '格式为"YYYYMMDD"，字符串类型输入'},
 
         'test_end':
             {'Default':   '20210201',
              'Validator': lambda value: isinstance(value, str)
                                         and _is_datelike(value),
              'level':     0,
              'text':      '优化模式下的策略测试区间结束日期\n'
-                          '格式为"YYYYMMDD"'
-                          '字符串类型输入'},
+                          '格式为"YYYYMMDD"，字符串类型输入'},
 
         'test_cash_amounts':
             {'Default':   [100000.0],
              'Validator': lambda value: isinstance(value, (tuple, list))
                                         and all(isinstance(item, (float, int))
                                                 for item in value)
                                         and all(item > 1 for item in value),
@@ -815,70 +816,70 @@
                           '["20100104", "20100202", "20100304"]'},
 
         'test_type':
             {'Default':   'single',
              'Validator': lambda value: isinstance(value, str) and
                                         value in ['single', 'multiple', 'montecarlo'],
              'level':     3,
-             'text':      '测试类型。指测试数据的利用方式:\n'
+             'text':      '测试类型。指测试数据的利用方式，取值范围如下:\n'
                           '"single"     - 在每一回合的优化测试中，在测试区间上进行覆盖整个区间的单次回测\n'
                           '               并评价回测结果\n'
                           '"multiple"   - 在每一回合的优化测试中，将测试区间的数据划分为多个子区间，在这\n'
                           '               些子区间上分别测试，并根据所有测试的结果确定策略在整个区间上的\n'
                           '               评价结果\n'
                           '"montecarlo" - 蒙特卡洛测试，根据测试区间历史数据的统计性质，随机生成大量的模\n'
                           '               拟价格变化数据，用这些数据对策略的表现进行评价，最后给出统计意\n'
                           '               义的评价结果'},
 
         'test_indicators':
             {'Default':   'years,fv,return,mdd,v,ref,alpha,beta,sharp,info',
              'Validator': lambda value: isinstance(value, str),
              'level':     2,
              'text':      '对优化后的策略参数进行测试评价的评价指标。\n'
-                          '格式为逗号分隔的字符串，多个评价指标会以字典的形式输出，包含以下类型中的一种或多种\n'
+                          '格式为逗号分隔的字符串，多个评价指标会以字典的形式输出，取值范围如下：\n'
                           '"years"       - total year\n'
                           '"fv"          - final values\n'
                           '"return"      - total return rate\n'
                           '"mdd"         - max draw down\n'
                           '"ref"         - reference data return\n'
                           '"alpha"       - alpha rate\n'
                           '"beta"        - beta rate\n'
                           '"sharp"       - sharp rate\n'
                           '"info"        - info rate'},
 
         'indicator_plot_type':
             {'Default':   'histo',
              'Validator': lambda value: _validate_indicator_plot_type(value),
              'level':     2,
-             'text':      '优化或测试结果评价指标的可视化图表类型:\n'
+             'text':      '优化或测试结果评价指标的可视化图表类型，取值范围如下:\n'
                           '0  - errorbar 类型\n'
                           '1  - scatter 类型\n'
                           '2  - histo 类型\n'
                           '3  - violin 类型\n'
                           '4  - box 类型'},
 
         'test_sub_periods':
             {'Default':   3,
              'Validator': lambda value: isinstance(value, int) and value >= 1,
              'level':     3,
-             'text':      '仅当测试类型为"multiple"时有效。将测试区间切分为子区间的数量'},
+             'text':      '仅当测试类型为"multiple"时有效。将测试区间切分为子区间的数量，输入值为大于等于1的整数'},
 
         'test_sub_prd_length':
             {'Default':   0.75,
              'Validator': lambda value: isinstance(value, float) and 0 <= value <= 1.,
              'level':     3,
              'text':      '仅当测试类型为"multiple"时有效。每一个测试子区间长度占整个测试区间长度的比例\n'
-                          '例如，当测试区间长度为4年时，本参数0.75代表每个测试子区间长度为3年'},
+                          '例如，当测试区间长度为4年时，本参数0.75代表每个测试子区间长度为3年，取值范围[0, 1]'},
 
         'test_cycle_count':
             {'Default':   100,
              'Validator': lambda value: isinstance(value, int) and value >= 1,
              'level':     3,
              'text':      '仅当测试类型为"montecarlo"时有效。生成的模拟测试数据的数量。\n'
-                          '默认情况下生成100组模拟价格数据，并进行100次策略回测并评价其统计结果'},
+                          '默认情况下生成100组模拟价格数据，并进行100次策略回测并评价其统计结果，输入值为大于等于1的整数'},
 
         'optimize_target':
             {'Default':   'final_value',
              'Validator': lambda value: isinstance(value, str)
                                         and value in ['final_value', 'FV', 'SHARP'],
              'level':     1,
              'text':      '策略的优化目标。即优化时以找到该指标最佳的策略为目标'},
@@ -890,76 +891,78 @@
              'text':      '为True时寻找目标值最大的策略，为False时寻找目标值最低的策略'},
 
         'opti_method':
             {'Default':   1,
              'Validator': lambda value: isinstance(value, int)
                                         and value <= 3,
              'level':     1,
-             'text':      '策略优化算法，可选值如下:\n'
+             'text':      '策略优化算法，取值范围如下:\n'
                           '0 - 网格法，按照一定间隔对整个向量空间进行网格搜索\n'
                           '1 - 蒙特卡洛法，在向量空间中随机取出一定的点搜索最佳策略\n'
                           '2 - 递进步长法，对向量空间进行多轮搜索，每一轮搜索结束后根据结果选择部分子\n'
                           '    空间，缩小步长进一步搜索\n'
                           '3 - 遗传算法，模拟生物种群在环境压力下不断进化的方法寻找全局最优（尚未完成）\n'
-                          '4 - ML方法，基于机器学习的最佳策略搜索算法（尚未完成）\n'},
+                          '4 - ML方法，基于机器学习的最佳策略搜索算法（To be Implemented）'},
 
         'opti_grid_size':
             {'Default':   1,
              'Validator': lambda value: _num_or_seq_of_num(value) and value > 0,
              'level':     3,
-             'text':      '使用穷举法搜索最佳策略时有用，搜索步长'},
+             'text':      '使用穷举法搜索最佳策略时有用，搜索步长，取值范围为大于0的整数或list'},
 
         'opti_sample_count':
             {'Default':   256,
              'Validator': lambda value: isinstance(value, int) and value > 0,
              'level':     3,
-             'text':      '使用蒙特卡洛法搜索最佳策略时有用，在向量空间中采样的数量'},
+             'text':      '使用蒙特卡洛法搜索最佳策略时有用，在向量空间中采样的数量，取值范围为大于0的整数'},
 
         'opti_r_sample_count':
             {'Default':   16,
              'Validator': lambda value: _num_or_seq_of_num(value)
                                         and value >= 0,
              'level':     3,
-             'text':      '在使用递进步长法搜索最佳策略时有用，每一轮随机取样的数量'},
+             'text':      '在使用递进步长法搜索最佳策略时有用，每一轮随机取样的数量，取值范围为大于等于0的整数'},
 
         'opti_reduce_ratio':
             {'Default':   0.1,
              'Validator': lambda value: isinstance(value, float)
                                         and 0 < value < 1,
              'level':     3,
              'text':      '在使用递进步长法搜索最佳策略时有用，\n'
-                          '每一轮随机取样后择优留用的比例，同样也是子空间缩小的比例\n'},
+                          '每一轮随机取样后择优留用的比例，同样也是子空间缩小的比例，取值范围为(0, 1)'},
 
         'opti_max_rounds':
             {'Default':   5,
              'Validator': lambda value: isinstance(value, int)
                                         and value > 1,
              'level':     3,
-             'text':      '在使用递进步长法搜索最佳策略时有用，多轮搜索的最大轮数，轮数大于该值时停止搜索'},
+             'text':      '在使用递进步长法搜索最佳策略时有用，多轮搜索的最大轮数，轮数大于该值时停止搜索，'
+                          '取值范围为大于1的整数'},
 
         'opti_min_volume':
             {'Default':   1000,
              'Validator': lambda value: isinstance(value, (float, int))
                                         and value > 0,
              'level':     3,
-             'text':      '在使用递进步长法搜索最佳策略时有用，空间最小体积，当空间volume低于该值时停止搜索'},
+             'text':      '在使用递进步长法搜索最佳策略时有用，空间最小体积，当空间volume低于该值时停止搜索，'
+                          '取值范围为大于0的数'},
 
         'opti_population':
             {'Default':   1000.0,
              'Validator': lambda value: isinstance(value, float)
                                         and value >= 0,
              'level':     3,
-             'text':      '在使用遗传算法搜索最佳策略时有用，种群的数量'},
+             'text':      '在使用遗传算法搜索最佳策略时有用，种群的数量，取值范围为大于等于0的整数'},
 
         'opti_output_count':
             {'Default':   30,
              'Validator': lambda value: isinstance(value, int)
                                         and value > 0,
              'level':     3,
-             'text':      '策略参数优化后输出的最优参数数量'},
+             'text':      '策略参数优化后输出的最优参数数量，取值范围为大于0的整数'},
 
     }
     _validate_vkwargs_dict(vkwargs)
 
     return vkwargs
```

### Comparing `qteasy-1.1.9/qteasy/backtest.py` & `qteasy-1.2.0/qteasy/backtest.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/blender.py` & `qteasy-1.2.0/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/broker.py` & `qteasy-1.2.0/qteasy/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from queue import Queue
 from abc import abstractmethod, ABCMeta
 
 import numpy as np
 import time
 
 from qteasy import QT_CONFIG
-from .utilfuncs import get_current_tz_datetime
+from .utilfuncs import get_current_timezone_datetime
 
 CASH_DECIMAL_PLACES = QT_CONFIG['cash_decimal_places']
 AMOUNT_DECIMAL_PLACES = QT_CONFIG['amount_decimal_places']
 
 
 def _verify_trade_result(trade_result, order_qty):
     """ 检查result，确认是否符合基本要求:
@@ -119,15 +119,15 @@
         self.password = ''
         self.token = ''
         self.status = 'init'  # init, running, stopped, paused
         self.debug = False
         self.is_registered = False
 
         self.time_zone = 'local'
-        self.init_time = get_current_tz_datetime(self.time_zone).strftime('%Y-%m-%d %H:%M:%S')
+        self.init_time = get_current_timezone_datetime(self.time_zone).strftime('%Y-%m-%d %H:%M:%S')
 
         self.order_queue = Queue()
         self.result_queue = Queue()
         self.broker_messages = Queue()
 
     @property
     def data_source(self):
@@ -337,15 +337,15 @@
             if result_type in ['filled', 'partial-filled']:
                 filled_qty = qty
             elif result_type == 'canceled':
                 canceled_qty = qty
             else:
                 raise ValueError(f'Unknown result_type: {result_type}, should be one of ["filled", "canceled"]')
 
-            current_datetime = get_current_tz_datetime(self.time_zone)
+            current_datetime = get_current_timezone_datetime(self.time_zone)
             raw_trade_result = {
                 'order_id':        order['order_id'],
                 'filled_qty':      filled_qty,
                 'price':           filled_price,
                 'transaction_fee': transaction_fee,
                 'execution_time':  current_datetime.strftime('%Y-%m-%d %H:%M:%S'),
                 'canceled_qty':    canceled_qty,
```

### Comparing `qteasy-1.1.9/qteasy/built_in.py` & `qteasy-1.2.0/qteasy/built_in.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/core.py` & `qteasy-1.2.0/qteasy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,16 +648,25 @@
         asset_types: Str of List of Str, default: None
             通过指定tables或dtypes来确定需要更新的表单时，指定asset_types可以限定表单的范围
             如果tables != all时，给出asset_type会排除掉与之不符的数据表
         start_date: DateTime Like, default: None
             限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
         end_date: DateTime Like, default: None
             限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
-        code_range: str or list of str, default: None
-            **注意，不是所有情况下code_range参数都有效
+        list_arg_filter: str or list of str, default: None  **注意，不是所有情况下该参数都有效**
+            限定下载数据时的筛选参数，某些数据表以列表的形式给出可筛选参数，如stock_basic表，它有一个可筛选
+            参数"exchange"，选项包含 'SSE', 'SZSE', 'BSE'，可以通过此参数限定下载数据的范围。
+            如果filter_arg为None，则下载所有数据。
+            例如，下载stock_basic表数据时，下载以下输入均为合法输入：
+            - 'SZSE'
+                仅下载深圳交易所的股票数据
+            - ['SSE', 'SZSE']
+            - 'SSE, SZSE'
+                上面两种写法等效，下载上海和深圳交易所的股票数据
+        symbols: str or list of str, default: None  **注意，不是所有情况下该参数都有效**
             限定下载数据的证券代码范围，代码不需要给出类型后缀，只需要给出数字代码即可。
             可以多种形式确定范围，以下输入均为合法输入：
             - '000001'
                 没有指定asset_types时，000001.SZ, 000001.SH ... 等所有代码都会被选中下载
                 如果指定asset_types，只有符合类型的证券数据会被下载
             - '000001, 000002, 000003'
             - ['000001', '000002', '000003']
@@ -689,15 +698,26 @@
     """
     from .database import DataSource
     if data_source is None:
         data_source = qteasy.QT_DATA_SOURCE
     if not isinstance(data_source, DataSource):
         raise TypeError(f'A DataSource object must be passed, got {type(data_source)} instead.')
     print(f'Filling data source {data_source} ...')
-    data_source.refill_local_source(**kwargs)
+    hist_dnld_delay = None
+    hist_dnld_delay_evy = None
+    if 'download_batch_size' not in kwargs:
+        hist_dnld_delay = QT_CONFIG.hist_dnld_delay
+    if 'download_batch_interval' not in kwargs:
+        hist_dnld_delay_evy = QT_CONFIG.hist_dnld_delay_evy
+
+    data_source.refill_local_source(
+            download_batch_size=hist_dnld_delay_evy,
+            download_batch_interval=hist_dnld_delay,
+            **kwargs,
+    )
 
 
 def get_history_data(htypes,
                      shares=None,
                      symbols=None,
                      start=None,
                      end=None,
@@ -2033,17 +2053,17 @@
 
     # 赋值给参考数据和运行模式
     benchmark_data_type = config['benchmark_asset']
     run_mode = config['mode']
 
     if run_mode == 0 or run_mode == 'live':
         # 进入实时信号生成模式:
-        from qteasy.trader import start_trader
+        from qteasy.trader import start_trader_ui
         from qteasy import QT_DATA_SOURCE
-        start_trader(
+        start_trader_ui(
                 operator=operator,
                 account_id=config['live_trade_account_id'],
                 user_name=config['live_trade_account'],
                 init_cash=config['live_trade_init_cash'],
                 init_holdings=config['live_trade_init_holdings'],
                 config=config,
                 datasource=QT_DATA_SOURCE,
```

### Comparing `qteasy-1.1.9/qteasy/database.py` & `qteasy-1.2.0/qteasy/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # ======================================
 import os
 from os import path
 import pandas as pd
 import numpy as np
 import warnings
 
-from concurrent.futures import ProcessPoolExecutor, as_completed
+from concurrent.futures import as_completed, ThreadPoolExecutor
 from functools import lru_cache
 
 from .utilfuncs import progress_bar, sec_to_duration, nearest_market_trade_day, input_to_list
 from .utilfuncs import is_market_trade_day, str_to_list, regulate_date_format
 from .utilfuncs import _wildcard_match, _partial_lev_ratio, _lev_ratio, human_file_size, human_units
 from .utilfuncs import freq_dither
 
@@ -4794,16 +4794,18 @@
             if shares is not None:
                 weight_df.drop(columns=columns_to_drop, inplace=True)
                 weight_df = weight_df.reindex(columns=shares)
             df_by_index['wt-' + idx] = weight_df
         return df_by_index
 
     def refill_local_source(self, tables=None, dtypes=None, freqs=None, asset_types=None, start_date=None,
-                            end_date=None, symbols=None, merge_type='update', reversed_par_seq=False, parallel=True,
-                            process_count=None, chunk_size=100, refresh_trade_calendar=False, log=False) -> None:
+                            end_date=None, list_arg_filter=None, symbols=None, merge_type='update',
+                            reversed_par_seq=False, parallel=True, process_count=None, chunk_size=100,
+                            download_batch_size=0, download_batch_interval=0, refresh_trade_calendar=False,
+                            log=False) -> None:
         """ 批量下载历史数据并保存到本地数据仓库
 
         Parameters
         ----------
         tables: str or list of str
             需要补充的本地数据表，可以同时给出多个table的名称，逗号分隔字符串和字符串列表都合法：
             例如，下面两种方式都合法且相同：
@@ -4827,14 +4829,24 @@
         asset_types: str or list of str
             通过指定tables或dtypes来确定需要更新的表单时，指定asset_types可以限定表单的范围
             如果tables != all时，给出asset_type会排除掉与之不符的数据表
         start_date: str YYYYMMDD
             限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
         end_date: str YYYYMMDD
             限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
+        list_arg_filter: str or list of str, default: None  **注意，不是所有情况下filter_arg参数都有效**
+            限定下载数据时的筛选参数，某些数据表以列表的形式给出可筛选参数，如stock_basic表，它有一个可筛选
+            参数"exchange"，选项包含 'SSE', 'SZSE', 'BSE'，可以通过此参数限定下载数据的范围。
+            如果filter_arg为None，则下载所有数据。
+            例如，下载stock_basic表数据时，下载以下输入均为合法输入：
+            - 'SZSE'
+                仅下载深圳交易所的股票数据
+            - ['SSE', 'SZSE']
+            - 'SSE, SZSE'
+                上面两种写法等效，下载上海和深圳交易所的股票数据
         symbols: str or list of str
             限定下载数据的证券代码范围，代码不需要给出类型后缀，只需要给出数字代码即可。
             可以多种形式确定范围，以下输入均为合法输入：
             - '000001'
                 没有指定asset_types时，000001.SZ, 000001.SH ... 等所有代码都会被选中下载
                 如果指定asset_types，只有符合类型的证券数据会被下载
             - '000001, 000002, 000003'
@@ -4855,27 +4867,35 @@
             - True:  启用多线程下载数据
             - False: 禁用多线程下载
         process_count: int
             启用多线程下载时，同时开启的线程数，默认值为设备的CPU核心数
         chunk_size: int
             保存数据到本地时，为了减少文件/数据库读取次数，将下载的数据累计一定数量后
             再批量保存到本地，chunk_size即批量，默认值100
-        refresh_trade_calendar: Bool, Default True
-            是否刷新交易日历，默认True
+        download_batch_size: int, default 0
+            为了降低下载数据时的网络请求频率，可以在完成一批数据下载后，暂停一段时间再继续下载
+            该参数指定了每次暂停之前最多可以下载的次数，该参数只有在parallel=False时有效
+            如果为0，则不暂停，一次性下载所有数据
+        download_batch_interval: int, default 0
+            为了降低下载数据时的网络请求频率，可以在完成一批数据下载后，暂停一段时间再继续下载
+            该参数指定了每次暂停的时间，单位为秒，该参数只有在parallel=False时有效
+            如果<=0，则不暂停，立即开始下一批数据下载
+        refresh_trade_calendar: Bool, Default False
+            是否强制刷新交易日历，如果为True，将下载最新的交易日历数据，如果为False，仅在交易日历数据不足时下载
         log: Bool, Default False
             是否记录数据下载日志
 
         Returns
         -------
         None
 
         """
 
         from .tsfuncs import acquire_data
-        # 1 参数合法性检查
+        # 1 参数合法性检查 TODO: 参数检查在core.py中完成，这里只需要调用即可
         if (tables is None) and (dtypes is None):
             raise KeyError(f'tables and dtypes can not both be None.')
         if tables is None:
             tables = []
         if dtypes is None:
             dtypes = []
         valid_table_values = list(TABLE_MASTERS.keys()) + TABLE_USAGES + ['all']
@@ -4887,26 +4907,41 @@
             raise KeyError(f'some items in tables list are not valid: '
                            f'{[item for item in tables if item not in valid_table_values]}')
         if not isinstance(dtypes, (str, list)):
             raise TypeError(f'dtypes should be a list of a string, got {type(dtypes)} instead.')
         if isinstance(dtypes, str):
             dtypes = str_to_list(dtypes)
 
+        if chunk_size <= 0:
+            chunk_size = 100
+
+        if download_batch_size <= 0:
+            download_batch_size = 999999999999  # 一个很大的数，保证不会暂停下载
+
+        if download_batch_interval <= 0:
+            download_batch_interval = 0
+
         code_start = None
         code_end = None
         if symbols is not None:
             if not isinstance(symbols, (str, list)):
                 raise TypeError(f'code_range should be a string or list, got {type(symbols)} instead.')
             if isinstance(symbols, str):
                 if len(str_to_list(symbols, ':')) == 2:
                     code_start, code_end = str_to_list(symbols, ':')
                     symbols = None
                 else:
                     symbols = str_to_list(symbols, ',')
 
+        if list_arg_filter is not None:
+            if not isinstance(list_arg_filter, (str, list)):
+                raise TypeError(f'list_arg_filter should be a string or list, got {type(list_arg_filter)} instead.')
+            if isinstance(list_arg_filter, str):
+                list_arg_filter = str_to_list(list_arg_filter, ',')
+
         # 2 生成需要处理的数据表清单 tables
         table_master = get_table_master()
         tables_to_refill = set()
         tables = [item.lower() for item in tables]
         if 'all' in tables:
             tables_to_refill.update(TABLE_MASTERS)
         else:
@@ -4950,15 +4985,16 @@
                 cur_table = table_master.loc[table]
                 fill_type = cur_table.fill_arg_type
                 if fill_type == 'trade_date' and refresh_trade_calendar:
                     dependent_tables.add('trade_calendar')
                 elif fill_type == 'table_index':
                     dependent_tables.add(cur_table.arg_rng)
             tables_to_refill.update(dependent_tables)
-            # 为了避免parallel读取失败，需要确保tables_to_refill中包含trade_calendar表：
+
+            # 检查trade_calendar中是否有足够的数据，如果没有，需要包含trade_calendar表：
             if 'trade_calendar' not in tables_to_refill:
                 if refresh_trade_calendar:
                     tables_to_refill.add('trade_calendar')
                 else:
                     # 检查trade_calendar中是否已有数据，且最新日期是否足以覆盖今天，如果没有数据或数据不足，也需要添加该表
                     latest_calendar_date = self.get_table_info('trade_calendar', print_info=False)[11]
                     if latest_calendar_date == 'N/A':
@@ -4995,14 +5031,15 @@
             allow_start_end = (cur_table_info.arg_allow_start_end.lower() == 'y')
             start_end_chunk_size = 0
             if cur_table_info.start_end_chunk_size != '':
                 start_end_chunk_size = int(cur_table_info.start_end_chunk_size)
             additional_args = {}
             chunked_additional_args = []
             start_end_chunk_multiplier = 1
+            # 生成start和end参数，如果需要的话
             if allow_start_end:
                 additional_args = {'start': start, 'end': end}
             if start_end_chunk_size > 0:
                 start_end_chunk_lbounds = list(pd.date_range(start=start,
                                                              end=end,
                                                              freq=f'{start_end_chunk_size}d'
                                                              ).strftime('%Y%m%d'))
@@ -5014,28 +5051,29 @@
                     start_end_chunk_rbounds = pd.to_datetime(start_end_chunk_lbounds[1:]) - prev_day
                     start_end_chunk_rbounds = list(start_end_chunk_rbounds.strftime('%Y%m%d'))
 
                 start_end_chunk_rbounds.append(end)
                 chunked_additional_args = [{'start': s, 'end': e} for s, e in
                                            zip(start_end_chunk_lbounds, start_end_chunk_rbounds)]
                 start_end_chunk_multiplier = len(chunked_additional_args)
-
+            # 生成其他参数，根据不同的fill_type生成不同的参数序列
             if fill_type in ['datetime', 'trade_date']:
                 # 根据start_date和end_date生成数据获取区间
                 additional_args = {}  # 使用日期作为关键参数，不再需要additional_args
                 arg_coverage = pd.date_range(start=start, end=end, freq=freq)
                 if fill_type == 'trade_date':
                     if freq.lower() in ['m', 'w', 'w-Fri']:
                         # 当生成的日期不连续时，或要求生成交易日序列时，需要找到最近的交易日
                         arg_coverage = map(nearest_market_trade_day, arg_coverage)
                     if freq == 'd':
                         arg_coverage = (date for date in arg_coverage if is_market_trade_day(date))
                 arg_coverage = list(pd.to_datetime(list(arg_coverage)).strftime('%Y%m%d'))
             elif fill_type == 'list':
-                arg_coverage = str_to_list(cur_table_info.arg_rng)
+                # 如果参数是一个列表，直接使用这个列表作为参数序列，除非给出了list_arg_filter
+                arg_coverage = str_to_list(cur_table_info.arg_rng) if list_arg_filter is None else list_arg_filter
             elif fill_type == 'table_index':
                 suffix = str_to_list(cur_table_info.arg_allowed_code_suffix)
                 source_table = self.read_table_data(cur_table_info.arg_rng)
                 arg_coverage = source_table.index.to_list()
                 if code_start is not None:
                     arg_coverage = [code for code in arg_coverage if (code_start <= code.split('.')[0] <= code_end)]
                 if symbols is not None:
@@ -5067,20 +5105,32 @@
             st = time.time()
             dnld_data = pd.DataFrame()
             time_elapsed = 0
             rows_affected = 0
             try:
                 # 清单中的第一张表不使用parallel下载
                 if parallel and table_count != 1:
-                    with ProcessPoolExecutor(max_workers=process_count) as proc_pool:
-                        # 这里如果直接使用fetch_history_table_data会导致程序无法运行，原因不明，目前只能默认通过tushare接口获取数据
-                        #  通过TABLE_MASTERS获取tushare接口名称，并通过acquire_data直接通过tushare的API获取数据
+                    with ThreadPoolExecutor(max_workers=process_count) as worker:
+                        '''
+                        这里如果直接使用fetch_history_table_data会导致程序无法运行，原因不明，目前只能默认通过tushare接口获取数据
+                        通过TABLE_MASTERS获取tushare接口名称，并通过acquire_data直接通过tushare的API获取数据
+                        '''
                         api_name = TABLE_MASTERS[table][TABLE_MASTER_COLUMNS.index('tushare')]
-                        futures = {proc_pool.submit(acquire_data, api_name, **kw): kw
-                                   for kw in all_kwargs}
+                        futures = {}
+                        submitted = 0
+                        for kw in all_kwargs:
+                            futures.update({worker.submit(acquire_data, api_name, **kw): kw})
+                            submitted += 1
+                            if (download_batch_interval != 0) and (submitted % download_batch_size == 0):
+                                progress_bar(submitted, total, f'<{table}>: Submitting tasks, '
+                                                               f'Pausing for {download_batch_interval} sec...')
+                                time.sleep(download_batch_interval)
+                        # futures = {worker.submit(acquire_data, api_name, **kw): kw
+                        #            for kw in all_kwargs}
+                        progress_bar(0, total, f'<{table}>: estimating time left...')
                         for f in as_completed(futures):
                             df = f.result()
                             cur_kwargs = futures[f]
                             completed += 1
                             if completed % chunk_size:
                                 dnld_data = pd.concat([dnld_data, df])
                             else:
@@ -5088,36 +5138,43 @@
                                 rows_affected = self.update_table_data(table, dnld_data)
                                 dnld_data = pd.DataFrame()
                             total_written += rows_affected
                             time_elapsed = time.time() - st
                             time_remain = sec_to_duration((total - completed) * time_elapsed / completed,
                                                           estimation=True, short_form=False)
                             progress_bar(completed, total, f'<{table}:{list(cur_kwargs.values())[0]}>'
-                                                           f'{total_written}wrtn/{time_remain}left')
+                                                           f'{total_written}wrtn/{time_remain} left')
 
                         total_written += self.update_table_data(table, dnld_data)
                 else:
+                    progress_bar(0, total, f'<{table}:{all_kwargs}> estimating time left...')
                     for kwargs in all_kwargs:
-                        df = self.fetch_history_table_data(table, **kwargs)
+                        df = self.fetch_history_table_data(table, channel='tushare', **kwargs)
                         completed += 1
                         if completed % chunk_size:
                             dnld_data = pd.concat([dnld_data, df])
                         else:
                             dnld_data = pd.concat([dnld_data, df])
                             rows_affected = self.update_table_data(table, dnld_data)
                             dnld_data = pd.DataFrame()
                         total_written += rows_affected
                         time_elapsed = time.time() - st
                         time_remain = sec_to_duration(
                                 (total - completed) * time_elapsed / completed,
                                 estimation=True,
                                 short_form=False
                         )
-                        progress_bar(completed, total, f'<{table}:{list(kwargs.values())[0]}>'
-                                                       f'{total_written}wrtn/{time_remain}left')
+                        if (download_batch_interval != 0) and (completed % download_batch_size == 0):
+                            progress_bar(completed, total, f'<{table}:{list(kwargs.values())[0]}>'
+                                                           f'{total_written}wrtn/Pausing for '
+                                                           f'{download_batch_interval} sec...')
+                            time.sleep(download_batch_interval)
+                        else:
+                            progress_bar(completed, total, f'<{table}:{list(kwargs.values())[0]}>'
+                                                           f'{total_written}wrtn/{time_remain} left')
                     total_written += self.update_table_data(table, dnld_data)
                 strftime_elapsed = sec_to_duration(
                         time_elapsed,
                         estimation=True,
                         short_form=True
                 )
                 if len(arg_coverage) > 1:
@@ -5128,16 +5185,14 @@
                                                f'{total_written}wrtn in {strftime_elapsed}\n')
             except Exception as e:
                 total_written += self.update_table_data(table, dnld_data)
                 msg = f'\n{str(e)}: \ndownload process interrupted at [{table}]:' \
                               f'<{arg_coverage[0]}>-<{arg_coverage[completed - 1]}>\n' \
                               f'{total_written} rows downloaded, will proceed with next table!'
                 warnings.warn(msg)
-                # progress_bar(completed, total, f'[Interrupted! {table}] <{arg_coverage[0]} to {arg_coverage[-1]}>:'
-                #                                f'{total_written} written in {sec_to_duration(time_elapsed)}\n')
 
     def get_all_basic_table_data(self, refresh_cache=False, raise_error=True):
         """ 一个快速获取所有basic数据表的函数，通常情况缓存处理以加快速度
         如果设置refresh_cache为True，则清空缓存并重新下载数据
 
         Parameters
         ----------
```

### Comparing `qteasy-1.1.9/qteasy/emfuncs.py` & `qteasy-1.2.0/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/evaluate.py` & `qteasy-1.2.0/qteasy/evaluate.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/finance.py` & `qteasy-1.2.0/qteasy/finance.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/history.py` & `qteasy-1.2.0/qteasy/history.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/optimization.py` & `qteasy-1.2.0/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/qt_operator.py` & `qteasy-1.2.0/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/space.py` & `qteasy-1.2.0/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/strategy.py` & `qteasy-1.2.0/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/tafuncs.py` & `qteasy-1.2.0/qteasy/tafuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/trade_recording.py` & `qteasy-1.2.0/qteasy/trade_recording.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,23 +1177,23 @@
     data_source: str, optional
         数据源的名称, 默认为None, 表示使用默认的数据源
 
     Returns
     -------
     trade_results: pd.DataFrame, columns=['order_id', 'filled_qty', 'price', 'transaction_fee', 'execution_time',
                         'canceled_qty', 'delivery_amount', 'delivery_status']
-    交易结果:
-    order_id: int 交易信号的id
-    filled_qty: int 成交数量
-    price: float 成交价格
-    transaction_fee: float 交易费用
-    execution_time: datetime.datetime 成交时间
-    canceled_qty: int 撤单数量
-    delivery_amount: float 交割金额
-    delivery_status: str 交割状态
+    交易结果, 包含以下列:
+        - order_id: int 交易信号的id
+        - filled_qty: int 成交数量
+        - price: float 成交价格
+        - transaction_fee: float 交易费用
+        - execution_time: datetime.datetime 成交时间
+        - canceled_qty: int 撤单数量
+        - delivery_amount: float 交割金额
+        - delivery_status: str 交割状态
     """
     if not isinstance(order_id, (int, np.int64, np.ndarray, list, )):
         raise TypeError(f'order_id must be an integer, a list of integers or a numpy array of integers, '
                         f'got {type(order_id)} instead')
     if isinstance(order_id, np.ndarray):
         order_id = order_id.tolist()
     if isinstance(order_id, list):
```

### Comparing `qteasy-1.1.9/qteasy/trading_util.py` & `qteasy-1.2.0/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy/tsfuncs.py` & `qteasy-1.2.0/qteasy/tsfuncs.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,34 +11,54 @@
 import pandas as pd
 import tushare as ts
 
 from qteasy import logger_core, QT_CONFIG
 from .utilfuncs import regulate_date_format, list_to_str_format
 from .utilfuncs import retry
 
-data_download_retry_count = QT_CONFIG.hist_dnld_retry_cnt
-data_download_retry_wait = QT_CONFIG.hist_dnld_retry_wait
-data_download_retry_backoff = QT_CONFIG.hist_dnld_backoff
 
-# ERRORS_TO_CHECK_ON_RETRY = (ConnectionError, ConnectionResetError, RuntimeError,
-#                             BlockingIOError, ProxyError, Exception)
 ERRORS_TO_CHECK_ON_RETRY = Exception
 
+EXTRA_RETRY_API = [
+    'name_change',
+    'stk_managers',
+    'daily_basic',
+    'index_daily',
+    'options_daily',
+    'fund_share',
+    'fund_manager',
+    'hibor',
+    'libor',
+]
+
 
 # tsfuncs interface function, call this function to extract data
 def acquire_data(api_name, **kwargs):
     """ DataSource模块的接口函数，根据根据table的内容调用相应的tushare API下载数据，并以DataFrame的形式返回数据"""
+    data_download_retry_count = QT_CONFIG.hist_dnld_retry_cnt
+    data_download_retry_wait = QT_CONFIG.hist_dnld_retry_wait
+    data_download_retry_backoff = QT_CONFIG.hist_dnld_backoff
+
+    if api_name in EXTRA_RETRY_API:
+        data_download_retry_count += 3
+
+    retry_decorator = retry(
+            exception_to_check=ERRORS_TO_CHECK_ON_RETRY,
+            mute=True,
+            tries=data_download_retry_count,
+            delay=data_download_retry_wait,
+            backoff=data_download_retry_backoff,
+            logger=logger_core,
+    )
     func = globals()[api_name]
-    res = func(**kwargs)
+    decorated_func = retry_decorator(func)
+    res = decorated_func(**kwargs)
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
 def stock_basic(exchange: str = None):
     """ 获取基础信息数据，包括股票代码、名称、上市日期、退市日期等
 
     Parameters
     ----------
     optional, 交易所 SSE上交所 SZSE深交所 HKEX港交所(未上线)
 
@@ -74,17 +94,15 @@
                           fields=fields)
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stock_basic with exchange={exchange}, list_status={list_status}'
                      f'is_hs={is_hs}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def trade_calendar(exchange: str = 'SSE',
                    start: str = None,
                    end: str = None,
                    is_open: int = None):
     """ 获取各大交易所交易日历数据,默认提取的是上交所
         如果不指定is_open，则返回包含所有日期以及is_open代码的DataFrame
         如果指定is_open == 0 或者 1， 则返回相应的日期列表
@@ -119,17 +137,14 @@
                      f'end_date={end}, is_open={is_open}')
     if is_open is None:
         return trade_cal
     else:
         return list(pd.to_datetime(trade_cal.cal_date))
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count + 3, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
 def name_change(ts_code: str = None,
                 start: str = None,
                 end: str = None):
     """ 历史名称变更记录
 
     Parameters
     ----------
@@ -173,17 +188,15 @@
                          fields=fields)
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table name_change with ts_code={ts_code}, start_date={start}'
                      f'end_date={end}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def new_share(start: str = None,
               end: str = None) -> pd.DataFrame:
     """ 新股上网发行列表
 
     Parameters
     ----------
     start: str, 上网发行开始日期
@@ -245,17 +258,15 @@
     res = pro.new_share(start_date=start, end_date=end)
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table new_share with start_date={start}'
                      f'end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def stock_company(ts_code: str = None,
                   exchange: str = None,
                   fields: str = None) -> pd.DataFrame:
     """ 获取上市公司基本信息
 
     Parameters
     ----------
@@ -308,17 +319,14 @@
     res = pro.stock_company(ts_code=ts_code, exchange=exchange, fields=fields)
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stock_company with ts_code={ts_code}, exchange={exchange}'
                      f'fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count + 3, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
 def stk_managers(ts_code: str = None,
                  ann_date: str = None,
                  start: str = None,
                  end: str = None) -> pd.DataFrame:
     """ 获取上市公司高管持股变动情况
 
     Parameters
@@ -368,17 +376,15 @@
                      f' table stk_managers with ts_code={ts_code}, ann_date={ann_date}'
                      f' start={start}, end={end}')
     return res
 
 
 # Bar price data
 # ==================
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count + 3, delay=1,
-       backoff=2., logger=logger_core)
+
 def daily_basic(ts_code: object = None,
                 trade_date: object = None,
                 start: object = None,
                 end: object = None) -> pd.DataFrame:
     """ 获取个股行情 (日线)
     TODO: 以下字段需要进一步确认
     Parameters
@@ -433,17 +439,14 @@
                           end_date=end)
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table daily_basic with ts_code={ts_code}, trade_date={trade_date}'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=1.,
-       backoff=2., logger=logger_core)
 def daily_basic2(ts_code: object = None,
                  trade_date: object = None,
                  start: object = None,
                  end: object = None) -> pd.DataFrame:
     """ 获取个股行情
 
     Parameters
@@ -488,17 +491,15 @@
                         end_date=end)
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table back_basic with ts_code={ts_code}, trade_date={trade_date}'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def index_daily_basic(ts_code: object = None,
                       trade_date: object = None,
                       start: object = None,
                       end: object = None) -> pd.DataFrame:
     """ 获取指数行情
 
     Parameters
@@ -552,168 +553,146 @@
     pro = ts.pro_api()
     res = pro.rt_min(ts_code=ts_code, freq=freq)
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stk_mins with ts_code={ts_code}, freq={freq}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def mins1(ts_code,
           start=None,
           end=None):
     # 注意，分钟接口minsxx包含股票、基金、指数、期权的分钟数据，全部都在一张表中，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.stk_mins(ts_code=ts_code, start_date=start, end_date=end, freq='1min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stk_mins with ts_code={ts_code}, freq="1min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def mins5(ts_code,
           start=None,
           end=None):
     # 注意，分钟接口minsxx包含股票、基金、指数、期权的分钟数据，全部都在一张表中，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.stk_mins(ts_code=ts_code, start_date=start, end_date=end, freq='5min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stk_mins with ts_code={ts_code}, freq="5min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def mins15(ts_code,
            start=None,
            end=None):
     # 注意，分钟接口minsxx包含股票、基金、指数、期权的分钟数据，全部都在一张表中，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.stk_mins(ts_code=ts_code, start_date=start, end_date=end, freq='15min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stk_mins with ts_code={ts_code}, freq="15min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def mins30(ts_code,
            start=None,
            end=None):
     # 注意，分钟接口minsxx包含股票、基金、指数、期权的分钟数据，全部都在一张表中，必须先获取权限后下载
     pro = ts.pro_api()
     ts.pro_bar()
     res = pro.stk_mins(ts_code=ts_code, start_date=start, end_date=end, freq='30min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stk_mins with ts_code={ts_code}, freq="30min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def mins60(ts_code,
            start=None,
            end=None):
     # 注意，分钟接口minsxx包含股票、基金、指数、期权的分钟数据，全部都在一张表中，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.stk_mins(ts_code=ts_code, start_date=start, end_date=end, freq='60min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table stk_mins with ts_code={ts_code}, freq="60min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def ft_mins1(ts_code,
              start=None,
              end=None):
     # 注意，分钟接口ft_minsxx包含期货的分钟数据，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.ft_mins(ts_code=ts_code, start_date=start, end_date=end, freq='1min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table future_mins with ts_code={ts_code}, freq="1min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def ft_mins5(ts_code,
              start=None,
              end=None):
     # 注意，分钟接口ft_minsxx包含期货的分钟数据，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.ft_mins(ts_code=ts_code, start_date=start, end_date=end, freq='5min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table future_mins with ts_code={ts_code}, freq="5min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def ft_mins15(ts_code,
               start=None,
               end=None):
     # 注意，分钟接口ft_minsxx包含期货的分钟数据，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.ft_mins(ts_code=ts_code, start_date=start, end_date=end, freq='15min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table future_mins with ts_code={ts_code}, freq="15min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def ft_mins30(ts_code,
               start=None,
               end=None):
     # 注意，分钟接口ft_minsxx包含期货的分钟数据，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.ft_mins(ts_code=ts_code, start_date=start, end_date=end, freq='30min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table future_mins with ts_code={ts_code}, freq="30min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def ft_mins60(ts_code,
               start=None,
               end=None):
     # 注意，分钟接口ft_minsxx包含期货的分钟数据，必须先获取权限后下载
     pro = ts.pro_api()
     res = pro.ft_mins(ts_code=ts_code, start_date=start, end_date=end, freq='60min')
     logger_core.info(f'downloaded {len(res)} rows of data from tushare'
                      f' table future_mins with ts_code={ts_code}, freq="60min"'
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def daily(ts_code=None,
           trade_date=None,
           start=None,
           end=None):
     """
 
     ts_code:
@@ -727,17 +706,15 @@
     pro = ts.pro_api()
     res = pro.daily(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: daily with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def weekly(ts_code=None,
            trade_date=None,
            start=None,
            end=None):
     """
 
     ts_code:
@@ -751,17 +728,15 @@
     pro = ts.pro_api()
     res = pro.weekly(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: weekly with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def monthly(ts_code=None,
             trade_date=None,
             start=None,
             end=None):
     """
 
     ts_code:
@@ -775,17 +750,14 @@
     pro = ts.pro_api()
     res = pro.monthly(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: monthly with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count + 3, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
 def index_daily(ts_code=None,
                 trade_date=None,
                 start=None,
                 end=None):
     """
 
     ts_code:
@@ -799,17 +771,15 @@
     pro = ts.pro_api()
     res = pro.index_daily(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: index_daily with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def index_weekly(ts_code=None,
                  trade_date=None,
                  start=None,
                  end=None):
     """
 
     ts_code:
@@ -823,17 +793,15 @@
     pro = ts.pro_api()
     res = pro.index_weekly(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: index_weekly with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def index_monthly(ts_code=None,
                   trade_date=None,
                   start=None,
                   end=None):
     """
 
     ts_code:
@@ -847,17 +815,15 @@
     pro = ts.pro_api()
     res = pro.index_monthly(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: index_monthly with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def fund_daily(ts_code=None,
                trade_date=None,
                start=None,
                end=None):
     """
 
     ts_code:
@@ -871,17 +837,15 @@
     pro = ts.pro_api()
     res = pro.fund_daily(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: fund_daily with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def adj_factors(ts_code=None,
                 trade_date=None,
                 start=None,
                 end=None):
     """
 
     ts_code:
@@ -895,17 +859,15 @@
     pro = ts.pro_api()
     res = pro.adj_factor(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: adj_factors with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def fund_adj(ts_code=None,
              trade_date=None,
              start=None,
              end=None):
     """
 
     ts_code:
@@ -919,17 +881,15 @@
     pro = ts.pro_api()
     res = pro.fund_adj(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: fund_adj with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def fund_share(ts_code=None,
                trade_date=None,
                start=None,
                end=None):
     """
 
     ts_code: 基金代码，支持多只基金同时提取，用逗号分隔
@@ -943,17 +903,15 @@
     pro = ts.pro_api()
     res = pro.fund_share(ts_code=ts_code, trade_date=trade_date, start_date=start, end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: fund_share with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def fund_manager(ts_code=None,
                  ann_date=None,
                  offset=None):
     """
 
     ts_code: 基金代码，支持多只基金同时提取，用逗号分隔
     ann_date:  公告日期，格式YYYYMMDD
@@ -967,17 +925,15 @@
     logger_core.info(f'Downloaded {len(res)} rows from tushare: fund_manager with ts_code={ts_code}, '
                      f'ann_date={ann_date}, offset={offset}')
     return res
 
 
 # Finance Data
 # ================
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def income(ts_code: str,
            rpt_date: str = None,
            start: str = None,
            end: str = None,
            period: str = None,
            report_type: str = None,
            comp_type: str = None,
@@ -1128,17 +1084,15 @@
                          fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: income with ts_code={ts_code}, '
                      f'ann_date={rpt_date}, start_date={start}, end_date={end}, period={period}, '
                      f'report_type={report_type}, comp_type={comp_type}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def balance(ts_code: str,
             rpt_date: str = None,
             start: str = None,
             end: str = None,
             period: str = None,
             report_type: str = None,
             comp_type: str = None,
@@ -1379,17 +1333,15 @@
                                fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: balance with ts_code={ts_code}, '
                      f'ann_date={rpt_date}, start_date={start}, end_date={end}, period={period}, '
                      f'report_type={report_type}, comp_type={comp_type}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def cashflow(ts_code: str,
              rpt_date: str = None,
              start: str = None,
              end: str = None,
              period: str = None,
              report_type: str = None,
              comp_type: str = None,
@@ -1576,17 +1528,15 @@
                            fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: cashflow with ts_code={ts_code}, '
                      f'ann_date={rpt_date}, start_date={start}, end_date={end}, period={period}, '
                      f'report_type={report_type}, comp_type={comp_type}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def indicators(ts_code: str,
                rpt_date: str = None,
                start: str = None,
                end: str = None,
                period: str = None,
                fields: [str, list] = None) -> pd.DataFrame:
     """ 获取上市公司财务数据——财务指标
@@ -1836,17 +1786,15 @@
                                  period=period,
                                  fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: indicators with ts_code={ts_code}, '
                      f'ann_date={rpt_date}, start_date={start}, end_date={end}, period={period}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def forecast(ts_code: str = None,
              ann_date: str = None,
              start: str = None,
              end: str = None,
              period: str = None,
              type: str = None):
     """ 获取上市公司的业绩预报
@@ -1905,17 +1853,15 @@
                            fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: forecast with ts_code={ts_code}, '
                      f'ann_date={ann_date}, start_date={start}, end_date={end}, period={period}, '
                      f'type={type}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def express(ts_code: str = None,
             ann_date: str = None,
             start: str = None,
             end: str = None,
             period: str = None):
     """ 获取上市公司的业绩快报
 
@@ -1994,17 +1940,15 @@
     logger_core.info(f'Downloaded {len(res)} rows from tushare: express with ts_code={ts_code}, '
                      f'ann_date={ann_date}, start_date={start}, end_date={end}, period={period}')
     return res
 
 
 # Market Data
 # =================
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def top_list(trade_date: str = None,
              shares: str = None,
              fields: str = None) -> pd.DataFrame:
     """ 龙虎榜每日交易明细，2005年至今全部历史数据，单次获取数量不超过10000
 
     Parameters
     ----------
@@ -2054,17 +1998,15 @@
     logger_core.info(f'Downloaded {len(res)} rows from tushare: top_list with ts_code={shares}, '
                      f'trade_date={trade_date}, fields={fields}')
     return res
 
 
 # Index Data
 # ==================
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def index_basic(ts_code: str = None,
                 name: str = None,
                 market: str = None,
                 publisher: str = None,
                 category: str = None) -> pd.DataFrame:
     """ 获取大盘指数的基本信息如名称代码等
 
@@ -2135,17 +2077,15 @@
                           category=category,
                           fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: index_basic with ts_code={ts_code}, '
                      f'name={name}, market={market}, publisher={publisher}, category={category}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def index_indicators(trade_date: str = None,
                      ts_code: str = None,
                      start: str = None,
                      end: str = None,
                      fields: str = None) -> pd.DataFrame:
     """ 大盘指数每日指标如市盈率等, 目前只提供上证综指，深证成指，上证50，中证500，中小板指，创业板指的每日指标数据
         支持两三种数据获取方式：
@@ -2200,17 +2140,15 @@
                                end_date=end,
                                fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: index_indicators with ts_code={ts_code}, '
                      f'trade_date={trade_date}, start_date={start}, end_date={end}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def composite(index: str = None,
               trade_date: str = None,
               start: str = None,
               end: str = None) -> pd.DataFrame:
     """ 获取各类指数成分和权重，月度数据 ，如需日度指数成分和权重，请联系 waditu@163.com
 
     Parameters
@@ -2251,17 +2189,15 @@
                      f'trade_date={trade_date}, start_date={start}, end_date={end}')
     return res
 
 
 # Funds Data
 # =============
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def fund_basic(market: str = None,
                status: str = None) -> pd.DataFrame:
     """ 获取基金列表
 
     Parameters
     ----------
     market: str, 交易市场: E场内 O场外（默认E）
@@ -2319,17 +2255,15 @@
     pro = ts.pro_api()
     res = pro.fund_basic(market=market, status=status)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: fund_basic with market={market}, '
                      f'status={status}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def fund_net_value(ts_code: str = None,
                    nav_date: str = None,
                    market: str = None) -> pd.DataFrame:
     """ 获取公募基金净值数据
 
     Parameters
     ----------
@@ -2371,17 +2305,15 @@
                      f'nav_date={nav_date}, market={market}')
     return res
 
 
 # Futures & Options Data
 # ===============
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def future_basic(exchange: str = None,
                  future_type: str = None) -> pd.DataFrame:
     """ 获取期货合约列表数据
 
     Parameters
     ----------
     exchange: str, 交易所代码 CFFEX-中金所 DCE-大商所 CZCE-郑商所 SHFE-上期所 INE-上海国际能源交易中心
@@ -2430,17 +2362,15 @@
                         fut_type=future_type,
                         fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: future_basic with exchange={exchange}, '
                      f'fut_type={future_type}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def options_basic(exchange: str = None,
                   call_put: str = None) -> pd.DataFrame:
     """ 获取期权合约信息
 
     Parameters
     ----------
     exchange: str, 交易所代码 CFFEX-中金所 DCE-大商所 CZCE-郑商所 SHFE-上期所 INE-上海国际能源交易中心
@@ -2488,17 +2418,14 @@
                         call_put=call_put,
                         fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: options_basic with exchange={exchange}, '
                      f'call_put={call_put}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
 def future_daily(trade_date: str = None,
                  future: str = None,
                  exchange: str = None,
                  start: str = None,
                  end: str = None) -> pd.DataFrame:
     """ 期货日线行情数据
 
@@ -2553,17 +2480,14 @@
                         end_date=end,
                         fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: future_daily with trade_date={trade_date}, '
                      f'ts_code={future}, exchange={exchange}, start_date={start}, end_date={end}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count + 3, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)  # 接口有访问次数限制，因此增加delay
 def options_daily(trade_date: str = None,
                   option: str = None,
                   exchange: str = None,
                   start: str = None,
                   end: str = None) -> pd.DataFrame:
     """ 获取期权日线行情
 
@@ -2624,17 +2548,15 @@
                         fields=fields)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: options_daily with '
                      f'trade_date={trade_date}, ts_code={option}, exchange={exchange}, start_date={start}, '
                      f'end_date={end}, fields={fields}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
+
 def shibor(date=None, start=None, end=None):
     """ 获取上海银行间同业拆借利率SHIBOR利率
 
     Parameters
     ----------
     date: str 利率日期
     start: str 开始日期
@@ -2685,17 +2607,14 @@
                      start_date=start,
                      end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: shibor with date={date}, '
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count + 3, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
 def hibor(date=None, start=None, end=None):
     """ 获取HIBOR (Hongkong InterBank Offered Rate)，香港银行同行业拆借利率
 
     Parameters
     ----------
     date: str 利率日期
     start: str 开始日期
@@ -2746,17 +2665,14 @@
                     start_date=start,
                     end_date=end)
     logger_core.info(f'Downloaded {len(res)} rows from tushare: hibor with date={date}, '
                      f'start_date={start}, end_date={end}')
     return res
 
 
-@retry(exception_to_check=ERRORS_TO_CHECK_ON_RETRY, mute=True,
-       tries=data_download_retry_count + 3, delay=data_download_retry_wait,
-       backoff=data_download_retry_backoff, logger=logger_core)
 def libor(date=None, start=None, end=None, currency=None):
     """ 获取上海银行间同业拆借利率SHIBOR利率
 
     Parameters
     ----------
     date: str 利率日期
     start: str 开始日期
```

### Comparing `qteasy-1.1.9/qteasy/utilfuncs.py` & `qteasy-1.2.0/qteasy/utilfuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 # Contact:  jackie.pengzhao@gmail.com
 # Created:  2020-02-21
 # Desc:
 #   Commonly used utility functions.
 # ======================================
 
 import argparse
-import numpy as np
-import pandas as pd
-import sys
 import re
-import qteasy
+import shutil
+import sys
 import time
 import warnings
+import numpy as np
+import pandas as pd
+
 from numba import njit
 from functools import wraps, lru_cache
 
+import qteasy
+
 TIME_FREQ_LEVELS = {
     'Y':      10,
     'Q':      20,
     'M':      30,
     'W':      40,
     'D':      50,
     'H':      60,
@@ -92,14 +95,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument('-a', '--account', type=int, help='start trader with the given account id')
     parser.add_argument('-n', '--new_account', type=str, default=None,
                         help='if set, create a new account with the given user name')
     parser.add_argument('-r', '--restart', action='store_true', default=False,
                         help='if set, remove all record and restart account')
     parser.add_argument('-d', '--debug', action='store_true', help='if set, start trader in debug mode')
+    parser.add_argument('-u', '--ui', action='store_true', default=False, help='if True, start trader in terminal ui')
 
     return parser
 
 
 def freq_dither(freq, freq_list):
     """ 频率抖动，将一个目标频率抖动到频率列表中的一个频率上，
 
@@ -261,15 +265,15 @@
             target_pos += 1
         elif direction == 'down':
             target_pos -= 1
         if get_main_freq_level(target_freq) != level:
             return target_freq
 
 
-def retry(exception_to_check, tries=3, delay=1, backoff=2., mute=False, logger=None):
+def retry(exception_to_check, tries=3, delay=1., backoff=2., mute=False, logger=None):
     """一个装饰器，当被装饰的函数抛出异常时，反复重试直至次数耗尽，重试前等待并延长等待时间.
 
     Parameters
     ----------
     exception_to_check: Exception 或 tuple
         需要检测的异常，当发生此异常时重试，可以用tuple给出多个异常
     tries: int
@@ -289,15 +293,14 @@
         @wraps(f)
         def f_retry(*args, **kwargs):
             mtries, mdelay = tries, delay
             while mtries > 1:
                 try:
                     return f(*args, **kwargs)
                 except exception_to_check as e:
-                    # TODO: define the error to escape retry: no permission, no such file, etc.
                     exception_to_escape = [ValueError, TypeError, AttributeError, FileNotFoundError, PermissionError,]
                     error_str = str(e)
                     if ('没有访问该接口的权限' in error_str) or ('api init error' in error_str):
                         raise e
                     if e.__class__ in exception_to_escape:
                         raise e
                     msg = f'Error in {f.__name__}: {e.__class__}:{str(e)}, Retrying in {mdelay} seconds...'
@@ -763,39 +766,42 @@
     prog: int
         当前进度，用整数表示
     total: int
         总体进度，默认为100
     comments: str, optional
         需要显示在进度条中的文字信息
     """
+    column_width, _ = shutil.get_terminal_size()
+
     if total > 0:
         if prog > total:
             prog = total
         progress_str = f'\r \r[{PROGRESS_BAR[int(prog / total * 40)]}]' \
                        f'{prog}/{total}-{np.round(prog / total * 100, 1)}%  {comments}'
+        progress_str = adjust_string_length(progress_str, column_width)
         sys.stdout.write(progress_str)
         sys.stdout.flush()
 
 
-def get_current_tz_datetime(self, time_zone='local'):
+def get_current_timezone_datetime(time_zone='local'):
     """ 获取指定时区的当前时间，同时确保返回的时间是tz_naive的
 
     如果time_zone为'local', 获取当前时区的当前时间。
     如果指定time_zone的时间与本地时间相同，则直接返回当前时间
 
     Parameters
     ----------
     time_zone: str, default: 'local'
         符合标准的时区字符串
     """
     if time_zone == 'local':
         return pd.to_datetime('today')
     else:
         # create utc time and convert to time_zone time and remove time_zone information
-        dt = pd.to_datetime('now', utc=True).tz_convert(self.time_zone)
+        dt = pd.to_datetime('now', utc=True).tz_convert(time_zone)
         return pd.to_datetime(dt.tz_localize(None))
 
 
 @lru_cache(maxsize=16)
 def maybe_trade_day(date):
     """ 判断一个日期是否交易日（或然判断，只剔除明显不是交易日的日期）准确率有限但是效率高
 
@@ -1896,15 +1902,15 @@
         raise ValueError(f'num_spaces should be larger than 0 and smaller or equal to 50, got {num_spaces}')
     s = s.split('\n')
     s = [(num_spaces * ' ') + line.lstrip() for line in s]
     s = '\n'.join(s)
     return s
 
 
-def truncate_string(s, n, padder='.'):  # to be deprecated
+def truncate_string(s, n, padder='.') -> str:  # to be deprecated
     """ to be deprecated, 调整字符串为指定长度，为了保证兼容性，暂时保留此函数
     以后使用adjust_string_length代替
 
     Parameters
     ----------
     s: str
         字符串
@@ -1926,15 +1932,15 @@
     >>> truncate_string('hello world', 3)
     'h..'
     """
     warnings.warn('truncate_string will be deprecated, use adjust_string_length instead', DeprecationWarning)
     return adjust_string_length(s, n, ellipsis=padder)
 
 
-def adjust_string_length(s, n, ellipsis='.', padder=' ', hans_aware=False, padding='right', format_tags=False):
+def adjust_string_length(s, n, ellipsis='.', padder=' ', hans_aware=False, padding='right', format_tags=False) -> str:
     """ 调整字符串为指定长度，如果字符串过长则将其截短，并在末尾添加省略号提示，
         如果字符串过短则在末尾添加空格补齐长度
 
     默认情况下，认为汉字的长度为2，英文字符的长度为1，可以通过hans_aware参数设置是否考虑汉字的长度
     如果字符串中含有格式标签，如[bold]或[red]，则需要将format_tags参数设置为True，此时会先将格式标签去除，
     然后调整字符串长度，调整完成后再将格式标签添加回去
```

### Comparing `qteasy-1.1.9/qteasy/visual.py` & `qteasy-1.2.0/qteasy/visual.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/qteasy.egg-info/PKG-INFO` & `qteasy-1.2.0/qteasy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.9
+Version: 1.2.0
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -37,18 +37,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.6
+Requires-Python: <3.13,>=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: talib
 Provides-Extra: database
-Provides-Extra: hdf
 Provides-Extra: feather
 License-File: LICENSE
 
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
@@ -92,15 +92,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.9`
+- Latest Version: `1.2.0`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
@@ -128,17 +128,17 @@
 ### **实盘交易模拟**
 - 读取实时市场数据，实盘运行交易策略
 - 生成交易信号，模拟交易结果
 - 跟踪记录交易日志、股票持仓、账户资金变化等信息
 - 随时查看交易过程，检查盈亏情况
 - 手动控制交易进程、调整交易参数，手动下单
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_2.png)  
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_1.png)  
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png)  
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
 
 ## 安装
 
 ```bash
 $ pip install qteasy
 ```
 
@@ -148,18 +148,36 @@
 
 
 ### python 版本
 - *`python` version >= 3.6, < 3.13* 
 
 ### 安装可选依赖包
 
-`qteasy`所有必要的依赖包都可以在pip安装的同时安装好，但如果需要使用`qteasy`的全部功能，需要安装以下依赖包：
+`qteasy`所有必要的依赖包都可以在`pip`安装的同时安装好，但某些特殊情况下，您需要在安装时指定可选依赖包，以便在安装`qteasy`时同时安装，或者手动安装依赖包：
 
-- **`ta-lib`**, 以便使用所有的内置交易策略
-- **`pymysql`**, 用于连接MySQL数据库,将本地数据存储到MySQL数据库（qteasy默认使用csv文件作为本地数据源，但数据量大时推荐使用mysql数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+- **`pymysql`**, 用于连接`MySQL`数据库,将本地数据存储到`MySQL`数据库（`qteasy`默认使用`csv`文件作为本地数据源，但数据量大时推荐使用`mysql`数据库，详情参见[qteasy使用教程](https://qteasy.readthedocs.io)）
+`pymysql`可以在安装`qteasy`时自动安装，也可以手动安装：
+    ```bash
+    $ pip install 'qteasy[database]'  # 安装qteasy时自动安装pymysql
+    $ pip install pymysql  # 手动安装pymysql
+    ```
+- **`pyarrow`**, 用于操作`feather`文件，将本地数据存储为`feather`文件，`pyarrow`可以在安装`qteasy`时自动安装，也可以手动安装：
+    ```bash
+    $ pip install 'qteasy[feather]'  # 安装qteasy时自动安装pyarrow
+    $ pip install pyarrow  # 手动安装pyarrow
+    ```
+- **`pytables`**, 用于操作`HDF`文件，将本地数据存储到`HDF`文件，`pytables`不能自动安装，需要使用`conda`手动安装`pytables`：
+    ```bash
+    $ conda install pytables  # 安装pytables
+    ```
+- **`ta-lib`**, 以便使用所有的内置交易策略，下面的方法可以安装`ta-lib API`，但它还依赖C语言的`TA-Lib`包，安装方法请参考[FAQ](https://qteasy.readthedocs.io/zh/latest/faq.html#id2)
+    ```bash
+    $ pip install 'qteasy[talib]'  # 安装qteasy时自动安装ta-lib
+    $ pip install ta-lib  # 手动安装ta-lib
+    ```
 
 ##  10分钟了解qteasy的功能
 
 ### 导入`qteasy`
 基本的模块导入方法如下
 
 ```python
@@ -554,44 +572,19 @@
         sell_batch_size=1,  # 卖出数量为1股的整数倍
         live_trade_account_id=1,  # 实盘交易账户ID
         live_trade_account='user name',  # 实盘交易用户名
 )
 
 qt.run(op)
 ```
-此时`qteasy`会启动一个`Trader Shell`命令行界面，同时交易策略会自动定时运行，运行的参数随`QT_CONFIG`而定。启动TraderShell后，所有交易相关的重要信息都会显示在console中：
-
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)   
-
-此时控制台上会显示当前交易执行状态：
-- 当前日期、时间、运行状态
-- 产生的交易信号和交易订单
-- 交易订单的成交情况
-- 账户资金变动情况
-- 账户持仓变动情况
-- 开盘和收盘时间预告等
-
-在`TraderShell`运行过程中可以随时按`Ctrl+C`进入Shell选单：
-```commandline
-Current mode interrupted, Input 1 or 2 or 3 for below options: 
-[1], Enter command mode; 
-[2], Enter dashboard mode. 
-[3], Exit and stop the trader; 
-please input your choice: 
-```
+qteasy的实盘运行程序实际上是一个定时任务触发器，它能定时触发运行交易策略，提交策略到模拟交易Broker，并读取实时价格，模拟成交并自动记录交易过程。
 
-此时按1可以进入Interactive模式（交互模式）。在交互模式下，用户可以在(QTEASY)命令行提示符后输入
-命令来控制交易策略的运行：
+为了对策略运行过程进行监控，同时与qteasy进行互动，qteasy提供了两种不同的交互界面：
 
-![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_2.png)   
+- **`TraderShell`** 交互式命令行界面，可以在命令行中输入命令，查看交易日志、查看持仓、查看账户资金变化等信息：
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_1.png)  
 ![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/img/output_27_3.png) 
+- **`TraderApp`** (v1.2.0新增) 交互式图形界面，可以在图形界面中查看交易日志、查看持仓、查看账户资金变化等信息
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_light_theme.png) 
+![png](https://raw.githubusercontent.com/shepherdpp/qteasy/master/docs/source/examples/img/trader_app_2.png) 
 
-在命令行模式下可以与`TraderShell`实现交互，操作当前账户，查询交易历史、修改状态等：
-
-- `pause` / `resume`: 暂停/重新启动交易策略
-- `change`: 修改当前持仓和现金余额
-- `positions`: 查看当前持仓
-- `orders`: 查看当前订单
-- `history`: 查看历史交易记录
-- `exit`: 退出TraderShell
-- ... 更多`TraderShell`命令参见[`QTEASY`文档](https://qteasy.readthedocs.io)
-
+上面两种方式都可以在实盘运行时使用，根据qteasy的配置参数进入不同的交互界，关于更多实盘运行的介绍，请参见[`QTEASY`文档](https://qteasy.readthedocs.io)
```

### Comparing `qteasy-1.1.9/qteasy.egg-info/SOURCES.txt` & `qteasy-1.2.0/qteasy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 qteasy/optimization.py
 qteasy/qt_operator.py
 qteasy/space.py
 qteasy/strategy.py
 qteasy/tafuncs.py
 qteasy/trade_recording.py
 qteasy/trader.py
+qteasy/trader_cli.py
+qteasy/trader_tui.py
 qteasy/trading_util.py
 qteasy/tsfuncs.py
 qteasy/utilfuncs.py
 qteasy/visual.py
 qteasy.egg-info/PKG-INFO
 qteasy.egg-info/SOURCES.txt
 qteasy.egg-info/dependency_links.txt
@@ -47,10 +49,11 @@
 tests/test_operator_and_strategy.py
 tests/test_qt.py
 tests/test_space.py
 tests/test_ta_funcs.py
 tests/test_trader.py
 tests/test_trader_shell.py
 tests/test_trading.py
+tests/test_tui.py
 tests/test_tushare.py
 tests/test_utilityfuncs.py
 tests/test_visual.py
```

### Comparing `qteasy-1.1.9/setup.cfg` & `qteasy-1.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.1.9
+version = 1.2.0
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
@@ -39,18 +39,19 @@
 install_requires = 
 	pandas>=1.4.0
 	numpy>=1.18.1
 	numba>=0.47.0
 	tushare>=1.2.89
 	mplfinance
 	rich>=10.0.0
+	textual
 
 [options.extras_require]
+talib = ta-lib
 database = pymysql >= 1.0.0
-hdf = pytables >= 3.6.1
 feather = pyarrow >= 3
 
 [options.packages.find]
 where = qteasy
 
 [egg_info]
 tag_build =
```

### Comparing `qteasy-1.1.9/tests/test_broker.py` & `qteasy-1.2.0/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_cashplan.py` & `qteasy-1.2.0/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_config.py` & `qteasy-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_core_sub_funcs.py` & `qteasy-1.2.0/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_cost.py` & `qteasy-1.2.0/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_datasource.py` & `qteasy-1.2.0/tests/test_datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -2223,22 +2223,26 @@
                 self.assertIsNotNone(res)
                 for origin, read in zip(data.values(), res.values()):
                     print(f'origin: {origin}->{type(origin)}, read: {read}->{type(read)}')
                     if isinstance(origin, pd.Timestamp):
                         self.assertEqual(origin, pd.to_datetime(read))
                     else:
                         self.assertEqual(origin, read)
-                # if ds.table_data_exists(table):
-                #     ds.drop_table_data(table)
+                if ds.table_data_exists(table):
+                    ds.drop_table_data(table)
                 print(f'write and read shuffled data')
                 ds.insert_sys_table_data('sys_op_trade_orders', **test_shuffled_signal_data)
                 last_id = ds.get_sys_table_last_id('sys_op_trade_orders')
                 res = ds.read_sys_table_data('sys_op_trade_orders', record_id=last_id)
                 print(f'following data are read from table "sys_table_trade_signal" with id = {last_id}\n'
                       f'{res}\n')
+                if res is None:
+                    ids = ds.read_sys_table_data('sys_op_trade_orders').index.tolist()
+                    raise ValueError(f'here last_id is wrong if order ids are not continuous. now the ids are '
+                                     f'{ids}, the last id should be {ids[-1]}, but actually {last_id} is return')
                 self.assertIsNotNone(res)
                 self.assertEqual(test_shuffled_signal_data['pos_id'], res['pos_id'])
                 self.assertEqual(test_shuffled_signal_data['order_type'], res['order_type'])
                 self.assertEqual(test_shuffled_signal_data['status'], res['status'])
                 self.assertEqual(test_shuffled_signal_data['direction'], res['direction'])
                 self.assertEqual(test_shuffled_signal_data['price'], res['price'])
                 self.assertEqual(test_shuffled_signal_data['qty'], res['qty'])
@@ -2298,14 +2302,16 @@
                 for data in datas:
                     ds.insert_sys_table_data(table, **data)
                 id_to_read = int(np.random.randint(5, size=(1,)))
                 res = ds.read_sys_table_data(table, id_to_read + 1)
                 print(f'\nreading data with "id = {id_to_read}"...\n'
                       f'following data are read from table {table}\n'
                       f'{res}\n')
+                # if res is None:
+                #     import pdb; pdb.set_trace()
                 self.assertIsNotNone(res)
                 for origin, read in zip(datas[id_to_read].values(), res.values()):
                     print(f'origin: {origin}->{type(origin)}, read: {read}->{type(read)}')
                     if isinstance(origin, pd.Timestamp):
                         self.assertEqual(origin, pd.to_datetime(read))
                     else:
                         self.assertEqual(origin, read)
```

### Comparing `qteasy-1.1.9/tests/test_eastmoney.py` & `qteasy-1.2.0/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_evaluations.py` & `qteasy-1.2.0/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_fast_experiments.py` & `qteasy-1.2.0/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_historypanel.py` & `qteasy-1.2.0/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_loop.py` & `qteasy-1.2.0/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_operator_and_strategy.py` & `qteasy-1.2.0/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_qt.py` & `qteasy-1.2.0/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_space.py` & `qteasy-1.2.0/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_ta_funcs.py` & `qteasy-1.2.0/tests/test_ta_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_trader.py` & `qteasy-1.2.0/tests/test_trader.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,15 +754,15 @@
         """Test trader with simulated live trade task agenda"""
         # start the trader and broker in separate threads, set the trader to debug mode
         # and then manually generate task agenda and add task from agenda with twisted
         # current time, thus to test the trader in simulated real-time run.
 
         # 1, use trader._check_trade_day(sim_date) to simulate a trade day or non-trade day
         # 2, use trader._initialize_schedule(sim_time) to generate task agenda at a simulated time
-        # 3, use trader._add_task_from_agenda(sim_time) to add task from agenda at a simulated time
+        # 3, use trader._add_task_from_schedule(sim_time) to add task from agenda at a simulated time
 
         import datetime as dt
 
         ts = self.ts
         ts.debug = True
         ts.broker.debug = True
         ts.broker.broker_name = 'test_broker'
@@ -772,15 +772,15 @@
         broker_thread.start()
 
         # generate task agenda in a non-trade day and empty list will be generated
         sim_date = dt.date(2023, 1, 1)  # a non-trade day
         sim_time = dt.time(0, 0, 0)  # midnight
         ts._check_trade_day(sim_date)
         ts._initialize_schedule(sim_time)
-        ts._add_task_from_agenda(sim_time)
+        ts._add_task_from_schedule(sim_time)
 
         print('\n========generated task agenda in a non-trade day========\n')
         print(f'trader status: {ts.status}')
         print(f'broker status: {ts.broker.status}')
         print(f'is_trade_day: {ts.is_trade_day}')
         print(f'task daily agenda: {ts.task_daily_schedule}')
         self.assertEqual(ts.status, 'sleeping')
@@ -927,15 +927,15 @@
         # check all tasks are in the agenda
         for task, agenda_task in zip(target_agenda_tasks, ts.task_daily_schedule):
             self.assertEqual(task, agenda_task[1:])
         print('\n==========start simulation run, executing tasks from agenda============\n')
         for sim_time in test_sim_times:
             print(f'\n=========simulating time: {sim_time}=========\n')
             print(f'\n=========current task agenda: {ts.task_daily_schedule[0]}=========\n')
-            ts._add_task_from_agenda(sim_time)
+            ts._add_task_from_schedule(sim_time)
             # waite 1 second for orders to be generated
             time.sleep(2)
             print(f'current trader status: {ts.status}')
             print(f'current broker status: {ts.broker.status}')
             print(f'current cash and positions: \n{ts.account_positions}, \n{ts.account_cash}')
             print(f'count of trade orders in queue: {ts.broker.order_queue.unfinished_tasks} orders unprocessed')
             print(f'count of trade results in queue: {ts.broker.result_queue.unfinished_tasks} results generated')
```

### Comparing `qteasy-1.1.9/tests/test_trader_shell.py` & `qteasy-1.2.0/tests/test_trader_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # ======================================
 
 import unittest
 import time
 import pandas as pd
 
 from qteasy import DataSource, Operator
-from qteasy.trader import Trader, TraderShell
+from qteasy.trader import Trader
+from qteasy.trader_cli import TraderShell
 from qteasy.trading_util import process_account_delivery, process_trade_result, submit_order, update_position
 from qteasy.trade_recording import new_account, read_trade_order_detail, save_parsed_trade_orders
 from qteasy.trade_recording import get_or_create_position, get_position_by_id, get_account
 from qteasy.broker import SimulatorBroker
 
 
 class TestTraderShell(unittest.TestCase):
@@ -114,15 +115,21 @@
 
     def test_properties(self):
 
         tss = self.tss
 
         self.assertEqual(tss.trader, self.ts)
         self.assertEqual(tss.status, None)
-        self.assertEqual(tss.watch_list, ['000001.SH'])
+        self.assertEqual(tss.watch_list, ['000300.SH',
+                                          '000001.SZ',
+                                          '000002.SZ',
+                                          '000004.SZ',
+                                          '000005.SZ',
+                                          '000006.SZ',
+                                          '000007.SZ'])
 
     def test_command_status(self):
         """ test status command """
         tss = self.tss
 
         print('testing status command that runs normally and returns None')
         self.assertIsNone(tss.do_status(''))
@@ -233,23 +240,32 @@
         tss = self.tss
 
         print('testing watch command that runs normally and returns None')
         self.assertIsNone(tss.do_watch(''))
 
         print('testing add a new stock to watch list')
         self.assertIsNone(tss.do_watch('000002.SZ'))
-        self.assertEqual(tss.watch_list, ['000001.SH', '000002.SZ'])
+        self.assertEqual(tss.watch_list, ['000001.SZ',
+                                          '000002.SZ',
+                                          '000004.SZ',
+                                          '000005.SZ',
+                                          '000006.SZ',
+                                          '000007.SZ'])
         self.assertIsNone(tss.do_watch('000002.SZ'))
-        self.assertEqual(tss.watch_list, ['000001.SH', '000002.SZ'])
+        self.assertEqual(tss.watch_list, ['000002.SZ',
+                                          '000004.SZ',
+                                          '000005.SZ',
+                                          '000006.SZ',
+                                          '000007.SZ'])
 
         print('testing remove a stock from watch list')
         self.assertIsNone(tss.do_watch('-r 000001.SH'))
-        self.assertEqual(tss.watch_list, ['000002.SZ'])
+        self.assertEqual(tss.watch_list, ['000002.SZ', '000004.SZ', '000005.SZ', '000006.SZ', '000007.SZ'])
         self.assertIsNone(tss.do_watch('-r 000001.SH'))
-        self.assertEqual(tss.watch_list, ['000002.SZ'])
+        self.assertEqual(tss.watch_list, ['000002.SZ', '000004.SZ', '000005.SZ', '000006.SZ', '000007.SZ'])
 
         print('testing remove all stocks from watch list')
         self.assertIsNone(tss.do_watch('-c'))
         self.assertEqual(tss.watch_list, [])
 
         print(f'testing getting help and returns False')
         self.assertFalse(tss.do_watch('-h'))
```

### Comparing `qteasy-1.1.9/tests/test_trading.py` & `qteasy-1.2.0/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_tushare.py` & `qteasy-1.2.0/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_utilityfuncs.py` & `qteasy-1.2.0/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.9/tests/test_visual.py` & `qteasy-1.2.0/tests/test_visual.py`

 * *Files identical despite different names*

