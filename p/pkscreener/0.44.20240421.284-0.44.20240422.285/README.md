# Comparing `tmp/pkscreener-0.44.20240421.284.tar.gz` & `tmp/pkscreener-0.44.20240422.285.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240421.284.tar", last modified: Sun Apr 21 23:29:50 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240422.285.tar", last modified: Mon Apr 22 12:28:08 2024, max compression
```

## Comparing `pkscreener-0.44.20240421.284.tar` & `pkscreener-0.44.20240422.285.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 23:29:50.671437 pkscreener-0.44.20240421.284/
--rw-rw-rw-   0        0        0     1086 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-21 23:29:50.671437 pkscreener-0.44.20240421.284/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 23:29:50.655821 pkscreener-0.44.20240421.284/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 23:29:50.671437 pkscreener-0.44.20240421.284/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25172 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9489 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7038 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29415 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    18689 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   112347 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    48164 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79711 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-21 23:29:43.000000 pkscreener-0.44.20240421.284/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   121785 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    23455 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-21 23:29:50.655821 pkscreener-0.44.20240421.284/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-21 23:29:50.000000 pkscreener-0.44.20240421.284/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-21 23:29:50.000000 pkscreener-0.44.20240421.284/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 23:29:50.000000 pkscreener-0.44.20240421.284/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-21 23:29:50.000000 pkscreener-0.44.20240421.284/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-21 23:29:50.000000 pkscreener-0.44.20240421.284/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-21 23:29:50.000000 pkscreener-0.44.20240421.284/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-21 23:29:50.671437 pkscreener-0.44.20240421.284/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-21 23:25:40.000000 pkscreener-0.44.20240421.284/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/
+-rw-rw-rw-   0        0        0     1086 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.766025 pkscreener-0.44.20240422.285/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26011 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9925 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7038 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    18847 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   112580 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    49260 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79761 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-22 12:27:59.000000 pkscreener-0.44.20240422.285/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   121816 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    23583 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.766025 pkscreener-0.44.20240422.285/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/setup.py
```

### Comparing `pkscreener-0.44.20240421.284/LICENSE` & `pkscreener-0.44.20240422.285/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/LICENSE-Others` & `pkscreener-0.44.20240422.285/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/PKG-INFO` & `pkscreener-0.44.20240422.285/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240421.284
+Version: 0.44.20240422.285
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.284.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.285.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240421.284/README.md` & `pkscreener-0.44.20240422.285/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/__init__.py` & `pkscreener-0.44.20240422.285/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/ConfigManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,17 @@
         self.logger = None
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 6
+        self.calculatersiintraday = False
         self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:50,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10,X:12:12:i 1m,X:12:12:i 5m,X:12:13:i 1m"
+        #"X:12:9:2.5,|X:0:5:0:50,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10,X:12:12:i 1m,X:12:12:i 5m,X:12:13:i 1m"
 
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
@@ -152,14 +154,15 @@
             parser.set("config", "useEMA", "y" if self.useEMA else "n")
             parser.set(
                 "config", "showunknowntrends", "y" if self.showunknowntrends else "n"
             )
             parser.set("config", "logsEnabled", "y" if self.logsEnabled else "n")
             parser.set("config", "enablePortfolioCalculations", "y" if self.enablePortfolioCalculations else "n")
             parser.set("config", "showPastStrategyData", "y" if self.showPastStrategyData else "n")
+            parser.set("config", "calculatersiintraday", "y" if self.calculatersiintraday else "n")
             parser.set("config", "generalTimeout", str(self.generalTimeout))
             parser.set("config", "defaultIndex", str(self.defaultIndex))
             parser.set("config", "longTimeout", str(self.longTimeout))
             parser.set("config", "maxNetworkRetryCount", str(self.maxNetworkRetryCount))
             parser.set("config", "backtestPeriod", str(self.backtestPeriod))
             parser.set("config", "maxBacktestWindow", str(self.maxBacktestWindow))
             parser.set("config", "morninganalysiscandlenumber", str(self.morninganalysiscandlenumber))
