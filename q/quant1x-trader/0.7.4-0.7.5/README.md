# Comparing `tmp/quant1x-trader-0.7.4.tar.gz` & `tmp/quant1x-trader-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant1x-trader-0.7.4.tar", last modified: Mon Mar 18 03:34:24 2024, max compression
+gzip compressed data, was "quant1x-trader-0.7.5.tar", last modified: Mon Apr 22 05:09:42 2024, max compression
```

## Comparing `quant1x-trader-0.7.4.tar` & `quant1x-trader-0.7.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 03:34:24.429702 quant1x-trader-0.7.4/
--rw-rw-rw-   0        0        0     1087 2023-11-13 03:59:57.000000 quant1x-trader-0.7.4/LICENSE
--rw-rw-rw-   0        0        0     1342 2024-03-18 03:34:24.428703 quant1x-trader-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-12-07 15:33:00.000000 quant1x-trader-0.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 03:34:24.428703 quant1x-trader-0.7.4/quant1x_trader.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      290 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 03:34:24.429702 quant1x-trader-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0     2284 2024-01-21 09:52:15.000000 quant1x-trader-0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 03:34:24.426701 quant1x-trader-0.7.4/trader1x/
--rw-rw-rw-   0        0        0      103 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/__init__.py
--rw-rw-rw-   0        0        0      197 2023-12-11 07:07:15.000000 quant1x-trader-0.7.4/trader1x/__main__.py
--rw-rw-rw-   0        0        0    16143 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/auto.py
--rw-rw-rw-   0        0        0     8648 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/config.py
--rw-rw-rw-   0        0        0     7922 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/context.py
--rw-rw-rw-   0        0        0     1193 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/log4py.py
--rw-rw-rw-   0        0        0    18538 2024-03-18 03:34:16.000000 quant1x-trader-0.7.4/trader1x/proxy.py
--rw-rw-rw-   0        0        0     1266 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/qmt.py
--rw-rw-rw-   0        0        0    19739 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/thinktrader.py
--rw-rw-rw-   0        0        0     1368 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/utils.py
--rw-rw-rw-   0        0        0    38933 2024-01-21 09:52:15.000000 quant1x-trader-0.7.4/trader1x/win32serviceutil.py
+drwxrwxrwx   0        0        0        0 2024-04-22 05:09:42.142083 quant1x-trader-0.7.5/
+-rw-rw-rw-   0        0        0     1087 2023-11-13 03:59:57.000000 quant1x-trader-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0     1342 2024-04-22 05:09:42.141084 quant1x-trader-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-12-07 15:33:00.000000 quant1x-trader-0.7.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 05:09:42.140087 quant1x-trader-0.7.5/quant1x_trader.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-04-22 05:09:42.000000 quant1x-trader-0.7.5/quant1x_trader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2024-04-22 05:09:42.000000 quant1x-trader-0.7.5/quant1x_trader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 05:09:42.000000 quant1x-trader-0.7.5/quant1x_trader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2024-04-22 05:09:42.000000 quant1x-trader-0.7.5/quant1x_trader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 05:09:42.000000 quant1x-trader-0.7.5/quant1x_trader.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      290 2024-04-22 05:09:42.000000 quant1x-trader-0.7.5/quant1x_trader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-22 05:09:42.000000 quant1x-trader-0.7.5/quant1x_trader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 05:09:42.143086 quant1x-trader-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     2284 2024-04-22 05:07:51.000000 quant1x-trader-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 05:09:42.139074 quant1x-trader-0.7.5/trader1x/
+-rw-rw-rw-   0        0        0      103 2024-02-19 01:20:42.000000 quant1x-trader-0.7.5/trader1x/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-12-11 07:07:15.000000 quant1x-trader-0.7.5/trader1x/__main__.py
+-rw-rw-rw-   0        0        0    16143 2024-02-19 01:20:42.000000 quant1x-trader-0.7.5/trader1x/auto.py
+-rw-rw-rw-   0        0        0     8648 2024-02-19 01:20:42.000000 quant1x-trader-0.7.5/trader1x/config.py
+-rw-rw-rw-   0        0        0     7922 2024-02-19 01:20:42.000000 quant1x-trader-0.7.5/trader1x/context.py
+-rw-rw-rw-   0        0        0     1193 2024-02-19 01:20:42.000000 quant1x-trader-0.7.5/trader1x/log4py.py
+-rw-rw-rw-   0        0        0    18556 2024-04-22 05:08:01.000000 quant1x-trader-0.7.5/trader1x/proxy.py
+-rw-rw-rw-   0        0        0     1266 2024-04-22 04:56:33.000000 quant1x-trader-0.7.5/trader1x/qmt.py
+-rw-rw-rw-   0        0        0    19739 2024-04-22 05:07:58.000000 quant1x-trader-0.7.5/trader1x/thinktrader.py
+-rw-rw-rw-   0        0        0     1368 2024-02-19 01:20:42.000000 quant1x-trader-0.7.5/trader1x/utils.py
+-rw-rw-rw-   0        0        0    38933 2024-01-21 09:52:15.000000 quant1x-trader-0.7.5/trader1x/win32serviceutil.py
```

### Comparing `quant1x-trader-0.7.4/LICENSE` & `quant1x-trader-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/PKG-INFO` & `quant1x-trader-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-trader
-Version: 0.7.4
+Version: 0.7.5
 Summary: Quant1X程序化自动化交易
 Home-page: https://gitee.com/quant1x/trader
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x auto trader
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `quant1x-trader-0.7.4/quant1x_trader.egg-info/PKG-INFO` & `quant1x-trader-0.7.5/quant1x_trader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-trader
-Version: 0.7.4
+Version: 0.7.5
 Summary: Quant1X程序化自动化交易
 Home-page: https://gitee.com/quant1x/trader
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x auto trader
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `quant1x-trader-0.7.4/quant1x_trader.egg-info/SOURCES.txt` & `quant1x-trader-0.7.5/quant1x_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/setup.py` & `quant1x-trader-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/auto.py` & `quant1x-trader-0.7.5/trader1x/auto.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/config.py` & `quant1x-trader-0.7.5/trader1x/config.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/context.py` & `quant1x-trader-0.7.5/trader1x/context.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/log4py.py` & `quant1x-trader-0.7.5/trader1x/log4py.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/proxy.py` & `quant1x-trader-0.7.5/trader1x/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
              'volume': p.volume,
              'can_use_volume': p.can_use_volume,
              'open_price': base1x.fix_float(p.open_price),
              'market_value': base1x.fix_float(p.market_value),
              'frozen_volume': p.frozen_volume,
              'on_road_volume': p.on_road_volume,
              'yesterday_volume': p.yesterday_volume,
-             'avg_price': p.avg_price,
+             'avg_price': base1x.fix_float(p.avg_price),
              }
         )
     return holding
 
 
 @app.api_route('/query/trade', methods=['GET', 'POST'])
 async def query_trade():
```

### Comparing `quant1x-trader-0.7.4/trader1x/qmt.py` & `quant1x-trader-0.7.5/trader1x/qmt.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/thinktrader.py` & `quant1x-trader-0.7.5/trader1x/thinktrader.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/utils.py` & `quant1x-trader-0.7.5/trader1x/utils.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.4/trader1x/win32serviceutil.py` & `quant1x-trader-0.7.5/trader1x/win32serviceutil.py`

 * *Files identical despite different names*

