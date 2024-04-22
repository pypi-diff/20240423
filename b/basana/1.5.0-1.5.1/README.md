# Comparing `tmp/basana-1.5.0.tar.gz` & `tmp/basana-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basana-1.5.0.tar", max compression
+gzip compressed data, was "basana-1.5.1.tar", max compression
```

## Comparing `basana-1.5.0.tar` & `basana-1.5.1.tar`

### file list

```diff
@@ -1,73 +1,72 @@
--rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.5.0/LICENSE
--rw-r--r--   0        0        0     1314 2023-08-12 00:43:46.074975 basana-1.5.0/basana/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.5.0/basana/backtesting/__init__.py
--rw-r--r--   0        0        0     3922 2023-12-13 20:06:39.979789 basana-1.5.0/basana/backtesting/account_balances.py
--rw-r--r--   0        0        0    13606 2023-09-26 00:41:37.372025 basana-1.5.0/basana/backtesting/charts.py
--rw-r--r--   0        0        0      679 2023-08-16 01:35:42.085385 basana-1.5.0/basana/backtesting/errors.py
--rw-r--r--   0        0        0    22695 2023-12-13 20:06:39.980442 basana-1.5.0/basana/backtesting/exchange.py
--rw-r--r--   0        0        0     2786 2023-12-13 21:19:21.546409 basana-1.5.0/basana/backtesting/fees.py
--rw-r--r--   0        0        0     1683 2023-08-20 23:23:36.234419 basana-1.5.0/basana/backtesting/helpers.py
--rw-r--r--   0        0        0     6150 2023-04-28 03:07:23.325407 basana-1.5.0/basana/backtesting/liquidity.py
--rw-r--r--   0        0        0    16012 2023-12-13 20:06:39.981664 basana-1.5.0/basana/backtesting/orders.py
--rw-r--r--   0        0        0     7913 2023-04-28 03:07:23.326667 basana-1.5.0/basana/backtesting/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.5.0/basana/core/__init__.py
--rw-r--r--   0        0        0     6035 2023-09-07 17:37:18.572307 basana-1.5.0/basana/core/bar.py
--rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.5.0/basana/core/config.py
--rw-r--r--   0        0        0    17172 2023-09-26 00:41:25.358332 basana-1.5.0/basana/core/dispatcher.py
--rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.5.0/basana/core/dt.py
--rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.5.0/basana/core/enums.py
--rw-r--r--   0        0        0     3456 2023-07-15 22:07:34.279552 basana-1.5.0/basana/core/event.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.5.0/basana/core/event_sources/__init__.py
--rw-r--r--   0        0        0     3025 2023-04-28 03:07:23.329229 basana-1.5.0/basana/core/event_sources/csv.py
--rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.5.0/basana/core/event_sources/trading_signal.py
--rw-r--r--   0        0        0     4635 2023-08-12 00:43:46.076982 basana-1.5.0/basana/core/helpers.py
--rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.5.0/basana/core/logs.py
--rw-r--r--   0        0        0     1459 2023-04-03 17:28:32.841069 basana-1.5.0/basana/core/pair.py
--rw-r--r--   0        0        0     2280 2023-04-13 16:56:31.182428 basana-1.5.0/basana/core/token_bucket.py
--rw-r--r--   0        0        0     6010 2023-04-28 03:07:23.329823 basana-1.5.0/basana/core/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.5.0/basana/external/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.5.0/basana/external/binance/__init__.py
--rw-r--r--   0        0        0     2692 2023-07-31 21:34:13.074413 basana-1.5.0/basana/external/binance/client/__init__.py
--rw-r--r--   0        0        0     4971 2023-07-31 21:34:13.074675 basana-1.5.0/basana/external/binance/client/base.py
--rw-r--r--   0        0        0     8900 2023-07-31 21:34:13.074952 basana-1.5.0/basana/external/binance/client/margin.py
--rw-r--r--   0        0        0     6166 2023-07-31 21:34:13.075223 basana-1.5.0/basana/external/binance/client/spot.py
--rw-r--r--   0        0        0    10335 2023-10-03 19:58:29.854030 basana-1.5.0/basana/external/binance/common.py
--rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.5.0/basana/external/binance/config.py
--rw-r--r--   0        0        0     2161 2023-07-31 21:34:13.076181 basana-1.5.0/basana/external/binance/cross_margin.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.5.0/basana/external/binance/csv/__init__.py
--rw-r--r--   0        0        0     1648 2023-03-29 02:43:04.769173 basana-1.5.0/basana/external/binance/csv/bars.py
--rw-r--r--   0        0        0    10385 2023-04-16 21:31:22.354698 basana-1.5.0/basana/external/binance/exchange.py
--rw-r--r--   0        0        0     3052 2023-03-29 02:43:04.769989 basana-1.5.0/basana/external/binance/helpers.py
--rw-r--r--   0        0        0     3237 2023-07-31 21:34:13.076964 basana-1.5.0/basana/external/binance/isolated_margin.py
--rw-r--r--   0        0        0     1913 2023-04-13 16:56:31.186636 basana-1.5.0/basana/external/binance/klines.py
--rw-r--r--   0        0        0    12125 2023-12-13 20:04:30.581709 basana-1.5.0/basana/external/binance/margin.py
--rw-r--r--   0        0        0     6165 2023-04-28 03:07:23.331858 basana-1.5.0/basana/external/binance/margin_requests.py
--rw-r--r--   0        0        0     4143 2023-04-16 21:31:22.355396 basana-1.5.0/basana/external/binance/order_book.py
--rw-r--r--   0        0        0    12214 2023-07-31 21:34:13.079047 basana-1.5.0/basana/external/binance/spot.py
--rw-r--r--   0        0        0     5555 2023-04-28 03:07:23.332666 basana-1.5.0/basana/external/binance/spot_requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.5.0/basana/external/binance/tools/__init__.py
--rw-r--r--   0        0        0     4521 2023-07-31 21:34:13.079440 basana-1.5.0/basana/external/binance/tools/download_bars.py
--rw-r--r--   0        0        0     2710 2023-04-13 16:56:31.189265 basana-1.5.0/basana/external/binance/trades.py
--rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.5.0/basana/external/binance/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.5.0/basana/external/bitstamp/__init__.py
--rw-r--r--   0        0        0     9077 2023-07-31 21:34:13.081034 basana-1.5.0/basana/external/bitstamp/client.py
--rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.5.0/basana/external/bitstamp/config.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.5.0/basana/external/bitstamp/csv/__init__.py
--rw-r--r--   0        0        0     2047 2023-03-29 02:43:04.774543 basana-1.5.0/basana/external/bitstamp/csv/bars.py
--rw-r--r--   0        0        0    23031 2023-04-16 21:31:22.356361 basana-1.5.0/basana/external/bitstamp/exchange.py
--rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.5.0/basana/external/bitstamp/helpers.py
--rw-r--r--   0        0        0     4150 2023-04-16 21:31:22.357186 basana-1.5.0/basana/external/bitstamp/order_book.py
--rw-r--r--   0        0        0     3067 2023-04-16 21:31:22.357564 basana-1.5.0/basana/external/bitstamp/orders.py
--rw-r--r--   0        0        0     4283 2023-04-28 03:07:23.333551 basana-1.5.0/basana/external/bitstamp/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.5.0/basana/external/bitstamp/tools/__init__.py
--rw-r--r--   0        0        0     4098 2023-07-31 21:34:13.081920 basana-1.5.0/basana/external/bitstamp/tools/download_bars.py
--rw-r--r--   0        0        0     2968 2023-04-16 21:31:22.357932 basana-1.5.0/basana/external/bitstamp/trades.py
--rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.5.0/basana/external/bitstamp/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.5.0/basana/external/common/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.5.0/basana/external/common/csv/__init__.py
--rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.5.0/basana/external/common/csv/bars.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.5.0/basana/external/yahoo/__init__.py
--rw-r--r--   0        0        0     3384 2023-03-29 02:43:04.779788 basana-1.5.0/basana/external/yahoo/bars.py
--rw-r--r--   0        0        0     1189 2024-01-07 01:55:12.477091 basana-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 basana-1.5.0/setup.py
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 basana-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1314 2023-08-12 00:43:46.074975 basana-1.5.1/basana/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.5.1/basana/backtesting/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-21 14:47:19.059493 basana-1.5.1/basana/backtesting/account_balances.py
+-rw-r--r--   0        0        0    13606 2024-04-21 14:47:19.060947 basana-1.5.1/basana/backtesting/charts.py
+-rw-r--r--   0        0        0      679 2024-04-21 14:47:19.061677 basana-1.5.1/basana/backtesting/errors.py
+-rw-r--r--   0        0        0    22695 2024-04-21 14:47:19.062500 basana-1.5.1/basana/backtesting/exchange.py
+-rw-r--r--   0        0        0     2786 2024-03-17 02:17:43.056901 basana-1.5.1/basana/backtesting/fees.py
+-rw-r--r--   0        0        0     1683 2024-04-21 14:47:19.063239 basana-1.5.1/basana/backtesting/helpers.py
+-rw-r--r--   0        0        0     6150 2023-04-28 03:07:23.325407 basana-1.5.1/basana/backtesting/liquidity.py
+-rw-r--r--   0        0        0    16012 2024-04-21 14:47:19.064430 basana-1.5.1/basana/backtesting/orders.py
+-rw-r--r--   0        0        0     7913 2024-04-21 14:47:19.065246 basana-1.5.1/basana/backtesting/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.5.1/basana/core/__init__.py
+-rw-r--r--   0        0        0     6035 2023-09-07 17:37:18.572307 basana-1.5.1/basana/core/bar.py
+-rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.5.1/basana/core/config.py
+-rw-r--r--   0        0        0    18334 2024-03-23 19:13:35.712857 basana-1.5.1/basana/core/dispatcher.py
+-rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.5.1/basana/core/dt.py
+-rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.5.1/basana/core/enums.py
+-rw-r--r--   0        0        0     3456 2023-07-15 22:07:34.279552 basana-1.5.1/basana/core/event.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.5.1/basana/core/event_sources/__init__.py
+-rw-r--r--   0        0        0     3900 2024-04-21 22:41:04.597299 basana-1.5.1/basana/core/event_sources/csv.py
+-rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.5.1/basana/core/event_sources/trading_signal.py
+-rw-r--r--   0        0        0     5493 2024-03-23 19:13:35.713599 basana-1.5.1/basana/core/helpers.py
+-rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.5.1/basana/core/logs.py
+-rw-r--r--   0        0        0     1459 2024-03-08 02:30:28.708175 basana-1.5.1/basana/core/pair.py
+-rw-r--r--   0        0        0     2280 2023-04-13 16:56:31.182428 basana-1.5.1/basana/core/token_bucket.py
+-rw-r--r--   0        0        0     6010 2023-04-28 03:07:23.329823 basana-1.5.1/basana/core/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.5.1/basana/external/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.5.1/basana/external/binance/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-31 21:34:13.074413 basana-1.5.1/basana/external/binance/client/__init__.py
+-rw-r--r--   0        0        0     4971 2023-07-31 21:34:13.074675 basana-1.5.1/basana/external/binance/client/base.py
+-rw-r--r--   0        0        0     8900 2023-07-31 21:34:13.074952 basana-1.5.1/basana/external/binance/client/margin.py
+-rw-r--r--   0        0        0     6166 2023-07-31 21:34:13.075223 basana-1.5.1/basana/external/binance/client/spot.py
+-rw-r--r--   0        0        0    10335 2024-01-21 01:18:21.494623 basana-1.5.1/basana/external/binance/common.py
+-rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.5.1/basana/external/binance/config.py
+-rw-r--r--   0        0        0     2161 2023-07-31 21:34:13.076181 basana-1.5.1/basana/external/binance/cross_margin.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.5.1/basana/external/binance/csv/__init__.py
+-rw-r--r--   0        0        0     1631 2024-04-22 21:57:16.341148 basana-1.5.1/basana/external/binance/csv/bars.py
+-rw-r--r--   0        0        0    10385 2023-04-16 21:31:22.354698 basana-1.5.1/basana/external/binance/exchange.py
+-rw-r--r--   0        0        0     3037 2024-04-21 23:05:42.841742 basana-1.5.1/basana/external/binance/helpers.py
+-rw-r--r--   0        0        0     3237 2023-07-31 21:34:13.076964 basana-1.5.1/basana/external/binance/isolated_margin.py
+-rw-r--r--   0        0        0     1913 2023-04-13 16:56:31.186636 basana-1.5.1/basana/external/binance/klines.py
+-rw-r--r--   0        0        0    12125 2023-12-13 20:04:30.581709 basana-1.5.1/basana/external/binance/margin.py
+-rw-r--r--   0        0        0     6165 2023-04-28 03:07:23.331858 basana-1.5.1/basana/external/binance/margin_requests.py
+-rw-r--r--   0        0        0     4143 2023-04-16 21:31:22.355396 basana-1.5.1/basana/external/binance/order_book.py
+-rw-r--r--   0        0        0    12214 2023-07-31 21:34:13.079047 basana-1.5.1/basana/external/binance/spot.py
+-rw-r--r--   0        0        0     5555 2023-04-28 03:07:23.332666 basana-1.5.1/basana/external/binance/spot_requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.5.1/basana/external/binance/tools/__init__.py
+-rw-r--r--   0        0        0     4867 2024-04-21 23:05:42.842439 basana-1.5.1/basana/external/binance/tools/download_bars.py
+-rw-r--r--   0        0        0     2710 2023-04-13 16:56:31.189265 basana-1.5.1/basana/external/binance/trades.py
+-rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.5.1/basana/external/binance/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.5.1/basana/external/bitstamp/__init__.py
+-rw-r--r--   0        0        0     9077 2023-07-31 21:34:13.081034 basana-1.5.1/basana/external/bitstamp/client.py
+-rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.5.1/basana/external/bitstamp/config.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.5.1/basana/external/bitstamp/csv/__init__.py
+-rw-r--r--   0        0        0     2030 2024-04-22 21:57:16.341909 basana-1.5.1/basana/external/bitstamp/csv/bars.py
+-rw-r--r--   0        0        0    23031 2023-04-16 21:31:22.356361 basana-1.5.1/basana/external/bitstamp/exchange.py
+-rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.5.1/basana/external/bitstamp/helpers.py
+-rw-r--r--   0        0        0     4135 2024-04-21 23:05:42.843081 basana-1.5.1/basana/external/bitstamp/order_book.py
+-rw-r--r--   0        0        0     3067 2023-04-16 21:31:22.357564 basana-1.5.1/basana/external/bitstamp/orders.py
+-rw-r--r--   0        0        0     4283 2023-04-28 03:07:23.333551 basana-1.5.1/basana/external/bitstamp/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.5.1/basana/external/bitstamp/tools/__init__.py
+-rw-r--r--   0        0        0     4444 2024-04-21 23:05:42.843715 basana-1.5.1/basana/external/bitstamp/tools/download_bars.py
+-rw-r--r--   0        0        0     2953 2024-04-21 23:05:42.844443 basana-1.5.1/basana/external/bitstamp/trades.py
+-rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.5.1/basana/external/bitstamp/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.5.1/basana/external/common/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.5.1/basana/external/common/csv/__init__.py
+-rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.5.1/basana/external/common/csv/bars.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.5.1/basana/external/yahoo/__init__.py
+-rw-r--r--   0        0        0     3350 2024-04-22 21:57:16.342499 basana-1.5.1/basana/external/yahoo/bars.py
+-rw-r--r--   0        0        0     1187 2024-04-22 22:02:40.215823 basana-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 basana-1.5.1/PKG-INFO
```

### Comparing `basana-1.5.0/LICENSE` & `basana-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/__init__.py` & `basana-1.5.1/basana/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/__init__.py` & `basana-1.5.1/basana/backtesting/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/account_balances.py` & `basana-1.5.1/basana/backtesting/account_balances.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/charts.py` & `basana-1.5.1/basana/backtesting/charts.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/errors.py` & `basana-1.5.1/basana/backtesting/errors.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/exchange.py` & `basana-1.5.1/basana/backtesting/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/fees.py` & `basana-1.5.1/basana/backtesting/fees.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/helpers.py` & `basana-1.5.1/basana/backtesting/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/liquidity.py` & `basana-1.5.1/basana/backtesting/liquidity.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/orders.py` & `basana-1.5.1/basana/backtesting/orders.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/backtesting/requests.py` & `basana-1.5.1/basana/backtesting/requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/__init__.py` & `basana-1.5.1/basana/core/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/bar.py` & `basana-1.5.1/basana/core/bar.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/config.py` & `basana-1.5.1/basana/core/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/dispatcher.py` & `basana-1.5.1/basana/core/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import cast, Any, Awaitable, Callable, Dict, Generator, List, Optional, Set, Tuple
 import abc
 import asyncio
