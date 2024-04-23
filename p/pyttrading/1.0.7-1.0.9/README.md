# Comparing `tmp/pyttrading-1.0.7.tar.gz` & `tmp/pyttrading-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttrading-1.0.7.tar", last modified: Sat Feb 17 10:26:23 2024, max compression
+gzip compressed data, was "pyttrading-1.0.9.tar", last modified: Sat Feb 17 15:56:31 2024, max compression
```

## Comparing `pyttrading-1.0.7.tar` & `pyttrading-1.0.9.tar`

### file list

```diff
@@ -1,69 +1,74 @@
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:23.006724 pyttrading-1.0.7/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      119 2024-02-17 10:26:23.005905 pyttrading-1.0.7/PKG-INFO
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.954393 pyttrading-1.0.7/pyttrading/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      268 2024-02-17 10:16:22.000000 pyttrading-1.0.7/pyttrading/__init__.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.958490 pyttrading-1.0.7/pyttrading/backtesting_custom/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       34 2023-12-27 15:14:17.000000 pyttrading-1.0.7/pyttrading/backtesting_custom/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3450 2024-01-07 12:43:02.000000 pyttrading-1.0.7/pyttrading/backtesting_custom/generic_backtesting.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.962999 pyttrading-1.0.7/pyttrading/brokers/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       21 2023-12-31 11:58:47.000000 pyttrading-1.0.7/pyttrading/brokers/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3448 2024-01-29 20:48:23.000000 pyttrading-1.0.7/pyttrading/brokers/alpaca.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.966963 pyttrading-1.0.7/pyttrading/indicators/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      122 2023-12-27 14:39:07.000000 pyttrading-1.0.7/pyttrading/indicators/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     2343 2023-12-27 14:39:01.000000 pyttrading-1.0.7/pyttrading/indicators/bollinger_bands.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      710 2023-12-27 14:39:01.000000 pyttrading-1.0.7/pyttrading/indicators/cmma.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      733 2023-12-27 14:41:09.000000 pyttrading-1.0.7/pyttrading/indicators/days_ago.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.968367 pyttrading-1.0.7/pyttrading/labels/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      135 2023-12-27 15:07:01.000000 pyttrading-1.0.7/pyttrading/labels/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     4597 2024-02-09 17:16:14.000000 pyttrading-1.0.7/pyttrading/labels/labels.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.970386 pyttrading-1.0.7/pyttrading/market_data/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       35 2024-02-14 20:11:30.000000 pyttrading-1.0.7/pyttrading/market_data/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)    11635 2024-02-14 20:53:04.000000 pyttrading-1.0.7/pyttrading/market_data/opensearch_collector.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.975279 pyttrading-1.0.7/pyttrading/stop_loss/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       92 2024-01-07 12:42:12.000000 pyttrading-1.0.7/pyttrading/stop_loss/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3430 2024-01-07 15:40:15.000000 pyttrading-1.0.7/pyttrading/stop_loss/constant_stop_loss.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     7182 2024-01-06 15:51:14.000000 pyttrading-1.0.7/pyttrading/stop_loss/stop_loss.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     2658 2024-01-07 15:40:11.000000 pyttrading-1.0.7/pyttrading/stop_loss/trailing_stop_loss.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.977964 pyttrading-1.0.7/pyttrading/strategies/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      170 2024-01-04 14:43:46.000000 pyttrading-1.0.7/pyttrading/strategies/__init__.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.979623 pyttrading-1.0.7/pyttrading/strategies/breakout/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:16.000000 pyttrading-1.0.7/pyttrading/strategies/breakout/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3436 2023-12-27 17:56:21.000000 pyttrading-1.0.7/pyttrading/strategies/breakout/strategy.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.980831 pyttrading-1.0.7/pyttrading/strategies/dummy/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2024-02-14 19:39:52.000000 pyttrading-1.0.7/pyttrading/strategies/dummy/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     4484 2024-01-04 15:38:05.000000 pyttrading-1.0.7/pyttrading/strategies/dummy/strategy.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.982299 pyttrading-1.0.7/pyttrading/strategies/ema/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:10.000000 pyttrading-1.0.7/pyttrading/strategies/ema/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     5618 2024-01-16 20:11:02.000000 pyttrading-1.0.7/pyttrading/strategies/ema/strategy.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.983652 pyttrading-1.0.7/pyttrading/strategies/macd/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:21.000000 pyttrading-1.0.7/pyttrading/strategies/macd/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     7051 2024-01-16 07:16:20.000000 pyttrading-1.0.7/pyttrading/strategies/macd/strategy.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.985288 pyttrading-1.0.7/pyttrading/strategies/rsi/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:28.000000 pyttrading-1.0.7/pyttrading/strategies/rsi/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     6560 2024-01-16 20:13:56.000000 pyttrading-1.0.7/pyttrading/strategies/rsi/strategy.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     5090 2024-01-06 20:39:25.000000 pyttrading-1.0.7/pyttrading/strategies/selector copy.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     5090 2024-01-06 20:39:41.000000 pyttrading-1.0.7/pyttrading/strategies/selector.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:22.988871 pyttrading-1.0.7/pyttrading/strategies/sma/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       31 2023-12-27 18:19:33.000000 pyttrading-1.0.7/pyttrading/strategies/sma/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     5810 2024-01-04 19:42:12.000000 pyttrading-1.0.7/pyttrading/strategies/sma/strategy.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:23.000637 pyttrading-1.0.7/pyttrading/utils/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      240 2024-01-13 20:35:08.000000 pyttrading-1.0.7/pyttrading/utils/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1332 2024-01-14 07:34:31.000000 pyttrading-1.0.7/pyttrading/utils/df_actions_market_value.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      291 2023-12-28 14:21:34.000000 pyttrading-1.0.7/pyttrading/utils/fake_model.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      689 2024-02-08 20:18:16.000000 pyttrading-1.0.7/pyttrading/utils/get_datetime_now_trade.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1185 2024-01-04 13:30:48.000000 pyttrading-1.0.7/pyttrading/utils/inflection_points.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      165 2024-01-04 08:04:35.000000 pyttrading-1.0.7/pyttrading/utils/logs.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)    14183 2024-01-03 12:24:04.000000 pyttrading-1.0.7/pyttrading/utils/opensearch.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     2028 2024-01-07 15:35:09.000000 pyttrading-1.0.7/pyttrading/utils/plots.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1236 2024-01-14 06:39:46.000000 pyttrading-1.0.7/pyttrading/utils/pre_processing.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      779 2023-12-31 15:59:58.000000 pyttrading-1.0.7/pyttrading/utils/strategy_quality.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:23.005013 pyttrading-1.0.7/pyttrading.egg-info/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      119 2024-02-17 10:26:22.000000 pyttrading-1.0.7/pyttrading.egg-info/PKG-INFO
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1719 2024-02-17 10:26:22.000000 pyttrading-1.0.7/pyttrading.egg-info/SOURCES.txt
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)        1 2024-02-17 10:26:22.000000 pyttrading-1.0.7/pyttrading.egg-info/dependency_links.txt
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       17 2024-02-17 10:26:22.000000 pyttrading-1.0.7/pyttrading.egg-info/top_level.txt
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       38 2024-02-17 10:26:23.006908 pyttrading-1.0.7/setup.cfg
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      674 2024-02-17 10:17:06.000000 pyttrading-1.0.7/setup.py
-drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 10:26:23.001428 pyttrading-1.0.7/tests/
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)        0 2023-12-27 11:46:49.000000 pyttrading-1.0.7/tests/__init__.py
--rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1080 2024-01-02 11:36:21.000000 pyttrading-1.0.7/tests/test_strategy_dummy.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.590909 pyttrading-1.0.9/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      119 2024-02-17 15:56:31.590499 pyttrading-1.0.9/PKG-INFO
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.573580 pyttrading-1.0.9/pyttrading/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      268 2024-02-17 10:16:22.000000 pyttrading-1.0.9/pyttrading/__init__.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.574970 pyttrading-1.0.9/pyttrading/backtesting_custom/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       34 2023-12-27 15:14:17.000000 pyttrading-1.0.9/pyttrading/backtesting_custom/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3450 2024-01-07 12:43:02.000000 pyttrading-1.0.9/pyttrading/backtesting_custom/generic_backtesting.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.575712 pyttrading-1.0.9/pyttrading/brokers/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       21 2023-12-31 11:58:47.000000 pyttrading-1.0.9/pyttrading/brokers/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3448 2024-01-29 20:48:23.000000 pyttrading-1.0.9/pyttrading/brokers/alpaca.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.576954 pyttrading-1.0.9/pyttrading/indicators/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      122 2023-12-27 14:39:07.000000 pyttrading-1.0.9/pyttrading/indicators/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     2343 2023-12-27 14:39:01.000000 pyttrading-1.0.9/pyttrading/indicators/bollinger_bands.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      710 2023-12-27 14:39:01.000000 pyttrading-1.0.9/pyttrading/indicators/cmma.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      733 2023-12-27 14:41:09.000000 pyttrading-1.0.9/pyttrading/indicators/days_ago.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.577455 pyttrading-1.0.9/pyttrading/labels/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      135 2023-12-27 15:07:01.000000 pyttrading-1.0.9/pyttrading/labels/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     4597 2024-02-09 17:16:14.000000 pyttrading-1.0.9/pyttrading/labels/labels.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.578503 pyttrading-1.0.9/pyttrading/market_data/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       66 2024-02-17 12:34:36.000000 pyttrading-1.0.9/pyttrading/market_data/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      810 2024-02-17 12:59:41.000000 pyttrading-1.0.9/pyttrading/market_data/get_data_market.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)    11635 2024-02-14 20:53:04.000000 pyttrading-1.0.9/pyttrading/market_data/opensearch_collector.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.579257 pyttrading-1.0.9/pyttrading/models/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       25 2024-02-17 12:17:28.000000 pyttrading-1.0.9/pyttrading/models/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1087 2024-02-17 12:19:04.000000 pyttrading-1.0.9/pyttrading/models/experiment.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.580675 pyttrading-1.0.9/pyttrading/stop_loss/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       92 2024-01-07 12:42:12.000000 pyttrading-1.0.9/pyttrading/stop_loss/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3430 2024-01-07 15:40:15.000000 pyttrading-1.0.9/pyttrading/stop_loss/constant_stop_loss.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     7182 2024-01-06 15:51:14.000000 pyttrading-1.0.9/pyttrading/stop_loss/stop_loss.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     2658 2024-01-07 15:40:11.000000 pyttrading-1.0.9/pyttrading/stop_loss/trailing_stop_loss.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.581399 pyttrading-1.0.9/pyttrading/strategies/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      229 2024-02-17 15:54:23.000000 pyttrading-1.0.9/pyttrading/strategies/__init__.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.582162 pyttrading-1.0.9/pyttrading/strategies/breakout/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:16.000000 pyttrading-1.0.9/pyttrading/strategies/breakout/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     3757 2024-02-17 15:40:25.000000 pyttrading-1.0.9/pyttrading/strategies/breakout/strategy.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.582793 pyttrading-1.0.9/pyttrading/strategies/dummy/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2024-02-14 19:39:52.000000 pyttrading-1.0.9/pyttrading/strategies/dummy/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     4484 2024-01-04 15:38:05.000000 pyttrading-1.0.9/pyttrading/strategies/dummy/strategy.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.583466 pyttrading-1.0.9/pyttrading/strategies/ema/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:10.000000 pyttrading-1.0.9/pyttrading/strategies/ema/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     5618 2024-01-16 20:11:02.000000 pyttrading-1.0.9/pyttrading/strategies/ema/strategy.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.584116 pyttrading-1.0.9/pyttrading/strategies/macd/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:21.000000 pyttrading-1.0.9/pyttrading/strategies/macd/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     6797 2024-02-17 15:33:02.000000 pyttrading-1.0.9/pyttrading/strategies/macd/strategy.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.584720 pyttrading-1.0.9/pyttrading/strategies/rsi/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       30 2023-12-27 18:19:28.000000 pyttrading-1.0.9/pyttrading/strategies/rsi/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     6560 2024-01-16 20:13:56.000000 pyttrading-1.0.9/pyttrading/strategies/rsi/strategy.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     5388 2024-02-17 15:42:32.000000 pyttrading-1.0.9/pyttrading/strategies/selector.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.585374 pyttrading-1.0.9/pyttrading/strategies/sma/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       31 2023-12-27 18:19:33.000000 pyttrading-1.0.9/pyttrading/strategies/sma/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     5810 2024-01-04 19:42:12.000000 pyttrading-1.0.9/pyttrading/strategies/sma/strategy.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.589092 pyttrading-1.0.9/pyttrading/utils/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      267 2024-02-17 13:52:27.000000 pyttrading-1.0.9/pyttrading/utils/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1332 2024-01-14 07:34:31.000000 pyttrading-1.0.9/pyttrading/utils/df_actions_market_value.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      291 2023-12-28 14:21:34.000000 pyttrading-1.0.9/pyttrading/utils/fake_model.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      689 2024-02-08 20:18:16.000000 pyttrading-1.0.9/pyttrading/utils/get_datetime_now_trade.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1185 2024-01-04 13:30:48.000000 pyttrading-1.0.9/pyttrading/utils/inflection_points.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      656 2024-02-17 14:40:04.000000 pyttrading-1.0.9/pyttrading/utils/init_mlflow.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      165 2024-01-04 08:04:35.000000 pyttrading-1.0.9/pyttrading/utils/logs.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)    14183 2024-01-03 12:24:04.000000 pyttrading-1.0.9/pyttrading/utils/opensearch.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     2028 2024-01-07 15:35:09.000000 pyttrading-1.0.9/pyttrading/utils/plots.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1236 2024-01-14 06:39:46.000000 pyttrading-1.0.9/pyttrading/utils/pre_processing.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      779 2023-12-31 15:59:58.000000 pyttrading-1.0.9/pyttrading/utils/strategy_quality.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.574542 pyttrading-1.0.9/pyttrading.egg-info/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      119 2024-02-17 15:56:31.000000 pyttrading-1.0.9/pyttrading.egg-info/PKG-INFO
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     1853 2024-02-17 15:56:31.000000 pyttrading-1.0.9/pyttrading.egg-info/SOURCES.txt
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)        1 2024-02-17 15:56:31.000000 pyttrading-1.0.9/pyttrading.egg-info/dependency_links.txt
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       17 2024-02-17 15:56:31.000000 pyttrading-1.0.9/pyttrading.egg-info/top_level.txt
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)       38 2024-02-17 15:56:31.591018 pyttrading-1.0.9/setup.cfg
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      901 2024-02-17 15:56:29.000000 pyttrading-1.0.9/setup.py
+drwxr-xr-x   0 ceciliocannavaciuolo   (501) staff       (20)        0 2024-02-17 15:56:31.589922 pyttrading-1.0.9/tests/
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)        0 2023-12-27 11:46:49.000000 pyttrading-1.0.9/tests/__init__.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)      537 2024-02-17 13:03:30.000000 pyttrading-1.0.9/tests/test_01_get_market_data.py
+-rw-r--r--   0 ceciliocannavaciuolo   (501) staff       (20)     2418 2024-02-17 15:43:12.000000 pyttrading-1.0.9/tests/test_02_run_experiments.py
```

### Comparing `pyttrading-1.0.7/pyttrading/backtesting_custom/generic_backtesting.py` & `pyttrading-1.0.9/pyttrading/backtesting_custom/generic_backtesting.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/brokers/alpaca.py` & `pyttrading-1.0.9/pyttrading/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/indicators/bollinger_bands.py` & `pyttrading-1.0.9/pyttrading/indicators/bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/indicators/cmma.py` & `pyttrading-1.0.9/pyttrading/indicators/cmma.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/indicators/days_ago.py` & `pyttrading-1.0.9/pyttrading/indicators/days_ago.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/labels/labels.py` & `pyttrading-1.0.9/pyttrading/labels/labels.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/market_data/opensearch_collector.py` & `pyttrading-1.0.9/pyttrading/market_data/opensearch_collector.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/stop_loss/constant_stop_loss.py` & `pyttrading-1.0.9/pyttrading/stop_loss/constant_stop_loss.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/stop_loss/stop_loss.py` & `pyttrading-1.0.9/pyttrading/stop_loss/stop_loss.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/stop_loss/trailing_stop_loss.py` & `pyttrading-1.0.9/pyttrading/stop_loss/trailing_stop_loss.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/strategies/breakout/strategy.py` & `pyttrading-1.0.9/pyttrading/strategies/breakout/strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,31 @@
 from ...utils.pre_processing import remove_noise_trading
 from scipy.optimize import minimize
 
 # this strategy is breakout
 
 class Strategy: 
 
