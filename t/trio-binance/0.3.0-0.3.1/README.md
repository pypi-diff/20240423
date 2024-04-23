# Comparing `tmp/trio_binance-0.3.0.tar.gz` & `tmp/trio_binance-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trio_binance-0.3.0.tar", max compression
+gzip compressed data, was "trio_binance-0.3.1.tar", max compression
```

## Comparing `trio_binance-0.3.0.tar` & `trio_binance-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.3.0/LICENSE
--rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.3.0/README.rst
--rw-r--r--   0        0        0     1055 2024-04-23 02:07:29.165386 trio_binance-0.3.0/pyproject.toml
--rwxr-xr-x   0        0        0       67 2024-04-23 01:56:20.850254 trio_binance-0.3.0/trio_binance/__init__.py
--rwxr-xr-x   0        0        0    77725 2024-04-23 03:34:11.343931 trio_binance-0.3.0/trio_binance/client.py
--rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.3.0/trio_binance/enums.py
--rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.3.0/trio_binance/exceptions.py
--rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.3.0/trio_binance/helpers.py
--rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.3.0/trio_binance/streams.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 trio_binance-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.3.1/LICENSE
+-rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.3.1/README.rst
+-rw-r--r--   0        0        0     1055 2024-04-23 07:31:54.523131 trio_binance-0.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0       67 2024-04-23 07:32:06.912749 trio_binance-0.3.1/trio_binance/__init__.py
+-rwxr-xr-x   0        0        0    78234 2024-04-23 07:30:58.714259 trio_binance-0.3.1/trio_binance/client.py
+-rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.3.1/trio_binance/enums.py
+-rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.3.1/trio_binance/exceptions.py
+-rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.3.1/trio_binance/helpers.py
+-rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.3.1/trio_binance/streams.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 trio_binance-0.3.1/PKG-INFO
```

### Comparing `trio_binance-0.3.0/LICENSE` & `trio_binance-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.0/README.rst` & `trio_binance-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.0/pyproject.toml` & `trio_binance-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trio-binance"
-version = "0.3.0"
+version = "0.3.1"
 description = "trio based asynchronous binance SDK"
 authors = ["Shu Wang <halfelf.ronin@gmail.com>"]
 keywords = ["binance", "python-trio"]
 readme = "README.rst"
 license = "MIT"
 homepage = "https://github.com/halfelf/trio-binance"
 repository = "https://github.com/halfelf/trio-binance"
```

### Comparing `trio_binance-0.3.0/trio_binance/client.py` & `trio_binance-0.3.1/trio_binance/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -946,14 +946,23 @@
 
     async def futures_time(self):
         return await self._request_futures_api("get", "time")
 
     async def futures_exchange_info(self):
         return await self._request_futures_api("get", "exchangeInfo")
 
+    async def futures_get_symbol_info(self, symbol) -> Optional[Dict]:
+        res = await self.get_exchange_info()
+
+        for item in res["symbols"]:
+            if item["symbol"] == symbol.upper():
+                return item
+
+        return None
+
     async def futures_order_book(self, **params):
         return await self._request_futures_api("get", "depth", data=params)
 
     async def futures_recent_trades(self, **params):
         return await self._request_futures_api("get", "trades", data=params)
 
     async def futures_historical_trades(self, **params):
@@ -1127,14 +1136,23 @@
 
     async def futures_coin_time(self):
         return await self._request_futures_coin_api("get", "time")
 
     async def futures_coin_exchange_info(self):
         return await self._request_futures_coin_api("get", "exchangeInfo")
 
+    async def futures_coin_get_symbol_info(self, symbol) -> Optional[Dict]:
+        res = await self.get_exchange_info()
+
+        for item in res["symbols"]:
+            if item["symbol"] == symbol.upper():
+                return item
+
+        return None
+
     async def futures_coin_order_book(self, **params):
         return await self._request_futures_coin_api("get", "depth", data=params)
 
     async def futures_coin_recent_trades(self, **params):
         return await self._request_futures_coin_api("get", "trades", data=params)
 
     async def futures_coin_historical_trades(self, **params):
```

### Comparing `trio_binance-0.3.0/trio_binance/enums.py` & `trio_binance-0.3.1/trio_binance/enums.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.0/trio_binance/exceptions.py` & `trio_binance-0.3.1/trio_binance/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.0/trio_binance/helpers.py` & `trio_binance-0.3.1/trio_binance/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.0/trio_binance/streams.py` & `trio_binance-0.3.1/trio_binance/streams.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.0/PKG-INFO` & `trio_binance-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-binance
-Version: 0.3.0
+Version: 0.3.1
 Summary: trio based asynchronous binance SDK
 Home-page: https://github.com/halfelf/trio-binance
 License: MIT
 Keywords: binance,python-trio
 Author: Shu Wang
 Author-email: halfelf.ronin@gmail.com
 Requires-Python: >=3.11,<4.0
```