+import contextlib
 import dataclasses
 import datetime
 import heapq
 import logging
 import platform
 import signal
 
@@ -135,15 +136,18 @@
         self._sniffers_post: List[EventHandler] = []
         self._producers: Set[event.Producer] = set()
         self._active_tasks: Optional[helpers.TaskGroup] = None
         self._running = False
         self._stopped = False
         self._scheduler_queue = SchedulerQueue()
         self._event_mux = EventMultiplexer()
-        self._task_pool = helpers.TaskPool(max_concurrent)
+        # Used to execute event and scheduler handlers.
+        self._handlers_task_pool = helpers.TaskPool(max_concurrent)
+        # Set to True for the dispatcher to stop if a handler raises an exception.
+        self.stop_on_handler_exceptions = False
 
     @property
     def current_event_dt(self) -> Optional[datetime.datetime]:
         helpers.deprecation("Use now() instead")
         return self.now()
 
     @abc.abstractmethod
@@ -157,15 +161,15 @@
 
     def stop(self):
         """Requests the event dispatcher to stop the event processing loop."""
         logger.debug("Stop requested")
         self._stopped = True
         if self._active_tasks:
             self._active_tasks.cancel()
-        self._task_pool.cancel()
+        self._handlers_task_pool.cancel()
 
     def subscribe(self, source: event.EventSource, event_handler: EventHandler):
         """Registers an async callable that will be called when an event source has new events.
 
         :param source: An event source.
         :param event_handler: An async callable that receives an event.
         """