@@ -256,14 +259,19 @@
                 )
             ).lower()
             self.showPastStrategyData = str(
                 input(
                     "[+] Enable showing past strategy data? [Y/N]: "
                 )
             ).lower()
+            self.calculatersiintraday = str(
+                input(
+                    "[+] Calculate intraday RSI during trading hours? [Y/N]: "
+                )
+            ).lower()
             self.generalTimeout = input(
                 "[+] General network timeout (in seconds)(Optimal = 2 for good networks): "
             )
             self.longTimeout = input(
                 "[+] Long network timeout for heavier downloads(in seconds)(Optimal = 4 for good networks): "
             )
             self.maxNetworkRetryCount = input(
@@ -302,14 +310,15 @@
             parser.set("config", "shuffle", self.shuffle)
             parser.set("config", "cacheStockData", self.cacheStockData)
             parser.set("config", "onlyStageTwoStocks", self.stageTwoPrompt)
             parser.set("config", "useEMA", self.useEmaPrompt)
             parser.set("config", "showunknowntrends", self.showunknowntrendsPrompt)
             parser.set("config", "enablePortfolioCalculations", self.enablePortfolioCalculations)
             parser.set("config", "showPastStrategyData", self.showPastStrategyData)
+            parser.set("config", "calculatersiintraday", self.calculatersiintraday)
             parser.set("config", "logsEnabled", self.logsEnabledPrompt)
             parser.set("config", "generalTimeout", self.generalTimeout)
             parser.set("config", "defaultIndex", self.defaultIndex)
             parser.set("config", "longTimeout", self.longTimeout)
             parser.set("config", "maxNetworkRetryCount", self.maxNetworkRetryCount)
             parser.set("config", "backtestPeriod", self.backtestPeriod)
             parser.set("config", "maxBacktestWindow", self.maxBacktestWindow)
@@ -399,14 +408,19 @@
                     else True
                 )
                 self.showPastStrategyData = (
                     False
                     if "y" not in str(parser.get("config", "showPastStrategyData")).lower()
                     else True
                 )
+                self.calculatersiintraday = (
+                    False
+                    if "y" not in str(parser.get("config", "calculatersiintraday")).lower()
+                    else True
+                )
                 self.generalTimeout = float(parser.get("config", "generalTimeout"))
                 self.defaultIndex = int(parser.get("config", "defaultIndex"))
                 self.longTimeout = float(parser.get("config", "longTimeout"))
                 self.maxNetworkRetryCount = int(
                     parser.get("config", "maxNetworkRetryCount")
                 )
                 self.backtestPeriod = int(parser.get("config", "backtestPeriod"))
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/Fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import warnings
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 import yfinance as yf
 from concurrent.futures import ThreadPoolExecutor
+from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.Fetcher import StockDataEmptyException
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.SuppressOutput import SuppressOutput
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
 from pkscreener.classes.PKTask import PKTask
 from PKDevTools.classes.OutputControls import OutputControls
@@ -92,14 +93,20 @@
     ):
         if isinstance(stockCode,list):
             if len(exchangeSuffix) > 0:
                 stockCode = [(f"{x}{exchangeSuffix}" if not x.endswith(exchangeSuffix) else x) for x in stockCode]
         elif isinstance(stockCode,str):
             if len(exchangeSuffix) > 0:
                 stockCode = f"{stockCode}{exchangeSuffix}" if not stockCode.endswith(exchangeSuffix) else stockCode