-    def __init__(self, df=None):
-        
-        pass         
+    def __init__(self, df=None, strategy_name :str = "StrategyName", bk_initial_money :float = 2000.0, bk_commission :float = 0.02):
+        self.name = 'BREAKOUT'
+        self.open_long = 1
+        self.close_long = 2
+        self.keep = 0
+        self.strategy_name = strategy_name,
+
+        self.bk_initial_money=bk_initial_money
+        self.bk_commission=bk_commission
+            
     def eval(self,df=None, params= None):
         
         breakout_threshold = int(params)
         
         print(breakout_threshold)
         # Calcular el rango de ruptura (breakout range)
-        df['breakout_range'] = df['height'] - df['low']
+        df['breakout_range'] = df['high'] - df['low']
 
         df['actions'] = 0  # Inicializar todas las acciones como "mantener"
         df.loc[df['close'] > df['open'] + breakout_threshold * df['breakout_range'], 'actions'] = 1  # Señal de compra
         df.loc[df['close'] < df['open'] - breakout_threshold * df['breakout_range'], 'actions'] = 2  # Señal de venta
 
         # Eliminar señales consecutivas repetidas
         df['actions'] = df['actions'].mask(df['actions'].eq(df['actions'].shift()))
```

### Comparing `pyttrading-1.0.7/pyttrading/strategies/dummy/strategy.py` & `pyttrading-1.0.9/pyttrading/strategies/dummy/strategy.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/strategies/ema/strategy.py` & `pyttrading-1.0.9/pyttrading/strategies/ema/strategy.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/strategies/macd/strategy.py` & `pyttrading-1.0.9/pyttrading/strategies/macd/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,38 +20,39 @@
 for param in params_default:
     param_low = param[0]
     params_init.append(param_low)
 
 
 class Strategy: 
 