@@ -219,62 +223,88 @@
         if platform.system() != "Windows":  # pragma: no cover
             for stop_signal in stop_signals:
                 asyncio.get_event_loop().add_signal_handler(stop_signal, self.stop)
 
         self._running = True
         try:
             # Initialize producers.
-            async with helpers.TaskGroup() as tg:
-                self._active_tasks = tg  # So it can be canceled.
+            async with self._task_group() as tg:
                 for producer in self._producers:
                     tg.create_task(producer.initialize())
             # Run producers and dispatch loop.
-            async with helpers.TaskGroup() as tg:
-                self._active_tasks = tg  # So it can be canceled.
+            async with self._task_group() as tg:
                 for producer in self._producers:
                     tg.create_task(producer.main())
                 tg.create_task(self._dispatch_loop())
         except asyncio.CancelledError:
             pass
         finally:
             # Cancel any pending task in the event pool.
-            self._task_pool.cancel()
-            await self._task_pool.wait_all()
+            self._handlers_task_pool.cancel()
+            await self._handlers_task_pool.wait()
             # No more cancelation at this point.
             self._active_tasks = None
             # Finalize producers.
             await gather_no_raise(*[producer.finalize() for producer in self._producers])
 
     def on_error(self, error: Any):
         logger.error(error)
 
     @abc.abstractmethod
     async def _dispatch_loop(self):
         raise NotImplementedError()
 