+        if (period == '1d' or duration[-1] == "m"):
+            # Since this is intraday data, we'd just need to start from the last trading session
+            if start is None:
+                start = PKDateUtilities.nthPastTradingDateStringFromFutureDate(1)
+            if end is None:
+                end = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
         with SuppressOutput(suppress_stdout=True, suppress_stderr=True):
             data = yf.download(
                 tickers=stockCode,
                 period=period,
                 interval=duration,
                 proxy=proxyServer,
                 progress=False,
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/PKScanRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from PKDevTools.classes.PKGitFolderDownloader import downloadFolder
 from PKDevTools.classes.PKMultiProcessorClient import PKMultiProcessorClient
 
 from pkscreener.classes.StockScreener import StockScreener
 from pkscreener.classes.CandlePatterns import CandlePatterns
 from pkscreener.classes.ConfigManager import parser, tools
 from PKDevTools.classes.OutputControls import OutputControls
+# from PKDevTools.classes.PKJoinableQueue import PKJoinableQueue
 
 import pkscreener.classes.Fetcher as Fetcher
 import pkscreener.classes.ScreeningStatistics as ScreeningStatistics
 import pkscreener.classes.Utility as Utility
 
 class PKScanRunner:
     configManager = tools()
@@ -102,14 +103,15 @@
         if totalConsumers == 1:
             totalConsumers = 2  # This is required for single core machine
         if PKScanRunner.configManager.cacheEnabled is True and multiprocessing.cpu_count() > 2:
             totalConsumers -= 1
         return tasks_queue, results_queue, totalConsumers
 
     def populateQueues(items, tasks_queue, exit=False):
+        # default_logger().debug(f"Unfinished items in task_queue: {tasks_queue.qsize()}")
         for item in items:
             tasks_queue.put(item)
         if exit:
             # Append exit signal for each process indicated by None
             for _ in range(multiprocessing.cpu_count()):
                 tasks_queue.put(None)
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,14 +699,16 @@
         ts = diff_df.tail(len(diff_df)-index +1).head(1).index[-1]
         return ts, df[df.index == ts] #df.head(len(df) -index +1).tail(1)
     
     # Find stock showing RSI crossing with RSI 9 SMA
     def findRSICrossingMA(self, df, screenDict, saveDict,lookFor=1, maLength=9, rsiKey="RSI"):
         if df is None or len(df) == 0:
             return False
+        if rsiKey not in df.columns:
+            return False
         data = df.copy()
         data = data[::-1]
         maRsi = pktalib.MA(data[rsiKey], timeperiod=maLength)
         data = data[::-1].head(3)
         maRsi = maRsi[::-1].head(3)
         saved = self.findCurrentSavedValue(screenDict,saveDict,"Trend")
         if lookFor in [1,3] and maRsi.iloc[0] <= data[rsiKey].iloc[0] and maRsi.iloc[1] > data[rsiKey].iloc[1]:
@@ -719,14 +721,16 @@
             return True if (rsiKey == "RSIi") else (self.findRSICrossingMA(df, screenDict, saveDict,lookFor=lookFor, maLength=maLength, rsiKey="RSIi") or True)
         return False if (rsiKey == "RSIi") else (self.findRSICrossingMA(df, screenDict, saveDict,lookFor=lookFor, maLength=maLength, rsiKey="RSIi"))
     
     # Find stocks with rising RSI from lower levels
     def findRisingRSI(self, df, rsiKey="RSI"):
         if df is None or len(df) == 0:
             return False
+        if rsiKey not in df.columns:
+            return False
         data = df.copy()
         data = data[::-1]
         data = data.tail(3)
         dayMinus2RSI = data["RSI"].iloc[0]
         dayMinus1RSI = data["RSI"].iloc[1]
         dayRSI = data["RSI"].iloc[2]
         returnValue = (dayMinus2RSI <= 35 and dayMinus1RSI > dayMinus2RSI and dayRSI > dayMinus1RSI) or \
@@ -1339,15 +1343,15 @@
         return result_df[::-1]
 
     # Preprocess the acquired data
     def preprocessData(self, df, daysToLookback=None):
         assert isinstance(df, pd.DataFrame)
         data = df.copy()
         data = data.replace(np.inf, np.nan).replace(-np.inf, np.nan).dropna(how="all")
-        self.default_logger.info(f"Preprocessing data:\n{data.head(1)}\n")
+        # self.default_logger.info(f"Preprocessing data:\n{data.head(1)}\n")
         if daysToLookback is None:
             daysToLookback = self.configManager.daysToLookback
         if self.configManager.useEMA:
             sma = pktalib.EMA(data["Close"], timeperiod=50)
             lma = pktalib.EMA(data["Close"], timeperiod=200)
             ssma = pktalib.EMA(data["Close"], timeperiod=9)
             data.insert(len(data.columns), "SMA", sma)
@@ -1362,20 +1366,22 @@
             data.insert(len(data.columns), "SSMA", ssma)
         vol = pktalib.SMA(data["Volume"], timeperiod=20)
         rsi = pktalib.RSI(data["Close"], timeperiod=14)
         data.insert(len(data.columns), "VolMA", vol)
         data.insert(len(data.columns), "RSI", rsi)
         cci = pktalib.CCI(data["High"], data["Low"], data["Close"], timeperiod=14)
         data.insert(len(data.columns), "CCI", cci)
-        # len(data["Close"])
-        fastk, fastd = pktalib.STOCHRSI(
-            data["Close"], timeperiod=14, fastk_period=5, fastd_period=3, fastd_matype=0
-        )
-        data.insert(len(data.columns), "FASTK", fastk)
-        data.insert(len(data.columns), "FASTD", fastd)
+        try:
+            fastk, fastd = pktalib.STOCHRSI(
+                data["Close"], timeperiod=14, fastk_period=5, fastd_period=3, fastd_matype=0
+            )
+            data.insert(len(data.columns), "FASTK", fastk)
+            data.insert(len(data.columns), "FASTD", fastd)
+        except:
+            pass
         data = data[::-1]  # Reverse the dataframe
         # data = data.fillna(0)
         # data = data.replace([np.inf, -np.inf], 0)
         fullData = data
         trimmedData = data.head(daysToLookback)
         return (fullData, trimmedData)
 
@@ -2132,14 +2138,16 @@
         return False
 
     #@measure_time
     # validate if RSI is within given range
     def validateRSI(self, df, screenDict, saveDict, minRSI, maxRSI,rsiKey="RSI"):
         if df is None or len(df) == 0:
             return False
+        if rsiKey not in df.columns:
+            return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         rsi = int(data.head(1)[rsiKey].iloc[0])
         saveDict[rsiKey] = rsi
         # https://chartink.com/screener/rsi-screening
         if rsi> 0 and rsi >= minRSI and rsi <= maxRSI:  # or (rsi <= 71 and rsi >= 67):
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,39 +98,50 @@
                 hostRef.processingCounter.value += 1
 
             volumeRatio, period = self.determineBasicConfigs(stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog)
             # hostRef.default_logger.info(
             #     f"For stock:{stock}, stock exists in objectDictionary:{hostRef.objectDictionary.get(stock)}, cacheEnabled:{configManager.cacheEnabled}, isTradingTime:{self.isTradingTime}, downloadOnly:{downloadOnly}"
             # )
             data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,hostRef.objectDictionary, configManager, fetcher, period, testData,exchangeName)