-    def __init__(self, df=None):
+    def __init__(self, df=None, strategy_name :str = "StrategyName", bk_initial_money :float = 2000.0, bk_commission :float = 0.02):
         self.name = 'MACD'
         self.open_long = 1
         self.close_long = 2
         self.keep = 0
+        self.strategy_name = strategy_name,
+
+        self.bk_initial_money=bk_initial_money
+        self.bk_commission=bk_commission
     
         
     def plot(self, df=None, show_graph :bool = True, save_figure: bool = False, params=None, title: str = 'Title figure'):
         
         fig = make_subplots(rows=2, cols=1, shared_xaxes=True, vertical_spacing=0.05, row_heights=[0.7, 0.3], subplot_titles=('Price and EMA', 'RSI'))
         fig.add_trace(go.Scatter(x=df.index, y=df['close'], mode='lines', name='Close Price', line=dict(color='blue')), row=1, col=1)
         buy_indices = df.index[df['actions'] == 1]
         sell_indices = df.index[df['actions'] == 2]
         fig.add_trace(go.Scatter(x=buy_indices, y=df['close'].loc[buy_indices], mode='markers', name='Buy', marker=dict(color='green', symbol='circle', size=10)), row=1, col=1)
         fig.add_trace(go.Scatter(x=sell_indices, y=df['close'].loc[sell_indices], mode='markers', name='Sell', marker=dict(color='red', symbol='circle', size=10)), row=1, col=1)
         
         fig.add_trace(go.Scatter(x=df.index, y=df['macd_line'], mode='lines', name='EMA', line=dict(color='red', width=1)), row=2, col=1)