+    @contextlib.asynccontextmanager
+    async def _task_group(self):
+        try:
+            async with helpers.TaskGroup() as tg:
+                self._active_tasks = tg  # So it can be canceled.
+                yield tg
+        finally:
+            self._active_tasks = None
+
     async def _dispatch_event(self, event_dispatch: EventDispatch):
         logger.debug(logs.StructuredMessage(
             "Dispatching event", when=event_dispatch.event.when, type=type(event_dispatch.event)
         ))
         if self._sniffers_pre:
-            await gather_no_raise(
-                *[event_handler(event_dispatch.event) for event_handler in self._sniffers_pre]
+            await asyncio.gather(
+                *[self._call_event_handler(event_dispatch.event, handler) for handler in self._sniffers_pre]
             )
         if event_dispatch.handlers:
-            await gather_no_raise(
-                *[event_handler(event_dispatch.event) for event_handler in event_dispatch.handlers]
+            await asyncio.gather(
+                *[self._call_event_handler(event_dispatch.event, handler) for handler in event_dispatch.handlers]
             )
         if self._sniffers_post:
-            await gather_no_raise(
-                *[event_handler(event_dispatch.event) for event_handler in self._sniffers_post]
+            await asyncio.gather(
+                *[self._call_event_handler(event_dispatch.event, handler) for handler in self._sniffers_post]
             )
 
+    async def _call_event_handler(self, event: event.Event, handler: EventHandler):
+        try:
+            return await handler(event)
+        except Exception as e:
+            logger.exception(logs.StructuredMessage(
+                "Unhandled exception in event handler", error=e, event=dict(type=type(event), when=event.when),
+                handler=handler
+            ))
+            if self.stop_on_handler_exceptions:
+                self.stop()
+
     async def _execute_scheduled(self, dt: datetime.datetime, job: SchedulerJob):
         logger.debug(logs.StructuredMessage("Executing scheduled job", scheduled=dt))
-        await await_no_raise(job(), message="Unhandled exception executing scheduled job")
+
+        try:
+            await job()
+        except Exception as e:
+            logger.exception(logs.StructuredMessage(
+                "Unhandled exception in handler", error=e, dt=dt, scheduler_job=job
+            ))
+            if self.stop_on_handler_exceptions:
+                self.stop()
 
 
 class BacktestingDispatcher(EventDispatcher):
     """Event dispatcher for backtesting.
 
     :param max_concurrent: The maximum number of events to process concurrently.
     """
@@ -312,28 +342,28 @@
         next_scheduled_dt = self._scheduler_queue.peek_next_event_dt()
         while next_scheduled_dt and next_scheduled_dt <= dt:
             # If self._last_dt is already set in the future, don't move it backwards in time.
             next_scheduled_dt, job = self._scheduler_queue.pop()
             if self._last_dt is None or next_scheduled_dt > self._last_dt:
                 self._last_dt = next_scheduled_dt
 
-            await self._task_pool.push(self._execute_scheduled(next_scheduled_dt, job))
+            await self._handlers_task_pool.push(self._execute_scheduled(next_scheduled_dt, job))
             # Waiting here and not outside of the loop to prevent executing distant scheduled jobs at the same time.
-            await self._task_pool.wait_all()
+            await self._handlers_task_pool.wait()
 
             next_scheduled_dt = self._scheduler_queue.peek_next_event_dt()
 
     async def _dispatch_events(self, dt: datetime.datetime):
         # Pop events, push them into the task pool, and wait those to finish executing.
         self._last_dt = dt
         for source, evnt in self._event_mux.pop_while(dt):
-            await self._task_pool.push(
+            await self._handlers_task_pool.push(
                 self._dispatch_event(EventDispatch(event=evnt, handlers=self._event_handlers.get(source, [])))
             )
-        await self._task_pool.wait_all()
+        await self._handlers_task_pool.wait()
 
 
 class RealtimeDispatcher(EventDispatcher):
     """Event dispatcher for live trading.
 
     :param max_concurrent: The maximum number of events to process concurrently.
     """
@@ -364,32 +394,32 @@
             now = dt.utc_now()
             # Feed the task pool with scheduled jobs and events that are ready for processing.
             await asyncio.gather(
                 self._push_scheduled(now),
                 self._push_events(now),
             )
             # Give some time for tasks to execute, and keep on pushing tasks.
-            idle = await self._task_pool.wait_all(timeout=self._wait_all_timeout)
-            if idle:
+            await self._handlers_task_pool.wait(timeout=self._wait_all_timeout)
+            if self._handlers_task_pool.idle:
                 await self._on_idle()
 
     async def _on_idle(self):
         if self._idle_handlers:
             await gather_no_raise(*[
-                self._task_pool.push(idle_handler()) for idle_handler in self._idle_handlers
+                self._handlers_task_pool.push(idle_handler()) for idle_handler in self._idle_handlers
             ])
         else:
             # Otherwise we'll monopolize the event loop.
             await asyncio.sleep(self.idle_sleep)
 
     async def _push_scheduled(self, dt: datetime.datetime):
         while (next_scheduled_dt := self._scheduler_queue.peek_next_event_dt()) and next_scheduled_dt <= dt:
             next_scheduled_dt, job = self._scheduler_queue.pop()
             # Push scheduled job into the task pool for processing.
-            await self._task_pool.push(self._execute_scheduled(next_scheduled_dt, job))
+            await self._handlers_task_pool.push(self._execute_scheduled(next_scheduled_dt, job))
 
     async def _push_events(self, dt: datetime.datetime):
         # Pop events and feed the pool.
         for source, evnt in self._event_mux.pop_while(dt):
             # Check that events from the same source are returned in order.
             prev_event_dt = self._prev_event_dt.get(source)
             if prev_event_dt is not None and evnt.when < prev_event_dt:
@@ -397,15 +427,15 @@
                     "Events returned out of order", source=type(source), previous=prev_event_dt, current=evnt.when
                 ))
                 # TODO: Not ignoring out-of-order events should be an option.
                 continue
             self._prev_event_dt[source] = evnt.when
 
             # Push event into the task pool for processing.
-            await self._task_pool.push(
+            await self._handlers_task_pool.push(
                 self._dispatch_event(EventDispatch(
                     event=evnt,
                     handlers=self._event_handlers.get(source, [])
                 ))
             )
```

### Comparing `basana-1.5.0/basana/core/dt.py` & `basana-1.5.1/basana/core/dt.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/enums.py` & `basana-1.5.1/basana/core/enums.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/event.py` & `basana-1.5.1/basana/core/event.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/event_sources/__init__.py` & `basana-1.5.1/basana/core/event_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/event_sources/trading_signal.py` & `basana-1.5.1/basana/core/event_sources/trading_signal.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/helpers.py` & `basana-1.5.1/basana/core/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -61,46 +61,75 @@
         return ret
 
     def cancel(self):
         self._cancel()
 
 
 class TaskPool:
+    """
+    A class for managing a pool of asyncio tasks.
+
+    :param size: The maximum size of the task pool.
+    """
     def __init__(self, size: int):
         assert size > 0, "Invalid size"
         self._max_size = size
         self._tasks: Set[asyncio.Task] = set()
+        self._done: List[asyncio.Task] = []
+
+    @property
+    def idle(self) -> int:
+        """
+        True if there are no active tasks in the pool, False otherwise.
+        """
+        return len(self._tasks) == 0
 
     async def push(self, coroutine: Coroutine[Any, Any, Any]):
+        """
+        Adds a coroutine to the task pool. If the pool is full it will block until there is room for the new task.
+
+        :param coroutine: The coroutine to be added to the task pool.
+        """
         # Wait for some task to complete if there is no more room.
         while len(self._tasks) >= self._max_size:
             await self._wait_impl(timeout=None, return_when=asyncio.FIRST_COMPLETED)
         self._tasks.add(asyncio.create_task(coroutine))
 
-    def cancel(self) -> List[asyncio.Task]:
+    def pop_done(self) -> List[asyncio.Task]:
+        """
+        Returns the tasks that are done running since the last call to pop_done.
+        """
+        ret = self._done
+        self._done = []
+        return ret
+
+    def cancel(self):
+        """
+        Requests all tasks in the pool to be canceled.
+        """
         pending = [task for task in self._tasks if not task.done()]
         for task in pending:
-            if not task.done():
-                task.cancel()
-        return pending
-
-    # async def wait_one(self, timeout: Optional[Union[int, float]] = None) -> bool:
-    #     if self._tasks:
-    #         await self._wait_impl(timeout=timeout, return_when=asyncio.FIRST_COMPLETED)
-    #     return not self._tasks
+            task.cancel()
 
-    async def wait_all(self, timeout: Optional[Union[int, float]] = None) -> bool:
-        if self._tasks:
-            await self._wait_impl(timeout=timeout, return_when=asyncio.ALL_COMPLETED)
-        return not self._tasks
+    async def wait(self, timeout: Optional[Union[int, float]] = None) -> bool:
+        """
+        Waits for all tasks in the pool to complete. Returns True if all tasks are done, False otherwise.
+
+        :param timeout: The maximum number of seconds to wait for tasks to complete. If None, wait indefinitely.
+        """
+        return await self._wait_impl(timeout=timeout, return_when=asyncio.ALL_COMPLETED)
 
-    async def _wait_impl(self, timeout: Optional[Union[int, float]], return_when: str):
-        done, _ = await asyncio.wait(self._tasks, timeout=timeout, return_when=return_when)
+    async def _wait_impl(self, timeout: Optional[Union[int, float]], return_when: str) -> bool:
+        done: List[asyncio.Task] = []
+        if self._tasks:
+            done, _ = await asyncio.wait(self._tasks, timeout=timeout, return_when=return_when)
         for task in done:
             self._tasks.remove(task)
+            self._done.append(task)
+        return len(done) > 0
 
 
 @contextlib.contextmanager
 def no_raise(logger: logging.Logger, msg: str, **kwargs):
     try:
         yield
     except Exception as e:
```

### Comparing `basana-1.5.0/basana/core/logs.py` & `basana-1.5.1/basana/core/logs.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/pair.py` & `basana-1.5.1/basana/core/pair.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/token_bucket.py` & `basana-1.5.1/basana/core/token_bucket.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/core/websockets.py` & `basana-1.5.1/basana/core/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/__init__.py` & `basana-1.5.1/basana/external/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/__init__.py` & `basana-1.5.1/basana/external/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/client/__init__.py` & `basana-1.5.1/basana/external/binance/client/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/client/base.py` & `basana-1.5.1/basana/external/binance/client/base.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/client/margin.py` & `basana-1.5.1/basana/external/binance/client/margin.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/client/spot.py` & `basana-1.5.1/basana/external/binance/client/spot.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/common.py` & `basana-1.5.1/basana/external/binance/common.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/config.py` & `basana-1.5.1/basana/external/binance/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/cross_margin.py` & `basana-1.5.1/basana/external/binance/cross_margin.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/csv/__init__.py` & `basana-1.5.1/basana/external/binance/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/csv/bars.py` & `basana-1.5.1/basana/external/binance/csv/bars.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from basana.core import pair
 from basana.core.event_sources import csv
 from basana.external.binance.tools.download_bars import period_to_step
 from basana.external.common.csv.bars import RowParser
 
 
 period_to_timedelta = {
-    period_str: datetime.timedelta(seconds=period_secs, microseconds=-1)
+    period_str: datetime.timedelta(seconds=period_secs)
     for period_str, period_secs in period_to_step.items()
 }
 
 
 class BarSource(csv.EventSource):
     def __init__(
             self, pair: pair.Pair, csv_path: str, period: str,
```

### Comparing `basana-1.5.0/basana/external/binance/exchange.py` & `basana-1.5.1/basana/external/binance/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/helpers.py` & `basana-1.5.1/basana/external/binance/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,12 +84,12 @@
     if price is not None:
         price = Decimal(price)
         ret = None if price == Decimal(0) and skip_zero else price
     return ret
 
 
 def timestamp_to_datetime(timestamp: int) -> datetime.datetime:
-    return datetime.datetime.utcfromtimestamp(timestamp / 1e3).replace(tzinfo=datetime.timezone.utc)
+    return datetime.datetime.fromtimestamp(timestamp / 1e3, tz=datetime.timezone.utc)
 
 
 def datetime_to_timestamp(datetime: datetime.datetime) -> int:
     return int(dt.to_utc_timestamp(datetime) * 1e3)
```

### Comparing `basana-1.5.0/basana/external/binance/isolated_margin.py` & `basana-1.5.1/basana/external/binance/isolated_margin.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/klines.py` & `basana-1.5.1/basana/external/binance/klines.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/margin.py` & `basana-1.5.1/basana/external/binance/margin.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/margin_requests.py` & `basana-1.5.1/basana/external/binance/margin_requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/order_book.py` & `basana-1.5.1/basana/external/binance/order_book.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/spot.py` & `basana-1.5.1/basana/external/binance/spot.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/spot_requests.py` & `basana-1.5.1/basana/external/binance/spot_requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/tools/__init__.py` & `basana-1.5.1/basana/external/binance/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/tools/download_bars.py` & `basana-1.5.1/basana/external/binance/tools/download_bars.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 import argparse
 import datetime
+import sys
 
 import aiohttp
 import asyncio
 
 from basana.core import dt, token_bucket
 from basana.external.binance import client, helpers
 
@@ -64,39 +65,43 @@
 
 def to_binance_currency_pair(currency_pair: str):
     parts = currency_pair.upper().split("/")
     return "".join(parts)
 
 
 class CSVWriter:
-    def __init__(self):
+    def __init__(self, output_file: Optional[str]):
         self._header_written = False
+        self._output_file = open(output_file, "w") if output_file else sys.stdout
 
     def write_candlestick(self, candlestick: Candlestick):
         if not self._header_written:
-            print("datetime,open,high,low,close,volume")
+            print("datetime,open,high,low,close,volume", file=self._output_file)
             self._header_written = True
+
+        dt_col = datetime.datetime.fromtimestamp(candlestick.open_timestamp / 1000, tz=datetime.timezone.utc)
         print(",".join([
-            str(datetime.datetime.utcfromtimestamp(candlestick.open_timestamp / 1000)),
+            str(dt_col.replace(tzinfo=None)),
             candlestick.open, candlestick.high, candlestick.low, candlestick.close, candlestick.volume
-        ]))
+        ]), file=self._output_file)
 
 
 async def main(params: Optional[List[str]] = None, config_overrides: dict = {}):
     parser = argparse.ArgumentParser()
     parser.add_argument("-c", "--currency-pair", help="The currency pair.", required=True)
     parser.add_argument(
         "-p", "--period", help="The period for the bars.", choices=period_to_step.keys(), required=True
     )
     parser.add_argument(
         "-s", "--start", help="The starting date YYYY-MM-DD format. Included in the range.", required=True
     )
     parser.add_argument(
         "-e", "--end", help="The ending date YYYY-MM-DD format. Included in the range.", required=True
     )
+    parser.add_argument("-o", "--output", help="The output file.", required=False, default=None)
     args = parser.parse_args(args=params)
 
     step = period_to_step[args.period]
     start = parse_date(args.start)
     end = parse_date(args.end)
     assert start <= end, "Invalid start/end"
     # start/end are set as dates so to get past the end we need to use a step >= 1 day.
@@ -104,15 +109,15 @@
 
     start_ts = helpers.datetime_to_timestamp(start)
     past_the_end_ts = helpers.datetime_to_timestamp(past_the_end)
     step = step * 1000
 
     tb = token_bucket.TokenBucketLimiter(10, 1)
     now_ts = helpers.datetime_to_timestamp(dt.utc_now())
-    writer = CSVWriter()
+    writer = CSVWriter(args.output)
     async with aiohttp.ClientSession() as session:
         cli = client.APIClient(session=session, tb=tb, config_overrides=config_overrides)
         eof = False
         currency_pair = to_binance_currency_pair(args.currency_pair)
         while not eof:
             response = await cli.get_candlestick_data(
                 currency_pair, args.period, start_time=start_ts, end_time=past_the_end_ts, limit=1000
```

### Comparing `basana-1.5.0/basana/external/binance/trades.py` & `basana-1.5.1/basana/external/binance/trades.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/binance/websockets.py` & `basana-1.5.1/basana/external/binance/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/__init__.py` & `basana-1.5.1/basana/external/bitstamp/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/client.py` & `basana-1.5.1/basana/external/bitstamp/client.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/config.py` & `basana-1.5.1/basana/external/bitstamp/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/csv/__init__.py` & `basana-1.5.1/basana/external/bitstamp/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/csv/bars.py` & `basana-1.5.1/basana/external/bitstamp/csv/bars.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from basana.core import pair
 from basana.core.event_sources import csv
 from basana.external.bitstamp.tools.download_bars import period_to_step
 from basana.external.common.csv.bars import RowParser
 
 
 period_to_timedelta = {
-    period_str: datetime.timedelta(seconds=period_secs, microseconds=-1)
+    period_str: datetime.timedelta(seconds=period_secs)
     for period_str, period_secs in period_to_step.items()
 }
 
 
 # TODO: Deprecate at v2.
 @enum.unique
 class BarPeriod(enum.Enum):
```

### Comparing `basana-1.5.0/basana/external/bitstamp/exchange.py` & `basana-1.5.1/basana/external/bitstamp/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/helpers.py` & `basana-1.5.1/basana/external/bitstamp/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/order_book.py` & `basana-1.5.1/basana/external/bitstamp/order_book.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.pair: Pair = pair
         #: The JSON representation.
         self.json: dict = json
 
     @property
     def datetime(self) -> datetime.datetime:
         timestamp = int(self.json["microtimestamp"]) / 1e6
-        return datetime.datetime.utcfromtimestamp(timestamp).replace(tzinfo=datetime.timezone.utc)
+        return datetime.datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc)
 
     @property
     def bids(self) -> List[Entry]:
         """Returns the top bid entries."""
         return [
             Entry(price=Decimal(entry[0]), volume=Decimal(entry[1])) for entry in self.json["bids"]
         ]
```

### Comparing `basana-1.5.0/basana/external/bitstamp/orders.py` & `basana-1.5.1/basana/external/bitstamp/orders.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/requests.py` & `basana-1.5.1/basana/external/bitstamp/requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/tools/__init__.py` & `basana-1.5.1/basana/external/bitstamp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/bitstamp/tools/download_bars.py` & `basana-1.5.1/basana/external/bitstamp/tools/download_bars.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 import argparse
 import datetime
+import sys
 
 import aiohttp
 import asyncio
 
 from basana.core import dt, token_bucket
 from basana.external.bitstamp import client
 
@@ -62,53 +63,57 @@
 
 def to_bitstamp_currency_pair(currency_pair: str):
     parts = currency_pair.lower().split("/")
     return "".join(parts)
 
 
 class CSVWriter:
-    def __init__(self):
+    def __init__(self, output_file: Optional[str]):
         self._header_written = False
+        self._output_file = open(output_file, "w") if output_file else sys.stdout
 
     def write_ohlc(self, ohlc: OHLC):
         if not self._header_written:
-            print("datetime,open,high,low,close,volume")
+            print("datetime,open,high,low,close,volume", file=self._output_file)
             self._header_written = True
+
+        dt_col = datetime.datetime.fromtimestamp(ohlc.open_timestamp, tz=datetime.timezone.utc)
         print(",".join([
-            str(datetime.datetime.utcfromtimestamp(ohlc.open_timestamp)),
+            str(dt_col.replace(tzinfo=None)),
             ohlc.open, ohlc.high, ohlc.low, ohlc.close, ohlc.volume
-        ]))
+        ]), file=self._output_file)
 
 
 async def main(params: Optional[List[str]] = None, config_overrides: dict = {}):
     parser = argparse.ArgumentParser()
     parser.add_argument("-c", "--currency-pair", help="The currency pair.", required=True)
     parser.add_argument(
         "-p", "--period", help="The period for the bars.", choices=period_to_step.keys(), required=True
     )
     parser.add_argument(
         "-s", "--start", help="The starting date YYYY-MM-DD format. Included in the range.", required=True
     )
     parser.add_argument(
         "-e", "--end", help="The ending date YYYY-MM-DD format. Included in the range.", required=True
     )
