# Comparing `tmp/pkscreener-0.44.20240422.285.tar.gz` & `tmp/pkscreener-0.44.20240422.286.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240422.285.tar", last modified: Mon Apr 22 12:28:08 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240422.286.tar", last modified: Mon Apr 22 22:15:58 2024, max compression
```

## Comparing `pkscreener-0.44.20240422.285.tar` & `pkscreener-0.44.20240422.286.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/
--rw-rw-rw-   0        0        0     1086 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.766025 pkscreener-0.44.20240422.285/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26011 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9925 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7038 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29415 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    18847 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   112580 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    49260 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79761 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-22 12:27:59.000000 pkscreener-0.44.20240422.285/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   121816 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    23583 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-22 12:28:08.766025 pkscreener-0.44.20240422.285/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-22 12:28:08.000000 pkscreener-0.44.20240422.285/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-22 12:28:08.781652 pkscreener-0.44.20240422.285/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-22 12:23:12.000000 pkscreener-0.44.20240422.285/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/
+-rw-rw-rw-   0        0        0     1086 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.359072 pkscreener-0.44.20240422.286/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26011 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9925 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7038 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    18737 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   112580 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    49099 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79894 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-22 22:15:51.000000 pkscreener-0.44.20240422.286/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   122052 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    23583 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:15:58.359072 pkscreener-0.44.20240422.286/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-22 22:15:58.000000 pkscreener-0.44.20240422.286/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-22 22:15:58.374098 pkscreener-0.44.20240422.286/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-22 22:10:38.000000 pkscreener-0.44.20240422.286/setup.py
```

### Comparing `pkscreener-0.44.20240422.285/LICENSE` & `pkscreener-0.44.20240422.286/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/LICENSE-Others` & `pkscreener-0.44.20240422.286/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/PKG-INFO` & `pkscreener-0.44.20240422.286/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240422.285
+Version: 0.44.20240422.286
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.285.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.286.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240422.285/README.md` & `pkscreener-0.44.20240422.286/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240422.285/pkscreener/__init__.py` & `pkscreener-0.44.20240422.286/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/PKScanRunner.py`

 * *Files 5% similar despite different names*

```diff
@@ -240,24 +240,20 @@
         choices = f"{choices}{'_i' if isIntraday else ''}"
         return choices
 
     def refreshDatabase():
         for worker in PKScanRunner.consumers:
             worker.refreshDatabase = True
             
-    def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDict,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb):
-        if PKScanRunner.tasks_queue is None or \
-            PKScanRunner.results_queue is None or \
-            PKScanRunner.scr is None or \
-            PKScanRunner.consumers is None:
-            tasks_queue, results_queue, scr, consumers = PKScanRunner.prepareToRunScan(keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDict, items)
-            PKScanRunner.tasks_queue = tasks_queue
-            PKScanRunner.results_queue = results_queue
-            PKScanRunner.scr = scr
-            PKScanRunner.consumers = consumers
+    def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDict,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb,tasks_queue, results_queue, consumers):
+        if tasks_queue is None or results_queue is None or consumers is None:
+            tasks_queue, results_queue, consumers = PKScanRunner.prepareToRunScan(keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDict, items)
+        PKScanRunner.tasks_queue = tasks_queue
+        PKScanRunner.results_queue = results_queue
+        PKScanRunner.consumers = consumers
         screenResults, saveResults, backtest_df = scanningCb(
                     menuOption,
                     items,
                     PKScanRunner.tasks_queue,
                     PKScanRunner.results_queue,
                     len(items),
                     backtestPeriod,
@@ -268,15 +264,15 @@
                     backtest_df,
                     testing=testing,
                 )
 
         OutputControls().printOutput(colorText.END)
         if userPassedArgs is not None and userPassedArgs.monitor is None:
             PKScanRunner.terminateAllWorkers(consumers, tasks_queue, testing)
-        return screenResults, saveResults,backtest_df,PKScanRunner.scr
+        return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers
 
     def prepareToRunScan(keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDict, items):
         tasks_queue, results_queue, totalConsumers = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
         consumers = [
                     PKMultiProcessorClient(
@@ -294,15 +290,15 @@
                         PKScanRunner.configManager,
                         PKScanRunner.candlePatterns,
                         scr,
                     )
                     for _ in range(totalConsumers)
                 ]
         PKScanRunner.startWorkers(consumers)
-        return tasks_queue,results_queue,scr,consumers
+        return tasks_queue,results_queue,consumers
     
     def startWorkers(consumers):
         try:
             from pytest_cov.embed import cleanup_on_signal, cleanup_on_sigterm
         except ImportError:
             pass
         else:
```

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         logLevel=logging.NOTSET,
         portfolio=False,
         testData = None,
         hostRef=None,
     ):
         assert (
             hostRef is not None
-        ), "hostRef argument must not be None. It should b an instance of PKMultiProcessorClient"
+        ), "hostRef argument must not be None. It should be an instance of PKMultiProcessorClient"
         configManager = hostRef.configManager
         self.configManager = configManager
         screeningDictionary, saveDictionary = self.initResultDictionaries()
         fullData = None
         processedData = None
         fetcher = hostRef.fetcher
         screener = hostRef.screener
@@ -131,17 +131,14 @@
                     processedData = processedData.head(len(intraday_processedData))
                     intraday_processedData = intraday_processedData.head(len(processedData))
                     data = data.tail(len(intraday_data))
                     intraday_data = intraday_data.tail(len(data))
                     # Indexes won't match. Hence, we'd need to fallback on tolist
                     processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
                     fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
-                else:
-                    processedData.loc[:,"RSIi"] = [0]*len(processedData)
-                    fullData.loc[:,"RSIi"] = [0]*len(fullData)
 
             def returnLegibleData():
                 if backtestDuration == 0 or menuOption not in ["B"]:
                     return None
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
                     screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
@@ -855,15 +852,15 @@
                 hostRef.default_logger.debug(e, exc_info=True)
                 pass
             sys.stdout.write("\r\033[K")
     
     def setupLoggers(self, hostRef, screener, logLevel, stock):
         # Set the loglevels for both the caller and screener
         # Also add handlers that are specific to this sub-process which
-        # will co ntinue with the screening. Each sub-process would have
+        # will continue with the screening. Each sub-process would have
         # its own logger but going into the same file/console > to that
         # of the parent logger.
         if hostRef.default_logger.level > 0:
             return
         else:
             hostRef.default_logger.info(f"Beginning the stock screening for stock:{stock}")
         hostRef.default_logger.level = logLevel
```

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -809,15 +809,15 @@
             task = PKTask(f"DataDownload-{queueCounter}",long_running_fn=fetcher.fetchStockDataWithArgs,long_running_fn_args=fn_args)
             task.userData = stocks
             if len(stocks) > 0:
                 tasksList.append(task)
             queueCounter += 1
         
         if len(tasksList) > 0:
-            PKScheduler.scheduleTasks(tasksList=tasksList, label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",timeout=10,minAcceptableCompletionPercentage=80)
+            PKScheduler.scheduleTasks(tasksList=tasksList, label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",timeout=3*configManager.longTimeout,minAcceptableCompletionPercentage=80)
             for task in tasksList:
                 if task.result is not None:
                     for stock in task.userData:
                         taskResult = task.result.get(f"{stock}{exchangeSuffix}")
                         if taskResult is not None:
                             stockDict[stock] = taskResult.to_dict("split")
         return stockDict
@@ -1063,14 +1063,15 @@
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Cache unavailable on pkscreener server, Continuing.."
                 + colorText.END
             )
         # See if we need to save stock data
+        stockDataLoaded = stockDataLoaded or (len(stockDict) > 0 and (len(stockDict) != initialLoadCount))
         if stockDataLoaded:
             tools.saveStockData(stockDict,configManager,initialLoadCount,isIntraday,downloadOnly, forceSave=stockDataLoaded)
         return stockDict
 
     # Save screened results to excel
     def promptSaveResults(df, defaultAnswer=None):
         """
```

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/classes/keys.py` & `pkscreener-0.44.20240422.286/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/courbd.ttf` & `pkscreener-0.44.20240422.286/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/globals.py` & `pkscreener-0.44.20240422.286/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,17 @@
 stockDict = None
 userPassedArgs = None
 elapsed_time = 0
 start_time = 0
 test_messages_queue = []
 strategyFilter=[]
 listStockCodes = None
+tasks_queue = None
+results_queue = None
+consumers = None
 
 def finishScreening(
     downloadOnly,
     testing,
     stockDict,
     configManager,
     loadCount,
@@ -1186,21 +1189,22 @@
                     )
                 fillerPlaceHolder = fillerPlaceHolder + 1
                 actualHistoricalDuration = samplingDuration - fillerPlaceHolder
                 if actualHistoricalDuration >= 0:
                     progressbar()
         sys.stdout.write(f"\x1b[1A") # Replace the download progress bar and start writing on the same line
         if not keyboardInterruptEventFired:
-            screenResults, saveResults, backtest_df, scr = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDict,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners)
+            global tasks_queue, results_queue, consumers
+            screenResults, saveResults, backtest_df, tasks_queue, results_queue, consumers = PKScanRunner.runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDict,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb=runScanners,tasks_queue=tasks_queue, results_queue=results_queue, consumers=consumers)
             if menuOption in ["C"]:
                 runOptionName = PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)
                 PKMarketOpenCloseAnalyser.runOpenCloseAnalysis(stockDict,endOfdayCandles,screenResults, saveResults,runOptionName=runOptionName)
             if downloadOnly and menuOption in ["X"]:
-                scr.getFreshMFIStatus(stock="LatestCheckedOnDate")
-                scr.getFairValue(stock="LatestCheckedOnDate", force=True)
+                screener.getFreshMFIStatus(stock="LatestCheckedOnDate")
+                screener.getFairValue(stock="LatestCheckedOnDate", force=True)
             if not downloadOnly and menuOption in ["X", "G", "C"]:
                 if menuOption == "G":
                     userPassedArgs.backtestdaysago = backtestPeriod
                 if screenResults is not None and len(screenResults) > 0:
                     screenResults, saveResults = labelDataForPrinting(
                         screenResults, saveResults, configManager, volumeRatio, executeOption, reversalOption or respChartPattern
                     )
```

### Comparing `pkscreener-0.44.20240422.285/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240422.286/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240422.286/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240422.286/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240422.286/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240422.285
+Version: 0.44.20240422.286
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.285.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240422.286.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.284/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240422.285/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240422.285/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240422.286/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240422.285/setup.py` & `pkscreener-0.44.20240422.286/setup.py`

 * *Files identical despite different names*