-        # fig.add_trace(go.Scatter(x=df.index, y=df['macd_line'], mode='lines', name='EMA_S', line=dict(color='yellow', width=1)), row=2, col=1)
 
         fig.add_trace(go.Scatter(x=buy_indices, y=df['macd_line'].loc[buy_indices], mode='markers', name='Buy', marker=dict(color='green', symbol='circle', size=10)), row=2, col=1)
         fig.add_trace(go.Scatter(x=sell_indices, y=df['macd_line'].loc[sell_indices], mode='markers', name='Sell', marker=dict(color='red', symbol='circle', size=10)), row=2, col=1)
 
-        # fig.add_trace(go.Scatter(x=df.index, y=[params[0]] * len(df), mode='lines', name='Buy Threshold', line=dict(color='green', width=1, dash='dash')), row=2, col=1)
-        # fig.add_trace(go.Scatter(x=df.index, y=[params[1]] * len(df), mode='lines', name='Sell Threshold', line=dict(color='blue', width=1, dash='dash')), row=2, col=1)
 
         fig.update_layout(template='plotly_dark', title=title, xaxis_title='Date', height=600)
 
         if show_graph:
             fig.show()
 
         if save_figure:
```

### Comparing `pyttrading-1.0.7/pyttrading/strategies/rsi/strategy.py` & `pyttrading-1.0.9/pyttrading/strategies/rsi/strategy.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/strategies/selector copy.py` & `pyttrading-1.0.9/pyttrading/strategies/selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,26 +41,25 @@
 
         if not os.path.exists(image_folder):
             os.mkdir(image_folder)
     
     def run_experiments(self):
 
         self.basic_strategies  = self.basic_models()
