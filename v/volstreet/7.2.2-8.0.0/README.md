# Comparing `tmp/volstreet-7.2.2.tar.gz` & `tmp/volstreet-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.2.2.tar", last modified: Mon Apr 22 06:14:37 2024, max compression
+gzip compressed data, was "volstreet-8.0.0.tar", last modified: Tue Apr 23 09:02:18 2024, max compression
```

## Comparing `volstreet-7.2.2.tar` & `volstreet-8.0.0.tar`

### file list

```diff
@@ -1,89 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:37.008657 volstreet-7.2.2/
--rw-rw-rw-   0        0        0     1293 2024-04-22 06:14:37.008657 volstreet-7.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.2.2/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.2.2/pyproject.toml
--rw-rw-rw-   0        0        0     1104 2024-04-22 06:14:37.008657 volstreet-7.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.898680 volstreet-7.2.2/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.2.2/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.930448 volstreet-7.2.2/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.2.2/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.2.2/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18049 2024-04-22 01:56:59.000000 volstreet-7.2.2/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.2.2/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30663 2024-04-22 05:33:33.000000 volstreet-7.2.2/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.2.2/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.946091 volstreet-7.2.2/volstreet/backtests/
--rw-rw-rw-   0        0        0      157 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.2.2/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    46315 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-7.2.2/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0      972 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0       66 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/state.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-7.2.2/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     2441 2024-04-13 07:18:24.000000 volstreet-7.2.2/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20783 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6152 2024-04-22 04:46:05.000000 volstreet-7.2.2/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.961761 volstreet-7.2.2/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-7.2.2/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-7.2.2/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.2.2/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.961761 volstreet-7.2.2/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18674 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.2.2/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.961761 volstreet-7.2.2/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.977395 volstreet-7.2.2/volstreet/strategies/
--rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    56277 2024-04-22 05:03:30.000000 volstreet-7.2.2/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.2.2/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    91100 2024-04-22 06:10:10.000000 volstreet-7.2.2/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-7.2.2/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.992946 volstreet-7.2.2/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26544 2024-04-22 01:51:54.000000 volstreet-7.2.2/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19700 2024-04-22 04:16:47.000000 volstreet-7.2.2/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    19897 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.992946 volstreet-7.2.2/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.2.2/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:37.008657 volstreet-7.2.2/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.2.2/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.2.2/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:14:37.008657 volstreet-7.2.2/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2584 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/
+-rw-rw-rw-   0        0        0     1293 2024-04-23 09:02:18.075609 volstreet-8.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.0.0/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-04-23 09:02:18.075609 volstreet-8.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:17.981516 volstreet-8.0.0/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.0.0/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:17.997100 volstreet-8.0.0/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-8.0.0/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-8.0.0/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18271 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.0.0/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30663 2024-04-22 06:48:57.000000 volstreet-8.0.0/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-8.0.0/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.013111 volstreet-8.0.0/volstreet/backtests/
+-rw-rw-rw-   0        0        0      242 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.0.0/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.0.0/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     5071 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     7764 2024-04-23 08:59:42.000000 volstreet-8.0.0/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.0.0/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     2479 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20854 2024-04-23 07:13:34.000000 volstreet-8.0.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     5574 2024-04-23 07:14:56.000000 volstreet-8.0.0/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.028745 volstreet-8.0.0/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.0.0/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-8.0.0/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.0.0/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.028745 volstreet-8.0.0/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-23 04:55:13.000000 volstreet-8.0.0/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    18590 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    16793 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.044367 volstreet-8.0.0/volstreet/models/
+-rw-rw-rw-   0        0        0      565 2024-04-23 07:16:41.000000 volstreet-8.0.0/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.0.0/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.044367 volstreet-8.0.0/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.059986 volstreet-8.0.0/volstreet/strategies/
+-rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    56703 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-8.0.0/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    91543 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.0.0/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.059986 volstreet-8.0.0/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19700 2024-04-22 06:48:57.000000 volstreet-8.0.0/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20198 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.0.0/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13115 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-8.0.0/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.0.0/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       20 2024-04-23 08:08:36.000000 volstreet-8.0.0/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.0.0/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.0.0/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.0.0/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.0.0/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:02:18.075609 volstreet-8.0.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2756 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-23 09:02:17.000000 volstreet-8.0.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.2.2/PKG-INFO` & `volstreet-8.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.2.2
+Version: 8.0.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.2.2/setup.cfg` & `volstreet-8.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 322e 320d 0a61  rsion = 7.2.2..a
+00000020: 7273 696f 6e20 3d20 382e 302e 300d 0a61  rsion = 8.0.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
@@ -22,48 +22,52 @@
 00000150: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000160: 6f6e 203a 3a20 330d 0a09 4f70 6572 6174  on :: 3...Operat
 00000170: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
 00000180: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
 00000190: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
 000001a0: 6765 7320 3d20 6669 6e64 3a0d 0a69 6e63  ges = find:..inc
 000001b0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-000001c0: 6120 3d20 5472 7565 0d0a 696e 7374 616c  a = True..instal