-            if not configManager.isIntradayConfig():
+            if not configManager.isIntradayConfig() and configManager.calculatersiintraday:
+                # Daily data is already available in "data" above.
+                # We need the intraday data for 1-d RSI values when config is not for intraday
                 intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.secondaryObjectDictionary, configManager, fetcher, period, testData,exchangeName)
+                # if intraday_data is not None:
+                #     if len(intraday_data) == 0:
+                #         return None
+                # else:
+                #     return None
             else:
                 intraday_data = data
             if data is not None:
                 if len(data) == 0 or len(data) < backtestDuration:
                     return None
             else:
                 return None
             # hostRef.default_logger.info(f"Will pre-process data:\n{data.tail(10)}")
             fullData, processedData, data = self.getCleanedDataForDuration(backtestDuration, portfolio, screeningDictionary, saveDictionary, configManager, screener, data)
-            if backtestDuration == 0:
-                intraday_fullData, intraday_processedData = screener.preprocessData(
-                    intraday_data, daysToLookback=configManager.effectiveDaysToLookback
-                )
-                # Match the index length and values length
-                fullData = fullData.head(len(intraday_fullData))
-                intraday_fullData = intraday_fullData.head(len(fullData))
-                processedData = processedData.head(len(intraday_processedData))
-                intraday_processedData = intraday_processedData.head(len(processedData))
-                data = data.tail(len(intraday_data))
-                intraday_data = intraday_data.tail(len(data))
-                # Indexes won't match. Hence, we'd need to fallback on tolist
-                processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
-                fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
+            if backtestDuration == 0 and configManager.calculatersiintraday:
+                if (intraday_data is not None and not intraday_data.empty):
+                    intraday_fullData, intraday_processedData = screener.preprocessData(
+                        intraday_data, daysToLookback=configManager.effectiveDaysToLookback
+                    )
+                    # Match the index length and values length
+                    fullData = fullData.head(len(intraday_fullData))
+                    intraday_fullData = intraday_fullData.head(len(fullData))
+                    processedData = processedData.head(len(intraday_processedData))
+                    intraday_processedData = intraday_processedData.head(len(processedData))
+                    data = data.tail(len(intraday_data))
+                    intraday_data = intraday_data.tail(len(data))
+                    # Indexes won't match. Hence, we'd need to fallback on tolist
+                    processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
+                    fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
+                else:
+                    processedData.loc[:,"RSIi"] = [0]*len(processedData)
+                    fullData.loc[:,"RSIi"] = [0]*len(fullData)
 
             def returnLegibleData():
                 if backtestDuration == 0 or menuOption not in ["B"]:
                     return None
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
                     screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