-        self.strategy = self.basic_strategies (
+        self.strategy = self.basic_strategies(
                     strategy_name=self.model_name
                 )
         method, best_return, best_parameters = self.strategy.experiment(
                     df=self.df
                 )
 
         return method, best_return, best_parameters
 
     def save_mlflow(self):
 
-
         self.mlflow.set_tag("strategy", self.model_name)
         self.mlflow.set_tag("method", self.params.get('method'))
         self.mlflow.log_param("optimized_params", json.dumps(self.params))
         self.mlflow.log_metric('best_return',  self.params.get('best_return'))
 
         for key, value in self.stats_json.items():
             key_s = key.replace(" ",'').replace('[%]','').replace('.','').replace('&','').replace('[$]','').replace('(','').replace(')','').replace('#','')
@@ -83,52 +82,62 @@
                     save_bk_figure=True,
                     bk_type=bk_type
                 )
 
         best_return, stats_json = back_testing_short.calculate_bk()
 
         return best_return, stats_json
+    
+    def run_experiment_get_backtesting(self):
 
-    def select(self):
         best_return = None
         best_return_short = None
 
 
         method, best_return, best_parameters = self.run_experiments()
 
         self.params = {
                     "type": self.type_model,
                     "method": method,
                     "best_return": best_return,
-                    "best_parameters": list(best_parameters),
-                    "params": list(best_parameters), 
+                    "best_parameters": best_parameters,
+                    "params": best_parameters, 
                     "strategy": self.model_name
                 }
 
 