+    parser.add_argument("-o", "--output", help="The output file.", required=False, default=None)
     args = parser.parse_args(args=params)
 
     step = period_to_step[args.period]
     start = parse_date(args.start)
     end = parse_date(args.end)
     assert start <= end, "Invalid start/end"
     # start/end are set as dates so to get past the end we need to use a step >= 1 day.
     past_the_end = end + datetime.timedelta(seconds=max(period_to_step["1d"], step))
 
     start_ts = dt.to_utc_timestamp(start)
     past_the_end_ts = dt.to_utc_timestamp(past_the_end)
 
     tb = token_bucket.TokenBucketLimiter(10, 1)
-    writer = CSVWriter()
+    writer = CSVWriter(args.output)
     async with aiohttp.ClientSession() as session:
         cli = client.APIClient(session=session, tb=tb, config_overrides=config_overrides)
         eof = False
         currency_pair = to_bitstamp_currency_pair(args.currency_pair)
         while not eof:
             response = await cli.get_ohlc_data(currency_pair, step, 1000, start=start_ts, exclude_current_candle=True)
             eof = True
```

### Comparing `basana-1.5.0/basana/external/bitstamp/trades.py` & `basana-1.5.1/basana/external/bitstamp/trades.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """The trade id."""
         return str(self.json["id"])
 
     @property
     def datetime(self) -> datetime.datetime:
         """The datetime when the trade occurred."""
         timestamp = int(self.json["microtimestamp"]) / 1e6