@@ -711,20 +722,24 @@
                 fullData, processedData = screener.preprocessData(
                         inputData, daysToLookback=configManager.daysToLookback
                     )
                 
         return fullData,processedData,data
 
     def getRelevantDataForStock(self, totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,objectDictionary, configManager, fetcher, period, testData=None,exchangeName="INDIA"):
-        hostData = objectDictionary.get(stock)
+        hostData = objectDictionary.get(stock) if (objectDictionary is not None and len(objectDictionary) > 0) else None
         data = None
         start = None
-        if (period == '1d' or configManager.duration[-1] == "m") and backtestDuration > 0:
-            start = PKDateUtilities.nthPastTradingDateStringFromFutureDate(backtestDuration)
-            end = start
+        if (period == '1d' or configManager.duration[-1] == "m"):
+            if backtestDuration > 0: # We are backtesting
+                start = PKDateUtilities.nthPastTradingDateStringFromFutureDate(backtestDuration)
+            else:
+                # Since this is intraday data, we'd just need to start from the last trading session
+                start = PKDateUtilities.nthPastTradingDateStringFromFutureDate(1)
+            end = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
         if (
                 not shouldCache
                 or (downloadOnly and hostData is None)
                 or (hostData is None and self.isTradingTime)
                 or hostData is None
             ):
             if testData is not None:
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -809,15 +809,15 @@
             task = PKTask(f"DataDownload-{queueCounter}",long_running_fn=fetcher.fetchStockDataWithArgs,long_running_fn_args=fn_args)
             task.userData = stocks
             if len(stocks) > 0:
                 tasksList.append(task)
             queueCounter += 1
         
         if len(tasksList) > 0:
-            PKScheduler.scheduleTasks(tasksList=tasksList, label=f"Downloading latest data (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",timeout=10,minAcceptableCompletionPercentage=80)
+            PKScheduler.scheduleTasks(tasksList=tasksList, label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",timeout=10,minAcceptableCompletionPercentage=80)
             for task in tasksList:
                 if task.result is not None:
                     for stock in task.userData:
                         taskResult = task.result.get(f"{stock}{exchangeSuffix}")
                         if taskResult is not None:
                             stockDict[stock] = taskResult.to_dict("split")
         return stockDict
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/classes/keys.py` & `pkscreener-0.44.20240422.285/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/courbd.ttf` & `pkscreener-0.44.20240422.285/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/globals.py` & `pkscreener-0.44.20240422.285/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1361,18 +1361,18 @@
                     configManager,
                     downloadOnly=downloadOnly,
                     defaultAnswer=defaultAnswer,
                     forceLoad=(menuOption in ["X", "B", "G", "S"]),
                     stockCodes = listStockCodes,
                     exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
             )
-    if not configManager.isIntradayConfig():
+    if not configManager.isIntradayConfig() and configManager.calculatersiintraday:
         candleDuration = (userPassedArgs.intraday if (userPassedArgs is not None and userPassedArgs.intraday is not None) else "1m")
         configManager.toggleConfig(candleDuration=candleDuration,clearCache=False)
-                # We also need to load the intraday data to be able to calculate intraday RSI
+        # We also need to load the intraday data to be able to calculate intraday RSI
         Utility.tools.loadStockData(
                         {},
                         configManager,
                         downloadOnly=downloadOnly,
                         defaultAnswer=defaultAnswer,
                         forceLoad=(menuOption in ["X", "B", "G", "S"]),
                         stockCodes = listStockCodes,
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240422.285/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240422.285/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,15 +313,14 @@
             try:
                 optionalFinalOutcome_df,_ = main(userArgs=args,optionalFinalOutcome_df=optionalFinalOutcome_df)
                 if isInterrupted():
                     break
             except Exception as e:
                 OutputControls().printOutput(e)
                 if args.log:
-                    import traceback
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
             final_df = None
             df_grouped = optionalFinalOutcome_df.groupby("Stock")
             for stock, df_group in df_grouped:
                 if stock == "PORTFOLIO":
                     if final_df is None:
@@ -354,14 +353,15 @@
                                 )
     else:
         if args.barometer:
             sendGlobalMarketBarometer(userArgs=args)
         else:
             global results, resultStocks, plainResults, dbTimestamp, elapsed_time, start_time
             monitorOption_org = ""
+            # args.monitor = configManager.defaultMonitorOptions
             if args.monitor:
                 args.answerdefault = args.answerdefault or 'Y'
                 if MarketMonitor().monitorIndex == 0:
                     dbTimestamp = PKDateUtilities.currentDateTime().strftime("%H:%M:%S")
                     elapsed_time = 0
                     if start_time is None:
                         start_time = time.time()
@@ -386,24 +386,25 @@
                 if monitorOption.startswith("|"):
                     monitorOption = monitorOption.replace("|","")
                     # We need to pipe the output from previous run into the next one
                     if resultStocks is not None:
                         resultStocks = ",".join(resultStocks)
                         monitorOption = f"{monitorOption}:{resultStocks}"
                 args.options = monitorOption
-            try:
+            try: 
                 results = None
                 plainResults = None
                 resultStocks = None
                 results, plainResults = main(userArgs=args)
                 if isInterrupted():
                     sys.exit(0)
             except SystemExit:
                 sys.exit(0)
             except Exception:
+                # traceback.print_exc()
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 resultStocks = plainResults.index
             if results is not None and args.monitor and len(monitorOption_org) > 0:
                 MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s")
 
@@ -422,14 +423,15 @@
                 traceback.print_exc()
             pass
 
         OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
         
     configManager.getConfig(ConfigManager.parser)
     # configManager.restartRequestsCache()
+    # args.monitor = configManager.defaultMonitorOptions
     if args.monitor is not None:
         MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","),maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow)
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
         if not args.prodbuild and args.answerdefault is None:
             input("Press <Enter> to continue...")
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240422.285/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240421.284
+Version: 0.44.20240422.285
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.284.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.285.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.283/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240421.284/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240422.285/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.284/setup.py` & `pkscreener-0.44.20240422.285/setup.py`

 * *Files identical despite different names*