-        df_actions = self.strategy.eval(df=self.df, params=best_parameters)
+        self.df_actions = self.strategy.eval(df=self.df, params=best_parameters)
+
+        self.return_data, self.stats_json = self.get_backtesting(df=self.df_actions, bk_type='long')
+
+
+        return self.stats_json, best_return, best_return_short, best_parameters, self.df_actions
+
+    def select(self):
+        
+        stats_json, best_return, best_return_short, best_parameters, df_actions = self.run_experiment_get_backtesting()
 
-        return_data, stats_json = self.get_backtesting(df=df_actions, bk_type='long')
         self.stats_json = stats_json
+
         self.save_mlflow()
         self.init_tmp_path()
 
         back_testing = GenericBacktesting(
-                    df=df_actions,
+                    df=self.df_actions,
                     skip=True,
                     initial_money=self.bk_initial_money,
                     commission=self.bk_commission,
                     plot_result=False,
                     path_save_result=self.path_model,
                     print_stacks=False,
                     save_bk_figure=True
                 )
 
         return_data, self.stats_json = back_testing.calculate_bk()
-        self.strategy.plot(df=df_actions, save_figure=True, show_graph=False, params=best_parameters, title=f"Strategy: {self.model_name} Return: {return_data}")
+        self.strategy.plot(df=self.df_actions, save_figure=True, show_graph=False, params=best_parameters, title=f"Strategy: {self.model_name} Return: {return_data}")
 
         best_return_short, _ = self.get_backtesting(df=df_actions, bk_type='short')
                 
         return self.basic_strategies, self.params, best_return, best_return_short
         
         
     def basic_models(self):