-        return datetime.datetime.utcfromtimestamp(timestamp).replace(tzinfo=datetime.timezone.utc)
+        return datetime.datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc)
 
     @property
     def amount(self) -> Decimal:
         """The amount."""
         return Decimal(self.json["amount_str"])
 
     @property
```

### Comparing `basana-1.5.0/basana/external/bitstamp/websockets.py` & `basana-1.5.1/basana/external/bitstamp/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/common/__init__.py` & `basana-1.5.1/basana/external/common/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/common/csv/__init__.py` & `basana-1.5.1/basana/external/common/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/common/csv/bars.py` & `basana-1.5.1/basana/external/common/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/yahoo/__init__.py` & `basana-1.5.1/basana/external/yahoo/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.5.0/basana/external/yahoo/bars.py` & `basana-1.5.1/basana/external/yahoo/bars.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         high = close
     return open, high, low, close
 
 
 class RowParser(csv.RowParser):
     def __init__(
             self, pair: pair.Pair, adjust_ohlc: bool = False, tzinfo: datetime.tzinfo = tz.tzlocal(),
-            timedelta: datetime.timedelta = datetime.timedelta(hours=24, microseconds=-1)
+            timedelta: datetime.timedelta = datetime.timedelta(hours=24)
     ):
         self.pair = pair
         self.tzinfo = tzinfo
         self.timedelta = timedelta
         self.sanitize = False
         self.adjust_ohlc = adjust_ohlc
 