-000001d0: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-000001e0: 6169 6f68 7474 703e 3d33 2e39 2e31 2c3c  aiohttp>=3.9.1,<
-000001f0: 342e 300d 0a09 6174 7472 733e 3d32 322e  4.0...attrs>=22.
-00000200: 322e 302c 3c32 332e 300d 0a09 4265 6175  2.0,<23.0...Beau
-00000210: 7469 6675 6c53 6f75 7034 3e3d 342e 3132  tifulSoup4>=4.12
-00000220: 2e33 2c3c 352e 300d 0a09 656f 643e 3d30  .3,<5.0...eod>=0
-00000230: 2e32 2e31 2c3c 312e 300d 0a09 6675 7a7a  .2.1,<1.0...fuzz
-00000240: 7977 757a 7a79 3e3d 302e 3138 2e30 2c3c  ywuzzy>=0.18.0,<
-00000250: 312e 300d 0a09 6a6f 626c 6962 3e3d 312e  1.0...joblib>=1.
-00000260: 332e 322c 3c32 2e30 0d0a 096c 6f67 7a65  3.2,<2.0...logze
-00000270: 726f 3e3d 312e 372e 302c 3c32 2e30 0d0a  ro>=1.7.0,<2.0..
-00000280: 096e 756d 7079 3e3d 312e 3236 2e34 2c3c  .numpy>=1.26.4,<
-00000290: 322e 300d 0a09 7061 6e64 6173 3e3d 322e  2.0...pandas>=2.
-000002a0: 302e 312c 3c33 2e30 0d0a 0970 756c 703e  0.1,<3.0...pulp>
-000002b0: 3d32 2e38 2e30 2c3c 332e 300d 0a09 7079  =2.8.0,<3.0...py
-000002c0: 6f74 703e 3d32 2e38 2e30 2c3c 332e 300d  otp>=2.8.0,<3.0.
-000002d0: 0a09 7079 7468 6f6e 2d4c 6576 656e 7368  ..python-Levensh
-000002e0: 7465 696e 3e3d 302e 3235 2e30 2c3c 312e  tein>=0.25.0,<1.
-000002f0: 300d 0a09 7265 7175 6573 7473 3e3d 322e  0...requests>=2.
-00000300: 3238 2e32 2c3c 332e 300d 0a09 7363 696b  28.2,<3.0...scik
-00000310: 6974 2d6c 6561 726e 3e3d 312e 322e 322c  it-learn>=1.2.2,
-00000320: 3c32 2e30 0d0a 0973 6369 7079 3e3d 312e  <2.0...scipy>=1.
-00000330: 3132 2e30 2c3c 322e 300d 0a09 7369 783e  12.0,<2.0...six>
-00000340: 3d31 2e31 362e 302c 3c32 2e30 0d0a 0973  =1.16.0,<2.0...s
-00000350: 6d61 7274 6170 692d 7079 7468 6f6e 3e3d  martapi-python>=
-00000360: 312e 342e 372c 3c31 2e35 2e30 0d0a 0973  1.4.7,<1.5.0...s
-00000370: 716c 616c 6368 656d 793e 3d32 2e30 2e32  qlalchemy>=2.0.2
-00000380: 302c 3c33 2e30 0d0a 0974 7769 6c69 6f3e  0,<3.0...twilio>
-00000390: 3d38 2e31 312e 312c 3c39 2e30 0d0a 0975  =8.11.1,<9.0...u
-000003a0: 726c 6c69 6233 3e3d 312e 3236 2e31 342c  rllib3>=1.26.14,
-000003b0: 3c32 2e30 0d0a 0977 6562 736f 636b 6574  <2.0...websocket
-000003c0: 2d63 6c69 656e 743e 3d31 2e35 2e31 2c3c  -client>=1.5.1,<
-000003d0: 322e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  2.0....[options.
-000003e0: 7061 636b 6167 655f 6461 7461 5d0d 0a76  package_data]..v
-000003f0: 6f6c 7374 7265 6574 203d 2068 6973 746f  olstreet = histo
-00000400: 7269 6361 6c5f 696e 666f 2f2a 2e70 6b6c  rical_info/*.pkl
-00000410: 2c20 7673 6c6f 6767 696e 672f 2a2e 6a73  , vslogging/*.js
-00000420: 6f6e 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  on....[egg_info]
-00000430: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000440: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000001c0: 6120 3d20 5472 7565 0d0a 6578 636c 7564  a = True..exclud
+000001d0: 6520 3d20 0d0a 096d 6f64 656c 732f 2a2e  e = ...models/*.
+000001e0: 6a6f 626c 6962 0d0a 696e 7374 616c 6c5f  joblib..install_
+000001f0: 7265 7175 6972 6573 203d 200d 0a09 6169  requires = ...ai
+00000200: 6f68 7474 703e 3d33 2e39 2e31 2c3c 342e  ohttp>=3.9.1,<4.
+00000210: 300d 0a09 6174 7472 733e 3d32 322e 322e  0...attrs>=22.2.
+00000220: 302c 3c32 332e 300d 0a09 4265 6175 7469  0,<23.0...Beauti
+00000230: 6675 6c53 6f75 7034 3e3d 342e 3132 2e33  fulSoup4>=4.12.3
+00000240: 2c3c 352e 300d 0a09 656f 643e 3d30 2e32  ,<5.0...eod>=0.2
+00000250: 2e31 2c3c 312e 300d 0a09 6675 7a7a 7977  .1,<1.0...fuzzyw
+00000260: 757a 7a79 3e3d 302e 3138 2e30 2c3c 312e  uzzy>=0.18.0,<1.
+00000270: 300d 0a09 6a6f 626c 6962 3e3d 312e 332e  0...joblib>=1.3.
+00000280: 322c 3c32 2e30 0d0a 096c 6f67 7a65 726f  2,<2.0...logzero
+00000290: 3e3d 312e 372e 302c 3c32 2e30 0d0a 096e  >=1.7.0,<2.0...n
+000002a0: 756d 7079 3e3d 312e 3236 2e34 2c3c 322e  umpy>=1.26.4,<2.
+000002b0: 300d 0a09 7061 6e64 6173 3e3d 322e 302e  0...pandas>=2.0.
+000002c0: 312c 3c33 2e30 0d0a 0970 756c 703e 3d32  1,<3.0...pulp>=2
+000002d0: 2e38 2e30 2c3c 332e 300d 0a09 7079 6f74  .8.0,<3.0...pyot
+000002e0: 703e 3d32 2e38 2e30 2c3c 332e 300d 0a09  p>=2.8.0,<3.0...
+000002f0: 7079 7468 6f6e 2d4c 6576 656e 7368 7465  python-Levenshte
+00000300: 696e 3e3d 302e 3235 2e30 2c3c 312e 300d  in>=0.25.0,<1.0.
+00000310: 0a09 7265 7175 6573 7473 3e3d 322e 3238  ..requests>=2.28
+00000320: 2e32 2c3c 332e 300d 0a09 7363 696b 6974  .2,<3.0...scikit
+00000330: 2d6c 6561 726e 3e3d 312e 322e 322c 3c32  -learn>=1.2.2,<2
+00000340: 2e30 0d0a 0973 6369 7079 3e3d 312e 3132  .0...scipy>=1.12
+00000350: 2e30 2c3c 322e 300d 0a09 7369 783e 3d31  .0,<2.0...six>=1
+00000360: 2e31 362e 302c 3c32 2e30 0d0a 0973 6d61  .16.0,<2.0...sma
+00000370: 7274 6170 692d 7079 7468 6f6e 3e3d 312e  rtapi-python>=1.
+00000380: 342e 372c 3c31 2e35 2e30 0d0a 0973 716c  4.7,<1.5.0...sql
+00000390: 616c 6368 656d 793e 3d32 2e30 2e32 302c  alchemy>=2.0.20,
+000003a0: 3c33 2e30 0d0a 0974 7769 6c69 6f3e 3d38  <3.0...twilio>=8
+000003b0: 2e31 312e 312c 3c39 2e30 0d0a 0975 726c  .11.1,<9.0...url
+000003c0: 6c69 6233 3e3d 312e 3236 2e31 342c 3c32  lib3>=1.26.14,<2
+000003d0: 2e30 0d0a 0977 6562 736f 636b 6574 2d63  .0...websocket-c
+000003e0: 6c69 656e 743e 3d31 2e35 2e31 2c3c 322e  lient>=1.5.1,<2.
+000003f0: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  0....[options.pa
+00000400: 636b 6167 655f 6461 7461 5d0d 0a76 6f6c  ckage_data]..vol
+00000410: 7374 7265 6574 203d 2068 6973 746f 7269  street = histori
+00000420: 6361 6c5f 696e 666f 2f2a 2e70 6b6c 2c20  cal_info/*.pkl, 
+00000430: 7673 6c6f 6767 696e 672f 2a2e 6a73 6f6e  vslogging/*.json
+00000440: 2c20 766f 6c73 7472 6565 745f 6d6f 6465  , volstreet_mode
+00000450: 2e6a 736f 6e0d 0a0d 0a5b 6567 675f 696e  .json....[egg_in
+00000460: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000470: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000480: 0a0d 0a                                  ...
```

### Comparing `volstreet-7.2.2/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-8.0.0/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/angel_interface/async_interface.py` & `volstreet-8.0.0/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/angel_interface/base_websocket.py` & `volstreet-8.0.0/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/angel_interface/interface.py` & `volstreet-8.0.0/volstreet/angel_interface/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,21 @@
         of = OrderWebsocket.from_active_session(manager, **kwargs)
         process = Process(target=of.connect)
         cls.order_feed_process = process
         cls.order_feed = of
         process.start()
 
 
+if config.backtest_mode:
+    logger.info(
+        f"Importing proxy functions in module: {__name__} since backtesting is enabled."
+    )
+    from volstreet.backtests.proxy_functions import ProxyFeeds as LiveFeeds
+
+
 def retry_angel_api(
     data_type: str | Callable = None,
     max_attempts: int = 10,
     wait_increase_factor: float = 1.1,
 ):
     def handle_retry_logic(
         function: str,
```

### Comparing `volstreet-7.2.2/volstreet/angel_interface/login.py` & `volstreet-8.0.0/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/angel_interface/order_websocket.py` & `volstreet-8.0.0/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/angel_interface/price_websocket.py` & `volstreet-8.0.0/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/angel_interface/smart_connect.py` & `volstreet-8.0.0/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/backtests/database.py` & `volstreet-8.0.0/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/backtests/delta_hedging.py` & `volstreet-8.0.0/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/backtests/delta_optimizer.py` & `volstreet-8.0.0/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/backtests/framework.py` & `volstreet-8.0.0/volstreet/backtests/framework.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pandas as pd
 import numpy as np
 from enum import Enum
 from sqlalchemy import text
 from datetime import datetime, timedelta, time
 from attrs import define, field
+from volstreet.config import logger
 from volstreet.datamodule.eod_client import EODClient
-from volstreet.utils import find_strike, make_directory_if_needed
-from volstreet.blackscholes import call, put, calculate_strangle_iv
+from volstreet.utils import find_strike
+from volstreet.blackscholes import call, put, calculate_strangle_iv, iv_multiple_to_atm
 from volstreet.backtests.database import DataBaseConnection
 from volstreet.backtests.underlying_info import UnderlyingInfo, fetch_historical_expiry
 from volstreet.backtests.tools import (
     nav_drawdown_analyser,
     prepare_index_prices_for_backtest,
 )
 from volstreet.vectorized_blackscholes import add_greeks_to_dataframe
@@ -260,14 +261,87 @@
             merged["r"] = calculate_moving_interest_rate(
                 merged, "strike", "call_price", "put_price"
             )
             merged = add_greeks_to_dataframe(merged, r_col="r", use_one_iv=False)
 
         return merged
 
+    def get_prices_for_day(
+        self,
+        underlying_info: UnderlyingInfo,
+        day: str | datetime,
+        num_strikes: int = 25,
+        num_exp: int = 2,
+        start_time: tuple[int, int] = (9, 16),
+        end_time: tuple[int, int] = (15, 30),
+    ) -> pd.DataFrame:
+        """This also fills in missing option prices."""
+        day = day.date() if isinstance(day, datetime) else day
+        option_chain = self.build_option_chain(
+            index=underlying_info,
+            from_timestamp=f"{day} {time(*start_time)}",
+            to_timestamp=f"{day} {time(*end_time)}",
+            num_strikes=num_strikes,
+            num_exp=num_exp,
+            threshold_days_expiry=0,
+        )
+        option_chain["underlying"] = underlying_info.name
+        closest_strikes = option_chain.groupby(["timestamp", "expiry"]).apply(
+            lambda x: x.loc[
+                abs(x["strike"] - x["atm_strike"]).nsmallest(3).index,
+                [
+                    "open",
+                    "strike",
+                    "call_strike",
+                    "put_strike",
+                    "time_to_expiry",
+                    "call_price",
+                    "put_price",
+                ],
+            ].reset_index(drop=True),
+            include_groups=False,
+        )
+        closest_strikes["r"] = calculate_moving_interest_rate(closest_strikes)
+        closest_strikes = add_greeks_to_dataframe(closest_strikes, r_col="r")
+        closest_strikes = closest_strikes.groupby(["timestamp", "expiry"]).apply(
+            calculate_average_atm_info
+        )
+        closest_strikes = closest_strikes.reset_index()
+        option_chain = option_chain.merge(closest_strikes, on=["timestamp", "expiry"])
+        logger.info(
+            f"Missing option prices in {day}: "
+            f"{option_chain[option_chain['call_price'].isna() | option_chain['put_price'].isna()].values}"
+        )
+        option_chain = handle_missing_atm_info(option_chain)
+        option_chain = handle_missing_option_prices(option_chain, is_call=True)
+        option_chain = handle_missing_option_prices(option_chain, is_call=False)
+        melted_prices = option_chain.rename(
+            columns={"call_price": "CE", "put_price": "PE"}
+        ).melt(
+            id_vars=["timestamp", "underlying", "expiry", "strike"],
+            value_vars=["CE", "PE"],
+            var_name="option_type",
+            value_name="price",
+        )
+        melted_prices["symboltoken"] = melted_prices.apply(
+            lambda x: f"{x['underlying']}{x['expiry'].strftime('%d%b%y').upper()}{int(x['strike'])}{x['option_type']}",
+            axis=1,
+        )
+        index_prices = option_chain.drop_duplicates(
+            subset=["timestamp", "open"]
+        ).rename(columns={"open": "price", "underlying": "symboltoken"})[
+            ["timestamp", "price", "symboltoken"]
+        ]
+        melted_prices = pd.concat([index_prices, melted_prices], axis=0)
+        melted_prices["price"] = melted_prices["price"].round(4)
+        melted_prices = melted_prices.sort_values(
+            ["timestamp", "strike", "option_type", "expiry"]
+        )
+        return melted_prices
+
     def build_trade_df(
         self,
         underlying: UnderlyingInfo,
         trade_entry_time: tuple[int, int],
         square_up_time_delta: timedelta,
         threshold_days_expiry: (
             int | float
@@ -1142,64 +1216,14 @@
     ).to_frame(index=False)
     option_prices_data["call_price"] = np.random.uniform(5, 15, len(option_prices_data))
     option_prices_data["put_price"] = np.random.uniform(3, 10, len(option_prices_data))
 
     return option_prices_data
 
 
-def calculate_atm_ivs(
-    backtester: BackTester,
-    underlying: UnderlyingInfo,
-    from_timestamp: str | datetime,
-    to_timestamp: str | datetime,
-    **kwargs,
-) -> pd.DataFrame:
-    def _calculate_averages(group):
-        # Calculate the average 'r', 'call_iv', and 'put_iv', ignoring missing values
-        avg_r = group["r"].mean(skipna=True)
-        avg_call_iv = group["call_iv"].mean(skipna=True)
-        avg_put_iv = group["put_iv"].mean(skipna=True)
-
-        # Return a Series with the calculated averages
-        day_averages = pd.Series(
-            {
-                "r": avg_r,
-                "call_iv": avg_call_iv,
-                "put_iv": avg_put_iv,
-            }
-        )
-
-        return day_averages
-
-    option_chain = backtester.build_option_chain(
-        underlying, from_timestamp, to_timestamp, **kwargs
-    )
-    option_chain["r"] = calculate_moving_interest_rate(option_chain)
-    df = add_greeks_to_dataframe(option_chain, r_col="r")
-    averages = df.groupby(["timestamp", "expiry"]).apply(_calculate_averages)
-    averages["atm_iv"] = np.mean(averages[["call_iv", "put_iv"]], axis=1)
-    averages["atm_iv"] = averages["atm_iv"].ffill().bfill()
-    averages["underlying"] = underlying.name
-    averages = averages.reset_index()
-    averages = averages.drop(columns=["call_iv", "put_iv"])
-    return averages
-
-
-def store_atm_ivs(*args, **kwargs):
-    ivs = calculate_atm_ivs(*args, **kwargs)
-    underlying = ivs.underlying[0]
-    from_timestamp = ivs.timestamp.min()
-    to_timestamp = ivs.timestamp.max()
-    directory = f"data\\atm_ivs_new\\{underlying}"
-    file_name = f"{underlying}_atm_ivs_{from_timestamp.strftime('%Y-%m-%d')}_{to_timestamp.strftime('%Y-%m-%d')}.csv"
-    full_path = f"{directory}\\{file_name}"
-    make_directory_if_needed(full_path)
-    ivs.to_csv(full_path)
-
-
 def calculate_moving_interest_rate(
     dataframe: pd.DataFrame,
     strike_col: str = "strike",
     call_price_col: str = "call_price",
     put_price_col: str = "put_price",
 ) -> np.ndarray:
     dataframe = dataframe.copy()
@@ -1217,79 +1241,104 @@
         50,
         np.where(dataframe["r"] == -np.inf, -50, dataframe["r"]),
     )
 
     return r.astype(float)
 
 
-def calculate_intrinsic_value(df, open_col, strike_col, is_call=True):
-    """Calculate the intrinsic value for options."""
-    if is_call:
-        return np.maximum(0, df[open_col] - df[strike_col])
-    else:
-        return np.maximum(0, df[strike_col] - df[open_col])
+def calculate_average_atm_info(group):
+    """Works on a dataframe which is grouped by 'timestamp' and 'expiry' columns."""
 
+    # Calculate the average 'r', 'call_iv', and 'put_iv', ignoring missing values
+    avg_r = group["r"].mean(skipna=True)
+    avg_call_iv = group["call_iv"].mean(skipna=True)
+    avg_put_iv = group["put_iv"].mean(skipna=True)
+    atm_iv = (avg_call_iv + avg_put_iv) / 2
+
+    # Return a Series with the calculated averages
+    averages = pd.Series(
+        {
+            "r": avg_r,
+            "atm_iv": atm_iv,
+        }
+    )
 
-def calculate_option_price(
-    df, open_col, strike_col, time_to_expiry_col, iv_col, is_call=True
-):
-    """Calculate the option price using a model (e.g., Black-Scholes)."""
+    return averages
+
+
+def calculate_intrinsic_value(df, spot_col, strike_col, is_call=True):
+    """Calculate the intrinsic value for options."""
     if is_call:
-        return call(
-            df[open_col], df[strike_col], df[time_to_expiry_col], 0.05, df[iv_col]
-        )
+        return np.maximum(0, df[spot_col] - df[strike_col])
     else:
-        return put(
-            df[open_col], df[strike_col], df[time_to_expiry_col], 0.05, df[iv_col]
-        )
+        return np.maximum(0, df[strike_col] - df[spot_col])
 
 
-def fill_option_prices(
-    df, price_col, strike_col, time_to_expiry_col, iv_col, open_col, is_call=True
-):
-    """Fill missing option prices in the DataFrame."""
-    short_expiry = df[time_to_expiry_col] < (0.5 / (364 * 24))
-    intrinsic = calculate_intrinsic_value(df, open_col, strike_col, is_call)
-    option_price = calculate_option_price(
-        df, open_col, strike_col, time_to_expiry_col, iv_col, is_call
+def handle_missing_atm_info(df: pd.DataFrame) -> pd.DataFrame:
+    """
+    This function handles missing ATM information in the daily prices by grouping the data by timestamp and expiry
+    and interpolating the missing values. Grouping is essential as each expiry has its own ATM information.
+    """
+    sequential_atm_iv_r = (
+        df.groupby(
+            [
+                "timestamp",
+                "expiry",
+            ]
+        )
+        .agg({"atm_iv": "first", "r": "first"})
+        .reset_index()
     )
+    interpolated_ivs_r = (
+        sequential_atm_iv_r.groupby("expiry")
+        .apply(lambda x: x.interpolate("linear"), include_groups=False)
+        .reset_index()
+    )
+    interpolated_ivs_r = interpolated_ivs_r[
+        ["timestamp", "expiry", "atm_iv", "r"]
+    ].sort_values(["timestamp", "expiry"])
+
+    df[["atm_iv", "r"]] = df[["timestamp", "expiry"]].merge(
+        interpolated_ivs_r, on=["timestamp", "expiry"], how="left"
+    )[["atm_iv", "r"]]
 
-    df[price_col] = np.where(
-        df[price_col].isna() & short_expiry,
-        intrinsic,
-        np.where(df[price_col].isna(), option_price, df[price_col]),
-    )
     return df
 
 
-def fill_missing_option_prices(df: pd.DataFrame) -> pd.DataFrame:
-    df = df.copy()
-
-    # Fill regular call and put prices
-    df = fill_option_prices(
-        df, "call_price", "call_strike", "time_to_expiry", "iv", "open", is_call=True
-    )
-    df = fill_option_prices(
-        df, "put_price", "put_strike", "time_to_expiry", "iv", "open", is_call=False
-    )
-
-    # Fill square up call and put prices
-    df = fill_option_prices(
-        df,
-        "square_up_call_price",
-        "square_up_call_strike",
-        "square_up_time_to_expiry",
-        "iv",
-        "open",
-        is_call=True,
-    )
-    df = fill_option_prices(
-        df,
-        "square_up_put_price",
-        "square_up_put_strike",
-        "square_up_time_to_expiry",
-        "iv",
-        "open",
-        is_call=False,
+def handle_missing_option_prices(
+    dataframe: pd.DataFrame, is_call: bool
+) -> pd.DataFrame:
+    opt_type = "call" if is_call else "put"
+    price_func = call if is_call else put
+    missing_prices = dataframe[dataframe[f"{opt_type}_price"].isna()]
+    if len(missing_prices) == 0:
+        return dataframe
+    time_to_expiry = missing_prices["time_to_expiry"].apply(lambda x: max(0.000003, x))
+    iv_multiples = iv_multiple_to_atm(
+        missing_prices["atm_iv"],
+        time_to_expiry,
+        missing_prices["open"],
+        missing_prices["strike"],
+    )
+    simulated_ivs = missing_prices["atm_iv"] * iv_multiples
+
+    short_expiry = missing_prices["time_to_expiry"] < (
+        0.25 / (364 * 24)
+    )  # Expiry less than 15 minutes
+    intrinsics = calculate_intrinsic_value(
+        missing_prices, "open", "strike", is_call=is_call
+    )
+    option_prices = price_func(
+        missing_prices["open"],
+        missing_prices["strike"],
+        missing_prices["time_to_expiry"],
+        missing_prices["r"],
+        simulated_ivs,
+    )
+
+    dataframe.loc[missing_prices.index, f"{opt_type}_price"] = np.where(
+        short_expiry,
+        intrinsics,
+        option_prices,
     )
 
-    return df
+    return dataframe
```

### Comparing `volstreet-7.2.2/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.0.0/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/backtests/tools.py` & `volstreet-8.0.0/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/backtests/trend.py` & `volstreet-8.0.0/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/backtests/underlying_info.py` & `volstreet-8.0.0/volstreet/backtests/underlying_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 from datetime import datetime
 import pickle
 import numpy as np
-from volstreet.config import logger, historical_expiry_dates
+from volstreet.config import logger
+from volstreet.historical_info import historical_expiry_dates
 from volstreet.backtests.database import DataBaseConnection
 
 
 class UnderlyingInfo:
     def __init__(self, name):
         self.name = name.upper()
         self.base = self._get_base()
```

### Comparing `volstreet-7.2.2/volstreet/blackscholes.py` & `volstreet-8.0.0/volstreet/blackscholes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from scipy.stats import norm
 from scipy.optimize import brentq
 import numpy as np
 from attrs import define, field
+from volstreet.models import iv_curve_model, expiry_day_model
 from volstreet.exceptions import IntrinsicValueError
-from volstreet.config import iv_curve_model, expiry_day_model, logger
+from volstreet.config import logger
 import warnings
 
 N = norm.cdf
 binary_flag = {"c": 1, "p": -1}
 
 
 @define(repr=False)
@@ -132,20 +133,16 @@
 def pdf(x):
     """the probability density function"""
     one_over_sqrt_two_pi = 0.3989422804014326779399460599343818684758586311649
     return one_over_sqrt_two_pi * np.exp(-0.5 * x * x)
 
 
 def d1(S, K, t, r, sigma):
-    sigma_squared = sigma * sigma
-    numerator = np.log(S / float(K)) + (r + sigma_squared / 2.0) * t
+    numerator = np.log(S / K) + (r + (0.5 * sigma**2)) * t
     denominator = sigma * np.sqrt(t)
-
-    if not denominator:
-        print("")
     return numerator / denominator
 
 
 def d2(S, K, t, r, sigma):
     return d1(S, K, t, r, sigma) - sigma * np.sqrt(t)
 
 
@@ -451,30 +448,36 @@
         }
     )
 
 
 def iv_multiple_to_atm(atm_iv, time_to_expiry, spot, strike):
     distance = (strike / spot) - 1
     distance_squared = distance**2
-    moneyness = spot / strike
-    distance_time_interaction = distance_squared * time_to_expiry
+    money_ness = spot / strike
+    distance_time_interaction = distance / time_to_expiry
+
+    # Prepare input features as a 2D array for RandomForestRegressor
+    features = np.column_stack(
+        [
+            atm_iv,
+            time_to_expiry,
+            distance,
+            distance_squared,
+            money_ness,
+            distance_time_interaction,
+        ]
+    )
+
     with warnings.catch_warnings():
         warnings.filterwarnings(action="ignore", category=UserWarning)
-        return iv_curve_model.predict(
-            [
-                [
-                    atm_iv,
-                    time_to_expiry,
-                    distance,
-                    distance_squared,
-                    moneyness,
-                    distance_time_interaction,
-                ]
-            ]
-        )[0]
+        predictions = iv_curve_model.predict(features)
+        if len(predictions) == 1:
+            return predictions[0]
+        else:
+            return predictions
 
 
 def adjusted_iv_from_atm_iv(atm_iv, strike, spot, time_to_expiry):
     iv_multiple = iv_multiple_to_atm(atm_iv, time_to_expiry, spot, strike)
     return atm_iv * iv_multiple
```

### Comparing `volstreet-7.2.2/volstreet/config.py` & `volstreet-8.0.0/volstreet/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import urllib
 import requests
 import pandas as pd
-import pickle
 import os
 import joblib
+import json
+import sys
 from pathlib import Path
 from threading import local
 from bs4 import BeautifulSoup
 from twilio.rest import Client as TwilioClient
 from io import StringIO
 import logging
 from importlib.resources import files
+from collections import defaultdict
 from volstreet.vslogging import setup_logging
 
 
+def change_mode(mode: str):
+    mode_file = files("volstreet").joinpath("volstreet_mode.json")
+    with open(mode_file, "w") as f:
+        json.dump({"mode": mode}, f)
+    sys.exit()
+
+
 def get_ticker_file():
     url = "https://margincalculator.angelbroking.com/OpenAPI_File/files/OpenAPIScripMaster.json"
     data = urllib.request.urlopen(url).read().decode()
 
     # Use StringIO to mimic a file using the string data
     df = pd.read_json(StringIO(data))
     return df
@@ -79,49 +88,14 @@
         df["SYMBOL"] = df["SYMBOL"].str.strip()
         return df
     except Exception as e:
         logger.error(f"Error while fetching symbols: {e}")
         return pd.DataFrame()
 
 
-def load_historical_expiry_dates():
-    resource_path = files("volstreet").joinpath("historical_info")
-    # noinspection PyTypeChecker
-    expiry_path = Path(resource_path.joinpath("index_expiries.pkl"))
-    # noinspection PyTypeChecker
-    with open(expiry_path, "rb") as f:
-        historical_expiries = pickle.load(f)
-
-    return historical_expiries
-
-
-def load_iv_models():
-    resource_path = files("volstreet").joinpath("iv_models")
-
-    # noinspection PyTypeChecker
-    curve_model_path = Path(resource_path.joinpath("iv_curve_adjuster.joblib"))
-    # noinspection PyTypeChecker
-    vix_to_iv_model_path = Path(resource_path.joinpath("vix_to_iv.joblib"))
-    # noinspection PyTypeChecker
-    atm_iv_on_expiry_day_model_path = Path(
-        resource_path.joinpath("atm_iv_on_expiry_day.joblib")
-    )
-
-    models = []
-    for model_path in [
-        curve_model_path,
-        vix_to_iv_model_path,
-        atm_iv_on_expiry_day_model_path,
-    ]:
-        with open(model_path, "rb") as f:
-            model = joblib.load(f)
-            models.append(model)
-    return tuple(models)
-
-
 class Twilio:
     account_sid = os.getenv("TWILIO_ACCOUNT_SID")
     auth_token = os.getenv("TWILIO_AUTH_TOKEN")
     content_sid = os.getenv("TWILIO_CONTENT_SID")
     service_sid = os.getenv("TWILIO_SERVICE_SID")
     if account_sid is not None and auth_token is not None:
         client = TwilioClient(account_sid, auth_token)
@@ -143,58 +117,70 @@
     "FINNIFTY": 1,
     "BANKNIFTY": 2,
     "NIFTY": 3,
     "SENSEX": 4,
     "BANKEX": 0,
 }
 
+# Backtest settings
+try:
+    vs_mode_file = files("volstreet").joinpath("volstreet_mode.json")
+    with open(vs_mode_file, "r") as f:
+        data = json.load(f)
+except FileNotFoundError:
+    data = {}
+_mode = data.get("mode", "live")
+backtest_mode = "backtest" in _mode
+backtest_state = None
+
+
 # Create loggers
 setup_logging()
 logger = logging.getLogger("volstreet")
 
-# Get the list of scrips
-scrips = get_ticker_file()
-scrips["expiry_dt"] = pd.to_datetime(
-    scrips[scrips.expiry != ""]["expiry"], format="%d%b%Y"
-)
-scrips["expiry_formatted"] = scrips["expiry_dt"].dt.strftime("%d%b%y")
-scrips["expiry_formatted"] = scrips["expiry_formatted"].str.upper()
+if backtest_mode:
+    scrips = pd.DataFrame()
+    token_symbol_dict = {}
+    token_exchange_dict = defaultdict(lambda: "BACKTESTER")
+else:
+    # Get the list of scrips
+    scrips = get_ticker_file()
+    scrips["expiry_dt"] = pd.to_datetime(
+        scrips[scrips.expiry != ""]["expiry"], format="%d%b%Y"
+    )
+    scrips["expiry_formatted"] = scrips["expiry_dt"].dt.strftime("%d%b%y")
+    scrips["expiry_formatted"] = scrips["expiry_formatted"].str.upper()
+
+    # Create a dictionary of token and symbol
+    token_symbol_dict = dict(zip(scrips["token"], scrips["symbol"]))
+
+    # Create a dictionary of token and exchange segment
+    token_exchange_dict = dict(zip(scrips["token"], scrips["exch_seg"]))
+
 
 implemented_indices = [
     "NIFTY",
     "BANKNIFTY",
     "FINNIFTY",
     "MIDCPNIFTY",
     "SENSEX",
     "BANKEX",
     "INDIA VIX",
 ]
 
-# Create a dictionary of token and symbol
-token_symbol_dict = dict(zip(scrips["token"], scrips["symbol"]))
-
-# Create a dictionary of token and exchange segment
-token_exchange_dict = dict(zip(scrips["token"], scrips["exch_seg"]))
-
 # Get the list of holidays
 try:
     holidays = fetch_holidays()
 except Exception as e:
     logger.error(f"Error while fetching holidays: {e}")
     holidays = pd.to_datetime([])
 
 # Get the list of symbols
 symbol_df = get_symbol_df()
 
-# Load the iv models
-iv_curve_model, vix_to_iv_model, expiry_day_model = None, None, None
-
-# Load the historical expiry dates
-historical_expiry_dates = load_historical_expiry_dates()
-
 # Create a thread local object
 thread_local = local()
 
 modification_fields = [
     "orderid",
     "variety",
     "symboltoken",
```

### Comparing `volstreet-7.2.2/volstreet/database_connection.py` & `volstreet-8.0.0/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/analysis.py` & `volstreet-8.0.0/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/archive.py` & `volstreet-8.0.0/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/data_handling.py` & `volstreet-8.0.0/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/eod_client.py` & `volstreet-8.0.0/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/gambling.py` & `volstreet-8.0.0/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/intraday_data.py` & `volstreet-8.0.0/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/stockmock.py` & `volstreet-8.0.0/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/datamodule/trading_assistance.py` & `volstreet-8.0.0/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/dealingroom.py` & `volstreet-8.0.0/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/decorators.py` & `volstreet-8.0.0/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/discord_bot.py` & `volstreet-8.0.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/exceptions.py` & `volstreet-8.0.0/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.0.0/volstreet/historical_info/index_expiries.pkl`

 * *Files 2% similar despite different names*

```diff
@@ -1,1168 +1,1162 @@
-00000000: 8004 95e7 4800 0000 0000 007d 9428 8c05  ....H......}.(..
+00000000: 8004 9593 4800 0000 0000 007d 9428 8c05  ....H......}.(..
 00000010: 4e49 4654 5994 5d94 288c 1e70 616e 6461  NIFTY.].(..panda
 00000020: 732e 5f6c 6962 732e 7473 6c69 6273 2e74  s._libs.tslibs.t
 00000030: 696d 6573 7461 6d70 7394 8c13 5f75 6e70  imestamps..._unp
 00000040: 6963 6b6c 655f 7469 6d65 7374 616d 7094  ickle_timestamp.
-00000050: 9394 288a 0800 b0f9 3e35 e977 174e 4e4b  ..(.....>5.w.NNK
-00000060: 0a74 9452 9468 0528 8a08 00b0 d31b dad9  .t.R.h.(........
-00000070: f015 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000080: b036 8a85 4660 174e 4e4b 0a74 9452 9468  .6..F`.NNK.t.R.h
-00000090: 0528 8a08 00b0 2b0c 5673 3717 4e4e 4b0a  .(....+.Vs7.NNK.
-000000a0: 7494 5294 6805 288a 0800 b0bb 9e55 d459  t.R.h.(......U.Y
-000000b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000000c0: c2c8 47c9 ab16 4e4e 4b0a 7494 5294 6805  ..G...NNK.t.R.h.
-000000d0: 288a 0800 b0db c354 969e 174e 4e4b 0a74  (......T...NNK.t
-000000e0: 9452 9468 0528 8a08 00b0 9fa4 9ae0 c515  .R.h.(..........
-000000f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e7  NNK.t.R.h.(.....
-00000100: 6d1a 11d7 154e 4e4b 0a74 9452 9468 0528  m....NNK.t.R.h.(
-00000110: 8a08 00b0 ca47 c975 3316 4e4e 4b0a 7494  .....G.u3.NNK.t.
-00000120: 5294 6805 288a 0800 b0de 9909 ad19 164e  R.h.(..........N
-00000130: 4e4b 0a74 9452 9468 0528 8a08 00b0 a2a3  NK.t.R.h.(......
-00000140: 4807 6716 4e4e 4b0a 7494 5294 6805 288a  H.g.NNK.t.R.h.(.
-00000150: 0800 b032 3648 6889 164e 4e4b 0a74 9452  ...26Hh..NNK.t.R
-00000160: 9468 0528 8a08 00b0 193b 3b9b 9615 4e4e  .h.(.....;;...NN
-00000170: 4b0a 7494 5294 6805 288a 0800 b025 0efa  K.t.R.h.(....%..
-00000180: 25f5 154e 4e4b 0a74 9452 9468 0528 8a08  %..NNK.t.R.h.(..
-00000190: 00b0 63ae d93a 1316 4e4e 4b0a 7494 5294  ..c..:..NNK.t.R.
-000001a0: 6805 288a 0800 b098 7aa8 eb73 164e 4e4b  h.(.....z..s.NNK
-000001b0: 0a74 9452 9468 0528 8a08 00b0 ec16 e7a6  .t.R.h.(........
-000001c0: e316 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000001d0: b081 29ba 8dec 154e 4e4b 0a74 9452 9468  ..)....NNK.t.R.h
-000001e0: 0528 8a08 00b0 fbbf 5a48 bd15 4e4e 4b0a  .(......ZH..NNK.
-000001f0: 7494 5294 6805 288a 0800 b0aa 4bc3 c314  t.R.h.(.....K...
-00000200: 184e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000210: e641 8469 c717 4e4e 4b0a 7494 5294 6805  .A.i..NNK.t.R.h.
-00000220: 288a 0800 b080 d42a d6b6 154e 4e4b 0a74  (......*...NNK.t
-00000230: 9452 9468 0528 8a08 00b0 9150 b6f6 2117  .R.h.(.....P..!.
-00000240: 4e4e 4b0a 7494 5294 6805 288a 0800 b0c1  NNK.t.R.h.(.....
-00000250: 73b8 1176 164e 4e4b 0a74 9452 9468 0528  s..v.NNK.t.R.h.(
-00000260: 8a08 00b0 8335 b6d3 ba15 4e4e 4b0a 7494  .....5....NNK.t.
-00000270: 5294 6805 288a 0800 b083 d3d8 fc57 164e  R.h.(........W.N
-00000280: 4e4b 0a74 9452 9468 0528 8a08 00b0 ea6c  NK.t.R.h.(.....l
-00000290: c837 7816 4e4e 4b0a 7494 5294 6805 288a  .7x.NNK.t.R.h.(.
-000002a0: 0800 b0e9 1739 8042 164e 4e4b 0a74 9452  .....9.B.NNK.t.R
-000002b0: 9468 0528 8a08 00b0 5dd9 76fd f616 4e4e  .h.(....].v...NN
-000002c0: 4b0a 7494 5294 6805 288a 0800 b07c a9e6  K.t.R.h.(....|..
-000002d0: 0706 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000002e0: 00b0 d19a b47a ab17 4e4e 4b0a 7494 5294  .....z..NNK.t.R.
-000002f0: 6805 288a 0800 b033 8bd7 1fbf 164e 4e4b  h.(....3.....NNK
-00000300: 0a74 9452 9468 0528 8a08 00b0 50b1 28bb  .t.R.h.(....P.(.
-00000310: 6216 4e4e 4b0a 7494 5294 6805 288a 0800  b.NNK.t.R.h.(...
-00000320: b037 df14 fe95 174e 4e4b 0a74 9452 9468  .7.....NNK.t.R.h
-00000330: 0528 8a08 00b0 a504 d404 6b16 4e4e 4b0a  .(........k.NNK.
+00000050: 9394 288a 0800 b0a8 78ab 4483 154e 4e4b  ..(.....x.D..NNK
+00000060: 0a74 9452 9468 0528 8a08 00b0 d171 bb6a  .t.R.h.(.....q.j
+00000070: 8515 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000080: b0fa 6acb 9087 154e 4e4b 0a74 9452 9468  ..j....NNK.t.R.h
+00000090: 0528 8a08 00b0 2364 dbb6 8915 4e4e 4b0a  .(....#d....NNK.
+000000a0: 7494 5294 6805 288a 0800 b04c 5deb dc8b  t.R.h.(....L]...
+000000b0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000000c0: 26c5 66b4 8d15 4e4e 4b0a 7494 5294 6805  &.f...NNK.t.R.h.
+000000d0: 288a 0800 b09e 4f0b 2990 154e 4e4b 0a74  (.....O.)..NNK.t
+000000e0: 9452 9468 0528 8a08 00b0 c748 1b4f 9215  .R.h.(.....H.O..
+000000f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
+00000100: 412b 7594 154e 4e4b 0a74 9452 9468 0528  A+u..NNK.t.R.h.(
+00000110: 8a08 00b0 193b 3b9b 9615 4e4e 4b0a 7494  .....;;...NNK.t.
+00000120: 5294 6805 288a 0800 b042 344b c198 154e  R.h.(....B4K...N
+00000130: 4e4b 0a74 9452 9468 0528 8a08 00b0 6b2d  NK.t.R.h.(....k-
+00000140: 5be7 9a15 4e4e 4b0a 7494 5294 6805 288a  [...NNK.t.R.h.(.
+00000150: 0800 b094 266b 0d9d 154e 4e4b 0a74 9452  ....&k...NNK.t.R
+00000160: 9468 0528 8a08 00b0 bd1f 7b33 9f15 4e4e  .h.(......{3..NN
+00000170: 4b0a 7494 5294 6805 288a 0800 b0e6 188b  K.t.R.h.(.......
+00000180: 59a1 154e 4e4b 0a74 9452 9468 0528 8a08  Y..NNK.t.R.h.(..
+00000190: 00b0 0f12 9b7f a315 4e4e 4b0a 7494 5294  ........NNK.t.R.
+000001a0: 6805 288a 0800 b038 0bab a5a5 154e 4e4b  h.(....8.....NNK
+000001b0: 0a74 9452 9468 0528 8a08 00b0 6104 bbcb  .t.R.h.(....a...
+000001c0: a715 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000001d0: b08a fdca f1a9 154e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+000001e0: 0528 8a08 00b0 b3f6 da17 ac15 4e4e 4b0a  .(..........NNK.
+000001f0: 7494 5294 6805 288a 0800 b0dc efea 3dae  t.R.h.(.......=.
+00000200: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000210: 05e9 fa63 b015 4e4e 4b0a 7494 5294 6805  ...c..NNK.t.R.h.
+00000220: 288a 0800 b02e e20a 8ab2 154e 4e4b 0a74  (..........NNK.t
+00000230: 9452 9468 0528 8a08 00b0 57db 1ab0 b415  .R.h.(....W.....
+00000240: 4e4e 4b0a 7494 5294 6805 288a 0800 b080  NNK.t.R.h.(.....
+00000250: d42a d6b6 154e 4e4b 0a74 9452 9468 0528  .*...NNK.t.R.h.(
+00000260: 8a08 00b0 a9cd 3afc b815 4e4e 4b0a 7494  ......:...NNK.t.
+00000270: 5294 6805 288a 0800 b083 35b6 d3ba 154e  R.h.(.....5....N
+00000280: 4e4b 0a74 9452 9468 0528 8a08 00b0 fbbf  NK.t.R.h.(......
+00000290: 5a48 bd15 4e4e 4b0a 7494 5294 6805 288a  ZH..NNK.t.R.h.(.
+000002a0: 0800 b024 b96a 6ebf 154e 4e4b 0a74 9452  ...$.jn..NNK.t.R
+000002b0: 9468 0528 8a08 00b0 4db2 7a94 c115 4e4e  .h.(....M.z...NN
+000002c0: 4b0a 7494 5294 6805 288a 0800 b076 ab8a  K.t.R.h.(....v..
+000002d0: bac3 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000002e0: 00b0 9fa4 9ae0 c515 4e4e 4b0a 7494 5294  ........NNK.t.R.
+000002f0: 6805 288a 0800 b0c8 9daa 06c8 154e 4e4b  h.(..........NNK
+00000300: 0a74 9452 9468 0528 8a08 00b0 f196 ba2c  .t.R.h.(.......,
+00000310: ca15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000320: b01a 90ca 52cc 154e 4e4b 0a74 9452 9468  ....R..NNK.t.R.h
+00000330: 0528 8a08 00b0 4389 da78 ce15 4e4e 4b0a  .(....C..x..NNK.
 00000340: 7494 5294 6805 288a 0800 b06c 82ea 9ed0  t.R.h.(....l....
 00000350: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000360: b020 2601 3117 4e4e 4b0a 7494 5294 6805  . &.1.NNK.t.R.h.
-00000370: 288a 0800 b078 55a9 292f 164e 4e4b 0a74  (....xU.)/.NNK.t
-00000380: 9452 9468 0528 8a08 00b0 f340 d99b 3516  .R.h.(.....@..5.
-00000390: 4e4e 4b0a 7494 5294 6805 288a 0800 b05c  NNK.t.R.h.(....\
-000003a0: 84e7 45c1 164e 4e4b 0a74 9452 9468 0528  ..E..NNK.t.R.h.(
-000003b0: 8a08 00b0 6b56 54f7 c017 4e4e 4b0a 7494  ....kVT...NNK.t.
-000003c0: 5294 6805 288a 0800 b0cf 198f 1b66 194e  R.h.(........f.N
-000003d0: 4e4b 0a74 9452 9468 0528 8a08 00b0 c01e  NK.t.R.h.(......
-000003e0: 295a 4016 4e4e 4b0a 7494 5294 6805 288a  )Z@.NNK.t.R.h.(.
-000003f0: 0800 b028 36a1 5cbc 184e 4e4b 0a74 9452  ...(6.\..NNK.t.R
-00000400: 9468 0528 8a08 00b0 b74a 18f6 8216 4e4e  .h.(.....J....NN
-00000410: 4b0a 7494 5294 6805 288a 0800 b06b 2d5b  K.t.R.h.(....k-[
-00000420: e79a 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000430: 00b0 c748 1b4f 9215 4e4e 4b0a 7494 5294  ...H.O..NNK.t.R.
-00000440: 6805 288a 0800 b014 bb67 15b0 164e 4e4b  h.(......g...NNK
-00000450: 0a74 9452 9468 0528 8a08 00b0 eec0 0516  .t.R.h.(........
-00000460: 4f17 4e4e 4b0a 7494 5294 6805 288a 0800  O.NNK.t.R.h.(...
-00000470: b0b5 a0f9 8617 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00000480: 0528 8a08 00b0 e8c2 a9c8 0c16 4e4e 4b0a  .(..........NNK.
-00000490: 7494 5294 6805 288a 0800 b00f 129b 7fa3  t.R.h.(.........
+00000360: 957b fac4 d215 4e4e 4b0a 7494 5294 6805  .{....NNK.t.R.h.
+00000370: 288a 0800 b0be 740a ebd4 154e 4e4b 0a74  (.....t....NNK.t
+00000380: 9452 9468 0528 8a08 00b0 e76d 1a11 d715  .R.h.(.....m....
+00000390: 4e4e 4b0a 7494 5294 6805 288a 0800 b010  NNK.t.R.h.(.....
+000003a0: 672a 37d9 154e 4e4b 0a74 9452 9468 0528  g*7..NNK.t.R.h.(
+000003b0: 8a08 00b0 3960 3a5d db15 4e4e 4b0a 7494  ....9`:]..NNK.t.
+000003c0: 5294 6805 288a 0800 b062 594a 83dd 154e  R.h.(....bYJ...N
+000003d0: 4e4b 0a74 9452 9468 0528 8a08 00b0 8b52  NK.t.R.h.(.....R
+000003e0: 5aa9 df15 4e4e 4b0a 7494 5294 6805 288a  Z...NNK.t.R.h.(.
+000003f0: 0800 b0b4 4b6a cfe1 154e 4e4b 0a74 9452  ....Kj...NNK.t.R
+00000400: 9468 0528 8a08 00b0 dd44 7af5 e315 4e4e  .h.(.....Dz...NN
+00000410: 4b0a 7494 5294 6805 288a 0800 b006 3e8a  K.t.R.h.(.....>.
+00000420: 1be6 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00000430: 00b0 2f37 9a41 e815 4e4e 4b0a 7494 5294  ../7.A..NNK.t.R.
+00000440: 6805 288a 0800 b058 30aa 67ea 154e 4e4b  h.(....X0.g..NNK
+00000450: 0a74 9452 9468 0528 8a08 00b0 8129 ba8d  .t.R.h.(.....)..
+00000460: ec15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000470: b0aa 22ca b3ee 154e 4e4b 0a74 9452 9468  .."....NNK.t.R.h
+00000480: 0528 8a08 00b0 d31b dad9 f015 4e4e 4b0a  .(..........NNK.
+00000490: 7494 5294 6805 288a 0800 b0fc 14ea fff2  t.R.h.(.........
 000004a0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000004b0: d171 bb6a 8515 4e4e 4b0a 7494 5294 6805  .q.j..NNK.t.R.h.
-000004c0: 288a 0800 b027 b818 9560 164e 4e4b 0a74  (....'...`.NNK.t
-000004d0: 9452 9468 0528 8a08 00b0 fd69 79b7 2816  .R.h.(.....iy.(.
-000004e0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0cd  NNK.t.R.h.(.....
-000004f0: 4677 9cd4 164e 4e4b 0a74 9452 9468 0528  Fw...NNK.t.R.h.(
-00000500: 8a08 00b0 1366 d85d 7a16 4e4e 4b0a 7494  .....f.]z.NNK.t.
-00000510: 5294 6805 288a 0800 b00c 3ce6 6828 174e  R.h.(.....<.h(.N
-00000520: 4e4b 0a74 9452 9468 0528 8a08 00b0 accc  NK.t.R.h.(......
-00000530: e822 5a16 4e4e 4b0a 7494 5294 6805 288a  ."Z.NNK.t.R.h.(.
-00000540: 0800 b02d b674 e2a2 174e 4e4b 0a74 9452  ...-.t...NNK.t.R
-00000550: 9468 0528 8a08 00b0 9e78 0439 b617 4e4e  .h.(.....x.9..NN
-00000560: 4b0a 7494 5294 6805 288a 0800 b009 3d38  K.t.R.h.(.....=8
-00000570: 4287 164e 4e4b 0a74 9452 9468 0528 8a08  B..NNK.t.R.h.(..
-00000580: 00b0 0be7 56b1 f216 4e4e 4b0a 7494 5294  ....V...NNK.t.R.
-00000590: 6805 288a 0800 b038 0bab a5a5 154e 4e4b  h.(....8.....NNK
-000005a0: 0a74 9452 9468 0528 8a08 00b0 80fd 23e6  .t.R.h.(......#.
-000005b0: dc17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000005c0: b061 2db4 dbcd 174e 4e4b 0a74 9452 9468  .a-....NNK.t.R.h
-000005d0: 0528 8a08 00b0 1211 49a6 4416 4e4e 4b0a  .(......I.D.NNK.
-000005e0: 7494 5294 6805 288a 0800 b095 a4f3 d4f8  t.R.h.(.........
-000005f0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000600: ccf1 e7e4 9e16 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00000610: 288a 0800 b077 001a 72f9 154e 4e4b 0a74  (....w..r..NNK.t
-00000620: 9452 9468 0528 8a08 00b0 ff13 9826 9416  .R.h.(.......&..
-00000630: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d4  NNK.t.R.h.(.....
-00000640: 9962 a14c 184e 4e4b 0a74 9452 9468 0528  .b.L.NNK.t.R.h.(
-00000650: 8a08 00b0 3f5e 96aa 1d17 4e4e 4b0a 7494  ....?^....NNK.t.
-00000660: 5294 6805 288a 0800 b09a 24c7 5adf 164e  R.h.(.....$.Z..N
-00000670: 4e4b 0a74 9452 9468 0528 8a08 00b0 4e07  NK.t.R.h.(....N.
-00000680: 0a4c f715 4e4e 4b0a 7494 5294 6805 288a  .L..NNK.t.R.h.(.
-00000690: 0800 b018 0fa5 f386 174e 4e4b 0a74 9452  .........NNK.t.R
-000006a0: 9468 0528 8a08 00b0 1f39 97e8 d816 4e4e  .h.(.....9....NN
-000006b0: 4b0a 7494 5294 6805 288a 0800 b010 672a  K.t.R.h.(.....g*
-000006c0: 37d9 154e 4e4b 0a74 9452 9468 0528 8a08  7..NNK.t.R.h.(..
-000006d0: 00b0 d5c5 f848 5c16 4e4e 4b0a 7494 5294  .....H\.NNK.t.R.
-000006e0: 6805 288a 0800 b0d4 7069 9126 164e 4e4b  h.(.....pi.&.NNK
-000006f0: 0a74 9452 9468 0528 8a08 00b0 857d f76b  .t.R.h.(.....}.k
-00000700: c316 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000710: b08b 525a a9df 154e 4e4b 0a74 9452 9468  ..RZ...NNK.t.R.h
-00000720: 0528 8a08 00b0 712b b734 dd16 4e4e 4b0a  .(....q+.4..NNK.
-00000730: 7494 5294 6805 288a 0800 b0a4 4d67 76d2  t.R.h.(.....Mgv.
+000004b0: 250e fa25 f515 4e4e 4b0a 7494 5294 6805  %..%..NNK.t.R.h.
+000004c0: 288a 0800 b04e 070a 4cf7 154e 4e4b 0a74  (....N..L..NNK.t
+000004d0: 9452 9468 0528 8a08 00b0 7700 1a72 f915  .R.h.(....w..r..
+000004e0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a0  NNK.t.R.h.(.....
+000004f0: f929 98fb 154e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
+00000500: 8a08 00b0 c9f2 39be fd15 4e4e 4b0a 7494  ......9...NNK.t.
+00000510: 5294 6805 288a 0800 b0f2 eb49 e4ff 154e  R.h.(......I...N
+00000520: 4e4b 0a74 9452 9468 0528 8a08 00b0 cc53  NK.t.R.h.(.....S
+00000530: c5bb 0116 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00000540: 0800 b044 de69 3004 164e 4e4b 0a74 9452  ...D.i0..NNK.t.R
+00000550: 9468 0528 8a08 00b0 6dd7 7956 0616 4e4e  .h.(....m.yV..NN
+00000560: 4b0a 7494 5294 6805 288a 0800 b096 d089  K.t.R.h.(.......
+00000570: 7c08 164e 4e4b 0a74 9452 9468 0528 8a08  |..NNK.t.R.h.(..
+00000580: 00b0 bfc9 99a2 0a16 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00000590: 6805 288a 0800 b0e8 c2a9 c80c 164e 4e4b  h.(..........NNK
+000005a0: 0a74 9452 9468 0528 8a08 00b0 11bc b9ee  .t.R.h.(........
+000005b0: 0e16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000005c0: b03a b5c9 1411 164e 4e4b 0a74 9452 9468  .:.....NNK.t.R.h
+000005d0: 0528 8a08 00b0 63ae d93a 1316 4e4e 4b0a  .(....c..:..NNK.
+000005e0: 7494 5294 6805 288a 0800 b08c a7e9 6015  t.R.h.(.......`.
+000005f0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000600: b5a0 f986 1716 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00000610: 288a 0800 b0de 9909 ad19 164e 4e4b 0a74  (..........NNK.t
+00000620: 9452 9468 0528 8a08 00b0 0793 19d3 1b16  .R.h.(..........
+00000630: 4e4e 4b0a 7494 5294 6805 288a 0800 b030  NNK.t.R.h.(....0
+00000640: 8c29 f91d 164e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
+00000650: 8a08 00b0 5985 391f 2016 4e4e 4b0a 7494  ....Y.9. .NNK.t.
+00000660: 5294 6805 288a 0800 b082 7e49 4522 164e  R.h.(.....~IE".N
+00000670: 4e4b 0a74 9452 9468 0528 8a08 00b0 ab77  NK.t.R.h.(.....w
+00000680: 596b 2416 4e4e 4b0a 7494 5294 6805 288a  Yk$.NNK.t.R.h.(.
+00000690: 0800 b0d4 7069 9126 164e 4e4b 0a74 9452  ....pi.&.NNK.t.R
+000006a0: 9468 0528 8a08 00b0 fd69 79b7 2816 4e4e  .h.(.....iy.(.NN
+000006b0: 4b0a 7494 5294 6805 288a 0800 b026 6389  K.t.R.h.(....&c.
+000006c0: dd2a 164e 4e4b 0a74 9452 9468 0528 8a08  .*.NNK.t.R.h.(..
+000006d0: 00b0 4f5c 9903 2d16 4e4e 4b0a 7494 5294  ..O\..-.NNK.t.R.
+000006e0: 6805 288a 0800 b078 55a9 292f 164e 4e4b  h.(....xU.)/.NNK
+000006f0: 0a74 9452 9468 0528 8a08 00b0 a14e b94f  .t.R.h.(.....N.O
+00000700: 3116 4e4e 4b0a 7494 5294 6805 288a 0800  1.NNK.t.R.h.(...
+00000710: b0ca 47c9 7533 164e 4e4b 0a74 9452 9468  ..G.u3.NNK.t.R.h
+00000720: 0528 8a08 00b0 f340 d99b 3516 4e4e 4b0a  .(.....@..5.NNK.
+00000730: 7494 5294 6805 288a 0800 b01c 3ae9 c137  t.R.h.(.....:..7
 00000740: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000750: b9f4 3665 ee16 4e4e 4b0a 7494 5294 6805  ..6e..NNK.t.R.h.
-00000760: 288a 0800 b002 1346 4d35 174e 4e4b 0a74  (......FM5.NNK.t
-00000770: 9452 9468 0528 8a08 00b0 3834 a4b5 cb17  .R.h.(....84....
-00000780: 4e4e 4b0a 7494 5294 6805 288a 0800 b026  NNK.t.R.h.(....&
-00000790: c566 b48d 154e 4e4b 0a74 9452 9468 0528  .f...NNK.t.R.h.(
-000007a0: 8a08 00b0 2364 dbb6 8915 4e4e 4b0a 7494  ....#d....NNK.t.
-000007b0: 5294 6805 288a 0800 b09e 4f0b 2990 154e  R.h.(.....O.)..N
-000007c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 b3f6  NK.t.R.h.(......
-000007d0: da17 ac15 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-000007e0: 0800 b099 cf37 a3a9 164e 4e4b 0a74 9452  .....7...NNK.t.R
-000007f0: 9468 0528 8a08 00b0 525b 472a ce16 4e4e  .h.(....R[G*..NN
-00000800: 4b0a 7494 5294 6805 288a 0800 b053 b0d6  K.t.R.h.(....S..
-00000810: e103 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000820: 00b0 7280 46ec 1217 4e4e 4b0a 7494 5294  ..r.F...NNK.t.R.
-00000830: 6805 288a 0800 b003 68d5 046b 174e 4e4b  h.(.....h..k.NNK
-00000840: 0a74 9452 9468 0528 8a08 00b0 208e 26a0  .t.R.h.(.... .&.
-00000850: 0e17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000860: b0bf c999 a20a 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00000870: 0528 8a08 00b0 ab77 596b 2416 4e4e 4b0a  .(.....wYk$.NNK.
-00000880: 7494 5294 6805 288a 0800 b0cb 9c58 2d69  t.R.h.(......X-i
+00000750: 4533 f9e7 3916 4e4e 4b0a 7494 5294 6805  E3..9.NNK.t.R.h.
+00000760: 288a 0800 b06e 2c09 0e3c 164e 4e4b 0a74  (....n,..<.NNK.t
+00000770: 9452 9468 0528 8a08 00b0 9725 1934 3e16  .R.h.(.....%.4>.
+00000780: 4e4e 4b0a 7494 5294 6805 288a 0800 b0c0  NNK.t.R.h.(.....
+00000790: 1e29 5a40 164e 4e4b 0a74 9452 9468 0528  .)Z@.NNK.t.R.h.(
+000007a0: 8a08 00b0 e917 3980 4216 4e4e 4b0a 7494  ......9.B.NNK.t.
+000007b0: 5294 6805 288a 0800 b012 1149 a644 164e  R.h.(......I.D.N
+000007c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 3b0a  NK.t.R.h.(....;.
+000007d0: 59cc 4616 4e4e 4b0a 7494 5294 6805 288a  Y.F.NNK.t.R.h.(.
+000007e0: 0800 b064 0369 f248 164e 4e4b 0a74 9452  ...d.i.H.NNK.t.R
+000007f0: 9468 0528 8a08 00b0 8dfc 7818 4b16 4e4e  .h.(......x.K.NN
+00000800: 4b0a 7494 5294 6805 288a 0800 b0b6 f588  K.t.R.h.(.......
+00000810: 3e4d 164e 4e4b 0a74 9452 9468 0528 8a08  >M.NNK.t.R.h.(..
+00000820: 00b0 dfee 9864 4f16 4e4e 4b0a 7494 5294  .....dO.NNK.t.R.
+00000830: 6805 288a 0800 b008 e8a8 8a51 164e 4e4b  h.(........Q.NNK
+00000840: 0a74 9452 9468 0528 8a08 00b0 31e1 b8b0  .t.R.h.(....1...
+00000850: 5316 4e4e 4b0a 7494 5294 6805 288a 0800  S.NNK.t.R.h.(...
+00000860: b05a dac8 d655 164e 4e4b 0a74 9452 9468  .Z...U.NNK.t.R.h
+00000870: 0528 8a08 00b0 83d3 d8fc 5716 4e4e 4b0a  .(........W.NNK.
+00000880: 7494 5294 6805 288a 0800 b0ac cce8 225a  t.R.h.(......."Z
 00000890: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000008a0: ebc1 57ef ad16 4e4e 4b0a 7494 5294 6805  ..W...NNK.t.R.h.
-000008b0: 288a 0800 b090 fb26 3fec 164e 4e4b 0a74  (......&?..NNK.t
-000008c0: 9452 9468 0528 8a08 00b0 2663 89dd 2a16  .R.h.(....&c..*.
-000008d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b07b  NNK.t.R.h.(....{
-000008e0: 7d50 60f6 184e 4e4b 0a74 9452 9468 0528  }P`..NNK.t.R.h.(
-000008f0: 8a08 00b0 0ee6 04d8 9317 4e4e 4b0a 7494  ..........NNK.t.
-00000900: 5294 6805 288a 0800 b04a dcc5 7d46 174e  R.h.(....J..}F.N
-00000910: 4e4b 0a74 9452 9468 0528 8a08 00b0 05e9  NK.t.R.h.(......
-00000920: fa63 b015 4e4e 4b0a 7494 5294 6805 288a  .c..NNK.t.R.h.(.
-00000930: 0800 b0c6 7e62 7ee5 164e 4e4b 0a74 9452  ....~b~..NNK.t.R
-00000940: 9468 0528 8a08 00b0 9cce e5c9 4a17 4e4e  .h.(........J.NN
-00000950: 4b0a 7494 5294 6805 288a 0800 b045 33f9  K.t.R.h.(....E3.
-00000960: e739 164e 4e4b 0a74 9452 9468 0528 8a08  .9.NNK.t.R.h.(..
-00000970: 00b0 3b0a 59cc 4616 4e4e 4b0a 7494 5294  ..;.Y.F.NNK.t.R.
-00000980: 6805 288a 0800 b0a5 a2f6 2d08 174e 4e4b  h.(.......-..NNK
-00000990: 0a74 9452 9468 0528 8a08 00b0 f8e9 a531  .t.R.h.(.......1
-000009a0: 4217 4e4e 4b0a 7494 5294 6805 288a 0800  B.NNK.t.R.h.(...
-000009b0: b0bc f3e4 8b8f 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-000009c0: 0528 8a08 00b0 5106 b872 9816 4e4e 4b0a  .(....Q..r..NNK.
-000009d0: 7494 5294 6805 288a 0800 b047 dd17 57a5  t.R.h.(....G..W.
+000008a0: d5c5 f848 5c16 4e4e 4b0a 7494 5294 6805  ...H\.NNK.t.R.h.
+000008b0: 288a 0800 b0fe be08 6f5e 164e 4e4b 0a74  (.......o^.NNK.t
+000008c0: 9452 9468 0528 8a08 00b0 27b8 1895 6016  .R.h.(....'...`.
+000008d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b050  NNK.t.R.h.(....P
+000008e0: b128 bb62 164e 4e4b 0a74 9452 9468 0528  .(.b.NNK.t.R.h.(
+000008f0: 8a08 00b0 79aa 38e1 6416 4e4e 4b0a 7494  ....y.8.d.NNK.t.
+00000900: 5294 6805 288a 0800 b0a2 a348 0767 164e  R.h.(......H.g.N
+00000910: 4e4b 0a74 9452 9468 0528 8a08 00b0 cb9c  NK.t.R.h.(......
+00000920: 582d 6916 4e4e 4b0a 7494 5294 6805 288a  X-i.NNK.t.R.h.(.
+00000930: 0800 b0a5 04d4 046b 164e 4e4b 0a74 9452  .......k.NNK.t.R
+00000940: 9468 0528 8a08 00b0 1d8f 7879 6d16 4e4e  .h.(......xym.NN
+00000950: 4b0a 7494 5294 6805 288a 0800 b046 8888  K.t.R.h.(....F..
+00000960: 9f6f 164e 4e4b 0a74 9452 9468 0528 8a08  .o.NNK.t.R.h.(..
+00000970: 00b0 6f81 98c5 7116 4e4e 4b0a 7494 5294  ..o...q.NNK.t.R.
+00000980: 6805 288a 0800 b098 7aa8 eb73 164e 4e4b  h.(.....z..s.NNK
+00000990: 0a74 9452 9468 0528 8a08 00b0 c173 b811  .t.R.h.(.....s..
+000009a0: 7616 4e4e 4b0a 7494 5294 6805 288a 0800  v.NNK.t.R.h.(...
+000009b0: b0ea 6cc8 3778 164e 4e4b 0a74 9452 9468  ..l.7x.NNK.t.R.h
+000009c0: 0528 8a08 00b0 1366 d85d 7a16 4e4e 4b0a  .(.....f.]z.NNK.
+000009d0: 7494 5294 6805 288a 0800 b03c 5fe8 837c  t.R.h.(....<_..|
 000009e0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000009f0: b6f5 883e 4d16 4e4e 4b0a 7494 5294 6805  ...>M.NNK.t.R.h.
-00000a00: 288a 0800 b075 7ff4 12b4 174e 4e4b 0a74  (....u.....NNK.t
-00000a10: 9452 9468 0528 8a08 00b0 1665 8684 1b17  .R.h.(.....e....
-00000a20: 4e4e 4b0a 7494 5294 6805 288a 0800 b055  NNK.t.R.h.(....U
-00000a30: 5af5 506f 174e 4e4b 0a74 9452 9468 0528  Z.Po.NNK.t.R.h.(
-00000a40: 8a08 00b0 c9f2 39be fd15 4e4e 4b0a 7494  ......9...NNK.t.
-00000a50: 5294 6805 288a 0800 b03e 0907 f3e7 164e  R.h.(....>.....N
-00000a60: 4e4b 0a74 9452 9468 0528 8a08 00b0 e618  NK.t.R.h.(......
-00000a70: 8b59 a115 4e4e 4b0a 7494 5294 6805 288a  .Y..NNK.t.R.h.(.
-00000a80: 0800 b001 beb6 95ff 164e 4e4b 0a74 9452  .........NNK.t.R
-00000a90: 9468 0528 8a08 00b0 ce9b 0654 0a17 4e4e  .h.(.......T..NN
-00000aa0: 4b0a 7494 5294 6805 288a 0800 b0c6 1c85  K.t.R.h.(.......
-00000ab0: a782 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000ac0: 00b0 24b9 6a6e bf15 4e4e 4b0a 7494 5294  ..$.jn..NNK.t.R.
-00000ad0: 6805 288a 0800 b0d7 6f17 b8c7 164e 4e4b  h.(.....o....NNK
-00000ae0: 0a74 9452 9468 0528 8a08 00b0 0069 27de  .t.R.h.(.....i'.
-00000af0: c916 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000b00: b04b 3155 357c 174e 4e4b 0a74 9452 9468  .K1U5|.NNK.t.R.h
-00000b10: 0528 8a08 00b0 ddcf 50dc 6c17 4e4e 4b0a  .(......P.l.NNK.
-00000b20: 7494 5294 6805 288a 0800 b0dc 18e4 4dd4  t.R.h.(.......M.
-00000b30: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000b40: c31d d780 e116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00000b50: 288a 0800 b05f 8395 6c62 174e 4e4b 0a74  (...._..lb.NNK.t
-00000b60: 9452 9468 0528 8a08 00b0 febe 086f 5e16  .R.h.(.......o^.
-00000b70: 4e4e 4b0a 7494 5294 6805 288a 0800 b0c7  NNK.t.R.h.(.....
-00000b80: 7114 5fb8 174e 4e4b 0a74 9452 9468 0528  q._..NNK.t.R.h.(
-00000b90: 8a08 00b0 11bc b9ee 0e16 4e4e 4b0a 7494  ..........NNK.t.
-00000ba0: 5294 6805 288a 0800 b086 d286 23f9 164e  R.h.(.......#..N
-00000bb0: 4e4b 0a74 9452 9468 0528 8a08 00b0 fa6a  NK.t.R.h.(.....j
-00000bc0: cb90 8715 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00000bd0: 0800 b043 89da 78ce 154e 4e4b 0a74 9452  ...C..x..NNK.t.R
-00000be0: 9468 0528 8a08 00b0 e497 65fa 5b17 4e4e  .h.(......e.[.NN
-00000bf0: 4b0a 7494 5294 6805 288a 0800 b0f0 6a24  K.t.R.h.(.....j$
-00000c00: 85ba 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000c10: 00b0 171c f312 b416 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00000c20: 6805 288a 0800 b0a0 f929 98fb 154e 4e4b  h.(......)...NNK
-00000c30: 0a74 9452 9468 0528 8a08 00b0 fa93 c4a0  .t.R.h.(........
-00000c40: ad17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000c50: b054 6743 709c 164e 4e4b 0a74 9452 9468  .TgCp..NNK.t.R.h
-00000c60: 0528 8a08 00b0 da6e c5de 6817 4e4e 4b0a  .(.....n..h.NNK.
-00000c70: 7494 5294 6805 288a 0800 b0d8 c4a6 6ffd  t.R.h.(.......o.
+000009f0: 16c7 635b 7e16 4e4e 4b0a 7494 5294 6805  ..c[~.NNK.t.R.h.
+00000a00: 288a 0800 b08e 5108 d080 164e 4e4b 0a74  (.....Q....NNK.t
+00000a10: 9452 9468 0528 8a08 00b0 b74a 18f6 8216  .R.h.(.....J....
+00000a20: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e0  NNK.t.R.h.(.....
+00000a30: 4328 1c85 164e 4e4b 0a74 9452 9468 0528  C(...NNK.t.R.h.(
+00000a40: 8a08 00b0 093d 3842 8716 4e4e 4b0a 7494  .....=8B..NNK.t.
+00000a50: 5294 6805 288a 0800 b032 3648 6889 164e  R.h.(....26Hh..N
+00000a60: 4e4b 0a74 9452 9468 0528 8a08 00b0 5b2f  NK.t.R.h.(....[/
+00000a70: 588e 8b16 4e4e 4b0a 7494 5294 6805 288a  X...NNK.t.R.h.(.
+00000a80: 0800 b084 2868 b48d 164e 4e4b 0a74 9452  ....(h...NNK.t.R
+00000a90: 9468 0528 8a08 00b0 ad21 78da 8f16 4e4e  .h.(.....!x...NN
+00000aa0: 4b0a 7494 5294 6805 288a 0800 b0d6 1a88  K.t.R.h.(.......
+00000ab0: 0092 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00000ac0: 00b0 ff13 9826 9416 4e4e 4b0a 7494 5294  .....&..NNK.t.R.
+00000ad0: 6805 288a 0800 b028 0da8 4c96 164e 4e4b  h.(....(..L..NNK
+00000ae0: 0a74 9452 9468 0528 8a08 00b0 5106 b872  .t.R.h.(....Q..r
+00000af0: 9816 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000b00: b07a ffc7 989a 164e 4e4b 0a74 9452 9468  .z.....NNK.t.R.h
+00000b10: 0528 8a08 00b0 5467 4370 9c16 4e4e 4b0a  .(....TgCp..NNK.
+00000b20: 7494 5294 6805 288a 0800 b0cc f1e7 e49e  t.R.h.(.........
+00000b30: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000b40: f5ea f70a a116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00000b50: 288a 0800 b01e e407 31a3 164e 4e4b 0a74  (.......1..NNK.t
+00000b60: 9452 9468 0528 8a08 00b0 47dd 1757 a516  .R.h.(....G..W..
+00000b70: 4e4e 4b0a 7494 5294 6805 288a 0800 b070  NNK.t.R.h.(....p
+00000b80: d627 7da7 164e 4e4b 0a74 9452 9468 0528  .'}..NNK.t.R.h.(
+00000b90: 8a08 00b0 99cf 37a3 a916 4e4e 4b0a 7494  ......7...NNK.t.
+00000ba0: 5294 6805 288a 0800 b0c2 c847 c9ab 164e  R.h.(......G...N
+00000bb0: 4e4b 0a74 9452 9468 0528 8a08 00b0 ebc1  NK.t.R.h.(......
+00000bc0: 57ef ad16 4e4e 4b0a 7494 5294 6805 288a  W...NNK.t.R.h.(.
+00000bd0: 0800 b014 bb67 15b0 164e 4e4b 0a74 9452  .....g...NNK.t.R
+00000be0: 9468 0528 8a08 00b0 3db4 773b b216 4e4e  .h.(....=.w;..NN
+00000bf0: 4b0a 7494 5294 6805 288a 0800 b017 1cf3  K.t.R.h.(.......
+00000c00: 12b4 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00000c10: 00b0 8fa6 9787 b616 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00000c20: 6805 288a 0800 b0b8 9fa7 adb8 164e 4e4b  h.(..........NNK
+00000c30: 0a74 9452 9468 0528 8a08 00b0 e198 b7d3  .t.R.h.(........
+00000c40: ba16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000c50: b00a 92c7 f9bc 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00000c60: 0528 8a08 00b0 338b d71f bf16 4e4e 4b0a  .(....3.....NNK.
+00000c70: 7494 5294 6805 288a 0800 b05c 84e7 45c1  t.R.h.(....\..E.
 00000c80: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000c90: af56 6d30 8418 4e4e 4b0a 7494 5294 6805  .Vm0..NNK.t.R.h.
-00000ca0: 288a 0800 b0ba 49c6 1c24 174e 4e4b 0a74  (.....I..$.NNK.t
-00000cb0: 9452 9468 0528 8a08 00b0 70d6 277d a716  .R.h.(....p.'}..
-00000cc0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
-00000cd0: 412b 7594 154e 4e4b 0a74 9452 9468 0528  A+u..NNK.t.R.h.(
-00000ce0: 8a08 00b0 be74 0aeb d415 4e4e 4b0a 7494  .....t....NNK.t.
-00000cf0: 5294 6805 288a 0800 b05e 2e06 b52c 174e  R.h.(....^...,.N
-00000d00: 4e4b 0a74 9452 9468 0528 8a08 00b0 7dfe  NK.t.R.h.(....}.
-00000d10: 75bf 3b17 4e4e 4b0a 7494 5294 6805 288a  u.;.NNK.t.R.h.(.
-00000d20: 0800 b0ed 6b76 5e19 174e 4e4b 0a74 9452  ....kv^..NNK.t.R
-00000d30: 9468 0528 8a08 00b0 ef15 95cd 8417 4e4e  .h.(..........NN
-00000d40: 4b0a 7494 5294 6805 288a 0800 b056 af84  K.t.R.h.(....V..
-00000d50: 08a5 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000d60: 00b0 063e 8a1b e615 4e4e 4b0a 7494 5294  ...>....NNK.t.R.
-00000d70: 6805 288a 0800 b0dd 447a f5e3 154e 4e4b  h.(.....Dz...NNK
-00000d80: 0a74 9452 9468 0528 8a08 00b0 8e51 08d0  .t.R.h.(.....Q..
-00000d90: 8016 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000da0: b0ae 7607 92c5 164e 4e4b 0a74 9452 9468  ..v....NNK.t.R.h
-00000db0: 0528 8a08 00b0 8727 16db 2e17 4e4e 4b0a  .(.....'....NNK.
-00000dc0: 7494 5294 6805 288a 0800 b058 30aa 67ea  t.R.h.(....X0.g.
-00000dd0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000de0: e342 d642 2617 4e4e 4b0a 7494 5294 6805  .B.B&.NNK.t.R.h.
-00000df0: 288a 0800 b016 c763 5b7e 164e 4e4b 0a74  (......c[~.NNK.t
-00000e00: 9452 9468 0528 8a08 00b0 e043 281c 8516  .R.h.(.....C(...
-00000e10: 4e4e 4b0a 7494 5294 6805 288a 0800 b057  NNK.t.R.h.(....W
-00000e20: db1a b0b4 154e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00000e30: 8a08 00b0 5b2f 588e 8b16 4e4e 4b0a 7494  ....[/X...NNK.t.
-00000e40: 5294 6805 288a 0800 b092 a545 ae57 174e  R.h.(......E.W.N
-00000e50: 4e4b 0a74 9452 9468 0528 8a08 00b0 2238  NK.t.R.h.(...."8
-00000e60: 450f 7a17 4e4e 4b0a 7494 5294 6805 288a  E.z.NNK.t.R.h.(.
-00000e70: 0800 b08c a7e9 6015 164e 4e4b 0a74 9452  ......`..NNK.t.R
-00000e80: 9468 0528 8a08 00b0 0793 19d3 1b16 4e4e  .h.(..........NN
-00000e90: 4b0a 7494 5294 6805 288a 0800 b040 b325  K.t.R.h.(....@.%
-00000ea0: 6253 174e 4e4b 0a74 9452 9468 0528 8a08  bS.NNK.t.R.h.(..
-00000eb0: 00b0 e198 b7d3 ba16 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00000ec0: 6805 288a 0800 b093 fad4 658d 174e 4e4b  h.(.......e..NNK
-00000ed0: 0a74 9452 9468 0528 8a08 00b0 425d 44d1  .t.R.h.(....B]D.
-00000ee0: be17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000ef0: b00f 3b94 8fc9 174e 4e4b 0a74 9452 9468  ..;....NNK.t.R.h
-00000f00: 0528 8a08 00b0 4688 889f 6f16 4e4e 4b0a  .(....F...o.NNK.
-00000f10: 7494 5294 6805 288a 0800 b07c d2df 172c  t.R.h.(....|...,
-00000f20: 194e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000f30: 827e 4945 2216 4e4e 4b0a 7494 5294 6805  .~IE".NNK.t.R.h.
-00000f40: 288a 0800 b06e b7df f4c4 174e 4e4b 0a74  (....n.....NNK.t
-00000f50: 9452 9468 0528 8a08 00b0 a9cd 3afc b815  .R.h.(......:...
-00000f60: 4e4e 4b0a 7494 5294 6805 288a 0800 b01a  NNK.t.R.h.(.....
-00000f70: 90ca 52cc 154e 4e4b 0a74 9452 9468 0528  ..R..NNK.t.R.h.(
-00000f80: 8a08 00b0 a878 ab44 8315 4e4e 4b0a 7494  .....x.D..NNK.t.
-00000f90: 5294 6805 288a 0800 b0af cb96 49fb 164e  R.h.(.......I..N
-00000fa0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2ab7  NK.t.R.h.(....*.
-00000fb0: c6bb 0117 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00000c90: 857d f76b c316 4e4e 4b0a 7494 5294 6805  .}.k..NNK.t.R.h.
+00000ca0: 288a 0800 b0ae 7607 92c5 164e 4e4b 0a74  (.....v....NNK.t
+00000cb0: 9452 9468 0528 8a08 00b0 d76f 17b8 c716  .R.h.(.....o....
+00000cc0: 4e4e 4b0a 7494 5294 6805 288a 0800 b000  NNK.t.R.h.(.....
+00000cd0: 6927 dec9 164e 4e4b 0a74 9452 9468 0528  i'...NNK.t.R.h.(
+00000ce0: 8a08 00b0 2962 3704 cc16 4e4e 4b0a 7494  ....)b7...NNK.t.
+00000cf0: 5294 6805 288a 0800 b052 5b47 2ace 164e  R.h.(....R[G*..N
+00000d00: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b54  NK.t.R.h.(....{T
+00000d10: 5750 d016 4e4e 4b0a 7494 5294 6805 288a  WP..NNK.t.R.h.(.
+00000d20: 0800 b0a4 4d67 76d2 164e 4e4b 0a74 9452  ....Mgv..NNK.t.R
+00000d30: 9468 0528 8a08 00b0 cd46 779c d416 4e4e  .h.(.....Fw...NN
+00000d40: 4b0a 7494 5294 6805 288a 0800 b0f6 3f87  K.t.R.h.(.....?.
+00000d50: c2d6 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00000d60: 00b0 1f39 97e8 d816 4e4e 4b0a 7494 5294  ...9....NNK.t.R.
+00000d70: 6805 288a 0800 b048 32a7 0edb 164e 4e4b  h.(....H2....NNK
+00000d80: 0a74 9452 9468 0528 8a08 00b0 712b b734  .t.R.h.(....q+.4
+00000d90: dd16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000da0: b09a 24c7 5adf 164e 4e4b 0a74 9452 9468  ..$.Z..NNK.t.R.h
+00000db0: 0528 8a08 00b0 c31d d780 e116 4e4e 4b0a  .(..........NNK.
+00000dc0: 7494 5294 6805 288a 0800 b0ec 16e7 a6e3  t.R.h.(.........
+00000dd0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000de0: c67e 627e e516 4e4e 4b0a 7494 5294 6805  .~b~..NNK.t.R.h.
+00000df0: 288a 0800 b03e 0907 f3e7 164e 4e4b 0a74  (....>.....NNK.t
+00000e00: 9452 9468 0528 8a08 00b0 6702 1719 ea16  .R.h.(....g.....
+00000e10: 4e4e 4b0a 7494 5294 6805 288a 0800 b090  NNK.t.R.h.(.....
+00000e20: fb26 3fec 164e 4e4b 0a74 9452 9468 0528  .&?..NNK.t.R.h.(
+00000e30: 8a08 00b0 b9f4 3665 ee16 4e4e 4b0a 7494  ......6e..NNK.t.
+00000e40: 5294 6805 288a 0800 b0e2 ed46 8bf0 164e  R.h.(......F...N
+00000e50: 4e4b 0a74 9452 9468 0528 8a08 00b0 0be7  NK.t.R.h.(......
+00000e60: 56b1 f216 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
+00000e70: 0800 b034 e066 d7f4 164e 4e4b 0a74 9452  ...4.f...NNK.t.R
+00000e80: 9468 0528 8a08 00b0 5dd9 76fd f616 4e4e  .h.(....].v...NN
+00000e90: 4b0a 7494 5294 6805 288a 0800 b086 d286  K.t.R.h.(.......
+00000ea0: 23f9 164e 4e4b 0a74 9452 9468 0528 8a08  #..NNK.t.R.h.(..
+00000eb0: 00b0 afcb 9649 fb16 4e4e 4b0a 7494 5294  .....I..NNK.t.R.
+00000ec0: 6805 288a 0800 b0d8 c4a6 6ffd 164e 4e4b  h.(.......o..NNK
+00000ed0: 0a74 9452 9468 0528 8a08 00b0 01be b695  .t.R.h.(........
+00000ee0: ff16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000ef0: b02a b7c6 bb01 174e 4e4b 0a74 9452 9468  .*.....NNK.t.R.h
+00000f00: 0528 8a08 00b0 53b0 d6e1 0317 4e4e 4b0a  .(....S.....NNK.
+00000f10: 7494 5294 6805 288a 0800 b07c a9e6 0706  t.R.h.(....|....
+00000f20: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000f30: a5a2 f62d 0817 4e4e 4b0a 7494 5294 6805  ...-..NNK.t.R.h.
+00000f40: 288a 0800 b0ce 9b06 540a 174e 4e4b 0a74  (.......T..NNK.t
+00000f50: 9452 9468 0528 8a08 00b0 f794 167a 0c17  .R.h.(.......z..
+00000f60: 4e4e 4b0a 7494 5294 6805 288a 0800 b020  NNK.t.R.h.(.... 
+00000f70: 8e26 a00e 174e 4e4b 0a74 9452 9468 0528  .&...NNK.t.R.h.(
+00000f80: 8a08 00b0 4987 36c6 1017 4e4e 4b0a 7494  ....I.6...NNK.t.
+00000f90: 5294 6805 288a 0800 b072 8046 ec12 174e  R.h.(....r.F...N
+00000fa0: 4e4b 0a74 9452 9468 0528 8a08 00b0 9b79  NK.t.R.h.(.....y
+00000fb0: 5612 1517 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
 00000fc0: 0800 b0c4 7266 3817 174e 4e4b 0a74 9452  ....rf8..NNK.t.R
-00000fd0: 9468 0528 8a08 00b0 f2eb 49e4 ff15 4e4e  .h.(......I...NN
-00000fe0: 4b0a 7494 5294 6805 288a 0800 b03c 5fe8  K.t.R.h.(....<_.
-00000ff0: 837c 164e 4e4b 0a74 9452 9468 0528 8a08  .|.NNK.t.R.h.(..
-00001000: 00b0 6259 4a83 dd15 4e4e 4b0a 7494 5294  ..bYJ...NNK.t.R.
-00001010: 6805 288a 0800 b021 e3b5 5744 174e 4e4b  h.(....!..WD.NNK
-00001020: 0a74 9452 9468 0528 8a08 00b0 e5ec f4b1  .t.R.h.(........
-00001030: 9117 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001040: b044 de69 3004 164e 4e4b 0a74 9452 9468  .D.i0..NNK.t.R.h
-00001050: 0528 8a08 00b0 2962 3704 cc16 4e4e 4b0a  .(....)b7...NNK.
-00001060: 7494 5294 6805 288a 0800 b07b 5457 50d0  t.R.h.(....{TWP.
-00001070: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001080: cff0 950b 4017 4e4e 4b0a 7494 5294 6805  ....@.NNK.t.R.h.
-00001090: 288a 0800 b069 ac35 8855 174e 4e4b 0a74  (....i.5.U.NNK.t
-000010a0: 9452 9468 0528 8a08 00b0 6104 bbcb a715  .R.h.(....a.....
-000010b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b039  NNK.t.R.h.(....9
-000010c0: 603a 5ddb 154e 4e4b 0a74 9452 9468 0528  `:]..NNK.t.R.h.(
-000010d0: 8a08 00b0 742a 655b 7e17 4e4e 4b0a 7494  ....t*e[~.NNK.t.
-000010e0: 5294 6805 288a 0800 b068 57a6 d01f 174e  R.h.(....hW....N
-000010f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 0d91  NK.t.R.h.(......
-00001100: 7520 5e17 4e4e 4b0a 7494 5294 6805 288a  u ^.NNK.t.R.h.(.
-00001110: 0800 b04c 86e4 ecb1 174e 4e4b 0a74 9452  ...L.....NNK.t.R
-00001120: 9468 0528 8a08 00b0 fc14 eaff f215 4e4e  .h.(..........NN
-00001130: 4b0a 7494 5294 6805 288a 0800 b0ad 2178  K.t.R.h.(.....!x
-00001140: da8f 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001150: 00b0 1ee4 0731 a316 4e4e 4b0a 7494 5294  .....1..NNK.t.R.
-00001160: 6805 288a 0800 b0cc 53c5 bb01 164e 4e4b  h.(.....S....NNK
-00001170: 0a74 9452 9468 0528 8a08 00b0 887c a592  .t.R.h.(.....|..
-00001180: 6417 4e4e 4b0a 7494 5294 6805 288a 0800  d.NNK.t.R.h.(...
-00001190: b0b1 75b5 b866 174e 4e4b 0a74 9452 9468  ..u..f.NNK.t.R.h
-000011a0: 0528 8a08 00b0 9b79 5612 1517 4e4e 4b0a  .(.....yV...NNK.
-000011b0: 7494 5294 6805 288a 0800 b03a b5c9 1411  t.R.h.(....:....
-000011c0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000011d0: 8fa6 9787 b616 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-000011e0: 288a 0800 b089 d134 4a9a 174e 4e4b 0a74  (......4J..NNK.t
-000011f0: 9452 9468 0528 8a08 00b0 c5c7 f5ef 4c17  .R.h.(........L.
-00001200: 4e4e 4b0a 7494 5294 6805 288a 0800 b07a  NNK.t.R.h.(....z
-00001210: ffc7 989a 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00001220: 8a08 00b0 4c5d ebdc 8b15 4e4e 4b0a 7494  ....L]....NNK.t.
-00001230: 5294 6805 288a 0800 b0d9 1936 2733 174e  R.h.(......6'3.N
-00001240: 4e4b 0a74 9452 9468 0528 8a08 00b0 957b  NK.t.R.h.(.....{
-00001250: fac4 d215 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00001260: 0800 b064 0369 f248 164e 4e4b 0a74 9452  ...d.i.H.NNK.t.R
-00001270: 9468 0528 8a08 00b0 4832 a70e db16 4e4e  .h.(....H2....NN
-00001280: 4b0a 7494 5294 6805 288a 0800 b06e 2c09  K.t.R.h.(....n,.
-00001290: 0e3c 164e 4e4b 0a74 9452 9468 0528 8a08  .<.NNK.t.R.h.(..
-000012a0: 00b0 c828 81ed 5017 4e4e 4b0a 7494 5294  ...(..P.NNK.t.R.
-000012b0: 6805 288a 0800 b04d b27a 94c1 154e 4e4b  h.(....M.z...NNK
-000012c0: 0a74 9452 9468 0528 8a08 00b0 b89f a7ad  .t.R.h.(........
-000012d0: b816 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000012e0: b019 6434 abbc 174e 4e4b 0a74 9452 9468  ..d4...NNK.t.R.h
-000012f0: 0528 8a08 00b0 8428 68b4 8d16 4e4e 4b0a  .(.....(h...NNK.
-00001300: 7494 5294 6805 288a 0800 b0e2 ed46 8bf0  t.R.h.(......F..
-00001310: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001320: 2f37 9a41 e815 4e4e 4b0a 7494 5294 6805  /7.A..NNK.t.R.h.
-00001330: 288a 0800 b01c 3ae9 c137 164e 4e4b 0a74  (.....:..7.NNK.t
-00001340: 9452 9468 0528 8a08 00b0 8dfc 7818 4b16  .R.h.(......x.K.
-00001350: 4e4e 4b0a 7494 5294 6805 288a 0800 b094  NNK.t.R.h.(.....
-00001360: 266b 0d9d 154e 4e4b 0a74 9452 9468 0528  &k...NNK.t.R.h.(
-00001370: 8a08 00b0 5766 f196 3d17 4e4e 4b0a 7494  ....Wf..=.NNK.t.
-00001380: 5294 6805 288a 0800 b0c8 9daa 06c8 154e  R.h.(..........N
-00001390: 4e4b 0a74 9452 9468 0528 8a08 00b0 dfee  NK.t.R.h.(......
-000013a0: 9864 4f16 4e4e 4b0a 7494 5294 6805 288a  .dO.NNK.t.R.h.(.
-000013b0: 0800 b059 8539 1f20 164e 4e4b 0a74 9452  ...Y.9. .NNK.t.R
-000013c0: 9468 0528 8a08 00b0 08e8 a88a 5116 4e4e  .h.(........Q.NN
-000013d0: 4b0a 7494 5294 6805 288a 0800 b079 aa38  K.t.R.h.(....y.8
-000013e0: e164 164e 4e4b 0a74 9452 9468 0528 8a08  .d.NNK.t.R.h.(..
-000013f0: 00b0 6f81 98c5 7116 4e4e 4b0a 7494 5294  ..o...q.NNK.t.R.
-00001400: 6805 288a 0800 b041 08b5 1989 174e 4e4b  h.(....A.....NNK
-00001410: 0a74 9452 9468 0528 8a08 00b0 2ee2 0a8a  .t.R.h.(........
-00001420: b215 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001430: b073 d5d5 a348 174e 4e4b 0a74 9452 9468  .s...H.NNK.t.R.h
-00001440: 0528 8a08 00b0 7fa8 942e a717 4e4e 4b0a  .(..........NNK.
-00001450: 7494 5294 6805 288a 0800 b06a 01c5 3f8b  t.R.h.(....j..?.
+00000fd0: 9468 0528 8a08 00b0 ed6b 765e 1917 4e4e  .h.(.....kv^..NN
+00000fe0: 4b0a 7494 5294 6805 288a 0800 b016 6586  K.t.R.h.(.....e.
+00000ff0: 841b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00001000: 00b0 3f5e 96aa 1d17 4e4e 4b0a 7494 5294  ..?^....NNK.t.R.
+00001010: 6805 288a 0800 b068 57a6 d01f 174e 4e4b  h.(....hW....NNK
+00001020: 0a74 9452 9468 0528 8a08 00b0 9150 b6f6  .t.R.h.(.....P..
+00001030: 2117 4e4e 4b0a 7494 5294 6805 288a 0800  !.NNK.t.R.h.(...
+00001040: b0ba 49c6 1c24 174e 4e4b 0a74 9452 9468  ..I..$.NNK.t.R.h
+00001050: 0528 8a08 00b0 e342 d642 2617 4e4e 4b0a  .(.....B.B&.NNK.
+00001060: 7494 5294 6805 288a 0800 b00c 3ce6 6828  t.R.h.(.....<.h(
+00001070: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001080: 3535 f68e 2a17 4e4e 4b0a 7494 5294 6805  55..*.NNK.t.R.h.
+00001090: 288a 0800 b05e 2e06 b52c 174e 4e4b 0a74  (....^...,.NNK.t
+000010a0: 9452 9468 0528 8a08 00b0 8727 16db 2e17  .R.h.(.....'....
+000010b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0b0  NNK.t.R.h.(.....
+000010c0: 2026 0131 174e 4e4b 0a74 9452 9468 0528   &.1.NNK.t.R.h.(
+000010d0: 8a08 00b0 d919 3627 3317 4e4e 4b0a 7494  ......6'3.NNK.t.
+000010e0: 5294 6805 288a 0800 b002 1346 4d35 174e  R.h.(......FM5.N
+000010f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2b0c  NK.t.R.h.(....+.
+00001100: 5673 3717 4e4e 4b0a 7494 5294 6805 288a  Vs7.NNK.t.R.h.(.
+00001110: 0800 b054 0566 9939 174e 4e4b 0a74 9452  ...T.f.9.NNK.t.R
+00001120: 9468 0528 8a08 00b0 7dfe 75bf 3b17 4e4e  .h.(....}.u.;.NN
+00001130: 4b0a 7494 5294 6805 288a 0800 b057 66f1  K.t.R.h.(....Wf.
+00001140: 963d 174e 4e4b 0a74 9452 9468 0528 8a08  .=.NNK.t.R.h.(..
+00001150: 00b0 cff0 950b 4017 4e4e 4b0a 7494 5294  ......@.NNK.t.R.
+00001160: 6805 288a 0800 b0f8 e9a5 3142 174e 4e4b  h.(.......1B.NNK
+00001170: 0a74 9452 9468 0528 8a08 00b0 21e3 b557  .t.R.h.(....!..W
+00001180: 4417 4e4e 4b0a 7494 5294 6805 288a 0800  D.NNK.t.R.h.(...
+00001190: b04a dcc5 7d46 174e 4e4b 0a74 9452 9468  .J..}F.NNK.t.R.h
+000011a0: 0528 8a08 00b0 73d5 d5a3 4817 4e4e 4b0a  .(....s...H.NNK.
+000011b0: 7494 5294 6805 288a 0800 b09c cee5 c94a  t.R.h.(........J
+000011c0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000011d0: c5c7 f5ef 4c17 4e4e 4b0a 7494 5294 6805  ....L.NNK.t.R.h.
+000011e0: 288a 0800 b0ee c005 164f 174e 4e4b 0a74  (........O.NNK.t
+000011f0: 9452 9468 0528 8a08 00b0 c828 81ed 5017  .R.h.(.....(..P.
+00001200: 4e4e 4b0a 7494 5294 6805 288a 0800 b040  NNK.t.R.h.(....@
+00001210: b325 6253 174e 4e4b 0a74 9452 9468 0528  .%bS.NNK.t.R.h.(
+00001220: 8a08 00b0 69ac 3588 5517 4e4e 4b0a 7494  ....i.5.U.NNK.t.
+00001230: 5294 6805 288a 0800 b092 a545 ae57 174e  R.h.(......E.W.N
+00001240: 4e4b 0a74 9452 9468 0528 8a08 00b0 bb9e  NK.t.R.h.(......
+00001250: 55d4 5917 4e4e 4b0a 7494 5294 6805 288a  U.Y.NNK.t.R.h.(.
+00001260: 0800 b0e4 9765 fa5b 174e 4e4b 0a74 9452  .....e.[.NNK.t.R
+00001270: 9468 0528 8a08 00b0 0d91 7520 5e17 4e4e  .h.(......u ^.NN
+00001280: 4b0a 7494 5294 6805 288a 0800 b036 8a85  K.t.R.h.(....6..
+00001290: 4660 174e 4e4b 0a74 9452 9468 0528 8a08  F`.NNK.t.R.h.(..
+000012a0: 00b0 5f83 956c 6217 4e4e 4b0a 7494 5294  .._..lb.NNK.t.R.
+000012b0: 6805 288a 0800 b088 7ca5 9264 174e 4e4b  h.(.....|..d.NNK
+000012c0: 0a74 9452 9468 0528 8a08 00b0 b175 b5b8  .t.R.h.(.....u..
+000012d0: 6617 4e4e 4b0a 7494 5294 6805 288a 0800  f.NNK.t.R.h.(...
+000012e0: b0da 6ec5 de68 174e 4e4b 0a74 9452 9468  ..n..h.NNK.t.R.h
+000012f0: 0528 8a08 00b0 0368 d504 6b17 4e4e 4b0a  .(.....h..k.NNK.
+00001300: 7494 5294 6805 288a 0800 b0dd cf50 dc6c  t.R.h.(......P.l
+00001310: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001320: 555a f550 6f17 4e4e 4b0a 7494 5294 6805  UZ.Po.NNK.t.R.h.
+00001330: 288a 0800 b07e 5305 7771 174e 4e4b 0a74  (....~S.wq.NNK.t
+00001340: 9452 9468 0528 8a08 00b0 a74c 159d 7317  .R.h.(.....L..s.
+00001350: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d0  NNK.t.R.h.(.....
+00001360: 4525 c375 174e 4e4b 0a74 9452 9468 0528  E%.u.NNK.t.R.h.(
+00001370: 8a08 00b0 f93e 35e9 7717 4e4e 4b0a 7494  .....>5.w.NNK.t.
+00001380: 5294 6805 288a 0800 b022 3845 0f7a 174e  R.h.(...."8E.z.N
+00001390: 4e4b 0a74 9452 9468 0528 8a08 00b0 4b31  NK.t.R.h.(....K1
+000013a0: 5535 7c17 4e4e 4b0a 7494 5294 6805 288a  U5|.NNK.t.R.h.(.
+000013b0: 0800 b074 2a65 5b7e 174e 4e4b 0a74 9452  ...t*e[~.NNK.t.R
+000013c0: 9468 0528 8a08 00b0 9d23 7581 8017 4e4e  .h.(.....#u...NN
+000013d0: 4b0a 7494 5294 6805 288a 0800 b0c6 1c85  K.t.R.h.(.......
+000013e0: a782 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000013f0: 00b0 ef15 95cd 8417 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001400: 6805 288a 0800 b018 0fa5 f386 174e 4e4b  h.(..........NNK
+00001410: 0a74 9452 9468 0528 8a08 00b0 4108 b519  .t.R.h.(....A...
+00001420: 8917 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001430: b06a 01c5 3f8b 174e 4e4b 0a74 9452 9468  .j..?..NNK.t.R.h
+00001440: 0528 8a08 00b0 93fa d465 8d17 4e4e 4b0a  .(.......e..NNK.
+00001450: 7494 5294 6805 288a 0800 b0bc f3e4 8b8f  t.R.h.(.........
 00001460: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001470: b2ca 4470 9c17 4e4e 4b0a 7494 5294 6805  ..Dp..NNK.t.R.h.
-00001480: 288a 0800 b0a8 a1a4 54a9 174e 4e4b 0a74  (.......T..NNK.t
-00001490: 9452 9468 0528 8a08 00b0 96d0 897c 0816  .R.h.(.......|..
-000014a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b07e  NNK.t.R.h.(....~
-000014b0: 5305 7771 174e 4e4b 0a74 9452 9468 0528  S.wq.NNK.t.R.h.(
-000014c0: 8a08 00b0 d045 25c3 7517 4e4e 4b0a 7494  .....E%.u.NNK.t.
-000014d0: 5294 6805 288a 0800 b0d6 1a88 0092 164e  R.h.(..........N
-000014e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 9d23  NK.t.R.h.(.....#
-000014f0: 7581 8017 4e4e 4b0a 7494 5294 6805 288a  u...NNK.t.R.h.(.
-00001500: 0800 b05a dac8 d655 164e 4e4b 0a74 9452  ...Z...U.NNK.t.R
-00001510: 9468 0528 8a08 00b0 6702 1719 ea16 4e4e  .h.(....g.....NN
-00001520: 4b0a 7494 5294 6805 288a 0800 b08a fdca  K.t.R.h.(.......
-00001530: f1a9 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001540: 00b0 b44b 6acf e115 4e4e 4b0a 7494 5294  ...Kj...NNK.t.R.
-00001550: 6805 288a 0800 b049 8736 c610 174e 4e4b  h.(....I.6...NNK
-00001560: 0a74 9452 9468 0528 8a08 00b0 04bd 64bc  .t.R.h.(......d.
-00001570: a017 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001580: b017 ba15 3c51 174e 4e4b 0a74 9452 9468  ....<Q.NNK.t.R.h
-00001590: 0528 8a08 00b0 3535 f68e 2a17 4e4e 4b0a  .(....55..*.NNK.
-000015a0: 7494 5294 6805 288a 0800 b02c 61e5 2a6d  t.R.h.(....,a.*m
+00001470: e5ec f4b1 9117 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00001480: 288a 0800 b00e e604 d893 174e 4e4b 0a74  (..........NNK.t
+00001490: 9452 9468 0528 8a08 00b0 37df 14fe 9517  .R.h.(....7.....
+000014a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b060  NNK.t.R.h.(....`
+000014b0: d824 2498 174e 4e4b 0a74 9452 9468 0528  .$$..NNK.t.R.h.(
+000014c0: 8a08 00b0 89d1 344a 9a17 4e4e 4b0a 7494  ......4J..NNK.t.
+000014d0: 5294 6805 288a 0800 b0b2 ca44 709c 174e  R.h.(......Dp..N
+000014e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 dbc3  NK.t.R.h.(......
+000014f0: 5496 9e17 4e4e 4b0a 7494 5294 6805 288a  T...NNK.t.R.h.(.
+00001500: 0800 b004 bd64 bca0 174e 4e4b 0a74 9452  .....d...NNK.t.R
+00001510: 9468 0528 8a08 00b0 2db6 74e2 a217 4e4e  .h.(....-.t...NN
+00001520: 4b0a 7494 5294 6805 288a 0800 b056 af84  K.t.R.h.(....V..
+00001530: 08a5 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00001540: 00b0 7fa8 942e a717 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001550: 6805 288a 0800 b0a8 a1a4 54a9 174e 4e4b  h.(.......T..NNK
+00001560: 0a74 9452 9468 0528 8a08 00b0 d19a b47a  .t.R.h.(.......z
+00001570: ab17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001580: b0fa 93c4 a0ad 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00001590: 0528 8a08 00b0 238d d4c6 af17 4e4e 4b0a  .(....#.....NNK.
+000015a0: 7494 5294 6805 288a 0800 b04c 86e4 ecb1  t.R.h.(....L....
 000015b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000015c0: 76ab 8aba c315 4e4e 4b0a 7494 5294 6805  v.....NNK.t.R.h.
-000015d0: 288a 0800 b01d 8f78 796d 164e 4e4b 0a74  (......xym.NNK.t
-000015e0: 9452 9468 0528 8a08 00b0 f196 ba2c ca15  .R.h.(.......,..
-000015f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b06d  NNK.t.R.h.(....m
-00001600: d779 5606 164e 4e4b 0a74 9452 9468 0528  .yV..NNK.t.R.h.(
-00001610: 8a08 00b0 bd1f 7b33 9f15 4e4e 4b0a 7494  ......{3..NNK.t.
-00001620: 5294 6805 288a 0800 b028 0da8 4c96 164e  R.h.(....(..L..N
-00001630: 4e4b 0a74 9452 9468 0528 8a08 00b0 3db4  NK.t.R.h.(....=.
-00001640: 773b b216 4e4e 4b0a 7494 5294 6805 288a  w;..NNK.t.R.h.(.
-00001650: 0800 b00a 92c7 f9bc 164e 4e4b 0a74 9452  .........NNK.t.R
-00001660: 9468 0528 8a08 00b0 60d8 2424 9817 4e4e  .h.(....`.$$..NN
-00001670: 4b0a 7494 5294 6805 288a 0800 b023 8dd4  K.t.R.h.(....#..
-00001680: c6af 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001690: 00b0 31e1 b8b0 5316 4e4e 4b0a 7494 5294  ..1...S.NNK.t.R.
-000016a0: 6805 288a 0800 b0aa 22ca b3ee 154e 4e4b  h.(....."....NNK
-000016b0: 0a74 9452 9468 0528 8a08 00b0 4f5c 9903  .t.R.h.(....O\..
-000016c0: 2d16 4e4e 4b0a 7494 5294 6805 288a 0800  -.NNK.t.R.h.(...
-000016d0: b0f6 3f87 c2d6 164e 4e4b 0a74 9452 9468  ..?....NNK.t.R.h
-000016e0: 0528 8a08 00b0 5405 6699 3917 4e4e 4b0a  .(....T.f.9.NNK.
-000016f0: 7494 5294 6805 288a 0800 b0f5 eaf7 0aa1  t.R.h.(.........
-00001700: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001710: dcef ea3d ae15 4e4e 4b0a 7494 5294 6805  ...=..NNK.t.R.h.
-00001720: 288a 0800 b042 344b c198 154e 4e4b 0a74  (....B4K...NNK.t
-00001730: 9452 9468 0528 8a08 00b0 f794 167a 0c17  .R.h.(.......z..
-00001740: 4e4e 4b0a 7494 5294 6805 288a 0800 b097  NNK.t.R.h.(.....
-00001750: 2519 343e 164e 4e4b 0a74 9452 9468 0528  %.4>.NNK.t.R.h.(
-00001760: 8a08 00b0 308c 29f9 1d16 4e4e 4b0a 7494  ....0.)...NNK.t.
-00001770: 5294 6805 288a 0800 b034 e066 d7f4 164e  R.h.(....4.f...N
-00001780: 4e4b 0a74 9452 9468 0528 8a08 00b0 a74c  NK.t.R.h.(.....L
-00001790: 159d 7317 4e4e 4b0a 7494 5294 6805 288a  ..s.NNK.t.R.h.(.
-000017a0: 0800 b094 4f64 1dc3 174e 4e4b 0a74 9452  ....Od...NNK.t.R
-000017b0: 9468 0528 8a08 00b0 a14e b94f 3116 4e4e  .h.(.....N.O1.NN
-000017c0: 4b0a 7494 5294 658c 0942 414e 4b4e 4946  K.t.R.e..BANKNIF
-000017d0: 5459 945d 9428 6805 288a 0800 b0f9 3e35  TY.].(h.(.....>5
-000017e0: e977 174e 4e4b 0a74 9452 9468 0528 8a08  .w.NNK.t.R.h.(..
-000017f0: 00b0 d31b dad9 f015 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00001800: 6805 288a 0800 b07f 7f9b 1e81 154e 4e4b  h.(..........NNK
-00001810: 0a74 9452 9468 0528 8a08 00b0 2b0c 5673  .t.R.h.(....+.Vs
-00001820: 3717 4e4e 4b0a 7494 5294 6805 288a 0800  7.NNK.t.R.h.(...
-00001830: b0bb 9e55 d459 174e 4e4b 0a74 9452 9468  ...U.Y.NNK.t.R.h
-00001840: 0528 8a08 00b0 c2c8 47c9 ab16 4e4e 4b0a  .(......G...NNK.
-00001850: 7494 5294 6805 288a 0800 b036 8a85 4660  t.R.h.(....6..F`
-00001860: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001870: 9fa4 9ae0 c515 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00001880: 288a 0800 b0d4 fb3f 78af 174e 4e4b 0a74  (......?x..NNK.t
-00001890: 9452 9468 0528 8a08 00b0 316c 8f97 dc17  .R.h.(....1l....
-000018a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e7  NNK.t.R.h.(.....
-000018b0: 6d1a 11d7 154e 4e4b 0a74 9452 9468 0528  m....NNK.t.R.h.(
-000018c0: 8a08 00b0 ca47 c975 3316 4e4e 4b0a 7494  .....G.u3.NNK.t.
-000018d0: 5294 6805 288a 0800 b0de 9909 ad19 164e  R.h.(..........N
-000018e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 a2a3  NK.t.R.h.(......
-000018f0: 4807 6716 4e4e 4b0a 7494 5294 6805 288a  H.g.NNK.t.R.h.(.
-00001900: 0800 b032 3648 6889 164e 4e4b 0a74 9452  ...26Hh..NNK.t.R
-00001910: 9468 0528 8a08 00b0 193b 3b9b 9615 4e4e  .h.(.....;;...NN
-00001920: 4b0a 7494 5294 6805 288a 0800 b025 0efa  K.t.R.h.(....%..
-00001930: 25f5 154e 4e4b 0a74 9452 9468 0528 8a08  %..NNK.t.R.h.(..
-00001940: 00b0 a1d9 8f36 ba17 4e4e 4b0a 7494 5294  .....6..NNK.t.R.
-00001950: 6805 288a 0800 b063 aed9 3a13 164e 4e4b  h.(....c..:..NNK
-00001960: 0a74 9452 9468 0528 8a08 00b0 987a a8eb  .t.R.h.(.....z..
-00001970: 7316 4e4e 4b0a 7494 5294 6805 288a 0800  s.NNK.t.R.h.(...
-00001980: b0ec 16e7 a6e3 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00001990: 0528 8a08 00b0 8129 ba8d ec15 4e4e 4b0a  .(.....)....NNK.
-000019a0: 7494 5294 6805 288a 0800 b0f3 cbaf 82be  t.R.h.(.........
-000019b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000019c0: fbbf 5a48 bd15 4e4e 4b0a 7494 5294 6805  ..ZH..NNK.t.R.h.
-000019d0: 288a 0800 b0aa 4bc3 c314 184e 4e4b 0a74  (.....K....NNK.t
-000019e0: 9452 9468 0528 8a08 00b0 80d4 2ad6 b615  .R.h.(......*...
-000019f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b091  NNK.t.R.h.(.....
-00001a00: 50b6 f621 174e 4e4b 0a74 9452 9468 0528  P..!.NNK.t.R.h.(
-00001a10: 8a08 00b0 c173 b811 7616 4e4e 4b0a 7494  .....s..v.NNK.t.
+000015c0: 757f f412 b417 4e4e 4b0a 7494 5294 6805  u.....NNK.t.R.h.
+000015d0: 288a 0800 b09e 7804 39b6 174e 4e4b 0a74  (.....x.9..NNK.t
+000015e0: 9452 9468 0528 8a08 00b0 c771 145f b817  .R.h.(.....q._..
+000015f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
+00001600: 6a24 85ba 174e 4e4b 0a74 9452 9468 0528  j$...NNK.t.R.h.(
+00001610: 8a08 00b0 1964 34ab bc17 4e4e 4b0a 7494  .....d4...NNK.t.
+00001620: 5294 6805 288a 0800 b042 5d44 d1be 174e  R.h.(....B]D...N
+00001630: 4e4b 0a74 9452 9468 0528 8a08 00b0 6b56  NK.t.R.h.(....kV
+00001640: 54f7 c017 4e4e 4b0a 7494 5294 6805 288a  T...NNK.t.R.h.(.
+00001650: 0800 b094 4f64 1dc3 174e 4e4b 0a74 9452  ....Od...NNK.t.R
+00001660: 9468 0528 8a08 00b0 6eb7 dff4 c417 4e4e  .h.(....n.....NN
+00001670: 4b0a 7494 5294 6805 288a 0800 b0e6 4184  K.t.R.h.(.....A.
+00001680: 69c7 174e 4e4b 0a74 9452 9468 0528 8a08  i..NNK.t.R.h.(..
+00001690: 00b0 0f3b 948f c917 4e4e 4b0a 7494 5294  ...;....NNK.t.R.
+000016a0: 6805 288a 0800 b038 34a4 b5cb 174e 4e4b  h.(....84....NNK
+000016b0: 0a74 9452 9468 0528 8a08 00b0 612d b4db  .t.R.h.(....a-..
+000016c0: cd17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000016d0: b08a 26c4 01d0 174e 4e4b 0a74 9452 9468  ..&....NNK.t.R.h
+000016e0: 0528 8a08 00b0 b31f d427 d217 4e4e 4b0a  .(.......'..NNK.
+000016f0: 7494 5294 6805 288a 0800 b0dc 18e4 4dd4  t.R.h.(.......M.
+00001700: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001710: 80fd 23e6 dc17 4e4e 4b0a 7494 5294 6805  ..#...NNK.t.R.h.
+00001720: 288a 0800 b095 a4f3 d4f8 174e 4e4b 0a74  (..........NNK.t
+00001730: 9452 9468 0528 8a08 00b0 aa4b c3c3 1418  .R.h.(.....K....
+00001740: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d4  NNK.t.R.h.(.....
+00001750: 9962 a14c 184e 4e4b 0a74 9452 9468 0528  .b.L.NNK.t.R.h.(
+00001760: 8a08 00b0 af56 6d30 8418 4e4e 4b0a 7494  .....Vm0..NNK.t.
+00001770: 5294 6805 288a 0800 b028 36a1 5cbc 184e  R.h.(....(6.\..N
+00001780: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b7d  NK.t.R.h.(....{}
+00001790: 5060 f618 4e4e 4b0a 7494 5294 6805 288a  P`..NNK.t.R.h.(.
+000017a0: 0800 b07c d2df 172c 194e 4e4b 0a74 9452  ...|...,.NNK.t.R
+000017b0: 9468 0528 8a08 00b0 cf19 8f1b 6619 4e4e  .h.(........f.NN
+000017c0: 4b0a 7494 5294 6805 288a 0800 b023 b6cd  K.t.R.h.(....#..
+000017d0: d6d5 194e 4e4b 0a74 9452 9465 8c09 4241  ...NNK.t.R.e..BA
+000017e0: 4e4b 4e49 4654 5994 5d94 2868 0528 8a08  NKNIFTY.].(h.(..
+000017f0: 00b0 7f7f 9b1e 8115 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001800: 6805 288a 0800 b0a8 78ab 4483 154e 4e4b  h.(.....x.D..NNK
+00001810: 0a74 9452 9468 0528 8a08 00b0 d171 bb6a  .t.R.h.(.....q.j
+00001820: 8515 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001830: b0fa 6acb 9087 154e 4e4b 0a74 9452 9468  ..j....NNK.t.R.h
+00001840: 0528 8a08 00b0 2364 dbb6 8915 4e4e 4b0a  .(....#d....NNK.
+00001850: 7494 5294 6805 288a 0800 b04c 5deb dc8b  t.R.h.(....L]...
+00001860: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001870: 26c5 66b4 8d15 4e4e 4b0a 7494 5294 6805  &.f...NNK.t.R.h.
+00001880: 288a 0800 b09e 4f0b 2990 154e 4e4b 0a74  (.....O.)..NNK.t
+00001890: 9452 9468 0528 8a08 00b0 c748 1b4f 9215  .R.h.(.....H.O..
+000018a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
+000018b0: 412b 7594 154e 4e4b 0a74 9452 9468 0528  A+u..NNK.t.R.h.(
+000018c0: 8a08 00b0 193b 3b9b 9615 4e4e 4b0a 7494  .....;;...NNK.t.
+000018d0: 5294 6805 288a 0800 b042 344b c198 154e  R.h.(....B4K...N
+000018e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 6b2d  NK.t.R.h.(....k-
+000018f0: 5be7 9a15 4e4e 4b0a 7494 5294 6805 288a  [...NNK.t.R.h.(.
+00001900: 0800 b094 266b 0d9d 154e 4e4b 0a74 9452  ....&k...NNK.t.R
+00001910: 9468 0528 8a08 00b0 bd1f 7b33 9f15 4e4e  .h.(......{3..NN
+00001920: 4b0a 7494 5294 6805 288a 0800 b0e6 188b  K.t.R.h.(.......
+00001930: 59a1 154e 4e4b 0a74 9452 9468 0528 8a08  Y..NNK.t.R.h.(..
+00001940: 00b0 0f12 9b7f a315 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001950: 6805 288a 0800 b038 0bab a5a5 154e 4e4b  h.(....8.....NNK
+00001960: 0a74 9452 9468 0528 8a08 00b0 6104 bbcb  .t.R.h.(....a...
+00001970: a715 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001980: b08a fdca f1a9 154e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00001990: 0528 8a08 00b0 b3f6 da17 ac15 4e4e 4b0a  .(..........NNK.
+000019a0: 7494 5294 6805 288a 0800 b0dc efea 3dae  t.R.h.(.......=.
+000019b0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000019c0: 05e9 fa63 b015 4e4e 4b0a 7494 5294 6805  ...c..NNK.t.R.h.
+000019d0: 288a 0800 b02e e20a 8ab2 154e 4e4b 0a74  (..........NNK.t
+000019e0: 9452 9468 0528 8a08 00b0 57db 1ab0 b415  .R.h.(....W.....
+000019f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b080  NNK.t.R.h.(.....
+00001a00: d42a d6b6 154e 4e4b 0a74 9452 9468 0528  .*...NNK.t.R.h.(
+00001a10: 8a08 00b0 a9cd 3afc b815 4e4e 4b0a 7494  ......:...NNK.t.
 00001a20: 5294 6805 288a 0800 b083 35b6 d3ba 154e  R.h.(.....5....N
-00001a30: 4e4b 0a74 9452 9468 0528 8a08 00b0 83d3  NK.t.R.h.(......
-00001a40: d8fc 5716 4e4e 4b0a 7494 5294 6805 288a  ..W.NNK.t.R.h.(.
-00001a50: 0800 b0ea 6cc8 3778 164e 4e4b 0a74 9452  ....l.7x.NNK.t.R
-00001a60: 9468 0528 8a08 00b0 e917 3980 4216 4e4e  .h.(......9.B.NN
-00001a70: 4b0a 7494 5294 6805 288a 0800 b05d d976  K.t.R.h.(....].v
-00001a80: fdf6 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001a90: 00b0 7ca9 e607 0617 4e4e 4b0a 7494 5294  ..|.....NNK.t.R.
-00001aa0: 6805 288a 0800 b059 1010 06a9 174e 4e4b  h.(....Y.....NNK
-00001ab0: 0a74 9452 9468 0528 8a08 00b0 338b d71f  .t.R.h.(....3...
-00001ac0: bf16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001ad0: b026 ee5f c4b3 174e 4e4b 0a74 9452 9468  .&._...NNK.t.R.h
-00001ae0: 0528 8a08 00b0 50b1 28bb 6216 4e4e 4b0a  .(....P.(.b.NNK.
-00001af0: 7494 5294 6805 288a 0800 b0c0 a9ff 40c9  t.R.h.(.......@.
-00001b00: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001b10: a504 d404 6b16 4e4e 4b0a 7494 5294 6805  ....k.NNK.t.R.h.
-00001b20: 288a 0800 b06c 82ea 9ed0 154e 4e4b 0a74  (....l.....NNK.t
-00001b30: 9452 9468 0528 8a08 00b0 b020 2601 3117  .R.h.(..... &.1.
-00001b40: 4e4e 4b0a 7494 5294 6805 288a 0800 b078  NNK.t.R.h.(....x
-00001b50: 55a9 292f 164e 4e4b 0a74 9452 9468 0528  U.)/.NNK.t.R.h.(
-00001b60: 8a08 00b0 f340 d99b 3516 4e4e 4b0a 7494  .....@..5.NNK.t.
-00001b70: 5294 6805 288a 0800 b05c 84e7 45c1 164e  R.h.(....\..E..N
-00001b80: 4e4b 0a74 9452 9468 0528 8a08 00b0 6b56  NK.t.R.h.(....kV
-00001b90: 54f7 c017 4e4e 4b0a 7494 5294 6805 288a  T...NNK.t.R.h.(.
-00001ba0: 0800 b0c0 1e29 5a40 164e 4e4b 0a74 9452  .....)Z@.NNK.t.R
-00001bb0: 9468 0528 8a08 00b0 b74a 18f6 8216 4e4e  .h.(.....J....NN
-00001bc0: 4b0a 7494 5294 6805 288a 0800 b06b 2d5b  K.t.R.h.(....k-[
-00001bd0: e79a 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001be0: 00b0 c748 1b4f 9215 4e4e 4b0a 7494 5294  ...H.O..NNK.t.R.
-00001bf0: 6805 288a 0800 b014 bb67 15b0 164e 4e4b  h.(......g...NNK
-00001c00: 0a74 9452 9468 0528 8a08 00b0 eec0 0516  .t.R.h.(........
-00001c10: 4f17 4e4e 4b0a 7494 5294 6805 288a 0800  O.NNK.t.R.h.(...
-00001c20: b0b5 a0f9 8617 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00001c30: 0528 8a08 00b0 e8c2 a9c8 0c16 4e4e 4b0a  .(..........NNK.
-00001c40: 7494 5294 6805 288a 0800 b00f 129b 7fa3  t.R.h.(.........
+00001a30: 4e4b 0a74 9452 9468 0528 8a08 00b0 fbbf  NK.t.R.h.(......
+00001a40: 5a48 bd15 4e4e 4b0a 7494 5294 6805 288a  ZH..NNK.t.R.h.(.
+00001a50: 0800 b024 b96a 6ebf 154e 4e4b 0a74 9452  ...$.jn..NNK.t.R
+00001a60: 9468 0528 8a08 00b0 4db2 7a94 c115 4e4e  .h.(....M.z...NN
+00001a70: 4b0a 7494 5294 6805 288a 0800 b076 ab8a  K.t.R.h.(....v..
+00001a80: bac3 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00001a90: 00b0 9fa4 9ae0 c515 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001aa0: 6805 288a 0800 b0c8 9daa 06c8 154e 4e4b  h.(..........NNK
+00001ab0: 0a74 9452 9468 0528 8a08 00b0 f196 ba2c  .t.R.h.(.......,
+00001ac0: ca15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001ad0: b01a 90ca 52cc 154e 4e4b 0a74 9452 9468  ....R..NNK.t.R.h
+00001ae0: 0528 8a08 00b0 4389 da78 ce15 4e4e 4b0a  .(....C..x..NNK.
+00001af0: 7494 5294 6805 288a 0800 b06c 82ea 9ed0  t.R.h.(....l....
+00001b00: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001b10: 957b fac4 d215 4e4e 4b0a 7494 5294 6805  .{....NNK.t.R.h.
+00001b20: 288a 0800 b0be 740a ebd4 154e 4e4b 0a74  (.....t....NNK.t
+00001b30: 9452 9468 0528 8a08 00b0 e76d 1a11 d715  .R.h.(.....m....
+00001b40: 4e4e 4b0a 7494 5294 6805 288a 0800 b010  NNK.t.R.h.(.....
+00001b50: 672a 37d9 154e 4e4b 0a74 9452 9468 0528  g*7..NNK.t.R.h.(
+00001b60: 8a08 00b0 3960 3a5d db15 4e4e 4b0a 7494  ....9`:]..NNK.t.
+00001b70: 5294 6805 288a 0800 b062 594a 83dd 154e  R.h.(....bYJ...N
+00001b80: 4e4b 0a74 9452 9468 0528 8a08 00b0 8b52  NK.t.R.h.(.....R
+00001b90: 5aa9 df15 4e4e 4b0a 7494 5294 6805 288a  Z...NNK.t.R.h.(.
+00001ba0: 0800 b0b4 4b6a cfe1 154e 4e4b 0a74 9452  ....Kj...NNK.t.R
+00001bb0: 9468 0528 8a08 00b0 dd44 7af5 e315 4e4e  .h.(.....Dz...NN
+00001bc0: 4b0a 7494 5294 6805 288a 0800 b006 3e8a  K.t.R.h.(.....>.
+00001bd0: 1be6 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00001be0: 00b0 2f37 9a41 e815 4e4e 4b0a 7494 5294  ../7.A..NNK.t.R.
+00001bf0: 6805 288a 0800 b058 30aa 67ea 154e 4e4b  h.(....X0.g..NNK
+00001c00: 0a74 9452 9468 0528 8a08 00b0 8129 ba8d  .t.R.h.(.....)..
+00001c10: ec15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001c20: b0aa 22ca b3ee 154e 4e4b 0a74 9452 9468  .."....NNK.t.R.h
+00001c30: 0528 8a08 00b0 d31b dad9 f015 4e4e 4b0a  .(..........NNK.
+00001c40: 7494 5294 6805 288a 0800 b0fc 14ea fff2  t.R.h.(.........
 00001c50: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001c60: d171 bb6a 8515 4e4e 4b0a 7494 5294 6805  .q.j..NNK.t.R.h.
-00001c70: 288a 0800 b027 b818 9560 164e 4e4b 0a74  (....'...`.NNK.t
-00001c80: 9452 9468 0528 8a08 00b0 fd69 79b7 2816  .R.h.(.....iy.(.
-00001c90: 4e4e 4b0a 7494 5294 6805 288a 0800 b0cd  NNK.t.R.h.(.....
-00001ca0: 4677 9cd4 164e 4e4b 0a74 9452 9468 0528  Fw...NNK.t.R.h.(
-00001cb0: 8a08 00b0 8d87 4fff d317 4e4e 4b0a 7494  ......O...NNK.t.
-00001cc0: 5294 6805 288a 0800 b013 66d8 5d7a 164e  R.h.(.....f.]z.N
-00001cd0: 4e4b 0a74 9452 9468 0528 8a08 00b0 0c3c  NK.t.R.h.(.....<
-00001ce0: e668 2817 4e4e 4b0a 7494 5294 6805 288a  .h(.NNK.t.R.h.(.
-00001cf0: 0800 b0ac cce8 225a 164e 4e4b 0a74 9452  ......"Z.NNK.t.R
-00001d00: 9468 0528 8a08 00b0 093d 3842 8716 4e4e  .h.(.....=8B..NN
-00001d10: 4b0a 7494 5294 6805 288a 0800 b00b e756  K.t.R.h.(......V
-00001d20: b1f2 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001d30: 00b0 380b aba5 a515 4e4e 4b0a 7494 5294  ..8.....NNK.t.R.
-00001d40: 6805 288a 0800 b080 fd23 e6dc 174e 4e4b  h.(......#...NNK
-00001d50: 0a74 9452 9468 0528 8a08 00b0 1211 49a6  .t.R.h.(......I.
-00001d60: 4416 4e4e 4b0a 7494 5294 6805 288a 0800  D.NNK.t.R.h.(...
-00001d70: b095 a4f3 d4f8 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00001d80: 0528 8a08 00b0 ccf1 e7e4 9e16 4e4e 4b0a  .(..........NNK.
-00001d90: 7494 5294 6805 288a 0800 b077 001a 72f9  t.R.h.(....w..r.
-00001da0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001db0: ff13 9826 9416 4e4e 4b0a 7494 5294 6805  ...&..NNK.t.R.h.
-00001dc0: 288a 0800 b03f 5e96 aa1d 174e 4e4b 0a74  (....?^....NNK.t
-00001dd0: 9452 9468 0528 8a08 00b0 9a24 c75a df16  .R.h.(.....$.Z..
-00001de0: 4e4e 4b0a 7494 5294 6805 288a 0800 b04e  NNK.t.R.h.(....N
-00001df0: 070a 4cf7 154e 4e4b 0a74 9452 9468 0528  ..L..NNK.t.R.h.(
-00001e00: 8a08 00b0 180f a5f3 8617 4e4e 4b0a 7494  ..........NNK.t.
-00001e10: 5294 6805 288a 0800 b01f 3997 e8d8 164e  R.h.(.....9....N
-00001e20: 4e4b 0a74 9452 9468 0528 8a08 00b0 1067  NK.t.R.h.(.....g
-00001e30: 2a37 d915 4e4e 4b0a 7494 5294 6805 288a  *7..NNK.t.R.h.(.
-00001e40: 0800 b0a0 8400 7f84 174e 4e4b 0a74 9452  .........NNK.t.R
-00001e50: 9468 0528 8a08 00b0 d5c5 f848 5c16 4e4e  .h.(.......H\.NN
-00001e60: 4b0a 7494 5294 6805 288a 0800 b0d4 7069  K.t.R.h.(.....pi
-00001e70: 9126 164e 4e4b 0a74 9452 9468 0528 8a08  .&.NNK.t.R.h.(..
-00001e80: 00b0 857d f76b c316 4e4e 4b0a 7494 5294  ...}.k..NNK.t.R.
-00001e90: 6805 288a 0800 b08b 525a a9df 154e 4e4b  h.(.....RZ...NNK
-00001ea0: 0a74 9452 9468 0528 8a08 00b0 712b b734  .t.R.h.(....q+.4
-00001eb0: dd16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001ec0: b0a4 4d67 76d2 164e 4e4b 0a74 9452 9468  ..Mgv..NNK.t.R.h
-00001ed0: 0528 8a08 00b0 b9f4 3665 ee16 4e4e 4b0a  .(......6e..NNK.
-00001ee0: 7494 5294 6805 288a 0800 b002 1346 4d35  t.R.h.(......FM5
-00001ef0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001f00: b52b d06d a017 4e4e 4b0a 7494 5294 6805  .+.m..NNK.t.R.h.
-00001f10: 288a 0800 b01c c5bf a8c0 174e 4e4b 0a74  (..........NNK.t
-00001f20: 9452 9468 0528 8a08 00b0 26c5 66b4 8d15  .R.h.(....&.f...
-00001f30: 4e4e 4b0a 7494 5294 6805 288a 0800 b023  NNK.t.R.h.(....#
-00001f40: 64db b689 154e 4e4b 0a74 9452 9468 0528  d....NNK.t.R.h.(
-00001f50: 8a08 00b0 9e4f 0b29 9015 4e4e 4b0a 7494  .....O.)..NNK.t.
-00001f60: 5294 6805 288a 0800 b0b3 f6da 17ac 154e  R.h.(..........N
-00001f70: 4e4b 0a74 9452 9468 0528 8a08 00b0 99cf  NK.t.R.h.(......
-00001f80: 37a3 a916 4e4e 4b0a 7494 5294 6805 288a  7...NNK.t.R.h.(.
-00001f90: 0800 b052 5b47 2ace 164e 4e4b 0a74 9452  ...R[G*..NNK.t.R
-00001fa0: 9468 0528 8a08 00b0 53b0 d6e1 0317 4e4e  .h.(....S.....NN
-00001fb0: 4b0a 7494 5294 6805 288a 0800 b072 8046  K.t.R.h.(....r.F
-00001fc0: ec12 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001fd0: 00b0 0368 d504 6b17 4e4e 4b0a 7494 5294  ...h..k.NNK.t.R.
-00001fe0: 6805 288a 0800 b0c9 7d10 a586 174e 4e4b  h.(.....}....NNK
-00001ff0: 0a74 9452 9468 0528 8a08 00b0 bf54 7089  .t.R.h.(.....Tp.
-00002000: 9317 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002010: b082 0920 2cab 174e 4e4b 0a74 9452 9468  ... ,..NNK.t.R.h
-00002020: 0528 8a08 00b0 208e 26a0 0e17 4e4e 4b0a  .(.... .&...NNK.
-00002030: 7494 5294 6805 288a 0800 b0bf c999 a20a  t.R.h.(.........
+00001c60: 250e fa25 f515 4e4e 4b0a 7494 5294 6805  %..%..NNK.t.R.h.
+00001c70: 288a 0800 b04e 070a 4cf7 154e 4e4b 0a74  (....N..L..NNK.t
+00001c80: 9452 9468 0528 8a08 00b0 7700 1a72 f915  .R.h.(....w..r..
+00001c90: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a0  NNK.t.R.h.(.....
+00001ca0: f929 98fb 154e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
+00001cb0: 8a08 00b0 c9f2 39be fd15 4e4e 4b0a 7494  ......9...NNK.t.
+00001cc0: 5294 6805 288a 0800 b0f2 eb49 e4ff 154e  R.h.(......I...N
+00001cd0: 4e4b 0a74 9452 9468 0528 8a08 00b0 cc53  NK.t.R.h.(.....S
+00001ce0: c5bb 0116 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00001cf0: 0800 b044 de69 3004 164e 4e4b 0a74 9452  ...D.i0..NNK.t.R
+00001d00: 9468 0528 8a08 00b0 6dd7 7956 0616 4e4e  .h.(....m.yV..NN
+00001d10: 4b0a 7494 5294 6805 288a 0800 b096 d089  K.t.R.h.(.......
+00001d20: 7c08 164e 4e4b 0a74 9452 9468 0528 8a08  |..NNK.t.R.h.(..
+00001d30: 00b0 bfc9 99a2 0a16 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001d40: 6805 288a 0800 b0e8 c2a9 c80c 164e 4e4b  h.(..........NNK
+00001d50: 0a74 9452 9468 0528 8a08 00b0 11bc b9ee  .t.R.h.(........
+00001d60: 0e16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001d70: b03a b5c9 1411 164e 4e4b 0a74 9452 9468  .:.....NNK.t.R.h
+00001d80: 0528 8a08 00b0 63ae d93a 1316 4e4e 4b0a  .(....c..:..NNK.
+00001d90: 7494 5294 6805 288a 0800 b08c a7e9 6015  t.R.h.(.......`.
+00001da0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001db0: b5a0 f986 1716 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00001dc0: 288a 0800 b0de 9909 ad19 164e 4e4b 0a74  (..........NNK.t
+00001dd0: 9452 9468 0528 8a08 00b0 0793 19d3 1b16  .R.h.(..........
+00001de0: 4e4e 4b0a 7494 5294 6805 288a 0800 b030  NNK.t.R.h.(....0
+00001df0: 8c29 f91d 164e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
+00001e00: 8a08 00b0 5985 391f 2016 4e4e 4b0a 7494  ....Y.9. .NNK.t.
+00001e10: 5294 6805 288a 0800 b082 7e49 4522 164e  R.h.(.....~IE".N
+00001e20: 4e4b 0a74 9452 9468 0528 8a08 00b0 ab77  NK.t.R.h.(.....w
+00001e30: 596b 2416 4e4e 4b0a 7494 5294 6805 288a  Yk$.NNK.t.R.h.(.
+00001e40: 0800 b0d4 7069 9126 164e 4e4b 0a74 9452  ....pi.&.NNK.t.R
+00001e50: 9468 0528 8a08 00b0 fd69 79b7 2816 4e4e  .h.(.....iy.(.NN
+00001e60: 4b0a 7494 5294 6805 288a 0800 b026 6389  K.t.R.h.(....&c.
+00001e70: dd2a 164e 4e4b 0a74 9452 9468 0528 8a08  .*.NNK.t.R.h.(..
+00001e80: 00b0 4f5c 9903 2d16 4e4e 4b0a 7494 5294  ..O\..-.NNK.t.R.
+00001e90: 6805 288a 0800 b078 55a9 292f 164e 4e4b  h.(....xU.)/.NNK
+00001ea0: 0a74 9452 9468 0528 8a08 00b0 a14e b94f  .t.R.h.(.....N.O
+00001eb0: 3116 4e4e 4b0a 7494 5294 6805 288a 0800  1.NNK.t.R.h.(...
+00001ec0: b0ca 47c9 7533 164e 4e4b 0a74 9452 9468  ..G.u3.NNK.t.R.h
+00001ed0: 0528 8a08 00b0 f340 d99b 3516 4e4e 4b0a  .(.....@..5.NNK.
+00001ee0: 7494 5294 6805 288a 0800 b01c 3ae9 c137  t.R.h.(.....:..7
+00001ef0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001f00: 4533 f9e7 3916 4e4e 4b0a 7494 5294 6805  E3..9.NNK.t.R.h.
+00001f10: 288a 0800 b06e 2c09 0e3c 164e 4e4b 0a74  (....n,..<.NNK.t
+00001f20: 9452 9468 0528 8a08 00b0 9725 1934 3e16  .R.h.(.....%.4>.
+00001f30: 4e4e 4b0a 7494 5294 6805 288a 0800 b0c0  NNK.t.R.h.(.....
+00001f40: 1e29 5a40 164e 4e4b 0a74 9452 9468 0528  .)Z@.NNK.t.R.h.(
+00001f50: 8a08 00b0 e917 3980 4216 4e4e 4b0a 7494  ......9.B.NNK.t.
+00001f60: 5294 6805 288a 0800 b012 1149 a644 164e  R.h.(......I.D.N
+00001f70: 4e4b 0a74 9452 9468 0528 8a08 00b0 3b0a  NK.t.R.h.(....;.
+00001f80: 59cc 4616 4e4e 4b0a 7494 5294 6805 288a  Y.F.NNK.t.R.h.(.
+00001f90: 0800 b064 0369 f248 164e 4e4b 0a74 9452  ...d.i.H.NNK.t.R
+00001fa0: 9468 0528 8a08 00b0 8dfc 7818 4b16 4e4e  .h.(......x.K.NN
+00001fb0: 4b0a 7494 5294 6805 288a 0800 b0b6 f588  K.t.R.h.(.......
+00001fc0: 3e4d 164e 4e4b 0a74 9452 9468 0528 8a08  >M.NNK.t.R.h.(..
+00001fd0: 00b0 dfee 9864 4f16 4e4e 4b0a 7494 5294  .....dO.NNK.t.R.
+00001fe0: 6805 288a 0800 b008 e8a8 8a51 164e 4e4b  h.(........Q.NNK
+00001ff0: 0a74 9452 9468 0528 8a08 00b0 31e1 b8b0  .t.R.h.(....1...
+00002000: 5316 4e4e 4b0a 7494 5294 6805 288a 0800  S.NNK.t.R.h.(...
+00002010: b05a dac8 d655 164e 4e4b 0a74 9452 9468  .Z...U.NNK.t.R.h
+00002020: 0528 8a08 00b0 83d3 d8fc 5716 4e4e 4b0a  .(........W.NNK.
+00002030: 7494 5294 6805 288a 0800 b0ac cce8 225a  t.R.h.(......."Z
 00002040: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002050: ab77 596b 2416 4e4e 4b0a 7494 5294 6805  .wYk$.NNK.t.R.h.
-00002060: 288a 0800 b0cb 9c58 2d69 164e 4e4b 0a74  (......X-i.NNK.t
-00002070: 9452 9468 0528 8a08 00b0 ebc1 57ef ad16  .R.h.(......W...
-00002080: 4e4e 4b0a 7494 5294 6805 288a 0800 b090  NNK.t.R.h.(.....
-00002090: fb26 3fec 164e 4e4b 0a74 9452 9468 0528  .&?..NNK.t.R.h.(
-000020a0: 8a08 00b0 2663 89dd 2a16 4e4e 4b0a 7494  ....&c..*.NNK.t.
-000020b0: 5294 6805 288a 0800 b04a dcc5 7d46 174e  R.h.(....J..}F.N
-000020c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 05e9  NK.t.R.h.(......
-000020d0: fa63 b015 4e4e 4b0a 7494 5294 6805 288a  .c..NNK.t.R.h.(.
-000020e0: 0800 b0c6 7e62 7ee5 164e 4e4b 0a74 9452  ....~b~..NNK.t.R
-000020f0: 9468 0528 8a08 00b0 9cce e5c9 4a17 4e4e  .h.(........J.NN
-00002100: 4b0a 7494 5294 6805 288a 0800 b045 33f9  K.t.R.h.(....E3.
-00002110: e739 164e 4e4b 0a74 9452 9468 0528 8a08  .9.NNK.t.R.h.(..
-00002120: 00b0 3b0a 59cc 4616 4e4e 4b0a 7494 5294  ..;.Y.F.NNK.t.R.
-00002130: 6805 288a 0800 b0a5 a2f6 2d08 174e 4e4b  h.(.......-..NNK
-00002140: 0a74 9452 9468 0528 8a08 00b0 f8e9 a531  .t.R.h.(.......1
-00002150: 4217 4e4e 4b0a 7494 5294 6805 288a 0800  B.NNK.t.R.h.(...
-00002160: b051 06b8 7298 164e 4e4b 0a74 9452 9468  .Q..r..NNK.t.R.h
-00002170: 0528 8a08 00b0 47dd 1757 a516 4e4e 4b0a  .(....G..W..NNK.
-00002180: 7494 5294 6805 288a 0800 b0b6 f588 3e4d  t.R.h.(.......>M
+00002050: d5c5 f848 5c16 4e4e 4b0a 7494 5294 6805  ...H\.NNK.t.R.h.
+00002060: 288a 0800 b0fe be08 6f5e 164e 4e4b 0a74  (.......o^.NNK.t
+00002070: 9452 9468 0528 8a08 00b0 27b8 1895 6016  .R.h.(....'...`.
+00002080: 4e4e 4b0a 7494 5294 6805 288a 0800 b050  NNK.t.R.h.(....P
+00002090: b128 bb62 164e 4e4b 0a74 9452 9468 0528  .(.b.NNK.t.R.h.(
+000020a0: 8a08 00b0 79aa 38e1 6416 4e4e 4b0a 7494  ....y.8.d.NNK.t.
+000020b0: 5294 6805 288a 0800 b0a2 a348 0767 164e  R.h.(......H.g.N
+000020c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 cb9c  NK.t.R.h.(......
+000020d0: 582d 6916 4e4e 4b0a 7494 5294 6805 288a  X-i.NNK.t.R.h.(.
+000020e0: 0800 b0a5 04d4 046b 164e 4e4b 0a74 9452  .......k.NNK.t.R
+000020f0: 9468 0528 8a08 00b0 1d8f 7879 6d16 4e4e  .h.(......xym.NN
+00002100: 4b0a 7494 5294 6805 288a 0800 b046 8888  K.t.R.h.(....F..
+00002110: 9f6f 164e 4e4b 0a74 9452 9468 0528 8a08  .o.NNK.t.R.h.(..
+00002120: 00b0 6f81 98c5 7116 4e4e 4b0a 7494 5294  ..o...q.NNK.t.R.
+00002130: 6805 288a 0800 b098 7aa8 eb73 164e 4e4b  h.(.....z..s.NNK
+00002140: 0a74 9452 9468 0528 8a08 00b0 c173 b811  .t.R.h.(.....s..
+00002150: 7616 4e4e 4b0a 7494 5294 6805 288a 0800  v.NNK.t.R.h.(...
+00002160: b0ea 6cc8 3778 164e 4e4b 0a74 9452 9468  ..l.7x.NNK.t.R.h
+00002170: 0528 8a08 00b0 1366 d85d 7a16 4e4e 4b0a  .(.....f.]z.NNK.
+00002180: 7494 5294 6805 288a 0800 b03c 5fe8 837c  t.R.h.(....<_..|
 00002190: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000021a0: 1665 8684 1b17 4e4e 4b0a 7494 5294 6805  .e....NNK.t.R.h.
-000021b0: 288a 0800 b055 5af5 506f 174e 4e4b 0a74  (....UZ.Po.NNK.t
-000021c0: 9452 9468 0528 8a08 00b0 c9f2 39be fd15  .R.h.(......9...
-000021d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b03e  NNK.t.R.h.(....>
-000021e0: 0907 f3e7 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-000021f0: 8a08 00b0 e618 8b59 a115 4e4e 4b0a 7494  .......Y..NNK.t.
-00002200: 5294 6805 288a 0800 b001 beb6 95ff 164e  R.h.(..........N
-00002210: 4e4b 0a74 9452 9468 0528 8a08 00b0 ce9b  NK.t.R.h.(......
-00002220: 0654 0a17 4e4e 4b0a 7494 5294 6805 288a  .T..NNK.t.R.h.(.
-00002230: 0800 b0c6 1c85 a782 174e 4e4b 0a74 9452  .........NNK.t.R
-00002240: 9468 0528 8a08 00b0 6d62 503d 8f17 4e4e  .h.(....mbP=..NN
-00002250: 4b0a 7494 5294 6805 288a 0800 b0fd f44f  K.t.R.h.(......O
-00002260: 9eb1 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002270: 00b0 8c32 c047 9e17 4e4e 4b0a 7494 5294  ...2.G..NNK.t.R.
-00002280: 6805 288a 0800 b024 b96a 6ebf 154e 4e4b  h.(....$.jn..NNK
-00002290: 0a74 9452 9468 0528 8a08 00b0 d76f 17b8  .t.R.h.(.....o..
-000022a0: c716 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000022b0: b000 6927 dec9 164e 4e4b 0a74 9452 9468  ..i'...NNK.t.R.h
-000022c0: 0528 8a08 00b0 4b31 5535 7c17 4e4e 4b0a  .(....K1U5|.NNK.
-000022d0: 7494 5294 6805 288a 0800 b0dd cf50 dc6c  t.R.h.(......P.l
-000022e0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000022f0: c31d d780 e116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00002300: 288a 0800 b05f 8395 6c62 174e 4e4b 0a74  (...._..lb.NNK.t
-00002310: 9452 9468 0528 8a08 00b0 febe 086f 5e16  .R.h.(.......o^.
-00002320: 4e4e 4b0a 7494 5294 6805 288a 0800 b011  NNK.t.R.h.(.....
-00002330: bcb9 ee0e 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00002340: 8a08 00b0 86d2 8623 f916 4e4e 4b0a 7494  .......#..NNK.t.
-00002350: 5294 6805 288a 0800 b046 135f 86f8 174e  R.h.(....F._...N
-00002360: 4e4b 0a74 9452 9468 0528 8a08 00b0 fa6a  NK.t.R.h.(.....j
-00002370: cb90 8715 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00002380: 0800 b043 89da 78ce 154e 4e4b 0a74 9452  ...C..x..NNK.t.R
-00002390: 9468 0528 8a08 00b0 e497 65fa 5b17 4e4e  .h.(......e.[.NN
-000023a0: 4b0a 7494 5294 6805 288a 0800 b00c 299a  K.t.R.h.(.....).
-000023b0: 2614 184e 4e4b 0a74 9452 9468 0528 8a08  &..NNK.t.R.h.(..
-000023c0: 00b0 171c f312 b416 4e4e 4b0a 7494 5294  ........NNK.t.R.
-000023d0: 6805 288a 0800 b0a0 f929 98fb 154e 4e4b  h.(......)...NNK
-000023e0: 0a74 9452 9468 0528 8a08 00b0 fa93 c4a0  .t.R.h.(........
-000023f0: ad17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002400: b054 6743 709c 164e 4e4b 0a74 9452 9468  .TgCp..NNK.t.R.h
-00002410: 0528 8a08 00b0 da6e c5de 6817 4e4e 4b0a  .(.....n..h.NNK.
-00002420: 7494 5294 6805 288a 0800 b0d8 c4a6 6ffd  t.R.h.(.......o.
+000021a0: 16c7 635b 7e16 4e4e 4b0a 7494 5294 6805  ..c[~.NNK.t.R.h.
+000021b0: 288a 0800 b08e 5108 d080 164e 4e4b 0a74  (.....Q....NNK.t
+000021c0: 9452 9468 0528 8a08 00b0 b74a 18f6 8216  .R.h.(.....J....
+000021d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e0  NNK.t.R.h.(.....
+000021e0: 4328 1c85 164e 4e4b 0a74 9452 9468 0528  C(...NNK.t.R.h.(
+000021f0: 8a08 00b0 093d 3842 8716 4e4e 4b0a 7494  .....=8B..NNK.t.
+00002200: 5294 6805 288a 0800 b032 3648 6889 164e  R.h.(....26Hh..N
+00002210: 4e4b 0a74 9452 9468 0528 8a08 00b0 5b2f  NK.t.R.h.(....[/
+00002220: 588e 8b16 4e4e 4b0a 7494 5294 6805 288a  X...NNK.t.R.h.(.
+00002230: 0800 b084 2868 b48d 164e 4e4b 0a74 9452  ....(h...NNK.t.R
+00002240: 9468 0528 8a08 00b0 ad21 78da 8f16 4e4e  .h.(.....!x...NN
+00002250: 4b0a 7494 5294 6805 288a 0800 b0d6 1a88  K.t.R.h.(.......
+00002260: 0092 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002270: 00b0 ff13 9826 9416 4e4e 4b0a 7494 5294  .....&..NNK.t.R.
+00002280: 6805 288a 0800 b028 0da8 4c96 164e 4e4b  h.(....(..L..NNK
+00002290: 0a74 9452 9468 0528 8a08 00b0 5106 b872  .t.R.h.(....Q..r
+000022a0: 9816 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000022b0: b07a ffc7 989a 164e 4e4b 0a74 9452 9468  .z.....NNK.t.R.h
+000022c0: 0528 8a08 00b0 5467 4370 9c16 4e4e 4b0a  .(....TgCp..NNK.
+000022d0: 7494 5294 6805 288a 0800 b0cc f1e7 e49e  t.R.h.(.........
+000022e0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000022f0: f5ea f70a a116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00002300: 288a 0800 b01e e407 31a3 164e 4e4b 0a74  (.......1..NNK.t
+00002310: 9452 9468 0528 8a08 00b0 47dd 1757 a516  .R.h.(....G..W..
+00002320: 4e4e 4b0a 7494 5294 6805 288a 0800 b070  NNK.t.R.h.(....p
+00002330: d627 7da7 164e 4e4b 0a74 9452 9468 0528  .'}..NNK.t.R.h.(
+00002340: 8a08 00b0 99cf 37a3 a916 4e4e 4b0a 7494  ......7...NNK.t.
+00002350: 5294 6805 288a 0800 b0c2 c847 c9ab 164e  R.h.(......G...N
+00002360: 4e4b 0a74 9452 9468 0528 8a08 00b0 ebc1  NK.t.R.h.(......
+00002370: 57ef ad16 4e4e 4b0a 7494 5294 6805 288a  W...NNK.t.R.h.(.
+00002380: 0800 b014 bb67 15b0 164e 4e4b 0a74 9452  .....g...NNK.t.R
+00002390: 9468 0528 8a08 00b0 3db4 773b b216 4e4e  .h.(....=.w;..NN
+000023a0: 4b0a 7494 5294 6805 288a 0800 b017 1cf3  K.t.R.h.(.......
+000023b0: 12b4 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000023c0: 00b0 8fa6 9787 b616 4e4e 4b0a 7494 5294  ........NNK.t.R.
+000023d0: 6805 288a 0800 b0b8 9fa7 adb8 164e 4e4b  h.(..........NNK
+000023e0: 0a74 9452 9468 0528 8a08 00b0 e198 b7d3  .t.R.h.(........
+000023f0: ba16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002400: b00a 92c7 f9bc 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00002410: 0528 8a08 00b0 338b d71f bf16 4e4e 4b0a  .(....3.....NNK.
+00002420: 7494 5294 6805 288a 0800 b05c 84e7 45c1  t.R.h.(....\..E.
 00002430: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002440: ba49 c61c 2417 4e4e 4b0a 7494 5294 6805  .I..$.NNK.t.R.h.
-00002450: 288a 0800 b070 d627 7da7 164e 4e4b 0a74  (....p.'}..NNK.t
-00002460: 9452 9468 0528 8a08 00b0 f041 2b75 9415  .R.h.(.....A+u..
-00002470: 4e4e 4b0a 7494 5294 6805 288a 0800 b0be  NNK.t.R.h.(.....
-00002480: 740a ebd4 154e 4e4b 0a74 9452 9468 0528  t....NNK.t.R.h.(
-00002490: 8a08 00b0 5e2e 06b5 2c17 4e4e 4b0a 7494  ....^...,.NNK.t.
-000024a0: 5294 6805 288a 0800 b07d fe75 bf3b 174e  R.h.(....}.u.;.N
-000024b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 ed6b  NK.t.R.h.(.....k
-000024c0: 765e 1917 4e4e 4b0a 7494 5294 6805 288a  v^..NNK.t.R.h.(.
-000024d0: 0800 b0ef 1595 cd84 174e 4e4b 0a74 9452  .........NNK.t.R
-000024e0: 9468 0528 8a08 00b0 56af 8408 a517 4e4e  .h.(....V.....NN
-000024f0: 4b0a 7494 5294 6805 288a 0800 b006 3e8a  K.t.R.h.(.....>.
-00002500: 1be6 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002510: 00b0 dd44 7af5 e315 4e4e 4b0a 7494 5294  ...Dz...NNK.t.R.
-00002520: 6805 288a 0800 b08e 5108 d080 164e 4e4b  h.(.....Q....NNK
-00002530: 0a74 9452 9468 0528 8a08 00b0 ae76 0792  .t.R.h.(.....v..
-00002540: c516 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002550: b087 2716 db2e 174e 4e4b 0a74 9452 9468  ..'....NNK.t.R.h
-00002560: 0528 8a08 00b0 1b70 30f1 8a17 4e4e 4b0a  .(.....p0...NNK.
-00002570: 7494 5294 6805 288a 0800 b058 30aa 67ea  t.R.h.(....X0.g.
-00002580: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002590: e342 d642 2617 4e4e 4b0a 7494 5294 6805  .B.B&.NNK.t.R.h.
-000025a0: 288a 0800 b09a 117b 18cb 174e 4e4b 0a74  (......{...NNK.t
-000025b0: 9452 9468 0528 8a08 00b0 16c7 635b 7e16  .R.h.(......c[~.
-000025c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e0  NNK.t.R.h.(.....
-000025d0: 4328 1c85 164e 4e4b 0a74 9452 9468 0528  C(...NNK.t.R.h.(
-000025e0: 8a08 00b0 57db 1ab0 b415 4e4e 4b0a 7494  ....W.....NNK.t.
-000025f0: 5294 6805 288a 0800 b05b 2f58 8e8b 164e  R.h.(....[/X...N
-00002600: 4e4b 0a74 9452 9468 0528 8a08 00b0 92a5  NK.t.R.h.(......
-00002610: 45ae 5717 4e4e 4b0a 7494 5294 6805 288a  E.W.NNK.t.R.h.(.
-00002620: 0800 b022 3845 0f7a 174e 4e4b 0a74 9452  ..."8E.z.NNK.t.R
-00002630: 9468 0528 8a08 00b0 8ca7 e960 1516 4e4e  .h.(.......`..NN
-00002640: 4b0a 7494 5294 6805 288a 0800 b007 9319  K.t.R.h.(.......
-00002650: d31b 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002660: 00b0 40b3 2562 5317 4e4e 4b0a 7494 5294  ..@.%bS.NNK.t.R.
-00002670: 6805 288a 0800 b0e1 98b7 d3ba 164e 4e4b  h.(..........NNK
-00002680: 0a74 9452 9468 0528 8a08 00b0 0f3b 948f  .t.R.h.(.....;..
-00002690: c917 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000026a0: b046 8888 9f6f 164e 4e4b 0a74 9452 9468  .F...o.NNK.t.R.h
-000026b0: 0528 8a08 00b0 827e 4945 2216 4e4e 4b0a  .(.....~IE".NNK.
-000026c0: 7494 5294 6805 288a 0800 b06e b7df f4c4  t.R.h.(....n....
+00002440: 857d f76b c316 4e4e 4b0a 7494 5294 6805  .}.k..NNK.t.R.h.
+00002450: 288a 0800 b0ae 7607 92c5 164e 4e4b 0a74  (.....v....NNK.t
+00002460: 9452 9468 0528 8a08 00b0 d76f 17b8 c716  .R.h.(.....o....
+00002470: 4e4e 4b0a 7494 5294 6805 288a 0800 b000  NNK.t.R.h.(.....
+00002480: 6927 dec9 164e 4e4b 0a74 9452 9468 0528  i'...NNK.t.R.h.(
+00002490: 8a08 00b0 2962 3704 cc16 4e4e 4b0a 7494  ....)b7...NNK.t.
+000024a0: 5294 6805 288a 0800 b052 5b47 2ace 164e  R.h.(....R[G*..N
+000024b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b54  NK.t.R.h.(....{T
+000024c0: 5750 d016 4e4e 4b0a 7494 5294 6805 288a  WP..NNK.t.R.h.(.
+000024d0: 0800 b0a4 4d67 76d2 164e 4e4b 0a74 9452  ....Mgv..NNK.t.R
+000024e0: 9468 0528 8a08 00b0 cd46 779c d416 4e4e  .h.(.....Fw...NN
+000024f0: 4b0a 7494 5294 6805 288a 0800 b0f6 3f87  K.t.R.h.(.....?.
+00002500: c2d6 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002510: 00b0 1f39 97e8 d816 4e4e 4b0a 7494 5294  ...9....NNK.t.R.
+00002520: 6805 288a 0800 b048 32a7 0edb 164e 4e4b  h.(....H2....NNK
+00002530: 0a74 9452 9468 0528 8a08 00b0 712b b734  .t.R.h.(....q+.4
+00002540: dd16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002550: b09a 24c7 5adf 164e 4e4b 0a74 9452 9468  ..$.Z..NNK.t.R.h
+00002560: 0528 8a08 00b0 c31d d780 e116 4e4e 4b0a  .(..........NNK.
+00002570: 7494 5294 6805 288a 0800 b0ec 16e7 a6e3  t.R.h.(.........
+00002580: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002590: c67e 627e e516 4e4e 4b0a 7494 5294 6805  .~b~..NNK.t.R.h.
+000025a0: 288a 0800 b03e 0907 f3e7 164e 4e4b 0a74  (....>.....NNK.t
+000025b0: 9452 9468 0528 8a08 00b0 6702 1719 ea16  .R.h.(....g.....
+000025c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b090  NNK.t.R.h.(.....
+000025d0: fb26 3fec 164e 4e4b 0a74 9452 9468 0528  .&?..NNK.t.R.h.(
+000025e0: 8a08 00b0 b9f4 3665 ee16 4e4e 4b0a 7494  ......6e..NNK.t.
+000025f0: 5294 6805 288a 0800 b0e2 ed46 8bf0 164e  R.h.(......F...N
+00002600: 4e4b 0a74 9452 9468 0528 8a08 00b0 0be7  NK.t.R.h.(......
+00002610: 56b1 f216 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
+00002620: 0800 b034 e066 d7f4 164e 4e4b 0a74 9452  ...4.f...NNK.t.R
+00002630: 9468 0528 8a08 00b0 5dd9 76fd f616 4e4e  .h.(....].v...NN
+00002640: 4b0a 7494 5294 6805 288a 0800 b086 d286  K.t.R.h.(.......
+00002650: 23f9 164e 4e4b 0a74 9452 9468 0528 8a08  #..NNK.t.R.h.(..
+00002660: 00b0 afcb 9649 fb16 4e4e 4b0a 7494 5294  .....I..NNK.t.R.
+00002670: 6805 288a 0800 b0d8 c4a6 6ffd 164e 4e4b  h.(.......o..NNK
+00002680: 0a74 9452 9468 0528 8a08 00b0 01be b695  .t.R.h.(........
+00002690: ff16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000026a0: b02a b7c6 bb01 174e 4e4b 0a74 9452 9468  .*.....NNK.t.R.h
+000026b0: 0528 8a08 00b0 53b0 d6e1 0317 4e4e 4b0a  .(....S.....NNK.
+000026c0: 7494 5294 6805 288a 0800 b07c a9e6 0706  t.R.h.(....|....
 000026d0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000026e0: a9cd 3afc b815 4e4e 4b0a 7494 5294 6805  ..:...NNK.t.R.h.
-000026f0: 288a 0800 b01a 90ca 52cc 154e 4e4b 0a74  (.......R..NNK.t
-00002700: 9452 9468 0528 8a08 00b0 a878 ab44 8315  .R.h.(.....x.D..
-00002710: 4e4e 4b0a 7494 5294 6805 288a 0800 b048  NNK.t.R.h.(....H
-00002720: 1f5b ccc6 174e 4e4b 0a74 9452 9468 0528  .[...NNK.t.R.h.(
-00002730: 8a08 00b0 afcb 9649 fb16 4e4e 4b0a 7494  .......I..NNK.t.
-00002740: 5294 6805 288a 0800 b02a b7c6 bb01 174e  R.h.(....*.....N
-00002750: 4e4b 0a74 9452 9468 0528 8a08 00b0 c472  NK.t.R.h.(.....r
-00002760: 6638 1717 4e4e 4b0a 7494 5294 6805 288a  f8..NNK.t.R.h.(.
-00002770: 0800 b0f2 eb49 e4ff 154e 4e4b 0a74 9452  .....I...NNK.t.R
-00002780: 9468 0528 8a08 00b0 3c5f e883 7c16 4e4e  .h.(....<_..|.NN
-00002790: 4b0a 7494 5294 6805 288a 0800 b062 594a  K.t.R.h.(....bYJ
-000027a0: 83dd 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000027b0: 00b0 21e3 b557 4417 4e4e 4b0a 7494 5294  ..!..WD.NNK.t.R.
-000027c0: 6805 288a 0800 b0e5 ecf4 b191 174e 4e4b  h.(..........NNK
-000027d0: 0a74 9452 9468 0528 8a08 00b0 44de 6930  .t.R.h.(....D.i0
-000027e0: 0416 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000027f0: b029 6237 04cc 164e 4e4b 0a74 9452 9468  .)b7...NNK.t.R.h
-00002800: 0528 8a08 00b0 7b54 5750 d016 4e4e 4b0a  .(....{TWP..NNK.
-00002810: 7494 5294 6805 288a 0800 b0cf f095 0b40  t.R.h.(........@
+000026e0: a5a2 f62d 0817 4e4e 4b0a 7494 5294 6805  ...-..NNK.t.R.h.
+000026f0: 288a 0800 b0ce 9b06 540a 174e 4e4b 0a74  (.......T..NNK.t
+00002700: 9452 9468 0528 8a08 00b0 f794 167a 0c17  .R.h.(.......z..
+00002710: 4e4e 4b0a 7494 5294 6805 288a 0800 b020  NNK.t.R.h.(.... 
+00002720: 8e26 a00e 174e 4e4b 0a74 9452 9468 0528  .&...NNK.t.R.h.(
+00002730: 8a08 00b0 4987 36c6 1017 4e4e 4b0a 7494  ....I.6...NNK.t.
+00002740: 5294 6805 288a 0800 b072 8046 ec12 174e  R.h.(....r.F...N
+00002750: 4e4b 0a74 9452 9468 0528 8a08 00b0 9b79  NK.t.R.h.(.....y
+00002760: 5612 1517 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
+00002770: 0800 b0c4 7266 3817 174e 4e4b 0a74 9452  ....rf8..NNK.t.R
+00002780: 9468 0528 8a08 00b0 ed6b 765e 1917 4e4e  .h.(.....kv^..NN
+00002790: 4b0a 7494 5294 6805 288a 0800 b016 6586  K.t.R.h.(.....e.
+000027a0: 841b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000027b0: 00b0 3f5e 96aa 1d17 4e4e 4b0a 7494 5294  ..?^....NNK.t.R.
+000027c0: 6805 288a 0800 b068 57a6 d01f 174e 4e4b  h.(....hW....NNK
+000027d0: 0a74 9452 9468 0528 8a08 00b0 9150 b6f6  .t.R.h.(.....P..
+000027e0: 2117 4e4e 4b0a 7494 5294 6805 288a 0800  !.NNK.t.R.h.(...
+000027f0: b0ba 49c6 1c24 174e 4e4b 0a74 9452 9468  ..I..$.NNK.t.R.h
+00002800: 0528 8a08 00b0 e342 d642 2617 4e4e 4b0a  .(.....B.B&.NNK.
+00002810: 7494 5294 6805 288a 0800 b00c 3ce6 6828  t.R.h.(.....<.h(
 00002820: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002830: 69ac 3588 5517 4e4e 4b0a 7494 5294 6805  i.5.U.NNK.t.R.h.
-00002840: 288a 0800 b061 04bb cba7 154e 4e4b 0a74  (....a.....NNK.t
-00002850: 9452 9468 0528 8a08 00b0 3960 3a5d db15  .R.h.(....9`:]..
-00002860: 4e4e 4b0a 7494 5294 6805 288a 0800 b074  NNK.t.R.h.(....t
-00002870: 2a65 5b7e 174e 4e4b 0a74 9452 9468 0528  *e[~.NNK.t.R.h.(
-00002880: 8a08 00b0 6857 a6d0 1f17 4e4e 4b0a 7494  ....hW....NNK.t.
-00002890: 5294 6805 288a 0800 b0ca d29f 5cbc 174e  R.h.(.......\..N
-000028a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 45be  NK.t.R.h.(....E.
-000028b0: cfce c217 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-000028c0: 0800 b00d 9175 205e 174e 4e4b 0a74 9452  .....u ^.NNK.t.R
-000028d0: 9468 0528 8a08 00b0 fc14 eaff f215 4e4e  .h.(..........NN
-000028e0: 4b0a 7494 5294 6805 288a 0800 b0ad 2178  K.t.R.h.(.....!x
-000028f0: da8f 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002900: 00b0 1ee4 0731 a316 4e4e 4b0a 7494 5294  .....1..NNK.t.R.
-00002910: 6805 288a 0800 b0cc 53c5 bb01 164e 4e4b  h.(.....S....NNK
-00002920: 0a74 9452 9468 0528 8a08 00b0 887c a592  .t.R.h.(.....|..
-00002930: 6417 4e4e 4b0a 7494 5294 6805 288a 0800  d.NNK.t.R.h.(...
-00002940: b0b1 75b5 b866 174e 4e4b 0a74 9452 9468  ..u..f.NNK.t.R.h
-00002950: 0528 8a08 00b0 9b79 5612 1517 4e4e 4b0a  .(.....yV...NNK.
-00002960: 7494 5294 6805 288a 0800 b03a b5c9 1411  t.R.h.(....:....
-00002970: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002980: 8fa6 9787 b616 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00002990: 288a 0800 b0c5 c7f5 ef4c 174e 4e4b 0a74  (........L.NNK.t
-000029a0: 9452 9468 0528 8a08 00b0 7aff c798 9a16  .R.h.(....z.....
-000029b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e8  NNK.t.R.h.(.....
-000029c0: 4d80 af95 174e 4e4b 0a74 9452 9468 0528  M....NNK.t.R.h.(
-000029d0: 8a08 00b0 4c5d ebdc 8b15 4e4e 4b0a 7494  ....L]....NNK.t.
-000029e0: 5294 6805 288a 0800 b0d9 1936 2733 174e  R.h.(......6'3.N
-000029f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 957b  NK.t.R.h.(.....{
-00002a00: fac4 d215 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00002a10: 0800 b012 9c1f 8dcd 174e 4e4b 0a74 9452  .........NNK.t.R
-00002a20: 9468 0528 8a08 00b0 6403 69f2 4816 4e4e  .h.(....d.i.H.NN
-00002a30: 4b0a 7494 5294 6805 288a 0800 b048 32a7  K.t.R.h.(....H2.
-00002a40: 0edb 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002a50: 00b0 6e2c 090e 3c16 4e4e 4b0a 7494 5294  ..n,..<.NNK.t.R.
-00002a60: 6805 288a 0800 b0c8 2881 ed50 174e 4e4b  h.(.....(..P.NNK
-00002a70: 0a74 9452 9468 0528 8a08 00b0 4db2 7a94  .t.R.h.(....M.z.
-00002a80: c115 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002a90: b0b8 9fa7 adb8 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00002aa0: 0528 8a08 00b0 de24 e093 a217 4e4e 4b0a  .(.....$....NNK.
-00002ab0: 7494 5294 6805 288a 0800 b084 2868 b48d  t.R.h.(.....(h..
-00002ac0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002ad0: 4469 4017 8d17 4e4e 4b0a 7494 5294 6805  Di@...NNK.t.R.h.
-00002ae0: 288a 0800 b0e2 ed46 8bf0 164e 4e4b 0a74  (......F...NNK.t
-00002af0: 9452 9468 0528 8a08 00b0 2f37 9a41 e815  .R.h.(..../7.A..
-00002b00: 4e4e 4b0a 7494 5294 6805 288a 0800 b01c  NNK.t.R.h.(.....
-00002b10: 3ae9 c137 164e 4e4b 0a74 9452 9468 0528  :..7.NNK.t.R.h.(
-00002b20: 8a08 00b0 8dfc 7818 4b16 4e4e 4b0a 7494  ......x.K.NNK.t.
-00002b30: 5294 6805 288a 0800 b03a 40a0 fb99 174e  R.h.(....:@....N
-00002b40: 4e4b 0a74 9452 9468 0528 8a08 00b0 9426  NK.t.R.h.(.....&
-00002b50: 6b0d 9d15 4e4e 4b0a 7494 5294 6805 288a  k...NNK.t.R.h.(.
-00002b60: 0800 b057 66f1 963d 174e 4e4b 0a74 9452  ...Wf..=.NNK.t.R
-00002b70: 9468 0528 8a08 00b0 c89d aa06 c815 4e4e  .h.(..........NN
-00002b80: 4b0a 7494 5294 6805 288a 0800 b0df ee98  K.t.R.h.(.......
-00002b90: 644f 164e 4e4b 0a74 9452 9468 0528 8a08  dO.NNK.t.R.h.(..
-00002ba0: 00b0 5985 391f 2016 4e4e 4b0a 7494 5294  ..Y.9. .NNK.t.R.
-00002bb0: 6805 288a 0800 b008 e8a8 8a51 164e 4e4b  h.(........Q.NNK
-00002bc0: 0a74 9452 9468 0528 8a08 00b0 79aa 38e1  .t.R.h.(....y.8.
-00002bd0: 6416 4e4e 4b0a 7494 5294 6805 288a 0800  d.NNK.t.R.h.(...
-00002be0: b06f 8198 c571 164e 4e4b 0a74 9452 9468  .o...q.NNK.t.R.h
-00002bf0: 0528 8a08 00b0 4108 b519 8917 4e4e 4b0a  .(....A.....NNK.
-00002c00: 7494 5294 6805 288a 0800 b02e e20a 8ab2  t.R.h.(.........
-00002c10: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002c20: 73d5 d5a3 4817 4e4e 4b0a 7494 5294 6805  s...H.NNK.t.R.h.
-00002c30: 288a 0800 b06a 01c5 3f8b 174e 4e4b 0a74  (....j..?..NNK.t
-00002c40: 9452 9468 0528 8a08 00b0 b2ca 4470 9c17  .R.h.(......Dp..
-00002c50: 4e4e 4b0a 7494 5294 6805 288a 0800 b096  NNK.t.R.h.(.....
-00002c60: d089 7c08 164e 4e4b 0a74 9452 9468 0528  ..|..NNK.t.R.h.(
-00002c70: 8a08 00b0 7e53 0577 7117 4e4e 4b0a 7494  ....~S.wq.NNK.t.
-00002c80: 5294 6805 288a 0800 b0d0 4525 c375 174e  R.h.(.....E%.u.N
-00002c90: 4e4b 0a74 9452 9468 0528 8a08 00b0 d61a  NK.t.R.h.(......
-00002ca0: 8800 9216 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00002cb0: 0800 b09d 2375 8180 174e 4e4b 0a74 9452  ....#u...NNK.t.R
-00002cc0: 9468 0528 8a08 00b0 5ada c8d6 5516 4e4e  .h.(....Z...U.NN
-00002cd0: 4b0a 7494 5294 6805 288a 0800 b067 0217  K.t.R.h.(....g..
-00002ce0: 19ea 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002cf0: 00b0 8afd caf1 a915 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00002d00: 6805 288a 0800 b0b4 4b6a cfe1 154e 4e4b  h.(.....Kj...NNK
-00002d10: 0a74 9452 9468 0528 8a08 00b0 4987 36c6  .t.R.h.(....I.6.
-00002d20: 1017 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002d30: b017 ba15 3c51 174e 4e4b 0a74 9452 9468  ....<Q.NNK.t.R.h
-00002d40: 0528 8a08 00b0 3535 f68e 2a17 4e4e 4b0a  .(....55..*.NNK.
-00002d50: 7494 5294 6805 288a 0800 b02c 61e5 2a6d  t.R.h.(....,a.*m
+00002830: 3535 f68e 2a17 4e4e 4b0a 7494 5294 6805  55..*.NNK.t.R.h.
+00002840: 288a 0800 b05e 2e06 b52c 174e 4e4b 0a74  (....^...,.NNK.t
+00002850: 9452 9468 0528 8a08 00b0 8727 16db 2e17  .R.h.(.....'....
+00002860: 4e4e 4b0a 7494 5294 6805 288a 0800 b0b0  NNK.t.R.h.(.....
+00002870: 2026 0131 174e 4e4b 0a74 9452 9468 0528   &.1.NNK.t.R.h.(
+00002880: 8a08 00b0 d919 3627 3317 4e4e 4b0a 7494  ......6'3.NNK.t.
+00002890: 5294 6805 288a 0800 b002 1346 4d35 174e  R.h.(......FM5.N
+000028a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2b0c  NK.t.R.h.(....+.
+000028b0: 5673 3717 4e4e 4b0a 7494 5294 6805 288a  Vs7.NNK.t.R.h.(.
+000028c0: 0800 b054 0566 9939 174e 4e4b 0a74 9452  ...T.f.9.NNK.t.R
+000028d0: 9468 0528 8a08 00b0 7dfe 75bf 3b17 4e4e  .h.(....}.u.;.NN
+000028e0: 4b0a 7494 5294 6805 288a 0800 b057 66f1  K.t.R.h.(....Wf.
+000028f0: 963d 174e 4e4b 0a74 9452 9468 0528 8a08  .=.NNK.t.R.h.(..
+00002900: 00b0 cff0 950b 4017 4e4e 4b0a 7494 5294  ......@.NNK.t.R.
+00002910: 6805 288a 0800 b0f8 e9a5 3142 174e 4e4b  h.(.......1B.NNK
+00002920: 0a74 9452 9468 0528 8a08 00b0 21e3 b557  .t.R.h.(....!..W
+00002930: 4417 4e4e 4b0a 7494 5294 6805 288a 0800  D.NNK.t.R.h.(...
+00002940: b04a dcc5 7d46 174e 4e4b 0a74 9452 9468  .J..}F.NNK.t.R.h
+00002950: 0528 8a08 00b0 73d5 d5a3 4817 4e4e 4b0a  .(....s...H.NNK.
+00002960: 7494 5294 6805 288a 0800 b09c cee5 c94a  t.R.h.(........J
+00002970: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002980: c5c7 f5ef 4c17 4e4e 4b0a 7494 5294 6805  ....L.NNK.t.R.h.
+00002990: 288a 0800 b0ee c005 164f 174e 4e4b 0a74  (........O.NNK.t
+000029a0: 9452 9468 0528 8a08 00b0 c828 81ed 5017  .R.h.(.....(..P.
+000029b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b040  NNK.t.R.h.(....@
+000029c0: b325 6253 174e 4e4b 0a74 9452 9468 0528  .%bS.NNK.t.R.h.(
+000029d0: 8a08 00b0 69ac 3588 5517 4e4e 4b0a 7494  ....i.5.U.NNK.t.
+000029e0: 5294 6805 288a 0800 b092 a545 ae57 174e  R.h.(......E.W.N
+000029f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 bb9e  NK.t.R.h.(......
+00002a00: 55d4 5917 4e4e 4b0a 7494 5294 6805 288a  U.Y.NNK.t.R.h.(.
+00002a10: 0800 b0e4 9765 fa5b 174e 4e4b 0a74 9452  .....e.[.NNK.t.R
+00002a20: 9468 0528 8a08 00b0 0d91 7520 5e17 4e4e  .h.(......u ^.NN
+00002a30: 4b0a 7494 5294 6805 288a 0800 b036 8a85  K.t.R.h.(....6..
+00002a40: 4660 174e 4e4b 0a74 9452 9468 0528 8a08  F`.NNK.t.R.h.(..
+00002a50: 00b0 5f83 956c 6217 4e4e 4b0a 7494 5294  .._..lb.NNK.t.R.
+00002a60: 6805 288a 0800 b088 7ca5 9264 174e 4e4b  h.(.....|..d.NNK
+00002a70: 0a74 9452 9468 0528 8a08 00b0 b175 b5b8  .t.R.h.(.....u..
+00002a80: 6617 4e4e 4b0a 7494 5294 6805 288a 0800  f.NNK.t.R.h.(...
+00002a90: b0da 6ec5 de68 174e 4e4b 0a74 9452 9468  ..n..h.NNK.t.R.h
+00002aa0: 0528 8a08 00b0 0368 d504 6b17 4e4e 4b0a  .(.....h..k.NNK.
+00002ab0: 7494 5294 6805 288a 0800 b0dd cf50 dc6c  t.R.h.(......P.l
+00002ac0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002ad0: 555a f550 6f17 4e4e 4b0a 7494 5294 6805  UZ.Po.NNK.t.R.h.
+00002ae0: 288a 0800 b07e 5305 7771 174e 4e4b 0a74  (....~S.wq.NNK.t
+00002af0: 9452 9468 0528 8a08 00b0 a74c 159d 7317  .R.h.(.....L..s.
+00002b00: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d0  NNK.t.R.h.(.....
+00002b10: 4525 c375 174e 4e4b 0a74 9452 9468 0528  E%.u.NNK.t.R.h.(
+00002b20: 8a08 00b0 f93e 35e9 7717 4e4e 4b0a 7494  .....>5.w.NNK.t.
+00002b30: 5294 6805 288a 0800 b022 3845 0f7a 174e  R.h.(...."8E.z.N
+00002b40: 4e4b 0a74 9452 9468 0528 8a08 00b0 4b31  NK.t.R.h.(....K1
+00002b50: 5535 7c17 4e4e 4b0a 7494 5294 6805 288a  U5|.NNK.t.R.h.(.
+00002b60: 0800 b074 2a65 5b7e 174e 4e4b 0a74 9452  ...t*e[~.NNK.t.R
+00002b70: 9468 0528 8a08 00b0 9d23 7581 8017 4e4e  .h.(.....#u...NN
+00002b80: 4b0a 7494 5294 6805 288a 0800 b077 8bf0  K.t.R.h.(....w..
+00002b90: 5882 174e 4e4b 0a74 9452 9468 0528 8a08  X..NNK.t.R.h.(..
+00002ba0: 00b0 a084 007f 8417 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00002bb0: 6805 288a 0800 b0c9 7d10 a586 174e 4e4b  h.(.....}....NNK
+00002bc0: 0a74 9452 9468 0528 8a08 00b0 4108 b519  .t.R.h.(....A...
+00002bd0: 8917 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002be0: b01b 7030 f18a 174e 4e4b 0a74 9452 9468  ..p0...NNK.t.R.h
+00002bf0: 0528 8a08 00b0 4469 4017 8d17 4e4e 4b0a  .(....Di@...NNK.
+00002c00: 7494 5294 6805 288a 0800 b06d 6250 3d8f  t.R.h.(....mbP=.
+00002c10: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002c20: e5ec f4b1 9117 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00002c30: 288a 0800 b0bf 5470 8993 174e 4e4b 0a74  (.....Tp...NNK.t
+00002c40: 9452 9468 0528 8a08 00b0 e84d 80af 9517  .R.h.(.....M....
+00002c50: 4e4e 4b0a 7494 5294 6805 288a 0800 b011  NNK.t.R.h.(.....
+00002c60: 4790 d597 174e 4e4b 0a74 9452 9468 0528  G....NNK.t.R.h.(
+00002c70: 8a08 00b0 3a40 a0fb 9917 4e4e 4b0a 7494  ....:@....NNK.t.
+00002c80: 5294 6805 288a 0800 b0b2 ca44 709c 174e  R.h.(......Dp..N
+00002c90: 4e4b 0a74 9452 9468 0528 8a08 00b0 8c32  NK.t.R.h.(.....2
+00002ca0: c047 9e17 4e4e 4b0a 7494 5294 6805 288a  .G..NNK.t.R.h.(.
+00002cb0: 0800 b0b5 2bd0 6da0 174e 4e4b 0a74 9452  ....+.m..NNK.t.R
+00002cc0: 9468 0528 8a08 00b0 de24 e093 a217 4e4e  .h.(.....$....NN
+00002cd0: 4b0a 7494 5294 6805 288a 0800 b056 af84  K.t.R.h.(....V..
+00002ce0: 08a5 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002cf0: 00b0 3017 00e0 a617 4e4e 4b0a 7494 5294  ..0.....NNK.t.R.
+00002d00: 6805 288a 0800 b059 1010 06a9 174e 4e4b  h.(....Y.....NNK
+00002d10: 0a74 9452 9468 0528 8a08 00b0 8209 202c  .t.R.h.(...... ,
+00002d20: ab17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002d30: b0fa 93c4 a0ad 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00002d40: 0528 8a08 00b0 d4fb 3f78 af17 4e4e 4b0a  .(......?x..NNK.
+00002d50: 7494 5294 6805 288a 0800 b0fd f44f 9eb1  t.R.h.(......O..
 00002d60: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002d70: 76ab 8aba c315 4e4e 4b0a 7494 5294 6805  v.....NNK.t.R.h.
-00002d80: 288a 0800 b01d 8f78 796d 164e 4e4b 0a74  (......xym.NNK.t
-00002d90: 9452 9468 0528 8a08 00b0 f196 ba2c ca15  .R.h.(.......,..
-00002da0: 4e4e 4b0a 7494 5294 6805 288a 0800 b06d  NNK.t.R.h.(....m
-00002db0: d779 5606 164e 4e4b 0a74 9452 9468 0528  .yV..NNK.t.R.h.(
-00002dc0: 8a08 00b0 bd1f 7b33 9f15 4e4e 4b0a 7494  ......{3..NNK.t.
-00002dd0: 5294 6805 288a 0800 b028 0da8 4c96 164e  R.h.(....(..L..N
-00002de0: 4e4b 0a74 9452 9468 0528 8a08 00b0 3db4  NK.t.R.h.(....=.
-00002df0: 773b b216 4e4e 4b0a 7494 5294 6805 288a  w;..NNK.t.R.h.(.
-00002e00: 0800 b00a 92c7 f9bc 164e 4e4b 0a74 9452  .........NNK.t.R
-00002e10: 9468 0528 8a08 00b0 c771 145f b817 4e4e  .h.(.....q._..NN
-00002e20: 4b0a 7494 5294 6805 288a 0800 b011 4790  K.t.R.h.(.....G.
-00002e30: d597 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002e40: 00b0 31e1 b8b0 5316 4e4e 4b0a 7494 5294  ..1...S.NNK.t.R.
-00002e50: 6805 288a 0800 b0aa 22ca b3ee 154e 4e4b  h.(....."....NNK
-00002e60: 0a74 9452 9468 0528 8a08 00b0 4f5c 9903  .t.R.h.(....O\..
-00002e70: 2d16 4e4e 4b0a 7494 5294 6805 288a 0800  -.NNK.t.R.h.(...
-00002e80: b0f6 3f87 c2d6 164e 4e4b 0a74 9452 9468  ..?....NNK.t.R.h
-00002e90: 0528 8a08 00b0 5405 6699 3917 4e4e 4b0a  .(....T.f.9.NNK.
-00002ea0: 7494 5294 6805 288a 0800 b0f5 eaf7 0aa1  t.R.h.(.........
-00002eb0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002ec0: dcef ea3d ae15 4e4e 4b0a 7494 5294 6805  ...=..NNK.t.R.h.
-00002ed0: 288a 0800 b042 344b c198 154e 4e4b 0a74  (....B4K...NNK.t
-00002ee0: 9452 9468 0528 8a08 00b0 f794 167a 0c17  .R.h.(.......z..
-00002ef0: 4e4e 4b0a 7494 5294 6805 288a 0800 b097  NNK.t.R.h.(.....
-00002f00: 2519 343e 164e 4e4b 0a74 9452 9468 0528  %.4>.NNK.t.R.h.(
-00002f10: 8a08 00b0 308c 29f9 1d16 4e4e 4b0a 7494  ....0.)...NNK.t.
-00002f20: 5294 6805 288a 0800 b030 1700 e0a6 174e  R.h.(....0.....N
-00002f30: 4e4b 0a74 9452 9468 0528 8a08 00b0 34e0  NK.t.R.h.(....4.
-00002f40: 66d7 f416 4e4e 4b0a 7494 5294 6805 288a  f...NNK.t.R.h.(.
-00002f50: 0800 b0a7 4c15 9d73 174e 4e4b 0a74 9452  ....L..s.NNK.t.R
-00002f60: 9468 0528 8a08 00b0 778b f058 8217 4e4e  .h.(....w..X..NN
-00002f70: 4b0a 7494 5294 6805 288a 0800 b0a1 4eb9  K.t.R.h.(.....N.
-00002f80: 4f31 164e 4e4b 0a74 9452 9468 0528 8a08  O1.NNK.t.R.h.(..
-00002f90: 00b0 4fe7 6fea b517 4e4e 4b0a 7494 5294  ..O.o...NNK.t.R.
-00002fa0: 658c 0846 494e 4e49 4654 5994 5d94 2868  e..FINNIFTY.].(h
-00002fb0: 0528 8a08 00b0 1bd2 0dc8 ed16 4e4e 4b0a  .(..........NNK.
-00002fc0: 7494 5294 6805 288a 0800 b0c2 c847 c9ab  t.R.h.(......G..
+00002d70: 26ee 5fc4 b317 4e4e 4b0a 7494 5294 6805  &._...NNK.t.R.h.
+00002d80: 288a 0800 b04f e76f eab5 174e 4e4b 0a74  (....O.o...NNK.t
+00002d90: 9452 9468 0528 8a08 00b0 c771 145f b817  .R.h.(.....q._..
+00002da0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a1  NNK.t.R.h.(.....
+00002db0: d98f 36ba 174e 4e4b 0a74 9452 9468 0528  ..6..NNK.t.R.h.(
+00002dc0: 8a08 00b0 cad2 9f5c bc17 4e4e 4b0a 7494  .......\..NNK.t.
+00002dd0: 5294 6805 288a 0800 b0f3 cbaf 82be 174e  R.h.(..........N
+00002de0: 4e4b 0a74 9452 9468 0528 8a08 00b0 1cc5  NK.t.R.h.(......
+00002df0: bfa8 c017 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00002e00: 0800 b06b 5654 f7c0 174e 4e4b 0a74 9452  ...kVT...NNK.t.R
+00002e10: 9468 0528 8a08 00b0 45be cfce c217 4e4e  .h.(....E.....NN
+00002e20: 4b0a 7494 5294 6805 288a 0800 b06e b7df  K.t.R.h.(....n..
+00002e30: f4c4 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002e40: 00b0 481f 5bcc c617 4e4e 4b0a 7494 5294  ..H.[...NNK.t.R.
+00002e50: 6805 288a 0800 b0c0 a9ff 40c9 174e 4e4b  h.(.......@..NNK
+00002e60: 0a74 9452 9468 0528 8a08 00b0 9a11 7b18  .t.R.h.(......{.
+00002e70: cb17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002e80: b012 9c1f 8dcd 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00002e90: 0528 8a08 00b0 3b95 2fb3 cf17 4e4e 4b0a  .(....;./...NNK.
+00002ea0: 7494 5294 6805 288a 0800 b064 8e3f d9d1  t.R.h.(....d.?..
+00002eb0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002ec0: 8d87 4fff d317 4e4e 4b0a 7494 5294 6805  ..O...NNK.t.R.h.
+00002ed0: 288a 0800 b031 6c8f 97dc 174e 4e4b 0a74  (....1l....NNK.t
+00002ee0: 9452 9468 0528 8a08 00b0 4613 5f86 f817  .R.h.(....F._...
+00002ef0: 4e4e 4b0a 7494 5294 6805 288a 0800 b00c  NNK.t.R.h.(.....
+00002f00: 299a 2614 184e 4e4b 0a74 9452 9468 0528  ).&..NNK.t.R.h.(
+00002f10: 8a08 00b0 7061 fe63 3018 4e4e 4b0a 7494  ....pa.c0.NNK.t.
+00002f20: 5294 658c 0846 494e 4e49 4654 5994 5d94  R.e..FINNIFTY.].
+00002f30: 2868 0528 8a08 00b0 accc e822 5a16 4e4e  (h.(......."Z.NN
+00002f40: 4b0a 7494 5294 6805 288a 0800 b0d5 c5f8  K.t.R.h.(.......
+00002f50: 485c 164e 4e4b 0a74 9452 9468 0528 8a08  H\.NNK.t.R.h.(..
+00002f60: 00b0 febe 086f 5e16 4e4e 4b0a 7494 5294  .....o^.NNK.t.R.
+00002f70: 6805 288a 0800 b027 b818 9560 164e 4e4b  h.(....'...`.NNK
+00002f80: 0a74 9452 9468 0528 8a08 00b0 50b1 28bb  .t.R.h.(....P.(.
+00002f90: 6216 4e4e 4b0a 7494 5294 6805 288a 0800  b.NNK.t.R.h.(...
+00002fa0: b079 aa38 e164 164e 4e4b 0a74 9452 9468  .y.8.d.NNK.t.R.h
+00002fb0: 0528 8a08 00b0 a2a3 4807 6716 4e4e 4b0a  .(......H.g.NNK.
+00002fc0: 7494 5294 6805 288a 0800 b0cb 9c58 2d69  t.R.h.(......X-i
 00002fd0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002fe0: 8e3e bc8d 6c17 4e4e 4b0a 7494 5294 6805  .>..l.NNK.t.R.h.
-00002ff0: 288a 0800 b012 fefc 6330 174e 4e4b 0a74  (.......c0.NNK.t
-00003000: 9452 9468 0528 8a08 00b0 8415 1c72 7917  .R.h.(.......ry.
-00003010: 4e4e 4b0a 7494 5294 6805 288a 0800 b063  NNK.t.R.h.(....c
-00003020: 9b8d f8fe 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00003030: 8a08 00b0 9f91 4e9e b116 4e4e 4b0a 7494  ......N...NNK.t.
-00003040: 5294 6805 288a 0800 b0dd 312e b3cf 164e  R.h.(.....1....N
-00003050: 4e4b 0a74 9452 9468 0528 8a08 00b0 f482  NK.t.R.h.(......
-00003060: 1c11 5717 4e4e 4b0a 7494 5294 6805 288a  ..W.NNK.t.R.h.(.
-00003070: 0800 b078 425d e71a 174e 4e4b 0a74 9452  ...xB]...NNK.t.R
-00003080: 9468 0528 8a08 00b0 5b1c 0c4c 7717 4e4e  .h.(....[..Lw.NN
-00003090: 4b0a 7494 5294 6805 288a 0800 b0a2 a348  K.t.R.h.(......H
-000030a0: 0767 164e 4e4b 0a74 9452 9468 0528 8a08  .g.NNK.t.R.h.(..
-000030b0: 00b0 3236 4868 8916 4e4e 4b0a 7494 5294  ..26Hh..NNK.t.R.
-000030c0: 6805 288a 0800 b071 186b f2c8 174e 4e4b  h.(....q.k...NNK
-000030d0: 0a74 9452 9468 0528 8a08 00b0 8c94 9d1e  .t.R.h.(........
-000030e0: 0117 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000030f0: b0b5 8dad 4403 174e 4e4b 0a74 9452 9468  ....D..NNK.t.R.h
-00003100: 0528 8a08 00b0 aa0f 7e71 da16 4e4e 4b0a  .(......~q..NNK.
-00003110: 7494 5294 6805 288a 0800 b098 7aa8 eb73  t.R.h.(.....z..s
+00002fe0: a504 d404 6b16 4e4e 4b0a 7494 5294 6805  ....k.NNK.t.R.h.
+00002ff0: 288a 0800 b01d 8f78 796d 164e 4e4b 0a74  (......xym.NNK.t
+00003000: 9452 9468 0528 8a08 00b0 4688 889f 6f16  .R.h.(....F...o.
+00003010: 4e4e 4b0a 7494 5294 6805 288a 0800 b06f  NNK.t.R.h.(....o
+00003020: 8198 c571 164e 4e4b 0a74 9452 9468 0528  ...q.NNK.t.R.h.(
+00003030: 8a08 00b0 987a a8eb 7316 4e4e 4b0a 7494  .....z..s.NNK.t.
+00003040: 5294 6805 288a 0800 b0c1 73b8 1176 164e  R.h.(.....s..v.N
+00003050: 4e4b 0a74 9452 9468 0528 8a08 00b0 ea6c  NK.t.R.h.(.....l
+00003060: c837 7816 4e4e 4b0a 7494 5294 6805 288a  .7x.NNK.t.R.h.(.
+00003070: 0800 b013 66d8 5d7a 164e 4e4b 0a74 9452  ....f.]z.NNK.t.R
+00003080: 9468 0528 8a08 00b0 3c5f e883 7c16 4e4e  .h.(....<_..|.NN
+00003090: 4b0a 7494 5294 6805 288a 0800 b016 c763  K.t.R.h.(......c
+000030a0: 5b7e 164e 4e4b 0a74 9452 9468 0528 8a08  [~.NNK.t.R.h.(..
+000030b0: 00b0 8e51 08d0 8016 4e4e 4b0a 7494 5294  ...Q....NNK.t.R.
+000030c0: 6805 288a 0800 b0b7 4a18 f682 164e 4e4b  h.(.....J....NNK
+000030d0: 0a74 9452 9468 0528 8a08 00b0 e043 281c  .t.R.h.(.....C(.
+000030e0: 8516 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000030f0: b009 3d38 4287 164e 4e4b 0a74 9452 9468  ..=8B..NNK.t.R.h
+00003100: 0528 8a08 00b0 3236 4868 8916 4e4e 4b0a  .(....26Hh..NNK.
+00003110: 7494 5294 6805 288a 0800 b05b 2f58 8e8b  t.R.h.(....[/X..
 00003120: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003130: a347 6953 eb16 4e4e 4b0a 7494 5294 6805  .GiS..NNK.t.R.h.
-00003140: 288a 0800 b073 2467 3897 174e 4e4b 0a74  (....s$g8..NNK.t
-00003150: 9452 9468 0528 8a08 00b0 31ce 6c6e 3f17  .R.h.(....1.ln?.
-00003160: 4e4e 4b0a 7494 5294 6805 288a 0800 b04f  NNK.t.R.h.(....O
-00003170: 494d c118 174e 4e4b 0a74 9452 9468 0528  IM...NNK.t.R.h.(
-00003180: 8a08 00b0 1a7d 7e10 b816 4e4e 4b0a 7494  .....}~...NNK.t.
-00003190: 5294 6805 288a 0800 b0de 86bd 6a05 174e  R.h.(.......j..N
-000031a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 c173  NK.t.R.h.(.....s
-000031b0: b811 7616 4e4e 4b0a 7494 5294 6805 288a  ..v.NNK.t.R.h.(.
-000031c0: 0800 b0ea 6cc8 3778 164e 4e4b 0a74 9452  ....l.7x.NNK.t.R
-000031d0: 9468 0528 8a08 00b0 826b fd02 0e17 4e4e  .h.(.....k....NN
-000031e0: 4b0a 7494 5294 6805 288a 0800 b0b7 37cc  K.t.R.h.(.....7.
-000031f0: b36e 174e 4e4b 0a74 9452 9468 0528 8a08  .n.NNK.t.R.h.(..
-00003200: 00b0 50b1 28bb 6216 4e4e 4b0a 7494 5294  ..P.(.b.NNK.t.R.
-00003210: 6805 288a 0800 b044 cb1d eeef 164e 4e4b  h.(....D.....NNK
-00003220: 0a74 9452 9468 0528 8a08 00b0 a504 d404  .t.R.h.(........
-00003230: 6b16 4e4e 4b0a 7494 5294 6805 288a 0800  k.NNK.t.R.h.(...
-00003240: b006 2b3e d9d1 164e 4e4b 0a74 9452 9468  ..+>...NNK.t.R.h
-00003250: 0528 8a08 00b0 c160 6ccf 6117 4e4e 4b0a  .(.....`l.a.NNK.
-00003260: 7494 5294 6805 288a 0800 b0e1 856b 91a6  t.R.h.(......k..
-00003270: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003280: 3c4c 9c41 6817 4e4e 4b0a 7494 5294 6805  <L.Ah.NNK.t.R.h.
-00003290: 288a 0800 b099 bceb 6095 174e 4e4b 0a74  (.......`..NNK.t
-000032a0: 9452 9468 0528 8a08 00b0 d75c cb75 b317  .R.h.(.....\.u..
-000032b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0ff  NNK.t.R.h.(.....
-000032c0: 004c e47f 174e 4e4b 0a74 9452 9468 0528  .L...NNK.t.R.h.(
-000032d0: 8a08 00b0 b74a 18f6 8216 4e4e 4b0a 7494  .....J....NNK.t.
-000032e0: 5294 6805 288a 0800 b014 bb67 15b0 164e  R.h.(......g...N
-000032f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 27b8  NK.t.R.h.(....'.
-00003300: 1895 6016 4e4e 4b0a 7494 5294 6805 288a  ..`.NNK.t.R.h.(.
-00003310: 0800 b05a c77c 9441 174e 4e4b 0a74 9452  ...Z.|.A.NNK.t.R
-00003320: 9468 0528 8a08 00b0 f838 37c6 9017 4e4e  .h.(.....87...NN
-00003330: 4b0a 7494 5294 6805 288a 0800 b0e9 04ed  K.t.R.h.(.......
-00003340: 3d2e 174e 4e4b 0a74 9452 9468 0528 8a08  =..NNK.t.R.h.(..
-00003350: 00b0 0780 cd90 0717 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00003360: 6805 288a 0800 b0e7 5ace cec2 164e 4e4b  h.(.....Z....NNK
-00003370: 0a74 9452 9468 0528 8a08 00b0 1366 d85d  .t.R.h.(.....f.]
-00003380: 7a16 4e4e 4b0a 7494 5294 6805 288a 0800  z.NNK.t.R.h.(...
-00003390: b0ac cce8 225a 164e 4e4b 0a74 9452 9468  ...."Z.NNK.t.R.h
-000033a0: 0528 8a08 00b0 8b3f 0e67 cb16 4e4e 4b0a  .(.....?.g..NNK.
-000033b0: 7494 5294 6805 288a 0800 b009 3d38 4287  t.R.h.(.....=8B.
+00003130: 8428 68b4 8d16 4e4e 4b0a 7494 5294 6805  .(h...NNK.t.R.h.
+00003140: 288a 0800 b0ad 2178 da8f 164e 4e4b 0a74  (.....!x...NNK.t
+00003150: 9452 9468 0528 8a08 00b0 d61a 8800 9216  .R.h.(..........
+00003160: 4e4e 4b0a 7494 5294 6805 288a 0800 b0ff  NNK.t.R.h.(.....
+00003170: 1398 2694 164e 4e4b 0a74 9452 9468 0528  ..&..NNK.t.R.h.(
+00003180: 8a08 00b0 280d a84c 9616 4e4e 4b0a 7494  ....(..L..NNK.t.
+00003190: 5294 6805 288a 0800 b051 06b8 7298 164e  R.h.(....Q..r..N
+000031a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 7aff  NK.t.R.h.(....z.
+000031b0: c798 9a16 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+000031c0: 0800 b054 6743 709c 164e 4e4b 0a74 9452  ...TgCp..NNK.t.R
+000031d0: 9468 0528 8a08 00b0 ccf1 e7e4 9e16 4e4e  .h.(..........NN
+000031e0: 4b0a 7494 5294 6805 288a 0800 b0f5 eaf7  K.t.R.h.(.......
+000031f0: 0aa1 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00003200: 00b0 1ee4 0731 a316 4e4e 4b0a 7494 5294  .....1..NNK.t.R.
+00003210: 6805 288a 0800 b047 dd17 57a5 164e 4e4b  h.(....G..W..NNK
+00003220: 0a74 9452 9468 0528 8a08 00b0 70d6 277d  .t.R.h.(....p.'}
+00003230: a716 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003240: b099 cf37 a3a9 164e 4e4b 0a74 9452 9468  ...7...NNK.t.R.h
+00003250: 0528 8a08 00b0 c2c8 47c9 ab16 4e4e 4b0a  .(......G...NNK.
+00003260: 7494 5294 6805 288a 0800 b0eb c157 efad  t.R.h.(......W..
+00003270: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003280: 7698 3e78 af16 4e4e 4b0a 7494 5294 6805  v.>x..NNK.t.R.h.
+00003290: 288a 0800 b014 bb67 15b0 164e 4e4b 0a74  (......g...NNK.t
+000032a0: 9452 9468 0528 8a08 00b0 9f91 4e9e b116  .R.h.(......N...
+000032b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b03d  NNK.t.R.h.(....=
+000032c0: b477 3bb2 164e 4e4b 0a74 9452 9468 0528  .w;..NNK.t.R.h.(
+000032d0: 8a08 00b0 c88a 5ec4 b316 4e4e 4b0a 7494  ......^...NNK.t.
+000032e0: 5294 6805 288a 0800 b017 1cf3 12b4 164e  R.h.(..........N
+000032f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 f183  NK.t.R.h.(......
+00003300: 6eea b516 4e4e 4b0a 7494 5294 6805 288a  n...NNK.t.R.h.(.
+00003310: 0800 b08f a697 87b6 164e 4e4b 0a74 9452  .........NNK.t.R
+00003320: 9468 0528 8a08 00b0 1a7d 7e10 b816 4e4e  .h.(.....}~...NN
+00003330: 4b0a 7494 5294 6805 288a 0800 b0b8 9fa7  K.t.R.h.(.......
+00003340: adb8 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00003350: 00b0 4376 8e36 ba16 4e4e 4b0a 7494 5294  ..Cv.6..NNK.t.R.
+00003360: 6805 288a 0800 b06c 6f9e 5cbc 164e 4e4b  h.(....lo.\..NNK
+00003370: 0a74 9452 9468 0528 8a08 00b0 9568 ae82  .t.R.h.(.....h..
+00003380: be16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003390: b0be 61be a8c0 164e 4e4b 0a74 9452 9468  ..a....NNK.t.R.h
+000033a0: 0528 8a08 00b0 e75a cece c216 4e4e 4b0a  .(.....Z....NNK.
+000033b0: 7494 5294 6805 288a 0800 b010 54de f4c4  t.R.h.(.....T...
 000033c0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000033d0: 64f0 1cb0 3417 4e4e 4b0a 7494 5294 6805  d...4.NNK.t.R.h.
-000033e0: 288a 0800 b096 bd3d 3af4 164e 4e4b 0a74  (......=:..NNK.t
-000033f0: 9452 9468 0528 8a08 00b0 8f93 4b45 a217  .R.h.(......KE..
-00003400: 4e4e 4b0a 7494 5294 6805 288a 0800 b0cc  NNK.t.R.h.(.....
-00003410: f1e7 e49e 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00003420: 8a08 00b0 ff13 9826 9416 4e4e 4b0a 7494  .......&..NNK.t.
-00003430: 5294 6805 288a 0800 b01d 7c2c 3759 174e  R.h.(.....|,7Y.N
-00003440: 4e4b 0a74 9452 9468 0528 8a08 00b0 ae63  NK.t.R.h.(.....c
-00003450: bb4f b117 4e4e 4b0a 7494 5294 6805 288a  .O..NNK.t.R.h.(.
-00003460: 0800 b0e1 e748 6809 174e 4e4b 0a74 9452  .....Hh..NNK.t.R
-00003470: 9468 0528 8a08 00b0 2650 3d9b 1617 4e4e  .h.(....&P=...NN
-00003480: 4b0a 7494 5294 6805 288a 0800 b03a a27d  K.t.R.h.(....:.}
-00003490: d2fc 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000034a0: 00b0 1c27 9d7f 2317 4e4e 4b0a 7494 5294  ...'..#.NNK.t.R.
-000034b0: 6805 288a 0800 b0c8 8a5e c4b3 164e 4e4b  h.(......^...NNK
-000034c0: 0a74 9452 9468 0528 8a08 00b0 9712 cdf1  .t.R.h.(........
-000034d0: 2917 4e4e 4b0a 7494 5294 6805 288a 0800  ).NNK.t.R.h.(...
-000034e0: b050 9edc 784e 174e 4e4b 0a74 9452 9468  .P..xN.NNK.t.R.h
-000034f0: 0528 8a08 00b0 d5c5 f848 5c16 4e4e 4b0a  .(.......H\.NNK.
-00003500: 7494 5294 6805 288a 0800 b048 1f5b ccc6  t.R.h.(....H.[..
-00003510: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003520: 5c71 9b03 ad17 4e4e 4b0a 7494 5294 6805  \q....NNK.t.R.h.
-00003530: 288a 0800 b0e2 dafa 48dc 174e 4e4b 0a74  (.......H..NNK.t
-00003540: 9452 9468 0528 8a08 00b0 99cf 37a3 a916  .R.h.(......7...
-00003550: 4e4e 4b0a 7494 5294 6805 288a 0800 b01e  NNK.t.R.h.(.....
-00003560: d1bb ee8e 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00003570: 8a08 00b0 27a5 cc52 4c17 4e4e 4b0a 7494  ....'..RL.NNK.t.
-00003580: 5294 6805 288a 0800 b02b 5be7 0786 174e  R.h.(....+[....N
-00003590: 4e4b 0a74 9452 9468 0528 8a08 00b0 f5d7  NK.t.R.h.(......
-000035a0: abc8 8c17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-000035b0: 0800 b0f3 2d8d 5921 174e 4e4b 0a74 9452  ....-.Y!.NNK.t.R
-000035c0: 9468 0528 8a08 00b0 4ef4 bd09 e316 4e4e  .h.(....N.....NN
-000035d0: 4b0a 7494 5294 6805 288a 0800 b013 538c  K.t.R.h.(.....S.
-000035e0: 1b66 174e 4e4b 0a74 9452 9468 0528 8a08  .f.NNK.t.R.h.(..
-000035f0: 00b0 cb9c 582d 6916 4e4e 4b0a 7494 5294  ....X-i.NNK.t.R.
-00003600: 6805 288a 0800 b0eb c157 efad 164e 4e4b  h.(......W...NNK
-00003610: 0a74 9452 9468 0528 8a08 00b0 cd33 2b5a  .t.R.h.(.....3+Z
-00003620: c017 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003630: b066 9a3b 1fa0 174e 4e4b 0a74 9452 9468  .f.;...NNK.t.R.h
-00003640: 0528 8a08 00b0 a0e6 dd55 e716 4e4e 4b0a  .(.......U..NNK.
-00003650: 7494 5294 6805 288a 0800 b0d3 088e 97dc  t.R.h.(.........
-00003660: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003670: 5106 b872 9816 4e4e 4b0a 7494 5294 6805  Q..r..NNK.t.R.h.
-00003680: 288a 0800 b047 dd17 57a5 164e 4e4b 0a74  (....G..W..NNK.t
-00003690: 9452 9468 0528 8a08 00b0 ca34 7d33 1f17  .R.h.(.....4}3..
-000036a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b009  NNK.t.R.h.(.....
-000036b0: 2aec ff72 174e 4e4b 0a74 9452 9468 0528  *..r.NNK.t.R.h.(
-000036c0: 8a08 00b0 fc01 9ebd de16 4e4e 4b0a 7494  ..........NNK.t.
-000036d0: 5294 6805 288a 0800 b0b8 8c5b 6ba4 174e  R.h.(......[k..N
-000036e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 5248  NK.t.R.h.(....RH
-000036f0: fbe7 b917 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00003700: 0800 b06f 6e4c 835d 174e 4e4b 0a74 9452  ...onL.].NNK.t.R
-00003710: 9468 0528 8a08 00b0 6246 fe40 c916 4e4e  .h.(....bF.@..NN
-00003720: 4b0a 7494 5294 6805 288a 0800 b02f 244e  K.t.R.h.(..../$N
-00003730: ffd3 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003740: 00b0 ebae 0bad 9917 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00003750: 6805 288a 0800 b0b4 381e 8dcd 164e 4e4b  h.(.....8....NNK
-00003760: 0a74 9452 9468 0528 8a08 00b0 83c0 8cba  .t.R.h.(........
-00003770: 4317 4e4e 4b0a 7494 5294 6805 288a 0800  C.NNK.t.R.h.(...
+000033d0: ae76 0792 c516 4e4e 4b0a 7494 5294 6805  .v....NNK.t.R.h.
+000033e0: 288a 0800 b039 4dee 1ac7 164e 4e4b 0a74  (....9M....NNK.t
+000033f0: 9452 9468 0528 8a08 00b0 6246 fe40 c916  .R.h.(....bF.@..
+00003400: 4e4e 4b0a 7494 5294 6805 288a 0800 b08b  NNK.t.R.h.(.....
+00003410: 3f0e 67cb 164e 4e4b 0a74 9452 9468 0528  ?.g..NNK.t.R.h.(
+00003420: 8a08 00b0 b438 1e8d cd16 4e4e 4b0a 7494  .....8....NNK.t.
+00003430: 5294 6805 288a 0800 b0dd 312e b3cf 164e  R.h.(.....1....N
+00003440: 4e4b 0a74 9452 9468 0528 8a08 00b0 062b  NK.t.R.h.(.....+
+00003450: 3ed9 d116 4e4e 4b0a 7494 5294 6805 288a  >...NNK.t.R.h.(.
+00003460: 0800 b02f 244e ffd3 164e 4e4b 0a74 9452  .../$N...NNK.t.R
+00003470: 9468 0528 8a08 00b0 581d 5e25 d616 4e4e  .h.(....X.^%..NN
+00003480: 4b0a 7494 5294 6805 288a 0800 b032 85d9  K.t.R.h.(....2..
+00003490: fcd7 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000034a0: 00b0 aa0f 7e71 da16 4e4e 4b0a 7494 5294  ....~q..NNK.t.R.
+000034b0: 6805 288a 0800 b0d3 088e 97dc 164e 4e4b  h.(..........NNK
+000034c0: 0a74 9452 9468 0528 8a08 00b0 fc01 9ebd  .t.R.h.(........
+000034d0: de16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000034e0: b025 fbad e3e0 164e 4e4b 0a74 9452 9468  .%.....NNK.t.R.h
+000034f0: 0528 8a08 00b0 4ef4 bd09 e316 4e4e 4b0a  .(....N.....NNK.
+00003500: 7494 5294 6805 288a 0800 b077 edcd 2fe5  t.R.h.(....w../.
+00003510: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003520: a0e6 dd55 e716 4e4e 4b0a 7494 5294 6805  ...U..NNK.t.R.h.
+00003530: 288a 0800 b0c9 dfed 7be9 164e 4e4b 0a74  (.......{..NNK.t
+00003540: 9452 9468 0528 8a08 00b0 a347 6953 eb16  .R.h.(.....GiS..
+00003550: 4e4e 4b0a 7494 5294 6805 288a 0800 b01b  NNK.t.R.h.(.....
+00003560: d20d c8ed 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00003570: 8a08 00b0 44cb 1dee ef16 4e4e 4b0a 7494  ....D.....NNK.t.
+00003580: 5294 6805 288a 0800 b06d c42d 14f2 164e  R.h.(....m.-...N
+00003590: 4e4b 0a74 9452 9468 0528 8a08 00b0 96bd  NK.t.R.h.(......
+000035a0: 3d3a f416 4e4e 4b0a 7494 5294 6805 288a  =:..NNK.t.R.h.(.
+000035b0: 0800 b0bf b64d 60f6 164e 4e4b 0a74 9452  .....M`..NNK.t.R
+000035c0: 9468 0528 8a08 00b0 e8af 5d86 f816 4e4e  .h.(......]...NN
+000035d0: 4b0a 7494 5294 6805 288a 0800 b011 a96d  K.t.R.h.(......m
+000035e0: acfa 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000035f0: 00b0 3aa2 7dd2 fc16 4e4e 4b0a 7494 5294  ..:.}...NNK.t.R.
+00003600: 6805 288a 0800 b063 9b8d f8fe 164e 4e4b  h.(....c.....NNK
+00003610: 0a74 9452 9468 0528 8a08 00b0 8c94 9d1e  .t.R.h.(........
+00003620: 0117 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003630: b0b5 8dad 4403 174e 4e4b 0a74 9452 9468  ....D..NNK.t.R.h
+00003640: 0528 8a08 00b0 de86 bd6a 0517 4e4e 4b0a  .(.......j..NNK.
+00003650: 7494 5294 6805 288a 0800 b007 80cd 9007  t.R.h.(.........
+00003660: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003670: e1e7 4868 0917 4e4e 4b0a 7494 5294 6805  ..Hh..NNK.t.R.h.
+00003680: 288a 0800 b059 72ed dc0b 174e 4e4b 0a74  (....Yr....NNK.t
+00003690: 9452 9468 0528 8a08 00b0 826b fd02 0e17  .R.h.(.....k....
+000036a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0ab  NNK.t.R.h.(.....
+000036b0: 640d 2910 174e 4e4b 0a74 9452 9468 0528  d.)..NNK.t.R.h.(
+000036c0: 8a08 00b0 d45d 1d4f 1217 4e4e 4b0a 7494  .....].O..NNK.t.
+000036d0: 5294 6805 288a 0800 b0fd 562d 7514 174e  R.h.(.....V-u..N
+000036e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2650  NK.t.R.h.(....&P
+000036f0: 3d9b 1617 4e4e 4b0a 7494 5294 6805 288a  =...NNK.t.R.h.(.
+00003700: 0800 b04f 494d c118 174e 4e4b 0a74 9452  ...OIM...NNK.t.R
+00003710: 9468 0528 8a08 00b0 7842 5de7 1a17 4e4e  .h.(....xB]...NN
+00003720: 4b0a 7494 5294 6805 288a 0800 b0a1 3b6d  K.t.R.h.(.....;m
+00003730: 0d1d 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00003740: 00b0 ca34 7d33 1f17 4e4e 4b0a 7494 5294  ...4}3..NNK.t.R.
+00003750: 6805 288a 0800 b0f3 2d8d 5921 174e 4e4b  h.(.....-.Y!.NNK
+00003760: 0a74 9452 9468 0528 8a08 00b0 1c27 9d7f  .t.R.h.(.....'..
+00003770: 2317 4e4e 4b0a 7494 5294 6805 288a 0800  #.NNK.t.R.h.(...
 00003780: b0f6 8e18 5725 174e 4e4b 0a74 9452 9468  ....W%.NNK.t.R.h
-00003790: 0528 8a08 00b0 1054 def4 c416 4e4e 4b0a  .(.....T....NNK.
-000037a0: 7494 5294 6805 288a 0800 b000 56db 9bb5  t.R.h.(.....V...
+00003790: 0528 8a08 00b0 6e19 bdcb 2717 4e4e 4b0a  .(....n...'.NNK.
+000037a0: 7494 5294 6805 288a 0800 b097 12cd f129  t.R.h.(........)
 000037b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000037c0: 28fa 5b0a 8217 4e4e 4b0a 7494 5294 6805  (.[...NNK.t.R.h.
-000037d0: 288a 0800 b0fe be08 6f5e 164e 4e4b 0a74  (.......o^.NNK.t
-000037e0: 9452 9468 0528 8a08 00b0 394d ee1a c716  .R.h.(....9M....
-000037f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a3  NNK.t.R.h.(.....
-00003800: e58b 7c88 174e 4e4b 0a74 9452 9468 0528  ..|..NNK.t.R.h.(
-00003810: 8a08 00b0 53ff 6776 5217 4e4e 4b0a 7494  ....S.gvR.NNK.t.
-00003820: 5294 6805 288a 0800 b0a4 3a1b 34be 174e  R.h.(.....:.4..N
-00003830: 4e4b 0a74 9452 9468 0528 8a08 00b0 171c  NK.t.R.h.(......
-00003840: f312 b416 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00003850: 0800 b054 6743 709c 164e 4e4b 0a74 9452  ...TgCp..NNK.t.R
-00003860: 9468 0528 8a08 00b0 70d6 277d a716 4e4e  .h.(....p.'}..NN
-00003870: 4b0a 7494 5294 6805 288a 0800 b051 f36b  K.t.R.h.(....Q.k
-00003880: 3084 174e 4e4b 0a74 9452 9468 0528 8a08  0..NNK.t.R.h.(..
-00003890: 00b0 8e51 08d0 8016 4e4e 4b0a 7494 5294  ...Q....NNK.t.R.
-000038a0: 6805 288a 0800 b0ae 7607 92c5 164e 4e4b  h.(.....v....NNK
-000038b0: 0a74 9452 9468 0528 8a08 00b0 9568 ae82  .t.R.h.(.....h..
-000038c0: be16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000038d0: b043 768e 36ba 164e 4e4b 0a74 9452 9468  .Cv.6..NNK.t.R.h
-000038e0: 0528 8a08 00b0 9a11 7b18 cb17 4e4e 4b0a  .(......{...NNK.
-000038f0: 7494 5294 6805 288a 0800 b0ab 640d 2910  t.R.h.(.....d.).
+000037c0: c00b dd17 2c17 4e4e 4b0a 7494 5294 6805  ....,.NNK.t.R.h.
+000037d0: 288a 0800 b0e9 04ed 3d2e 174e 4e4b 0a74  (.......=..NNK.t
+000037e0: 9452 9468 0528 8a08 00b0 12fe fc63 3017  .R.h.(.......c0.
+000037f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b03b  NNK.t.R.h.(....;
+00003800: f70c 8a32 174e 4e4b 0a74 9452 9468 0528  ...2.NNK.t.R.h.(
+00003810: 8a08 00b0 64f0 1cb0 3417 4e4e 4b0a 7494  ....d...4.NNK.t.
+00003820: 5294 6805 288a 0800 b08d e92c d636 174e  R.h.(......,.6.N
+00003830: 4e4b 0a74 9452 9468 0528 8a08 00b0 b6e2  NK.t.R.h.(......
+00003840: 3cfc 3817 4e4e 4b0a 7494 5294 6805 288a  <.8.NNK.t.R.h.(.
+00003850: 0800 b0df db4c 223b 174e 4e4b 0a74 9452  .....L";.NNK.t.R
+00003860: 9468 0528 8a08 00b0 08d5 5c48 3d17 4e4e  .h.(......\H=.NN
+00003870: 4b0a 7494 5294 6805 288a 0800 b031 ce6c  K.t.R.h.(....1.l
+00003880: 6e3f 174e 4e4b 0a74 9452 9468 0528 8a08  n?.NNK.t.R.h.(..
+00003890: 00b0 5ac7 7c94 4117 4e4e 4b0a 7494 5294  ..Z.|.A.NNK.t.R.
+000038a0: 6805 288a 0800 b083 c08c ba43 174e 4e4b  h.(........C.NNK
+000038b0: 0a74 9452 9468 0528 8a08 00b0 acb9 9ce0  .t.R.h.(........
+000038c0: 4517 4e4e 4b0a 7494 5294 6805 288a 0800  E.NNK.t.R.h.(...
+000038d0: b0d5 b2ac 0648 174e 4e4b 0a74 9452 9468  .....H.NNK.t.R.h
+000038e0: 0528 8a08 00b0 af1a 28de 4917 4e4e 4b0a  .(......(.I.NNK.
+000038f0: 7494 5294 6805 288a 0800 b027 a5cc 524c  t.R.h.(....'..RL
 00003900: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003910: 16c7 635b 7e16 4e4e 4b0a 7494 5294 6805  ..c[~.NNK.t.R.h.
-00003920: 288a 0800 b0e0 4328 1c85 164e 4e4b 0a74  (.....C(...NNK.t
-00003930: 9452 9468 0528 8a08 00b0 5b2f 588e 8b16  .R.h.(....[/X...
-00003940: 4e4e 4b0a 7494 5294 6805 288a 0800 b085  NNK.t.R.h.(.....
-00003950: 6aab 29af 174e 4e4b 0a74 9452 9468 0528  j.)..NNK.t.R.h.(
-00003960: 8a08 00b0 4675 3c5d 5b17 4e4e 4b0a 7494  ....Fu<][.NNK.t.
-00003970: 5294 6805 288a 0800 b076 983e 78af 164e  R.h.(....v.>x..N
-00003980: 4e4b 0a74 9452 9468 0528 8a08 00b0 bfb6  NK.t.R.h.(......
-00003990: 4d60 f616 4e4e 4b0a 7494 5294 6805 288a  M`..NNK.t.R.h.(.
-000039a0: 0800 b0f6 2c3b 80c2 174e 4e4b 0a74 9452  ....,;...NNK.t.R
-000039b0: 9468 0528 8a08 00b0 1f26 4ba6 c417 4e4e  .h.(.....&K...NN
-000039c0: 4b0a 7494 5294 6805 288a 0800 b0a1 3b6d  K.t.R.h.(.....;m
-000039d0: 0d1d 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000039e0: 00b0 3bf7 0c8a 3217 4e4e 4b0a 7494 5294  ..;...2.NNK.t.R.
-000039f0: 6805 288a 0800 b046 8888 9f6f 164e 4e4b  h.(....F...o.NNK
-00003a00: 0a74 9452 9468 0528 8a08 00b0 25fb ade3  .t.R.h.(....%...
-00003a10: e016 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003a20: b00a 7f7b b7a8 174e 4e4b 0a74 9452 9468  ...{...NNK.t.R.h
-00003a30: 0528 8a08 00b0 6545 ac67 6a17 4e4e 4b0a  .(....eE.gj.NNK.
-00003a40: 7494 5294 6805 288a 0800 b079 97ec 9e50  t.R.h.(....y...P
+00003910: 509e dc78 4e17 4e4e 4b0a 7494 5294 6805  P..xN.NNK.t.R.h.
+00003920: 288a 0800 b079 97ec 9e50 174e 4e4b 0a74  (....y...P.NNK.t
+00003930: 9452 9468 0528 8a08 00b0 53ff 6776 5217  .R.h.(....S.gvR.
+00003940: 4e4e 4b0a 7494 5294 6805 288a 0800 b0cb  NNK.t.R.h.(.....
+00003950: 890c eb54 174e 4e4b 0a74 9452 9468 0528  ...T.NNK.t.R.h.(
+00003960: 8a08 00b0 f482 1c11 5717 4e4e 4b0a 7494  ........W.NNK.t.
+00003970: 5294 6805 288a 0800 b01d 7c2c 3759 174e  R.h.(.....|,7Y.N
+00003980: 4e4b 0a74 9452 9468 0528 8a08 00b0 4675  NK.t.R.h.(....Fu
+00003990: 3c5d 5b17 4e4e 4b0a 7494 5294 6805 288a  <][.NNK.t.R.h.(.
+000039a0: 0800 b06f 6e4c 835d 174e 4e4b 0a74 9452  ...onL.].NNK.t.R
+000039b0: 9468 0528 8a08 00b0 9867 5ca9 5f17 4e4e  .h.(.....g\._.NN
+000039c0: 4b0a 7494 5294 6805 288a 0800 b0c1 606c  K.t.R.h.(.....`l
+000039d0: cf61 174e 4e4b 0a74 9452 9468 0528 8a08  .a.NNK.t.R.h.(..
+000039e0: 00b0 ea59 7cf5 6317 4e4e 4b0a 7494 5294  ...Y|.c.NNK.t.R.
+000039f0: 6805 288a 0800 b013 538c 1b66 174e 4e4b  h.(.....S..f.NNK
+00003a00: 0a74 9452 9468 0528 8a08 00b0 3c4c 9c41  .t.R.h.(....<L.A
+00003a10: 6817 4e4e 4b0a 7494 5294 6805 288a 0800  h.NNK.t.R.h.(...
+00003a20: b065 45ac 676a 174e 4e4b 0a74 9452 9468  .eE.gj.NNK.t.R.h
+00003a30: 0528 8a08 00b0 8e3e bc8d 6c17 4e4e 4b0a  .(.....>..l.NNK.
+00003a40: 7494 5294 6805 288a 0800 b0b7 37cc b36e  t.R.h.(.....7..n
 00003a50: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003a60: 3c5f e883 7c16 4e4e 4b0a 7494 5294 6805  <_..|.NNK.t.R.h.
-00003a70: 288a 0800 b058 1d5e 25d6 164e 4e4b 0a74  (....X.^%..NNK.t
-00003a80: 9452 9468 0528 8a08 00b0 af1a 28de 4917  .R.h.(......(.I.
-00003a90: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e8  NNK.t.R.h.(.....
-00003aa0: af5d 86f8 164e 4e4b 0a74 9452 9468 0528  .]...NNK.t.R.h.(
-00003ab0: 8a08 00b0 08d5 5c48 3d17 4e4e 4b0a 7494  ......\H=.NNK.t.
-00003ac0: 5294 6805 288a 0800 b0ad 2178 da8f 164e  R.h.(.....!x...N
-00003ad0: 4e4b 0a74 9452 9468 0528 8a08 00b0 1ee4  NK.t.R.h.(......
-00003ae0: 0731 a316 4e4e 4b0a 7494 5294 6805 288a  .1..NNK.t.R.h.(.
-00003af0: 0800 b08f a697 87b6 164e 4e4b 0a74 9452  .........NNK.t.R
-00003b00: 9468 0528 8a08 00b0 9867 5ca9 5f17 4e4e  .h.(.....g\._.NN
-00003b10: 4b0a 7494 5294 6805 288a 0800 b0cc de9b  K.t.R.h.(.......
-00003b20: a28a 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003b30: 00b0 7aff c798 9a16 4e4e 4b0a 7494 5294  ..z.....NNK.t.R.
-00003b40: 6805 288a 0800 b033 788b ddaa 174e 4e4b  h.(....3x....NNK
-00003b50: 0a74 9452 9468 0528 8a08 00b0 3285 d9fc  .t.R.h.(....2...
-00003b60: d716 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003b70: b06c 6f9e 5cbc 164e 4e4b 0a74 9452 9468  .lo.\..NNK.t.R.h
-00003b80: 0528 8a08 00b0 dfdb 4c22 3b17 4e4e 4b0a  .(......L";.NNK.
-00003b90: 7494 5294 6805 288a 0800 b0ea 597c f563  t.R.h.(.....Y|.c
+00003a60: e030 dcd9 7017 4e4e 4b0a 7494 5294 6805  .0..p.NNK.t.R.h.
+00003a70: 288a 0800 b009 2aec ff72 174e 4e4b 0a74  (.....*..r.NNK.t
+00003a80: 9452 9468 0528 8a08 00b0 3223 fc25 7517  .R.h.(....2#.%u.
+00003a90: 4e4e 4b0a 7494 5294 6805 288a 0800 b05b  NNK.t.R.h.(....[
+00003aa0: 1c0c 4c77 174e 4e4b 0a74 9452 9468 0528  ..Lw.NNK.t.R.h.(
+00003ab0: 8a08 00b0 8415 1c72 7917 4e4e 4b0a 7494  .......ry.NNK.t.
+00003ac0: 5294 6805 288a 0800 b05e 7d97 497b 174e  R.h.(....^}.I{.N
+00003ad0: 4e4b 0a74 9452 9468 0528 8a08 00b0 d607  NK.t.R.h.(......
+00003ae0: 3cbe 7d17 4e4e 4b0a 7494 5294 6805 288a  <.}.NNK.t.R.h.(.
+00003af0: 0800 b0ff 004c e47f 174e 4e4b 0a74 9452  .....L...NNK.t.R
+00003b00: 9468 0528 8a08 00b0 28fa 5b0a 8217 4e4e  .h.(....(.[...NN
+00003b10: 4b0a 7494 5294 6805 288a 0800 b051 f36b  K.t.R.h.(....Q.k
+00003b20: 3084 174e 4e4b 0a74 9452 9468 0528 8a08  0..NNK.t.R.h.(..
+00003b30: 00b0 2b5b e707 8617 4e4e 4b0a 7494 5294  ..+[....NNK.t.R.
+00003b40: 6805 288a 0800 b0a3 e58b 7c88 174e 4e4b  h.(.......|..NNK
+00003b50: 0a74 9452 9468 0528 8a08 00b0 ccde 9ba2  .t.R.h.(........
+00003b60: 8a17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003b70: b0f5 d7ab c88c 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00003b80: 0528 8a08 00b0 1ed1 bbee 8e17 4e4e 4b0a  .(..........NNK.
+00003b90: 7494 5294 6805 288a 0800 b0f8 3837 c690  t.R.h.(.....87..
 00003ba0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003bb0: 11a9 6dac fa16 4e4e 4b0a 7494 5294 6805  ..m...NNK.t.R.h.
-00003bc0: 288a 0800 b0b8 9fa7 adb8 164e 4e4b 0a74  (..........NNK.t
-00003bd0: 9452 9468 0528 8a08 00b0 8428 68b4 8d16  .R.h.(.....(h...
-00003be0: 4e4e 4b0a 7494 5294 6805 288a 0800 b06e  NNK.t.R.h.(....n
-00003bf0: 19bd cb27 174e 4e4b 0a74 9452 9468 0528  ...'.NNK.t.R.h.(
-00003c00: 8a08 00b0 d45d 1d4f 1217 4e4e 4b0a 7494  .....].O..NNK.t.
-00003c10: 5294 6805 288a 0800 b032 23fc 2575 174e  R.h.(....2#.%u.N
-00003c20: 4e4b 0a74 9452 9468 0528 8a08 00b0 f183  NK.t.R.h.(......
-00003c30: 6eea b516 4e4e 4b0a 7494 5294 6805 288a  n...NNK.t.R.h.(.
-00003c40: 0800 b079 aa38 e164 164e 4e4b 0a74 9452  ...y.8.d.NNK.t.R
-00003c50: 9468 0528 8a08 00b0 6f81 98c5 7116 4e4e  .h.(....o...q.NN
-00003c60: 4b0a 7494 5294 6805 288a 0800 b014 a81b  K.t.R.h.(.......
-00003c70: d39b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003c80: 00b0 be61 bea8 c016 4e4e 4b0a 7494 5294  ...a....NNK.t.R.
-00003c90: 6805 288a 0800 b08d e92c d636 174e 4e4b  h.(......,.6.NNK
-00003ca0: 0a74 9452 9468 0528 8a08 00b0 5972 eddc  .t.R.h.(....Yr..
-00003cb0: 0b17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003cc0: b0d6 1a88 0092 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00003cd0: 0528 8a08 00b0 77ed cd2f e516 4e4e 4b0a  .(....w../..NNK.
-00003ce0: 7494 5294 6805 288a 0800 b0c3 0a8b 3ecd  t.R.h.(.......>.
+00003bb0: 70c3 db3a 9317 4e4e 4b0a 7494 5294 6805  p..:..NNK.t.R.h.
+00003bc0: 288a 0800 b099 bceb 6095 174e 4e4b 0a74  (.......`..NNK.t
+00003bd0: 9452 9468 0528 8a08 00b0 7324 6738 9717  .R.h.(....s$g8..
+00003be0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0eb  NNK.t.R.h.(.....
+00003bf0: ae0b ad99 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00003c00: 8a08 00b0 14a8 1bd3 9b17 4e4e 4b0a 7494  ..........NNK.t.
+00003c10: 5294 6805 288a 0800 b03d a12b f99d 174e  R.h.(....=.+...N
+00003c20: 4e4b 0a74 9452 9468 0528 8a08 00b0 669a  NK.t.R.h.(....f.
+00003c30: 3b1f a017 4e4e 4b0a 7494 5294 6805 288a  ;...NNK.t.R.h.(.
+00003c40: 0800 b08f 934b 45a2 174e 4e4b 0a74 9452  .....KE..NNK.t.R
+00003c50: 9468 0528 8a08 00b0 b88c 5b6b a417 4e4e  .h.(......[k..NN
+00003c60: 4b0a 7494 5294 6805 288a 0800 b0e1 856b  K.t.R.h.(......k
+00003c70: 91a6 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00003c80: 00b0 0a7f 7bb7 a817 4e4e 4b0a 7494 5294  ....{...NNK.t.R.
+00003c90: 6805 288a 0800 b033 788b ddaa 174e 4e4b  h.(....3x....NNK
+00003ca0: 0a74 9452 9468 0528 8a08 00b0 5c71 9b03  .t.R.h.(....\q..
+00003cb0: ad17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003cc0: b085 6aab 29af 174e 4e4b 0a74 9452 9468  ..j.)..NNK.t.R.h
+00003cd0: 0528 8a08 00b0 ae63 bb4f b117 4e4e 4b0a  .(.....c.O..NNK.
+00003ce0: 7494 5294 6805 288a 0800 b0d7 5ccb 75b3  t.R.h.(.....\.u.
 00003cf0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003d00: acb9 9ce0 4517 4e4e 4b0a 7494 5294 6805  ....E.NNK.t.R.h.
-00003d10: 288a 0800 b0fd 562d 7514 174e 4e4b 0a74  (.....V-u..NNK.t
-00003d20: 9452 9468 0528 8a08 00b0 c00b dd17 2c17  .R.h.(........,.
-00003d30: 4e4e 4b0a 7494 5294 6805 288a 0800 b01d  NNK.t.R.h.(.....
-00003d40: 8f78 796d 164e 4e4b 0a74 9452 9468 0528  .xym.NNK.t.R.h.(
-00003d50: 8a08 00b0 d5b2 ac06 4817 4e4e 4b0a 7494  ........H.NNK.t.
-00003d60: 5294 6805 288a 0800 b0e0 30dc d970 174e  R.h.(.....0..p.N
-00003d70: 4e4b 0a74 9452 9468 0528 8a08 00b0 c9df  NK.t.R.h.(......
-00003d80: ed7b e916 4e4e 4b0a 7494 5294 6805 288a  .{..NNK.t.R.h.(.
-00003d90: 0800 b028 0da8 4c96 164e 4e4b 0a74 9452  ...(..L..NNK.t.R
-00003da0: 9468 0528 8a08 00b0 3db4 773b b216 4e4e  .h.(....=.w;..NN
-00003db0: 4b0a 7494 5294 6805 288a 0800 b0d6 073c  K.t.R.h.(......<
-00003dc0: be7d 174e 4e4b 0a74 9452 9468 0528 8a08  .}.NNK.t.R.h.(..
-00003dd0: 00b0 6dc4 2d14 f216 4e4e 4b0a 7494 5294  ..m.-...NNK.t.R.
-00003de0: 6805 288a 0800 b0cb 890c eb54 174e 4e4b  h.(........T.NNK
-00003df0: 0a74 9452 9468 0528 8a08 00b0 f5ea f70a  .t.R.h.(........
-00003e00: a116 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003e10: b05e 7d97 497b 174e 4e4b 0a74 9452 9468  .^}.I{.NNK.t.R.h
-00003e20: 0528 8a08 00b0 b6e2 3cfc 3817 4e4e 4b0a  .(......<.8.NNK.
-00003e30: 7494 5294 6805 288a 0800 b03e f6ba b0d3  t.R.h.(....>....
-00003e40: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003e50: 7b41 0b0e bc17 4e4e 4b0a 7494 5294 6805  {A....NNK.t.R.h.
-00003e60: 288a 0800 b03d a12b f99d 174e 4e4b 0a74  (....=.+...NNK.t
-00003e70: 9452 9468 0528 8a08 00b0 70c3 db3a 9317  .R.h.(....p..:..
-00003e80: 4e4e 4b0a 7494 5294 6805 288a 0800 b029  NNK.t.R.h.(....)
-00003e90: 4feb c1b7 174e 4e4b 0a74 9452 9465 8c0a  O....NNK.t.R.e..
-00003ea0: 4d49 4443 504e 4946 5459 945d 9428 6805  MIDCPNIFTY.].(h.
-00003eb0: 288a 0800 b01b d20d c8ed 164e 4e4b 0a74  (..........NNK.t
-00003ec0: 9452 9468 0528 8a08 00b0 8e3e bc8d 6c17  .R.h.(.....>..l.
-00003ed0: 4e4e 4b0a 7494 5294 6805 288a 0800 b012  NNK.t.R.h.(.....
-00003ee0: fefc 6330 174e 4e4b 0a74 9452 9468 0528  ..c0.NNK.t.R.h.(
-00003ef0: 8a08 00b0 639b 8df8 fe16 4e4e 4b0a 7494  ....c.....NNK.t.
-00003f00: 5294 6805 288a 0800 b0dd 312e b3cf 164e  R.h.(.....1....N
-00003f10: 4e4b 0a74 9452 9468 0528 8a08 00b0 f482  NK.t.R.h.(......
-00003f20: 1c11 5717 4e4e 4b0a 7494 5294 6805 288a  ..W.NNK.t.R.h.(.
-00003f30: 0800 b078 425d e71a 174e 4e4b 0a74 9452  ...xB]...NNK.t.R
-00003f40: 9468 0528 8a08 00b0 aaad a09a 7717 4e4e  .h.(........w.NN
-00003f50: 4b0a 7494 5294 6805 288a 0800 b08c 949d  K.t.R.h.(.......
-00003f60: 1e01 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003f70: 00b0 b58d ad44 0317 4e4e 4b0a 7494 5294  .....D..NNK.t.R.
-00003f80: 6805 288a 0800 b0aa 0f7e 71da 164e 4e4b  h.(......~q..NNK
-00003f90: 0a74 9452 9468 0528 8a08 00b0 a347 6953  .t.R.h.(.....GiS
-00003fa0: eb16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003fb0: b073 2467 3897 174e 4e4b 0a74 9452 9468  .s$g8..NNK.t.R.h
-00003fc0: 0528 8a08 00b0 31ce 6c6e 3f17 4e4e 4b0a  .(....1.ln?.NNK.
-00003fd0: 7494 5294 6805 288a 0800 b04f 494d c118  t.R.h.(....OIM..
-00003fe0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003ff0: de86 bd6a 0517 4e4e 4b0a 7494 5294 6805  ...j..NNK.t.R.h.
-00004000: 288a 0800 b07c 4709 31a3 174e 4e4b 0a74  (....|G.1..NNK.t
-00004010: 9452 9468 0528 8a08 00b0 f276 20cb 8817  .R.h.(.....v ...
-00004020: 4e4e 4b0a 7494 5294 6805 288a 0800 b0bb  NNK.t.R.h.(.....
-00004030: ede6 68a8 174e 4e4b 0a74 9452 9468 0528  ..h..NNK.t.R.h.(
-00004040: 8a08 00b0 5fd2 2601 b117 4e4e 4b0a 7494  ...._.&...NNK.t.
-00004050: 5294 6805 288a 0800 b091 eed8 1fbf 174e  R.h.(..........N
-00004060: 4e4b 0a74 9452 9468 0528 8a08 00b0 826b  NK.t.R.h.(.....k
-00004070: fd02 0e17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00004080: 0800 b044 cb1d eeef 164e 4e4b 0a74 9452  ...D.....NNK.t.R
-00004090: 9468 0528 8a08 00b0 62e4 206a 6617 4e4e  .h.(....b. jf.NN
-000040a0: 4b0a 7494 5294 6805 288a 0800 b006 2b3e  K.t.R.h.(.....+>
-000040b0: d9d1 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000040c0: 00b0 a79b a631 c217 4e4e 4b0a 7494 5294  .....1..NNK.t.R.
-000040d0: 6805 288a 0800 b002 62d7 e183 174e 4e4b  h.(.....b....NNK
-000040e0: 0a74 9452 9468 0528 8a08 00b0 2fc2 7028  .t.R.h.(..../.p(
-000040f0: 7117 4e4e 4b0a 7494 5294 6805 288a 0800  q.NNK.t.R.h.(...
-00004100: b021 3247 ec92 174e 4e4b 0a74 9452 9468  .!2G...NNK.t.R.h
-00004110: 0528 8a08 00b0 5ac7 7c94 4117 4e4e 4b0a  .(....Z.|.A.NNK.
-00004120: 7494 5294 6805 288a 0800 b040 02b7 f6a1  t.R.h.(....@....
+00003d00: 0056 db9b b517 4e4e 4b0a 7494 5294 6805  .V....NNK.t.R.h.
+00003d10: 288a 0800 b029 4feb c1b7 174e 4e4b 0a74  (....)O....NNK.t
+00003d20: 9452 9468 0528 8a08 00b0 5248 fbe7 b917  .R.h.(....RH....
+00003d30: 4e4e 4b0a 7494 5294 6805 288a 0800 b07b  NNK.t.R.h.(....{
+00003d40: 410b 0ebc 174e 4e4b 0a74 9452 9468 0528  A....NNK.t.R.h.(
+00003d50: 8a08 00b0 a43a 1b34 be17 4e4e 4b0a 7494  .....:.4..NNK.t.
+00003d60: 5294 6805 288a 0800 b0cd 332b 5ac0 174e  R.h.(.....3+Z..N
+00003d70: 4e4b 0a74 9452 9468 0528 8a08 00b0 f62c  NK.t.R.h.(.....,
+00003d80: 3b80 c217 4e4e 4b0a 7494 5294 6805 288a  ;...NNK.t.R.h.(.
+00003d90: 0800 b01f 264b a6c4 174e 4e4b 0a74 9452  ....&K...NNK.t.R
+00003da0: 9468 0528 8a08 00b0 481f 5bcc c617 4e4e  .h.(....H.[...NN
+00003db0: 4b0a 7494 5294 6805 288a 0800 b071 186b  K.t.R.h.(....q.k
+00003dc0: f2c8 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00003dd0: 00b0 9a11 7b18 cb17 4e4e 4b0a 7494 5294  ....{...NNK.t.R.
+00003de0: 6805 288a 0800 b0c3 0a8b 3ecd 174e 4e4b  h.(.......>..NNK
+00003df0: 0a74 9452 9468 0528 8a08 00b0 ec03 9b64  .t.R.h.(.......d
+00003e00: cf17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003e10: b03e f6ba b0d3 174e 4e4b 0a74 9452 9468  .>.....NNK.t.R.h
+00003e20: 0528 8a08 00b0 e2da fa48 dc17 4e4e 4b0a  .(.......H..NNK.
+00003e30: 7494 5294 658c 0a4d 4944 4350 4e49 4654  t.R.e..MIDCPNIFT
+00003e40: 5994 5d94 2868 0528 8a08 00b0 b438 1e8d  Y.].(h.(.....8..
+00003e50: cd16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003e60: b0dd 312e b3cf 164e 4e4b 0a74 9452 9468  ..1....NNK.t.R.h
+00003e70: 0528 8a08 00b0 062b 3ed9 d116 4e4e 4b0a  .(.....+>...NNK.
+00003e80: 7494 5294 6805 288a 0800 b02f 244e ffd3  t.R.h.(..../$N..
+00003e90: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003ea0: 581d 5e25 d616 4e4e 4b0a 7494 5294 6805  X.^%..NNK.t.R.h.
+00003eb0: 288a 0800 b032 85d9 fcd7 164e 4e4b 0a74  (....2.....NNK.t
+00003ec0: 9452 9468 0528 8a08 00b0 aa0f 7e71 da16  .R.h.(......~q..
+00003ed0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d3  NNK.t.R.h.(.....
+00003ee0: 088e 97dc 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00003ef0: 8a08 00b0 fc01 9ebd de16 4e4e 4b0a 7494  ..........NNK.t.
+00003f00: 5294 6805 288a 0800 b025 fbad e3e0 164e  R.h.(....%.....N
+00003f10: 4e4b 0a74 9452 9468 0528 8a08 00b0 4ef4  NK.t.R.h.(....N.
+00003f20: bd09 e316 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00003f30: 0800 b077 edcd 2fe5 164e 4e4b 0a74 9452  ...w../..NNK.t.R
+00003f40: 9468 0528 8a08 00b0 a0e6 dd55 e716 4e4e  .h.(.......U..NN
+00003f50: 4b0a 7494 5294 6805 288a 0800 b0c9 dfed  K.t.R.h.(.......
+00003f60: 7be9 164e 4e4b 0a74 9452 9468 0528 8a08  {..NNK.t.R.h.(..
+00003f70: 00b0 a347 6953 eb16 4e4e 4b0a 7494 5294  ...GiS..NNK.t.R.
+00003f80: 6805 288a 0800 b01b d20d c8ed 164e 4e4b  h.(..........NNK
+00003f90: 0a74 9452 9468 0528 8a08 00b0 44cb 1dee  .t.R.h.(....D...
+00003fa0: ef16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003fb0: b06d c42d 14f2 164e 4e4b 0a74 9452 9468  .m.-...NNK.t.R.h
+00003fc0: 0528 8a08 00b0 96bd 3d3a f416 4e4e 4b0a  .(......=:..NNK.
+00003fd0: 7494 5294 6805 288a 0800 b0bf b64d 60f6  t.R.h.(......M`.
+00003fe0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003ff0: e8af 5d86 f816 4e4e 4b0a 7494 5294 6805  ..]...NNK.t.R.h.
+00004000: 288a 0800 b011 a96d acfa 164e 4e4b 0a74  (......m...NNK.t
+00004010: 9452 9468 0528 8a08 00b0 3aa2 7dd2 fc16  .R.h.(....:.}...
+00004020: 4e4e 4b0a 7494 5294 6805 288a 0800 b063  NNK.t.R.h.(....c
+00004030: 9b8d f8fe 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00004040: 8a08 00b0 8c94 9d1e 0117 4e4e 4b0a 7494  ..........NNK.t.
+00004050: 5294 6805 288a 0800 b0b5 8dad 4403 174e  R.h.(.......D..N
+00004060: 4e4b 0a74 9452 9468 0528 8a08 00b0 de86  NK.t.R.h.(......
+00004070: bd6a 0517 4e4e 4b0a 7494 5294 6805 288a  .j..NNK.t.R.h.(.
+00004080: 0800 b007 80cd 9007 174e 4e4b 0a74 9452  .........NNK.t.R
+00004090: 9468 0528 8a08 00b0 e1e7 4868 0917 4e4e  .h.(......Hh..NN
+000040a0: 4b0a 7494 5294 6805 288a 0800 b059 72ed  K.t.R.h.(....Yr.
+000040b0: dc0b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000040c0: 00b0 826b fd02 0e17 4e4e 4b0a 7494 5294  ...k....NNK.t.R.
+000040d0: 6805 288a 0800 b0ab 640d 2910 174e 4e4b  h.(.....d.)..NNK
+000040e0: 0a74 9452 9468 0528 8a08 00b0 d45d 1d4f  .t.R.h.(.....].O
+000040f0: 1217 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004100: b0fd 562d 7514 174e 4e4b 0a74 9452 9468  ..V-u..NNK.t.R.h
+00004110: 0528 8a08 00b0 2650 3d9b 1617 4e4e 4b0a  .(....&P=...NNK.
+00004120: 7494 5294 6805 288a 0800 b04f 494d c118  t.R.h.(....OIM..
 00004130: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004140: f838 37c6 9017 4e4e 4b0a 7494 5294 6805  .87...NNK.t.R.h.
-00004150: 288a 0800 b0e9 04ed 3d2e 174e 4e4b 0a74  (.......=..NNK.t
-00004160: 9452 9468 0528 8a08 00b0 81b4 9074 7517  .R.h.(.......tu.
-00004170: 4e4e 4b0a 7494 5294 6805 288a 0800 b007  NNK.t.R.h.(.....
-00004180: 80cd 9007 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00004190: 8a08 00b0 39eb 1044 6417 4e4e 4b0a 7494  ....9..Dd.NNK.t.
-000041a0: 5294 6805 288a 0800 b064 f01c b034 174e  R.h.(....d...4.N
-000041b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 96bd  NK.t.R.h.(......
-000041c0: 3d3a f416 4e4e 4b0a 7494 5294 6805 288a  =:..NNK.t.R.h.(.
-000041d0: 0800 b01d 7c2c 3759 174e 4e4b 0a74 9452  ....|,7Y.NNK.t.R
-000041e0: 9468 0528 8a08 00b0 e1e7 4868 0917 4e4e  .h.(......Hh..NN
-000041f0: 4b0a 7494 5294 6805 288a 0800 b026 503d  K.t.R.h.(....&P=
-00004200: 9b16 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00004210: 00b0 3aa2 7dd2 fc16 4e4e 4b0a 7494 5294  ..:.}...NNK.t.R.
-00004220: 6805 288a 0800 b01c 279d 7f23 174e 4e4b  h.(.....'..#.NNK
-00004230: 0a74 9452 9468 0528 8a08 00b0 e4e6 f68e  .t.R.h.(........
-00004240: aa17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00004250: b010 f200 1e62 174e 4e4b 0a74 9452 9468  .....b.NNK.t.R.h
-00004260: 0528 8a08 00b0 9712 cdf1 2917 4e4e 4b0a  .(........).NNK.
-00004270: 7494 5294 6805 288a 0800 b050 9edc 784e  t.R.h.(....P..xN
+00004140: 7842 5de7 1a17 4e4e 4b0a 7494 5294 6805  xB]...NNK.t.R.h.
+00004150: 288a 0800 b0a1 3b6d 0d1d 174e 4e4b 0a74  (.....;m...NNK.t
+00004160: 9452 9468 0528 8a08 00b0 ca34 7d33 1f17  .R.h.(.....4}3..
+00004170: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f3  NNK.t.R.h.(.....
+00004180: 2d8d 5921 174e 4e4b 0a74 9452 9468 0528  -.Y!.NNK.t.R.h.(
+00004190: 8a08 00b0 1c27 9d7f 2317 4e4e 4b0a 7494  .....'..#.NNK.t.
+000041a0: 5294 6805 288a 0800 b0f6 8e18 5725 174e  R.h.(.......W%.N
+000041b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 6e19  NK.t.R.h.(....n.
+000041c0: bdcb 2717 4e4e 4b0a 7494 5294 6805 288a  ..'.NNK.t.R.h.(.
+000041d0: 0800 b097 12cd f129 174e 4e4b 0a74 9452  .......).NNK.t.R
+000041e0: 9468 0528 8a08 00b0 c00b dd17 2c17 4e4e  .h.(........,.NN
+000041f0: 4b0a 7494 5294 6805 288a 0800 b0e9 04ed  K.t.R.h.(.......
+00004200: 3d2e 174e 4e4b 0a74 9452 9468 0528 8a08  =..NNK.t.R.h.(..
+00004210: 00b0 12fe fc63 3017 4e4e 4b0a 7494 5294  .....c0.NNK.t.R.
+00004220: 6805 288a 0800 b03b f70c 8a32 174e 4e4b  h.(....;...2.NNK
+00004230: 0a74 9452 9468 0528 8a08 00b0 64f0 1cb0  .t.R.h.(....d...
+00004240: 3417 4e4e 4b0a 7494 5294 6805 288a 0800  4.NNK.t.R.h.(...
+00004250: b08d e92c d636 174e 4e4b 0a74 9452 9468  ...,.6.NNK.t.R.h
+00004260: 0528 8a08 00b0 b6e2 3cfc 3817 4e4e 4b0a  .(......<.8.NNK.
+00004270: 7494 5294 6805 288a 0800 b0df db4c 223b  t.R.h.(......L";
 00004280: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004290: 27a5 cc52 4c17 4e4e 4b0a 7494 5294 6805  '..RL.NNK.t.R.h.
-000042a0: 288a 0800 b0ef 6426 62d3 174e 4e4b 0a74  (.....d&b..NNK.t
-000042b0: 9452 9468 0528 8a08 00b0 2b5b e707 8617  .R.h.(....+[....
-000042c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f3  NNK.t.R.h.(.....
-000042d0: 2d8d 5921 174e 4e4b 0a74 9452 9468 0528  -.Y!.NNK.t.R.h.(
-000042e0: 8a08 00b0 4ef4 bd09 e316 4e4e 4b0a 7494  ....N.....NNK.t.
-000042f0: 5294 6805 288a 0800 b04e 92e0 3280 174e  R.h.(....N..2..N
-00004300: 4e4b 0a74 9452 9468 0528 8a08 00b0 a0e6  NK.t.R.h.(......
-00004310: dd55 e716 4e4e 4b0a 7494 5294 6805 288a  .U..NNK.t.R.h.(.
-00004320: 0800 b0d3 088e 97dc 164e 4e4b 0a74 9452  .........NNK.t.R
-00004330: 9468 0528 8a08 00b0 ca34 7d33 1f17 4e4e  .h.(.....4}3..NN
-00004340: 4b0a 7494 5294 6805 288a 0800 b0fc 019e  K.t.R.h.(.......
-00004350: bdde 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00004360: 00b0 9c1d 775e 9917 4e4e 4b0a 7494 5294  ....w^..NNK.t.R.
-00004370: 6805 288a 0800 b0d0 94b6 57c4 174e 4e4b  h.(.......W..NNK
-00004380: 0a74 9452 9468 0528 8a08 00b0 7479 f6ef  .t.R.h.(....ty..
-00004390: cc17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000043a0: b095 06d1 ab5b 174e 4e4b 0a74 9452 9468  .....[.NNK.t.R.h
-000043b0: 0528 8a08 00b0 2f24 4eff d316 4e4e 4b0a  .(..../$N...NNK.
-000043c0: 7494 5294 6805 288a 0800 b0b4 381e 8dcd  t.R.h.(.....8...
-000043d0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000043e0: 83c0 8cba 4317 4e4e 4b0a 7494 5294 6805  ....C.NNK.t.R.h.
-000043f0: 288a 0800 b0f6 8e18 5725 174e 4e4b 0a74  (.......W%.NNK.t
-00004400: 9452 9468 0528 8a08 00b0 b4d6 40b6 6a17  .R.h.(......@.j.
-00004410: 4e4e 4b0a 7494 5294 6805 288a 0800 b017  NNK.t.R.h.(.....
-00004420: 09a7 d09f 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00004430: 8a08 00b0 4b80 e6c9 ca17 4e4e 4b0a 7494  ....K.....NNK.t.
-00004440: 5294 6805 288a 0800 b0a6 4617 7a8c 174e  R.h.(.....F.z..N
-00004450: 4e4b 0a74 9452 9468 0528 8a08 00b0 5454  NK.t.R.h.(....TT
-00004460: f72d 8817 4e4e 4b0a 7494 5294 6805 288a  .-..NNK.t.R.h.(.
-00004470: 0800 b053 ff67 7652 174e 4e4b 0a74 9452  ...S.gvR.NNK.t.R
-00004480: 9468 0528 8a08 00b0 e7f8 f0f7 5f17 4e4e  .h.(........_.NN
-00004490: 4b0a 7494 5294 6805 288a 0800 b02c b076  K.t.R.h.(....,.v
-000044a0: bfbb 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000044b0: 00b0 8bdd 3090 6817 4e4e 4b0a 7494 5294  ....0.h.NNK.t.R.
-000044c0: 6805 288a 0800 b0ab 640d 2910 174e 4e4b  h.(.....d.)..NNK
-000044d0: 0a74 9452 9468 0528 8a08 00b0 0de0 06b5  .t.R.h.(........
-000044e0: ac17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000044f0: b04a 2b57 1295 174e 4e4b 0a74 9452 9468  .J+W...NNK.t.R.h
-00004500: 0528 8a08 00b0 06c9 6002 6f17 4e4e 4b0a  .(......`.o.NNK.
-00004510: 7494 5294 6805 288a 0800 b0bf b64d 60f6  t.R.h.(......M`.
-00004520: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004530: 9349 66fa db17 4e4e 4b0a 7494 5294 6805  .If...NNK.t.R.h.
-00004540: 288a 0800 b0a1 3b6d 0d1d 174e 4e4b 0a74  (.....;m...NNK.t
-00004550: 9452 9468 0528 8a08 00b0 3bf7 0c8a 3217  .R.h.(....;...2.
-00004560: 4e4e 4b0a 7494 5294 6805 288a 0800 b025  NNK.t.R.h.(....%
-00004570: fbad e3e0 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00004580: 8a08 00b0 88cb 3627 b317 4e4e 4b0a 7494  ......6'..NNK.t.
-00004590: 5294 6805 288a 0800 b058 bb80 4e73 174e  R.h.(....X..Ns.N
-000045a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 fc9f  NK.t.R.h.(......
-000045b0: c0e6 7b17 4e4e 4b0a 7494 5294 6805 288a  ..{.NNK.t.R.h.(.
-000045c0: 0800 b0d9 68c7 bb81 174e 4e4b 0a74 9452  ....h....NNK.t.R
-000045d0: 9468 0528 8a08 00b0 7997 ec9e 5017 4e4e  .h.(....y...P.NN
-000045e0: 4b0a 7494 5294 6805 288a 0800 b058 1d5e  K.t.R.h.(....X.^
-000045f0: 25d6 164e 4e4b 0a74 9452 9468 0528 8a08  %..NNK.t.R.h.(..
-00004600: 00b0 af1a 28de 4917 4e4e 4b0a 7494 5294  ....(.I.NNK.t.R.
-00004610: 6805 288a 0800 b0cf 3f27 a08e 174e 4e4b  h.(.....?'...NNK
-00004620: 0a74 9452 9468 0528 8a08 00b0 8776 a76f  .t.R.h.(.....v.o
-00004630: 7d17 4e4e 4b0a 7494 5294 6805 288a 0800  }.NNK.t.R.h.(...
-00004640: b0e8 af5d 86f8 164e 4e4b 0a74 9452 9468  ...]...NNK.t.R.h
-00004650: 0528 8a08 00b0 08d5 5c48 3d17 4e4e 4b0a  .(......\H=.NNK.
-00004660: 7494 5294 6805 288a 0800 b055 a986 e5bd  t.R.h.(....U....
+00004290: 08d5 5c48 3d17 4e4e 4b0a 7494 5294 6805  ..\H=.NNK.t.R.h.
+000042a0: 288a 0800 b031 ce6c 6e3f 174e 4e4b 0a74  (....1.ln?.NNK.t
+000042b0: 9452 9468 0528 8a08 00b0 5ac7 7c94 4117  .R.h.(....Z.|.A.
+000042c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b083  NNK.t.R.h.(.....
+000042d0: c08c ba43 174e 4e4b 0a74 9452 9468 0528  ...C.NNK.t.R.h.(
+000042e0: 8a08 00b0 acb9 9ce0 4517 4e4e 4b0a 7494  ........E.NNK.t.
+000042f0: 5294 6805 288a 0800 b0d5 b2ac 0648 174e  R.h.(........H.N
+00004300: 4e4b 0a74 9452 9468 0528 8a08 00b0 af1a  NK.t.R.h.(......
+00004310: 28de 4917 4e4e 4b0a 7494 5294 6805 288a  (.I.NNK.t.R.h.(.
+00004320: 0800 b027 a5cc 524c 174e 4e4b 0a74 9452  ...'..RL.NNK.t.R
+00004330: 9468 0528 8a08 00b0 509e dc78 4e17 4e4e  .h.(....P..xN.NN
+00004340: 4b0a 7494 5294 6805 288a 0800 b079 97ec  K.t.R.h.(....y..
+00004350: 9e50 174e 4e4b 0a74 9452 9468 0528 8a08  .P.NNK.t.R.h.(..
+00004360: 00b0 53ff 6776 5217 4e4e 4b0a 7494 5294  ..S.gvR.NNK.t.R.
+00004370: 6805 288a 0800 b0cb 890c eb54 174e 4e4b  h.(........T.NNK
+00004380: 0a74 9452 9468 0528 8a08 00b0 f482 1c11  .t.R.h.(........
+00004390: 5717 4e4e 4b0a 7494 5294 6805 288a 0800  W.NNK.t.R.h.(...
+000043a0: b01d 7c2c 3759 174e 4e4b 0a74 9452 9468  ..|,7Y.NNK.t.R.h
+000043b0: 0528 8a08 00b0 9506 d1ab 5b17 4e4e 4b0a  .(........[.NNK.
+000043c0: 7494 5294 6805 288a 0800 b0be ffe0 d15d  t.R.h.(........]
+000043d0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000043e0: e7f8 f0f7 5f17 4e4e 4b0a 7494 5294 6805  ...._.NNK.t.R.h.
+000043f0: 288a 0800 b010 f200 1e62 174e 4e4b 0a74  (........b.NNK.t
+00004400: 9452 9468 0528 8a08 00b0 39eb 1044 6417  .R.h.(....9..Dd.
+00004410: 4e4e 4b0a 7494 5294 6805 288a 0800 b062  NNK.t.R.h.(....b
+00004420: e420 6a66 174e 4e4b 0a74 9452 9468 0528  . jf.NNK.t.R.h.(
+00004430: 8a08 00b0 8bdd 3090 6817 4e4e 4b0a 7494  ......0.h.NNK.t.
+00004440: 5294 6805 288a 0800 b0b4 d640 b66a 174e  R.h.(......@.j.N
+00004450: 4e4b 0a74 9452 9468 0528 8a08 00b0 8e3e  NK.t.R.h.(.....>
+00004460: bc8d 6c17 4e4e 4b0a 7494 5294 6805 288a  ..l.NNK.t.R.h.(.
+00004470: 0800 b006 c960 026f 174e 4e4b 0a74 9452  .....`.o.NNK.t.R
+00004480: 9468 0528 8a08 00b0 2fc2 7028 7117 4e4e  .h.(..../.p(q.NN
+00004490: 4b0a 7494 5294 6805 288a 0800 b058 bb80  K.t.R.h.(....X..
+000044a0: 4e73 174e 4e4b 0a74 9452 9468 0528 8a08  Ns.NNK.t.R.h.(..
+000044b0: 00b0 81b4 9074 7517 4e4e 4b0a 7494 5294  .....tu.NNK.t.R.
+000044c0: 6805 288a 0800 b0aa ada0 9a77 174e 4e4b  h.(........w.NNK
+000044d0: 0a74 9452 9468 0528 8a08 00b0 d3a6 b0c0  .t.R.h.(........
+000044e0: 7917 4e4e 4b0a 7494 5294 6805 288a 0800  y.NNK.t.R.h.(...
+000044f0: b0fc 9fc0 e67b 174e 4e4b 0a74 9452 9468  .....{.NNK.t.R.h
+00004500: 0528 8a08 00b0 8776 a76f 7d17 4e4e 4b0a  .(.....v.o}.NNK.
+00004510: 7494 5294 6805 288a 0800 b025 99d0 0c7e  t.R.h.(....%...~
+00004520: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00004530: b06f b795 7f17 4e4e 4b0a 7494 5294 6805  .o....NNK.t.R.h.
+00004540: 288a 0800 b04e 92e0 3280 174e 4e4b 0a74  (....N..2..NNK.t
+00004550: 9452 9468 0528 8a08 00b0 d968 c7bb 8117  .R.h.(.....h....
+00004560: 4e4e 4b0a 7494 5294 6805 288a 0800 b002  NNK.t.R.h.(.....
+00004570: 62d7 e183 174e 4e4b 0a74 9452 9468 0528  b....NNK.t.R.h.(
+00004580: 8a08 00b0 2b5b e707 8617 4e4e 4b0a 7494  ....+[....NNK.t.
+00004590: 5294 6805 288a 0800 b054 54f7 2d88 174e  R.h.(....TT.-..N
+000045a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 f276  NK.t.R.h.(.....v
+000045b0: 20cb 8817 4e4e 4b0a 7494 5294 6805 288a   ...NNK.t.R.h.(.
+000045c0: 0800 b090 9949 6889 174e 4e4b 0a74 9452  .....Ih..NNK.t.R
+000045d0: 9468 0528 8a08 00b0 a646 177a 8c17 4e4e  .h.(.....F.z..NN
+000045e0: 4b0a 7494 5294 6805 288a 0800 b0cf 3f27  K.t.R.h.(.....?'
+000045f0: a08e 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00004600: 00b0 f838 37c6 9017 4e4e 4b0a 7494 5294  ...87...NNK.t.R.
+00004610: 6805 288a 0800 b021 3247 ec92 174e 4e4b  h.(....!2G...NNK
+00004620: 0a74 9452 9468 0528 8a08 00b0 4a2b 5712  .t.R.h.(....J+W.
+00004630: 9517 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004640: b073 2467 3897 174e 4e4b 0a74 9452 9468  .s$g8..NNK.t.R.h
+00004650: 0528 8a08 00b0 9c1d 775e 9917 4e4e 4b0a  .(......w^..NNK.
+00004660: 7494 5294 6805 288a 0800 b0d8 62c9 989a  t.R.h.(.....b...
 00004670: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004680: beff e0d1 5d17 4e4e 4b0a 7494 5294 6805  ....].NNK.t.R.h.
-00004690: 288a 0800 b003 b766 99b9 174e 4e4b 0a74  (......f...NNK.t
-000046a0: 9452 9468 0528 8a08 00b0 d3a6 b0c0 7917  .R.h.(........y.
-000046b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d8  NNK.t.R.h.(.....
-000046c0: 62c9 989a 174e 4e4b 0a74 9452 9468 0528  b....NNK.t.R.h.(
-000046d0: 8a08 00b0 ee0f 97aa 9d17 4e4e 4b0a 7494  ..........NNK.t.
-000046e0: 5294 6805 288a 0800 b032 85d9 fcd7 164e  R.h.(....2.....N
-000046f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 dabd  NK.t.R.h.(......
-00004700: 5673 b717 4e4e 4b0a 7494 5294 6805 288a  Vs..NNK.t.R.h.(.
-00004710: 0800 b0df db4c 223b 174e 4e4b 0a74 9452  .....L";.NNK.t.R
-00004720: 9468 0528 8a08 00b0 11a9 6dac fa16 4e4e  .h.(......m...NN
-00004730: 4b0a 7494 5294 6805 288a 0800 b06e 19bd  K.t.R.h.(....n..
-00004740: cb27 174e 4e4b 0a74 9452 9468 0528 8a08  .'.NNK.t.R.h.(..
-00004750: 00b0 d45d 1d4f 1217 4e4e 4b0a 7494 5294  ...].O..NNK.t.R.
-00004760: 6805 288a 0800 b090 9949 6889 174e 4e4b  h.(......Ih..NNK
-00004770: 0a74 9452 9468 0528 8a08 00b0 8de9 2cd6  .t.R.h.(......,.
-00004780: 3617 4e4e 4b0a 7494 5294 6805 288a 0800  6.NNK.t.R.h.(...
-00004790: b059 72ed dc0b 174e 4e4b 0a74 9452 9468  .Yr....NNK.t.R.h
-000047a0: 0528 8a08 00b0 2599 d00c 7e17 4e4e 4b0a  .(....%...~.NNK.
-000047b0: 7494 5294 6805 288a 0800 b077 edcd 2fe5  t.R.h.(....w../.
-000047c0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000047d0: f98d c67d c617 4e4e 4b0a 7494 5294 6805  ...}..NNK.t.R.h.
-000047e0: 288a 0800 b0ac b99c e045 174e 4e4b 0a74  (........E.NNK.t
-000047f0: 9452 9468 0528 8a08 00b0 fd56 2d75 1417  .R.h.(.....V-u..
-00004800: 4e4e 4b0a 7494 5294 6805 288a 0800 b0b0  NNK.t.R.h.(.....
-00004810: 6fb7 957f 174e 4e4b 0a74 9452 9468 0528  o....NNK.t.R.h.(
-00004820: 8a08 00b0 c00b dd17 2c17 4e4e 4b0a 7494  ........,.NNK.t.
-00004830: 5294 6805 288a 0800 b092 f4d6 42a6 174e  R.h.(.......B..N
-00004840: 4e4b 0a74 9452 9468 0528 8a08 00b0 2287  NK.t.R.h.(....".
-00004850: d6a3 c817 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00004860: 0800 b0d5 b2ac 0648 174e 4e4b 0a74 9452  .......H.NNK.t.R
-00004870: 9468 0528 8a08 00b0 c9df ed7b e916 4e4e  .h.(.......{..NN
-00004880: 4b0a 7494 5294 6805 288a 0800 b06d c42d  K.t.R.h.(....m.-
-00004890: 14f2 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000048a0: 00b0 cb89 0ceb 5417 4e4e 4b0a 7494 5294  ......T.NNK.t.R.
-000048b0: 6805 288a 0800 b0b6 e23c fc38 174e 4e4b  h.(......<.8.NNK
-000048c0: 0a74 9452 9468 0528 8a08 00b0 b1c4 464d  .t.R.h.(......FM
-000048d0: b517 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000048e0: b036 d916 dbae 174e 4e4b 0a74 9452 9465  .6.....NNK.t.R.e
-000048f0: 752e                                     u.
+00004680: ee0f 97aa 9d17 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00004690: 288a 0800 b017 09a7 d09f 174e 4e4b 0a74  (..........NNK.t
+000046a0: 9452 9468 0528 8a08 00b0 4002 b7f6 a117  .R.h.(....@.....
+000046b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b07c  NNK.t.R.h.(....|
+000046c0: 4709 31a3 174e 4e4b 0a74 9452 9468 0528  G.1..NNK.t.R.h.(
+000046d0: 8a08 00b0 92f4 d642 a617 4e4e 4b0a 7494  .......B..NNK.t.
+000046e0: 5294 6805 288a 0800 b0bb ede6 68a8 174e  R.h.(.......h..N
+000046f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 e4e6  NK.t.R.h.(......
+00004700: f68e aa17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00004710: 0800 b00d e006 b5ac 174e 4e4b 0a74 9452  .........NNK.t.R
+00004720: 9468 0528 8a08 00b0 36d9 16db ae17 4e4e  .h.(....6.....NN
+00004730: 4b0a 7494 5294 6805 288a 0800 b05f d226  K.t.R.h.(...._.&
+00004740: 01b1 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00004750: 00b0 88cb 3627 b317 4e4e 4b0a 7494 5294  ....6'..NNK.t.R.
+00004760: 6805 288a 0800 b0b1 c446 4db5 174e 4e4b  h.(......FM..NNK
+00004770: 0a74 9452 9468 0528 8a08 00b0 dabd 5673  .t.R.h.(......Vs
+00004780: b717 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004790: b003 b766 99b9 174e 4e4b 0a74 9452 9468  ...f...NNK.t.R.h
+000047a0: 0528 8a08 00b0 2cb0 76bf bb17 4e4e 4b0a  .(....,.v...NNK.
+000047b0: 7494 5294 6805 288a 0800 b055 a986 e5bd  t.R.h.(....U....
+000047c0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000047d0: 91ee d81f bf17 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+000047e0: 288a 0800 b0a7 9ba6 31c2 174e 4e4b 0a74  (.......1..NNK.t
+000047f0: 9452 9468 0528 8a08 00b0 d094 b657 c417  .R.h.(.......W..
+00004800: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f9  NNK.t.R.h.(.....
+00004810: 8dc6 7dc6 174e 4e4b 0a74 9452 9468 0528  ..}..NNK.t.R.h.(
+00004820: 8a08 00b0 2287 d6a3 c817 4e4e 4b0a 7494  ....".....NNK.t.
+00004830: 5294 6805 288a 0800 b04b 80e6 c9ca 174e  R.h.(....K.....N
+00004840: 4e4b 0a74 9452 9468 0528 8a08 00b0 7479  NK.t.R.h.(....ty
+00004850: f6ef cc17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00004860: 0800 b09d 7206 16cf 174e 4e4b 0a74 9452  ....r....NNK.t.R
+00004870: 9468 0528 8a08 00b0 ef64 2662 d317 4e4e  .h.(.....d&b..NN
+00004880: 4b0a 7494 5294 6805 288a 0800 b093 4966  K.t.R.h.(.....If
+00004890: fadb 174e 4e4b 0a74 9452 9465 752e       ...NNK.t.R.eu.
```

### Comparing `volstreet-7.2.2/volstreet/parallelization.py` & `volstreet-8.0.0/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/performance_tracking.py` & `volstreet-8.0.0/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/position_dashboard/app.py` & `volstreet-8.0.0/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/position_dashboard/formatting.py` & `volstreet-8.0.0/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/strategies/deployment.py` & `volstreet-8.0.0/volstreet/strategies/deployment.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/strategies/error_handling.py` & `volstreet-8.0.0/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/strategies/helpers.py` & `volstreet-8.0.0/volstreet/strategies/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime, timedelta, time
 from time import sleep
 from itertools import product
 import inspect
 import traceback
 from typing import Callable
 from pulp import LpStatus
+import os
 from volstreet import config
 from volstreet.config import logger
 from volstreet.blackscholes import Greeks
 from volstreet.utils.core import (
     time_to_expiry,
     current_time,
     round_shares_to_lot_size,
@@ -39,14 +40,23 @@
 from volstreet.strategies.tools import filter_orders_by_strategy
 from volstreet.strategies.optimization import (
     filter_greeks_frame,
     delta_neutral_optimization_lp,
 )
 from volstreet.strategies.error_handling import log_error
 
+if config.backtest_mode:
+    logger.info(
+        f"Importing proxy functions in module: {__name__} since backtesting is enabled."
+    )
+    from volstreet.backtests.proxy_functions import (
+        execute_instructions,
+        ProxyFeeds as LiveFeeds,
+    )
+
 
 @define(slots=False, repr=False, eq=False)
 class ActiveOption(Option):
     """An extension of Option for more flexibility.
     Counterpart attribute is only implemented to conduct the hygiene check. It has no other use.
     """
 
@@ -913,22 +923,25 @@
             }
             for option in self.active_options
         }
         execution_details = execute_instructions(instructions, at_market=at_market)
         for option, avg_price in execution_details.items():
             option.update_active_qty_and_premium(-option.active_qty, avg_price)
 
-    def record_position_status(self) -> None:
+    def record_position_status(self, directory: str | None = None) -> None:
         """Designed to periodically save the position status to a file."""
         """
         Saves the current position status to a JSON file periodically.
         """
 
         date = current_time().strftime("%Y-%m-%d")
-        file_path = f"{ActiveSession.obj.userId}\\{self.underlying.name}_delta_data\\{date}.json"
+        if directory is None:
+            file_path = f"{ActiveSession.obj.userId}\\{self.underlying.name}_delta_data\\{date}.json"
+        else:
+            file_path = os.path.join(directory, f"{date}.json")
 
         position_status = {
             "timestamp": current_time(),
             "underlying": self.underlying.name,
             "underlying_price": self.underlying.fetch_ltp(),
             "expiry": self.expiry,
             "base_exposure_qty": self.base_exposure_qty,
```

### Comparing `volstreet-7.2.2/volstreet/strategies/monitoring.py` & `volstreet-8.0.0/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/strategies/optimization.py` & `volstreet-8.0.0/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/strategies/strats.py` & `volstreet-8.0.0/volstreet/strategies/strats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from datetime import datetime, timedelta, time
 from threading import Thread
 from time import sleep
 from typing import Optional
+from volstreet import config
 from volstreet.config import logger
 from volstreet.utils.core import (
     current_time,
     find_strike,
     time_to_expiry,
     check_for_weekend,
     calculate_ema,
@@ -47,14 +48,26 @@
     load_current_strangle,
     approve_execution,
     notify_pnl,
     process_stop_loss_order_statuses,
 )
 from volstreet.strategies.error_handling import exit_on_error
 
+if config.backtest_mode:
+    logger.info(
+        f"Importing proxy functions in module: {__name__} since backtesting is enabled."
+    )
+    from volstreet.backtests.proxy_functions import (
+        execute_instructions,
+        sleep_until_next_action,
+        notify_pnl,
+        increase_robustness,
+        exit_on_error,
+    )
+
 
 def quick_strangle_loop(
     underlying: Index | Stock,
     action: str,
     iv_threshold: float,
     take_profit: float,
     scan_exit_time: tuple[int, int],
@@ -293,14 +306,15 @@
     delta_threshold_pct: float = 0.04,
     hedge_margin: float | None = None,  # eg 0.2
     exit_time: Optional[tuple] = (15, 29),
     use_cache: Optional[bool] = True,
     at_market: bool = False,
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Delta hedged strangle",
+    data_directory: Optional[str] = None,
 ):
     """Theta time jump is defined in hours. Delta interval is in minutes. Delta threshold is in percentage terms
     eg: 0.02 for 2%
     """
 
     # Setting the exposure
     start_time = current_time()
@@ -385,25 +399,25 @@
         while not any(delta_position.exit_triggers.values()):
             sleep_until_next_action(
                 delta_interval_minutes,
                 exit_time,
                 special_condition=interruption_condition,
             )
             try:
-                delta_position.record_position_status()
+                delta_position.record_position_status(directory=data_directory)
             except Exception as e:
                 notifier(
                     f"{underlying.name} Error while recording position status: {e}\n"
                     f"Traceback: {e.__traceback__}",
                     notification_url,
                     "ERROR",
                 )
                 delta_position.record_position_status = lambda: None
 
-            if current_time().time() > time(*exit_time):
+            if current_time().time() >= time(*exit_time):
                 delta_position.exit_triggers["end_time"] = True
                 break
 
             delta_position.update_underlying()
             aggregate_delta: float = (
                 delta_position.aggregate_greeks().delta
             )  # The prices and greeks of the options are updated and cached here
```

### Comparing `volstreet-7.2.2/volstreet/trade_interface/instruments.py` & `volstreet-8.0.0/volstreet/trade_interface/instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,23 @@
 import volstreet.blackscholes as bs
 from volstreet.angel_interface.interface import (
     fetch_ltp,
     place_order,
     generate_order_params,
 )
 
+if config.backtest_mode:
+    logger.info(
+        f"Importing proxy functions in module: {__name__} since backtesting is enabled."
+    )
+    from volstreet.backtests.proxy_functions import (
+        get_symbol_token,
+        get_lot_size,
+    )
+
 
 class OptionType(Enum):
     CALL = "CE"
     PUT = "PE"
 
 
 class Action(Enum):
```

### Comparing `volstreet-7.2.2/volstreet/trade_interface/order_execution.py` & `volstreet-8.0.0/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/trade_interface/underlyings.py` & `volstreet-8.0.0/volstreet/trade_interface/underlyings.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,25 @@
     time_to_expiry,
     get_available_strikes,
     custom_cacher,
 )
 from volstreet.angel_interface.interface import fetch_ltp
 from volstreet.trade_interface.instruments import Straddle, Strangle, Option, OptionType
 
+if config.backtest_mode:
+    logger.info(
+        f"Importing proxy functions in module: {__name__} since backtesting is enabled."
+    )
+    from volstreet.backtests.proxy_functions import (
+        get_expiry_dates,
+        get_symbol_token,
+        get_base,
+        get_lot_size,
+    )
+
 
 class Index:
     """Initialize an index with the name of the index in uppercase"""
 
     def __init__(self, name, caching=False):
         self.name = name.upper()
         self.current_expiry = None
```

### Comparing `volstreet-7.2.2/volstreet/utils/change_config.py` & `volstreet-8.0.0/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/utils/communication.py` & `volstreet-8.0.0/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/utils/core.py` & `volstreet-8.0.0/volstreet/utils/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,16 @@
             total += current
             current = 0
     total += current
     return total
 
 
 def current_time():
+    if config.backtest_mode:
+        return config.backtest_state
     # Adjusting for timezones
     ist = timezone(timedelta(hours=5, minutes=30))
     return datetime.now(ist).replace(tzinfo=None)
 
 
 def market_hours():
     if time(9, 15) <= current_time().time() <= time(15, 30):
```

### Comparing `volstreet-7.2.2/volstreet/utils/data_io.py` & `volstreet-8.0.0/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/utils/scrip_processing.py` & `volstreet-8.0.0/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/vectorized_blackscholes.py` & `volstreet-8.0.0/volstreet/vectorized_blackscholes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 N = norm.cdf  # Normal distribution cumulative density function
 
 
 # Calculate d1 term in Black-Scholes formula
 def d1(
     S: np.ndarray, K: np.ndarray, t: np.ndarray, r: np.ndarray, sigma: np.ndarray
 ) -> np.ndarray:
-    numerator = np.log(S / K) + (r + 0.5 * sigma**2) * t
+    numerator = np.log(S / K) + (r + (0.5 * sigma**2)) * t
     denominator = sigma * np.sqrt(t)
     return numerator / denominator
 
 
 # Calculate d2 term in Black-Scholes formula
 def d2(
     S: np.ndarray, K: np.ndarray, t: np.ndarray, r: np.ndarray, sigma: np.ndarray
@@ -141,15 +141,15 @@
 
 def add_greeks_to_dataframe(
     data_frame: pd.DataFrame,
     price_col: str = "open",
     call_strike_col: str = "call_strike",
     put_strike_col: str = "put_strike",
     time_to_expiry_col: str = "time_to_expiry",
-    r_col: str = None,
+    r_col: str = "r",
     use_one_iv: bool = True,
 ) -> pd.DataFrame:
     data_frame = data_frame.copy()
 
     if r_col is None:
         r = np.array([0.06] * len(data_frame.index))
     else:
```

### Comparing `volstreet-7.2.2/volstreet/vslogging/formatters.py` & `volstreet-8.0.0/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/vslogging/logging_config.json` & `volstreet-8.0.0/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/vslogging/logging_setup.py` & `volstreet-8.0.0/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet/vslogging/parsing.py` & `volstreet-8.0.0/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.2/volstreet.egg-info/PKG-INFO` & `volstreet-8.0.0/volstreet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.2.2
+Version: 8.0.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.2.2/volstreet.egg-info/SOURCES.txt` & `volstreet-8.0.0/volstreet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 volstreet/dealingroom.py
 volstreet/decorators.py
 volstreet/discord_bot.py
 volstreet/exceptions.py
 volstreet/parallelization.py
 volstreet/performance_tracking.py
 volstreet/vectorized_blackscholes.py
+volstreet/volstreet_mode.json
 volstreet.egg-info/PKG-INFO
 volstreet.egg-info/SOURCES.txt
 volstreet.egg-info/dependency_links.txt
 volstreet.egg-info/requires.txt
 volstreet.egg-info/top_level.txt
 volstreet/angel_interface/__init__.py
 volstreet/angel_interface/access_rate_handlers.py
@@ -24,34 +25,38 @@
 volstreet/angel_interface/base_websocket.py
 volstreet/angel_interface/interface.py
 volstreet/angel_interface/login.py
 volstreet/angel_interface/order_websocket.py
 volstreet/angel_interface/price_websocket.py
 volstreet/angel_interface/smart_connect.py
 volstreet/backtests/__init__.py
+volstreet/backtests/analysis.py
 volstreet/backtests/database.py
 volstreet/backtests/delta_hedging.py
 volstreet/backtests/delta_optimizer.py
 volstreet/backtests/framework.py
 volstreet/backtests/intraday_backtest_abc.py
 volstreet/backtests/proxy_functions.py
-volstreet/backtests/state.py
+volstreet/backtests/runner.py
 volstreet/backtests/tools.py
 volstreet/backtests/trend.py
 volstreet/backtests/underlying_info.py
 volstreet/datamodule/__init__.py
 volstreet/datamodule/analysis.py
 volstreet/datamodule/archive.py
 volstreet/datamodule/data_handling.py
 volstreet/datamodule/eod_client.py
 volstreet/datamodule/gambling.py
 volstreet/datamodule/intraday_data.py
 volstreet/datamodule/stockmock.py
 volstreet/datamodule/trading_assistance.py
+volstreet/historical_info/__init__.py
 volstreet/historical_info/index_expiries.pkl
+volstreet/historical_info/market_days.pkl
+volstreet/models/__init__.py
 volstreet/position_dashboard/__init__.py
 volstreet/position_dashboard/app.py
 volstreet/position_dashboard/formatting.py
 volstreet/strategies/__init__.py
 volstreet/strategies/deployment.py
 volstreet/strategies/error_handling.py
 volstreet/strategies/helpers.py
```