```

### Comparing `pyttrading-1.0.7/pyttrading/strategies/sma/strategy.py` & `pyttrading-1.0.9/pyttrading/strategies/sma/strategy.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/utils/df_actions_market_value.py` & `pyttrading-1.0.9/pyttrading/utils/df_actions_market_value.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/utils/get_datetime_now_trade.py` & `pyttrading-1.0.9/pyttrading/utils/get_datetime_now_trade.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/utils/inflection_points.py` & `pyttrading-1.0.9/pyttrading/utils/inflection_points.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/utils/opensearch.py` & `pyttrading-1.0.9/pyttrading/utils/opensearch.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/utils/plots.py` & `pyttrading-1.0.9/pyttrading/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/utils/pre_processing.py` & `pyttrading-1.0.9/pyttrading/utils/pre_processing.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading/utils/strategy_quality.py` & `pyttrading-1.0.9/pyttrading/utils/strategy_quality.py`

 * *Files identical despite different names*

### Comparing `pyttrading-1.0.7/pyttrading.egg-info/SOURCES.txt` & `pyttrading-1.0.9/pyttrading.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 pyttrading/indicators/__init__.py
 pyttrading/indicators/bollinger_bands.py
 pyttrading/indicators/cmma.py
 pyttrading/indicators/days_ago.py
 pyttrading/labels/__init__.py
 pyttrading/labels/labels.py
 pyttrading/market_data/__init__.py
+pyttrading/market_data/get_data_market.py
 pyttrading/market_data/opensearch_collector.py
+pyttrading/models/__init__.py
+pyttrading/models/experiment.py
 pyttrading/stop_loss/__init__.py
 pyttrading/stop_loss/constant_stop_loss.py
 pyttrading/stop_loss/stop_loss.py
 pyttrading/stop_loss/trailing_stop_loss.py
 pyttrading/strategies/__init__.py
-pyttrading/strategies/selector copy.py
 pyttrading/strategies/selector.py
 pyttrading/strategies/breakout/__init__.py
 pyttrading/strategies/breakout/strategy.py
 pyttrading/strategies/dummy/__init__.py
 pyttrading/strategies/dummy/strategy.py
 pyttrading/strategies/ema/__init__.py
 pyttrading/strategies/ema/strategy.py
@@ -36,14 +38,16 @@
 pyttrading/strategies/sma/__init__.py
 pyttrading/strategies/sma/strategy.py
 pyttrading/utils/__init__.py
 pyttrading/utils/df_actions_market_value.py
 pyttrading/utils/fake_model.py
 pyttrading/utils/get_datetime_now_trade.py
 pyttrading/utils/inflection_points.py
+pyttrading/utils/init_mlflow.py
 pyttrading/utils/logs.py
 pyttrading/utils/opensearch.py
 pyttrading/utils/plots.py
 pyttrading/utils/pre_processing.py
 pyttrading/utils/strategy_quality.py
 tests/__init__.py
-tests/test_strategy_dummy.py
+tests/test_01_get_market_data.py
+tests/test_02_run_experiments.py
```

### Comparing `pyttrading-1.0.7/setup.py` & `pyttrading-1.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pyttrading',
     packages=find_packages(),
-    version='1.0.7',
+    version='1.0.9',
     description='Trading Library',
     author='CannavIT',
     install_requires=[],
     setup_requires=[
         'pytest-runner',
         'stock-dataframe==0.1.0',
-        'mlflow==2.9.2',
-        'backtesting==0.3.3'
+        # 'mlflow==2.9.2',
+        # 'backtesting==0.3.3',
+        # 'scipy==1.12.0',
+        # 'Backtesting==0.3.3',
+        # 'matplotlib==3.8.3',
+        # 'plotly==5.19.0',
+        # 'mlflow',
+        # 'numba==0.59.0',
+        # 'ta==0.11.0',
+        # 'python-dotenv==1.0.1'
     ],
     tests_require=['pytest==4.4.2'],
     test_suite='tests',
     python_requires='>=3.6'
 )
 
 # pip uninstall -y pyttrading && python setup.py sdist && twine upload dist/*
```