@@ -87,12 +87,12 @@
         ]
 
 
 class CSVBarSource(csv.EventSource):
     def __init__(
             self, pair: pair.Pair, csv_path: str, adjust_ohlc: bool = False, sort: bool = True,
             tzinfo: datetime.tzinfo = tz.tzlocal(),
-            timedelta: datetime.timedelta = datetime.timedelta(hours=24, microseconds=-1),
+            timedelta: datetime.timedelta = datetime.timedelta(hours=24),
             dict_reader_kwargs: dict = {}
     ):
         self.row_parser = RowParser(pair, adjust_ohlc=adjust_ohlc, tzinfo=tzinfo, timedelta=timedelta)
         super().__init__(csv_path, self.row_parser, sort=sort, dict_reader_kwargs=dict_reader_kwargs)
```

### Comparing `basana-1.5.0/pyproject.toml` & `basana-1.5.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basana"
-version = "1.5.0"
+version = "1.5.1"
 homepage = "https://github.com/gbeced/basana"
 repository = "https://github.com/gbeced/basana"
 documentation = "https://basana.readthedocs.io/en/latest/"
 description = "A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies."
 authors = ["Gabriel Becedillas <gabriel.becedillas@gmail.com>"]
 license = "Apache-2.0"
 packages = [{include = "basana"}]
@@ -18,22 +18,22 @@
 kaleido = {version = "0.2.1", optional = true}
 
 [tool.poetry.extras]
 charts = ["plotly", "kaleido"]
 
 [tool.poetry.group.dev.dependencies]
 aioresponses = "^0.7.4"
-flake8 = "^6.0.0"
-mypy = "^1.0.1"
-pytest = "^7.2.1"
+flake8 = "^7.0.0"
+mypy = "^1.9.0"
+pytest = "^8.1.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
-talipp = "^1.9.1"
+talipp = "^2.1.0"
 types-python-dateutil = "^2.8.19.8"
-websockets = "^10.4"
+websockets = "^12"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `basana-1.5.0/PKG-INFO` & `basana-1.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: basana
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies.
 Home-page: https://github.com/gbeced/basana
 License: Apache-2.0
 Author: Gabriel Becedillas
 Author-email: gabriel.becedillas@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: charts
 Requires-Dist: aiohttp[speedups] (>=3.8.6,<4.0.0)
 Requires-Dist: kaleido (==0.2.1) ; extra == "charts"
 Requires-Dist: plotly (>=5.14.1,<6.0.0) ; extra == "charts"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Documentation, https://basana.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/gbeced/basana
```

