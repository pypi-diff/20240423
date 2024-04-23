# Comparing `tmp/trio-binance-0.2.2.tar.gz` & `tmp/trio_binance-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trio-binance-0.2.2.tar", max compression
+gzip compressed data, was "trio_binance-0.3.0.tar", max compression
```

## Comparing `trio-binance-0.2.2.tar` & `trio_binance-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio-binance-0.2.2/LICENSE
--rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.908940 trio-binance-0.2.2/README.rst
--rw-r--r--   0        0        0      866 2023-01-13 08:50:21.552047 trio-binance-0.2.2/pyproject.toml
--rwxr-xr-x   0        0        0       67 2023-01-13 08:50:16.678568 trio-binance-0.2.2/trio_binance/__init__.py
--rwxr-xr-x   0        0        0    62008 2023-01-13 08:49:58.469275 trio-binance-0.2.2/trio_binance/client.py
--rw-r--r--   0        0        0     1891 2023-01-13 06:48:58.980630 trio-binance-0.2.2/trio_binance/enums.py
--rw-r--r--   0        0        0     2280 2021-11-03 03:13:02.000000 trio-binance-0.2.2/trio_binance/exceptions.py
--rw-r--r--   0        0        0     1493 2023-01-13 06:49:20.173558 trio-binance-0.2.2/trio_binance/helpers.py
--rw-r--r--   0        0        0     6088 2022-05-06 09:23:42.064404 trio-binance-0.2.2/trio_binance/streams.py
--rw-r--r--   0        0        0     1982 2023-01-13 08:50:47.521329 trio-binance-0.2.2/setup.py
--rw-r--r--   0        0        0     2086 2023-01-13 08:50:47.521530 trio-binance-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.3.0/README.rst
+-rw-r--r--   0        0        0     1055 2024-04-23 02:07:29.165386 trio_binance-0.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0       67 2024-04-23 01:56:20.850254 trio_binance-0.3.0/trio_binance/__init__.py
+-rwxr-xr-x   0        0        0    77725 2024-04-23 03:34:11.343931 trio_binance-0.3.0/trio_binance/client.py
+-rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.3.0/trio_binance/enums.py
+-rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.3.0/trio_binance/exceptions.py
+-rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.3.0/trio_binance/helpers.py
+-rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.3.0/trio_binance/streams.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 trio_binance-0.3.0/PKG-INFO
```

### Comparing `trio-binance-0.2.2/LICENSE` & `trio_binance-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trio-binance-0.2.2/README.rst` & `trio_binance-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `trio-binance-0.2.2/trio_binance/client.py` & `trio_binance-0.3.0/trio_binance/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,114 @@
-from typing import Dict, Optional, List, Tuple
+from typing import Dict, Optional, List, Tuple, Union
 
 import httpx
 import h2
 import trio
 import hashlib
 import hmac
 import time
 from operator import itemgetter
 from urllib.parse import urlencode
 
 from .helpers import convert_ts_str
-from .exceptions import BinanceAPIException, BinanceRequestException, NotImplementedException
+from .exceptions import (
+    BinanceAPIException,
+    BinanceRequestException,
+    NotImplementedException,
+)
 
 
 class BaseClient:
-    API_URL = 'https://api.binance.{}/api'
-    API_TESTNET_URL = 'https://testnet.binance.vision/api'
-    MARGIN_API_URL = 'https://api.binance.{}/sapi'
-    WEBSITE_URL = 'https://www.binance.{}'
-    FUTURES_URL = 'https://fapi.binance.{}/fapi'
-    FUTURES_TESTNET_URL = 'https://testnet.binancefuture.com/fapi'
-    FUTURES_DATA_URL = 'https://fapi.binance.{}/futures/data'
-    FUTURES_DATA_TESTNET_URL = 'https://testnet.binancefuture.com/futures/data'
+    API_URL = "https://api{}.binance.{}/api"
+    API_TESTNET_URL = "https://testnet.binance.vision/api"
+    MARGIN_API_URL = "https://api.binance.{}/sapi"
+    WEBSITE_URL = "https://www.binance.{}"
+    FUTURES_URL = "https://fapi.binance.{}/fapi"
+    FUTURES_TESTNET_URL = "https://testnet.binancefuture.com/fapi"
+    FUTURES_DATA_URL = "https://fapi.binance.{}/futures/data"
+    FUTURES_DATA_TESTNET_URL = "https://testnet.binancefuture.com/futures/data"
     FUTURES_COIN_URL = "https://dapi.binance.{}/dapi"
-    FUTURES_COIN_TESTNET_URL = 'https://testnet.binancefuture.com/dapi'
+    FUTURES_COIN_TESTNET_URL = "https://testnet.binancefuture.com/dapi"
     FUTURES_COIN_DATA_URL = "https://dapi.binance.{}/futures/data"
-    FUTURES_COIN_DATA_TESTNET_URL = 'https://testnet.binancefuture.com/futures/data'
-    OPTIONS_URL = 'https://vapi.binance.{}/vapi'
-    OPTIONS_TESTNET_URL = 'https://testnet.binanceops.{}/vapi'
-    PUBLIC_API_VERSION = 'v1'
-    PRIVATE_API_VERSION = 'v3'
-    MARGIN_API_VERSION = 'v1'
-    FUTURES_API_VERSION = 'v1'
+    FUTURES_COIN_DATA_TESTNET_URL = "https://testnet.binancefuture.com/futures/data"
+    OPTIONS_URL = "https://vapi.binance.{}/vapi"
+    OPTIONS_TESTNET_URL = "https://testnet.binanceops.{}/vapi"
+    PORTFOLIO_MARGIN_URL = "https://papi.binance.com/papi"
+    PUBLIC_API_VERSION = "v1"
+    PRIVATE_API_VERSION = "v3"
+    MARGIN_API_VERSION = "v1"
+    FUTURES_API_VERSION = "v1"
     FUTURES_API_VERSION2 = "v2"
-    OPTIONS_API_VERSION = 'v1'
+    OPTIONS_API_VERSION = "v1"
+    PORTFOLIO_MARGIN_VERSION = "v1"
 
     REQUEST_TIMEOUT: float = 10
 
-    SYMBOL_TYPE_SPOT = 'SPOT'
+    SYMBOL_TYPE_SPOT = "SPOT"
 
-    ORDER_STATUS_NEW = 'NEW'
-    ORDER_STATUS_PARTIALLY_FILLED = 'PARTIALLY_FILLED'
-    ORDER_STATUS_FILLED = 'FILLED'
-    ORDER_STATUS_CANCELED = 'CANCELED'
-    ORDER_STATUS_PENDING_CANCEL = 'PENDING_CANCEL'
-    ORDER_STATUS_REJECTED = 'REJECTED'
-    ORDER_STATUS_EXPIRED = 'EXPIRED'
-
-    KLINE_INTERVAL_1MINUTE = '1m'
-    KLINE_INTERVAL_3MINUTE = '3m'
-    KLINE_INTERVAL_5MINUTE = '5m'
-    KLINE_INTERVAL_15MINUTE = '15m'
-    KLINE_INTERVAL_30MINUTE = '30m'
-    KLINE_INTERVAL_1HOUR = '1h'
-    KLINE_INTERVAL_2HOUR = '2h'
-    KLINE_INTERVAL_4HOUR = '4h'
-    KLINE_INTERVAL_6HOUR = '6h'
-    KLINE_INTERVAL_8HOUR = '8h'
-    KLINE_INTERVAL_12HOUR = '12h'
-    KLINE_INTERVAL_1DAY = '1d'
-    KLINE_INTERVAL_3DAY = '3d'
-    KLINE_INTERVAL_1WEEK = '1w'
-    KLINE_INTERVAL_1MONTH = '1M'
-
-    SIDE_BUY = 'BUY'
-    SIDE_SELL = 'SELL'
-
-    ORDER_TYPE_LIMIT = 'LIMIT'
-    ORDER_TYPE_MARKET = 'MARKET'
-    ORDER_TYPE_STOP_LOSS = 'STOP_LOSS'
-    ORDER_TYPE_STOP_LOSS_LIMIT = 'STOP_LOSS_LIMIT'
-    ORDER_TYPE_TAKE_PROFIT = 'TAKE_PROFIT'
-    ORDER_TYPE_TAKE_PROFIT_LIMIT = 'TAKE_PROFIT_LIMIT'
-    ORDER_TYPE_LIMIT_MAKER = 'LIMIT_MAKER'
-
-    FUTURE_ORDER_TYPE_LIMIT = 'LIMIT'
-    FUTURE_ORDER_TYPE_MARKET = 'MARKET'
-    FUTURE_ORDER_TYPE_STOP = 'STOP'
-    FUTURE_ORDER_TYPE_STOP_MARKET = 'STOP_MARKET'
-    FUTURE_ORDER_TYPE_TAKE_PROFIT = 'TAKE_PROFIT'
-    FUTURE_ORDER_TYPE_TAKE_PROFIT_MARKET = 'TAKE_PROFIT_MARKET'
-    FUTURE_ORDER_TYPE_LIMIT_MAKER = 'LIMIT_MAKER'
-
-    TIME_IN_FORCE_GTC = 'GTC'  # Good till cancelled
-    TIME_IN_FORCE_IOC = 'IOC'  # Immediate or cancel
-    TIME_IN_FORCE_FOK = 'FOK'  # Fill or kill
-
-    ORDER_RESP_TYPE_ACK = 'ACK'
-    ORDER_RESP_TYPE_RESULT = 'RESULT'
-    ORDER_RESP_TYPE_FULL = 'FULL'
+    ORDER_STATUS_NEW = "NEW"
+    ORDER_STATUS_PARTIALLY_FILLED = "PARTIALLY_FILLED"
+    ORDER_STATUS_FILLED = "FILLED"
+    ORDER_STATUS_CANCELED = "CANCELED"
+    ORDER_STATUS_PENDING_CANCEL = "PENDING_CANCEL"
+    ORDER_STATUS_REJECTED = "REJECTED"
+    ORDER_STATUS_EXPIRED = "EXPIRED"
+
+    KLINE_INTERVAL_1MINUTE = "1m"
+    KLINE_INTERVAL_3MINUTE = "3m"
+    KLINE_INTERVAL_5MINUTE = "5m"
+    KLINE_INTERVAL_15MINUTE = "15m"
+    KLINE_INTERVAL_30MINUTE = "30m"
+    KLINE_INTERVAL_1HOUR = "1h"
+    KLINE_INTERVAL_2HOUR = "2h"
+    KLINE_INTERVAL_4HOUR = "4h"
+    KLINE_INTERVAL_6HOUR = "6h"
+    KLINE_INTERVAL_8HOUR = "8h"
+    KLINE_INTERVAL_12HOUR = "12h"
+    KLINE_INTERVAL_1DAY = "1d"
+    KLINE_INTERVAL_3DAY = "3d"
+    KLINE_INTERVAL_1WEEK = "1w"
+    KLINE_INTERVAL_1MONTH = "1M"
+
+    SIDE_BUY = "BUY"
+    SIDE_SELL = "SELL"
+
+    ORDER_TYPE_LIMIT = "LIMIT"
+    ORDER_TYPE_MARKET = "MARKET"
+    ORDER_TYPE_STOP_LOSS = "STOP_LOSS"
+    ORDER_TYPE_STOP_LOSS_LIMIT = "STOP_LOSS_LIMIT"
+    ORDER_TYPE_TAKE_PROFIT = "TAKE_PROFIT"
+    ORDER_TYPE_TAKE_PROFIT_LIMIT = "TAKE_PROFIT_LIMIT"
+    ORDER_TYPE_LIMIT_MAKER = "LIMIT_MAKER"
+
+    FUTURE_ORDER_TYPE_LIMIT = "LIMIT"
+    FUTURE_ORDER_TYPE_MARKET = "MARKET"
+    FUTURE_ORDER_TYPE_STOP = "STOP"
+    FUTURE_ORDER_TYPE_STOP_MARKET = "STOP_MARKET"
+    FUTURE_ORDER_TYPE_TAKE_PROFIT = "TAKE_PROFIT"
+    FUTURE_ORDER_TYPE_TAKE_PROFIT_MARKET = "TAKE_PROFIT_MARKET"
+    FUTURE_ORDER_TYPE_LIMIT_MAKER = "LIMIT_MAKER"
+
+    TIME_IN_FORCE_GTC = "GTC"  # Good till cancelled
+    TIME_IN_FORCE_IOC = "IOC"  # Immediate or cancel
+    TIME_IN_FORCE_FOK = "FOK"  # Fill or kill
+
+    ORDER_RESP_TYPE_ACK = "ACK"
+    ORDER_RESP_TYPE_RESULT = "RESULT"
+    ORDER_RESP_TYPE_FULL = "FULL"
 
     # For accessing the data returned by Client.aggregate_trades().
-    AGG_ID = 'a'
-    AGG_PRICE = 'p'
-    AGG_QUANTITY = 'q'
-    AGG_FIRST_TRADE_ID = 'f'
-    AGG_LAST_TRADE_ID = 'l'
-    AGG_TIME = 'T'
-    AGG_BUYER_MAKES = 'm'
-    AGG_BEST_MATCH = 'M'
+    AGG_ID = "a"
+    AGG_PRICE = "p"
+    AGG_QUANTITY = "q"
+    AGG_FIRST_TRADE_ID = "f"
+    AGG_LAST_TRADE_ID = "l"
+    AGG_TIME = "T"
+    AGG_BUYER_MAKES = "m"
+    AGG_BEST_MATCH = "M"
 
     # new asset transfer api enum
     SPOT_TO_FIAT = "MAIN_C2C"
     SPOT_TO_USDT_FUTURE = "MAIN_UMFUTURE"
     SPOT_TO_COIN_FUTURE = "MAIN_CMFUTURE"
     SPOT_TO_MARGIN_CROSS = "MAIN_MARGIN"
     SPOT_TO_MINING = "MAIN_MINING"
@@ -116,33 +122,39 @@
     MARGIN_CROSS_TO_SPOT = "MARGIN_MAIN"
     MARGIN_CROSS_TO_USDT_FUTURE = "MARGIN_UMFUTURE"
     MINING_TO_SPOT = "MINING_MAIN"
     MINING_TO_USDT_FUTURE = "MINING_UMFUTURE"
     MINING_TO_FIAT = "MINING_C2C"
 
     def __init__(
-            self, api_key: Optional[str] = None, api_secret: Optional[str] = None,
-            requests_params: Dict[str, str] = None, tld: str = 'com',
-            testnet: bool = False
+        self,
+        api_key: Optional[str] = None,
+        api_secret: Optional[str] = None,
+        requests_params: Dict[str, str] = None,
+        api_cluster_id: Union[int, str] = "",
+        tld: str = "com",
+        testnet: bool = False,
     ):
         """Binance API Client constructor
 
         :param api_key: Api Key
         :type api_key: str.
         :param api_secret: Api Secret
         :type api_secret: str.
         :param requests_params: optional - Dictionary of requests params to use for all calls
         :type requests_params: dict.
+        :param api_cluster_id: optional - Cluster ID for API
+        :type api_cluster_id: str or int
         :param testnet: Use testnet environment - only available for vanilla options at the moment
         :type testnet: bool
 
         """
 
         self.tld = tld
-        self.API_URL = self.API_URL.format(tld)
+        self.API_URL = self.API_URL.format(api_cluster_id, tld)
         self.MARGIN_API_URL = self.MARGIN_API_URL.format(tld)
         self.WEBSITE_URL = self.WEBSITE_URL.format(tld)
         self.FUTURES_URL = self.FUTURES_URL.format(tld)
         self.FUTURES_DATA_URL = self.FUTURES_DATA_URL.format(tld)
         self.FUTURES_COIN_URL = self.FUTURES_COIN_URL.format(tld)
         self.FUTURES_COIN_DATA_URL = self.FUTURES_COIN_DATA_URL.format(tld)
         self.OPTIONS_URL = self.OPTIONS_URL.format(tld)
@@ -153,47 +165,48 @@
         self._requests_params = requests_params
         self.response = None
         self.testnet = testnet
         self.timestamp_offset = 0
 
     def _get_headers(self) -> Dict:
         headers = {
-            'Accept': 'application/json',
-            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36',
+            "Accept": "application/json",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36",
             # noqa
         }
         if self.API_KEY:
             assert self.API_KEY
-            headers['X-MBX-APIKEY'] = self.API_KEY
+            headers["X-MBX-APIKEY"] = self.API_KEY
         return headers
 
     def _create_api_uri(self, path: str, signed: bool = True, version: str = PUBLIC_API_VERSION) -> str:
         url = self.API_URL
         if self.testnet:
             url = self.API_TESTNET_URL
         v = self.PRIVATE_API_VERSION if signed else version
-        return url + '/' + v + '/' + path
+        return url + "/" + v + "/" + path
 
     def _create_margin_api_uri(self, path: str, version: str = MARGIN_API_VERSION) -> str:
-        return self.MARGIN_API_URL + '/' + version + '/' + path
+        return self.MARGIN_API_URL + "/" + version + "/" + path
 
     def _create_website_uri(self, path: str) -> str:
-        return self.WEBSITE_URL + '/' + path
+        return self.WEBSITE_URL + "/" + path
 
-    def _create_futures_api_uri(self, path: str) -> str:
+    def _create_futures_api_uri(self, path: str, version=1) -> str:
         url = self.FUTURES_URL
         if self.testnet:
             url = self.FUTURES_TESTNET_URL
-        return url + '/' + self.FUTURES_API_VERSION + '/' + path
+        options = {1: self.FUTURES_API_VERSION, 2: self.FUTURES_API_VERSION2}
+        return url + "/" + options[version] + "/" + path
 
     def _create_futures_data_api_uri(self, path: str) -> str:
         url = self.FUTURES_DATA_URL
         if self.testnet:
             url = self.FUTURES_DATA_TESTNET_URL
-        return url + '/' + path
+        return url + "/" + path
 
     def _create_futures_coin_api_url(self, path: str, version=1) -> str:
         url = self.FUTURES_COIN_URL
         if self.testnet:
             url = self.FUTURES_COIN_TESTNET_URL
         options = {1: self.FUTURES_API_VERSION, 2: self.FUTURES_API_VERSION2}
         return url + "/" + options[version] + "/" + path
@@ -204,110 +217,124 @@
             url = self.FUTURES_COIN_DATA_TESTNET_URL
         return url + "/" + path
 
     def _create_options_api_uri(self, path: str) -> str:
         url = self.OPTIONS_URL
         if self.testnet:
             url = self.OPTIONS_TESTNET_URL
-        return url + '/' + self.OPTIONS_API_VERSION + '/' + path
+        return url + "/" + self.OPTIONS_API_VERSION + "/" + path
 
-    def _generate_signature(self, data: Dict) -> str:
+    def _create_portfolio_margin_api_uri(self, path: str, version: int = 1) -> str:
+        url = self.PORTFOLIO_MARGIN_URL
+        options = {1: self.PORTFOLIO_MARGIN_VERSION}
+        return url + "/" + options[version] + "/" + path
 
+    def _generate_signature(self, data: Dict) -> str:
         ordered_data = self._order_params(data)
-        query_string = '&'.join([f"{d[0]}={d[1]}" for d in ordered_data])
-        m = hmac.new(self.API_SECRET.encode('utf-8'), query_string.encode('utf-8'), hashlib.sha256)
+        query_string = "&".join([f"{d[0]}={d[1]}" for d in ordered_data])
+        m = hmac.new(
+            self.API_SECRET.encode("utf-8"),
+            query_string.encode("utf-8"),
+            hashlib.sha256,
+        )
         return m.hexdigest()
 
     @staticmethod
     def _order_params(data: Dict) -> List[Tuple[str, str]]:
         """Convert params to list with signature as last element
 
         :param data:
         :return:
 
         """
         data = dict(filter(lambda el: el[1] is not None, data.items()))
         has_signature = False
         params = []
         for key, value in data.items():
-            if key == 'signature':
+            if key == "signature":
                 has_signature = True
             else:
                 params.append((key, str(value)))
         # sort parameters by key
         params.sort(key=itemgetter(0))
         if has_signature:
-            params.append(('signature', data['signature']))
+            params.append(("signature", data["signature"]))
         return params
 
     def _get_request_kwargs(self, method, signed: bool, force_params: bool = False, **kwargs) -> Dict:
-
         # set default requests timeout
-        kwargs['timeout'] = self.REQUEST_TIMEOUT
+        kwargs["timeout"] = self.REQUEST_TIMEOUT
 
         # add our global requests params
         if self._requests_params:
             kwargs.update(self._requests_params)
 
-        data = kwargs.get('data', None)
+        data = kwargs.get("data", None)
         if data and isinstance(data, dict):
-            kwargs['data'] = data
+            kwargs["data"] = data
 
             # find any requests params passed and apply them
-            if 'requests_params' in kwargs['data']:
+            if "requests_params" in kwargs["data"]:
                 # merge requests params into kwargs
-                kwargs.update(kwargs['data']['requests_params'])
-                del (kwargs['data']['requests_params'])
+                kwargs.update(kwargs["data"]["requests_params"])
+                del kwargs["data"]["requests_params"]
 
         if signed:
             # generate signature
-            kwargs['data']['timestamp'] = int(time.time() * 1000 + self.timestamp_offset)
-            kwargs['data']['signature'] = self._generate_signature(kwargs['data'])
+            kwargs["data"]["timestamp"] = int(time.time() * 1000 + self.timestamp_offset)
+            kwargs["data"]["signature"] = self._generate_signature(kwargs["data"])
 
             # sort get and post params to match signature order
         if data:
             # sort post params and remove any arguments with values of None
-            kwargs['data'] = self._order_params(kwargs['data'])
+            kwargs["data"] = self._order_params(kwargs["data"])
             # Remove any arguments with values of None.
-            null_args = [i for i, (key, value) in enumerate(kwargs['data']) if value is None]
+            null_args = [i for i, (key, value) in enumerate(kwargs["data"]) if value is None]
             for i in reversed(null_args):
-                del kwargs['data'][i]
+                del kwargs["data"][i]
 
             # if get request assign data array to params value for requests lib
-        if data and (method == 'get' or force_params):
-            kwargs['params'] = '&'.join('%s=%s' % (data[0], data[1]) for data in kwargs['data'])
-            del (kwargs['data'])
+        if data and (method == "get" or force_params):
+            kwargs["params"] = "&".join("%s=%s" % (data[0], data[1]) for data in kwargs["data"])
+            del kwargs["data"]
 
         return kwargs
 
 
 class AsyncClient(BaseClient):
     def __init__(
-            self, api_key: Optional[str] = None, api_secret: Optional[str] = None,
-            requests_params: Dict[str, str] = None, tld: str = 'com',
-            testnet: bool = False
+        self,
+        api_key: Optional[str] = None,
+        api_secret: Optional[str] = None,
+        requests_params: Dict[str, str] = None,
+        api_cluster_id: Union[str, int] = "",
+        tld: str = "com",
+        testnet: bool = False,
     ):
-        super().__init__(api_key, api_secret, requests_params, tld, testnet)
+        super().__init__(api_key, api_secret, requests_params, api_cluster_id, tld, testnet)
         self.session: httpx.AsyncClient = httpx.AsyncClient(http2=True, headers=self._get_headers())
 
     @classmethod
     async def create(
-            cls, api_key: Optional[str] = None, api_secret: Optional[str] = None,
-            requests_params: Dict[str, str] = None, tld: str = 'com',
-            testnet: bool = False
+        cls,
+        api_key: Optional[str] = None,
+        api_secret: Optional[str] = None,
+        requests_params: Dict[str, str] = None,
+        api_cluster_id: Union[str, int] = "",
+        tld: str = "com",
+        testnet: bool = False,
     ):
-
-        self = cls(api_key, api_secret, requests_params, tld, testnet)
+        self = cls(api_key, api_secret, requests_params, api_cluster_id, tld, testnet)
 
         try:
             await self.ping()
 
             # calculate timestamp offset between local and trio_binance server
             res = await self.get_server_time()
-            self.timestamp_offset = res['serverTime'] - int(time.time() * 1000)
+            self.timestamp_offset = res["serverTime"] - int(time.time() * 1000)
 
             return self
         except Exception:
             # If ping throw an exception, the current self must be cleaned
             # else, we can receive a "asyncio:Unclosed client session"
             await self.close_connection()
             raise
@@ -330,27 +357,34 @@
 
     @staticmethod
     async def _handle_response(response: httpx.Response):
         """Internal helper for handling API responses from the Binance server.
         Raises the appropriate exceptions when necessary; otherwise, returns the
         response.
         """
-        if not str(response.status_code).startswith('2'):
+        if response.is_error:
             raise BinanceAPIException(response, response.status_code, response.text)
         try:
             return response.json()
         except ValueError:
-            raise BinanceRequestException(f'Invalid Response: {response.text}')
+            raise BinanceRequestException(f"Invalid Response: {response.text}")
 
-    async def _request_api(self, method, path, signed=False, version=BaseClient.PUBLIC_API_VERSION, **kwargs):
+    async def _request_api(
+        self,
+        method,
+        path,
+        signed=False,
+        version=BaseClient.PUBLIC_API_VERSION,
+        **kwargs,
+    ):
         uri = self._create_api_uri(path, signed, version)
         return await self._request(method, uri, signed, **kwargs)
 
-    async def _request_futures_api(self, method, path, signed=False, **kwargs) -> Dict:
-        uri = self._create_futures_api_uri(path)
+    async def _request_futures_api(self, method, path, signed=False, version=1, **kwargs) -> Dict:
+        uri = self._create_futures_api_uri(path, version=version)
 
         return await self._request(method, uri, signed, True, **kwargs)
 
     async def _request_futures_data_api(self, method, path, signed=False, **kwargs) -> Dict:
         uri = self._create_futures_data_api_uri(path)
 
         return await self._request(method, uri, signed, True, **kwargs)
@@ -371,82 +405,87 @@
         return await self._request(method, uri, signed, True, **kwargs)
 
     async def _request_margin_api(self, method, path, signed=False, **kwargs) -> Dict:
         uri = self._create_margin_api_uri(path)
 
         return await self._request(method, uri, signed, **kwargs)
 
+    async def _request_portfolio_margin_api(self, method, path, signed=False, version: int = 1, **kwargs) -> Dict:
+        uri = self._create_portfolio_margin_api_uri(path, version)
+
+        return await self._request(method, uri, signed, **kwargs)
+
     async def _request_website(self, method, path, signed=False, **kwargs) -> Dict:
         uri = self._create_website_uri(path)
         return await self._request(method, uri, signed, **kwargs)
 
     async def _get(self, path, signed=False, version=BaseClient.PUBLIC_API_VERSION, **kwargs):
-        return await self._request_api('get', path, signed, version, **kwargs)
+        return await self._request_api("get", path, signed, version, **kwargs)
 
     async def _post(self, path, signed=False, version=BaseClient.PUBLIC_API_VERSION, **kwargs) -> Dict:
-        return await self._request_api('post', path, signed, version, **kwargs)
+        return await self._request_api("post", path, signed, version, **kwargs)
 
     async def _put(self, path, signed=False, version=BaseClient.PUBLIC_API_VERSION, **kwargs) -> Dict:
-        return await self._request_api('put', path, signed, version, **kwargs)
+        return await self._request_api("put", path, signed, version, **kwargs)
 
     async def _delete(self, path, signed=False, version=BaseClient.PUBLIC_API_VERSION, **kwargs) -> Dict:
-        return await self._request_api('delete', path, signed, version, **kwargs)
+        return await self._request_api("delete", path, signed, version, **kwargs)
 
     # Exchange Endpoints
 
     async def get_products(self) -> Dict:
-        products = await self._request_website('get', 'exchange-api/v1/public/asset-service/product/get-products')
+        products = await self._request_website("get", "exchange-api/v1/public/asset-service/product/get-products")
         return products
 
     async def get_exchange_info(self) -> Dict:
-        return await self._get('exchangeInfo', version=self.PRIVATE_API_VERSION)
+        return await self._get("exchangeInfo", version=self.PRIVATE_API_VERSION)
 
     async def get_symbol_info(self, symbol) -> Optional[Dict]:
         res = await self.get_exchange_info()
 
-        for item in res['symbols']:
-            if item['symbol'] == symbol.upper():
+        for item in res["symbols"]:
+            if item["symbol"] == symbol.upper():
                 return item
 
         return None
 
     # General Endpoints
 
     async def ping(self) -> Dict:
-        return await self._get('ping', version=self.PRIVATE_API_VERSION)
+        return await self._get("ping", version=self.PRIVATE_API_VERSION)
 
     async def get_server_time(self) -> Dict:
-        return await self._get('time', version=self.PRIVATE_API_VERSION)
+        return await self._get("time", version=self.PRIVATE_API_VERSION)
 
     # Market Data Endpoints
 
     async def get_all_tickers(self, symbol: Optional[str] = None) -> List[Dict[str, str]]:
         params = {}
         if symbol:
-            params['symbol'] = symbol
-        return await self._get('ticker/price', version=self.PRIVATE_API_VERSION, data=params)
+            params["symbol"] = symbol
+        return await self._get("ticker/price", version=self.PRIVATE_API_VERSION, data=params)
 
     async def get_orderbook_tickers(self) -> Dict:
-        return await self._get('ticker/bookTicker', version=self.PRIVATE_API_VERSION)
+        return await self._get("ticker/bookTicker", version=self.PRIVATE_API_VERSION)
 
     async def get_order_book(self, **params) -> Dict:
-        return await self._get('depth', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("depth", data=params, version=self.PRIVATE_API_VERSION)
 
     async def get_recent_trades(self, **params) -> Dict:
-        return await self._get('trades', data=params)
+        return await self._get("trades", data=params)
 
     async def get_historical_trades(self, **params) -> Dict:
-        return await self._get('historicalTrades', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("historicalTrades", data=params, version=self.PRIVATE_API_VERSION)
 
     async def get_aggregate_trades(self, **params) -> Dict:
-        return await self._get('aggTrades', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("aggTrades", data=params, version=self.PRIVATE_API_VERSION)
 
     async def aggregate_trade_iter(self, symbol, start_str=None, last_id=None):
         if start_str is not None and last_id is not None:
-            raise ValueError('start_time and last_id may not be simultaneously specified.')
+            raise ValueError("start_time and last_id may not be simultaneously specified.")
 
         # If there's no last_id, get one.
         if last_id is None:
             # Without a last_id, we actually need the first trade.  Normally,
             # we'd get rid of it. See the next loop.
             if start_str is None:
                 trades = await self.get_aggregate_trades(symbol=symbol, fromId=0)
@@ -486,645 +525,604 @@
             if len(trades) == 0:
                 return
             for t in trades:
                 yield t
             last_id = trades[-1][self.AGG_ID]
 
     async def get_klines(self, **params) -> Dict:
-        return await self._get('klines', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("klines", data=params, version=self.PRIVATE_API_VERSION)
 
     async def get_avg_price(self, **params):
-        return await self._get('avgPrice', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("avgPrice", data=params, version=self.PRIVATE_API_VERSION)
 
     async def get_ticker(self, **params):
-        return await self._get('ticker/24hr', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("ticker/24hr", data=params, version=self.PRIVATE_API_VERSION)
 
     async def get_symbol_ticker(self, **params):
-        return await self._get('ticker/price', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("ticker/price", data=params, version=self.PRIVATE_API_VERSION)
 
     async def get_orderbook_ticker(self, **params):
-        return await self._get('ticker/bookTicker', data=params, version=self.PRIVATE_API_VERSION)
+        return await self._get("ticker/bookTicker", data=params, version=self.PRIVATE_API_VERSION)
 
     # Account Endpoints
 
     async def create_order(self, **params):
-        return await self._post('order', True, data=params)
+        return await self._post("order", True, data=params)
 
     async def order_limit(self, timeInForce=BaseClient.TIME_IN_FORCE_GTC, **params):
-        params.update({
-            'type': self.ORDER_TYPE_LIMIT,
-            'timeInForce': timeInForce
-        })
+        params.update({"type": self.ORDER_TYPE_LIMIT, "timeInForce": timeInForce})
         return await self.create_order(**params)
 
     async def order_limit_buy(self, timeInForce=BaseClient.TIME_IN_FORCE_GTC, **params):
-        params.update({
-            'side': self.SIDE_BUY,
-        })
+        params.update(
+            {
+                "side": self.SIDE_BUY,
+            }
+        )
         return await self.order_limit(timeInForce=timeInForce, **params)
 
     async def order_limit_sell(self, timeInForce=BaseClient.TIME_IN_FORCE_GTC, **params):
-        params.update({
-            'side': self.SIDE_SELL
-        })
+        params.update({"side": self.SIDE_SELL})
         return await self.order_limit(timeInForce=timeInForce, **params)
 
     async def order_market(self, **params):
-        params.update({
-            'type': self.ORDER_TYPE_MARKET
-        })
+        params.update({"type": self.ORDER_TYPE_MARKET})
         return await self.create_order(**params)
 
     async def order_market_buy(self, **params):
-        params.update({
-            'side': self.SIDE_BUY
-        })
+        params.update({"side": self.SIDE_BUY})
         return await self.order_market(**params)
 
     async def order_market_sell(self, **params):
-        params.update({
-            'side': self.SIDE_SELL
-        })
+        params.update({"side": self.SIDE_SELL})
         return await self.order_market(**params)
 
     async def create_oco_order(self, **params):
-        return await self._post('order/oco', True, data=params)
+        return await self._post("order/oco", True, data=params)
 
     async def order_oco_buy(self, **params):
-        params.update({
-            'side': self.SIDE_BUY
-        })
+        params.update({"side": self.SIDE_BUY})
         return await self.create_oco_order(**params)
 
     async def order_oco_sell(self, **params):
-        params.update({
-            'side': self.SIDE_SELL
-        })
+        params.update({"side": self.SIDE_SELL})
         return await self.create_oco_order(**params)
 
     async def create_test_order(self, **params):
-        return await self._post('order/test', True, data=params)
+        return await self._post("order/test", True, data=params)
 
     async def get_order(self, **params):
-        return await self._get('order', True, data=params)
+        return await self._get("order", True, data=params)
 
     async def get_all_orders(self, **params):
-        return await self._get('allOrders', True, data=params)
+        return await self._get("allOrders", True, data=params)
 
     async def cancel_order(self, **params):
-        return await self._delete('order', True, data=params)
+        return await self._delete("order", True, data=params)
 
     async def get_open_orders(self, **params):
-        return await self._get('openOrders', True, data=params)
+        return await self._get("openOrders", True, data=params)
 
     # User Stream Endpoints
     async def get_account(self, **params):
-        return await self._get('account', True, data=params)
+        return await self._get("account", True, data=params)
 
     async def get_asset_balance(self, asset, **params):
         res = await self.get_account(**params)
         # find asset balance in list of balances
         if "balances" in res:
-            for bal in res['balances']:
-                if bal['asset'].lower() == asset.lower():
+            for bal in res["balances"]:
+                if bal["asset"].lower() == asset.lower():
                     return bal
         return None
 
     async def get_my_trades(self, **params):
-        return await self._get('myTrades', True, data=params)
+        return await self._get("myTrades", True, data=params)
 
     async def get_system_status(self):
-        return await self._request_margin_api('get', 'system/status')
+        return await self._request_margin_api("get", "system/status")
 
     async def get_account_status(self, **params):
-        return await self._request_margin_api('get', 'account/status', True, data=params)
+        return await self._request_margin_api("get", "account/status", True, data=params)
 
     async def get_account_api_trading_status(self, **params):
-        return await self._request_margin_api('get', 'account/apiTradingStatus', True, data=params)
+        return await self._request_margin_api("get", "account/apiTradingStatus", True, data=params)
 
     async def get_account_api_permissions(self, **params):
-        return await self._request_margin_api('get', 'account/apiRestrictions', True, data=params)
+        return await self._request_margin_api("get", "account/apiRestrictions", True, data=params)
 
     async def get_dust_log(self, **params):
-        return await self._request_margin_api('get', 'asset/dribblet', True, data=params)
+        return await self._request_margin_api("get", "asset/dribblet", True, data=params)
 
     async def transfer_dust(self, **params):
-        return await self._request_margin_api('post', 'asset/dust', True, data=params)
+        return await self._request_margin_api("post", "asset/dust", True, data=params)
 
     async def get_asset_dividend_history(self, **params):
-        return await self._request_margin_api('get', 'asset/assetDividend', True, data=params)
+        return await self._request_margin_api("get", "asset/assetDividend", True, data=params)
 
     async def make_universal_transfer(self, **params):
-        return await self._request_margin_api('post', 'asset/transfer', signed=True, data=params)
+        return await self._request_margin_api("post", "asset/transfer", signed=True, data=params)
 
     async def query_universal_transfer_history(self, **params):
-        return await self._request_margin_api('get', 'asset/transfer', signed=True, data=params)
+        return await self._request_margin_api("get", "asset/transfer", signed=True, data=params)
 
     async def get_trade_fee(self, **params):
-        return await self._request_margin_api('get', 'asset/tradeFee', True, data=params)
+        return await self._request_margin_api("get", "asset/tradeFee", True, data=params)
 
     async def get_asset_details(self, **params):
-        return await self._request_margin_api('get', 'asset/assetDetail', True, data=params)
+        return await self._request_margin_api("get", "asset/assetDetail", True, data=params)
 
     # Withdraw Endpoints
 
     async def withdraw(self, **params):
         # force a name for the withdrawal if one not set
-        if 'coin' in params and 'name' not in params:
-            params['name'] = params['coin']
-        return await self._request_margin_api('post', 'capital/withdraw/apply', True, data=params)
+        if "coin" in params and "name" not in params:
+            params["name"] = params["coin"]
+        return await self._request_margin_api("post", "capital/withdraw/apply", True, data=params)
 
     async def get_deposit_history(self, **params):
-        return await self._request_margin_api('get', 'capital/deposit/hisrec', True, data=params)
+        return await self._request_margin_api("get", "capital/deposit/hisrec", True, data=params)
 
     async def get_withdraw_history(self, **params):
-        return await self._request_margin_api('get', 'capital/withdraw/history', True, data=params)
+        return await self._request_margin_api("get", "capital/withdraw/history", True, data=params)
 
     async def get_withdraw_history_id(self, withdraw_id, **params):
         result = await self.get_withdraw_history(**params)
 
         for entry in result:
-            if 'id' in entry and entry['id'] == withdraw_id:
+            if "id" in entry and entry["id"] == withdraw_id:
                 return entry
 
         raise Exception("There is no entry with withdraw id", result)
 
     async def get_deposit_address(self, coin: str, network: Optional[str] = None, **params):
-        params['coin'] = coin
+        params["coin"] = coin
         if network:
-            params['network'] = network
-        return await self._request_margin_api('get', 'capital/deposit/address', True, data=params)
+            params["network"] = network
+        return await self._request_margin_api("get", "capital/deposit/address", True, data=params)
 
     # User Stream Endpoints
 
     async def stream_get_listen_key(self):
-        res = await self._post('userDataStream', False, data={})
-        return res['listenKey']
+        res = await self._post("userDataStream", False, data={})
+        return res["listenKey"]
 
-    async def stream_keepalive(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._put('userDataStream', False, data=params)
+    async def stream_keepalive(self):
+        return await self._put("userDataStream", False, data={})
 
-    async def stream_close(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._delete('userDataStream', False, data=params)
+    async def stream_close(self):
+        return await self._delete("userDataStream", False, data={})
 
     # Margin Trading Endpoints
     async def get_margin_account(self, **params):
-        return await self._request_margin_api('get', 'margin/account', True, data=params)
+        return await self._request_margin_api("get", "margin/account", True, data=params)
 
     async def get_isolated_margin_account(self, **params):
-        return await self._request_margin_api('get', 'margin/isolated/account', True, data=params)
+        return await self._request_margin_api("get", "margin/isolated/account", True, data=params)
 
     async def get_margin_asset(self, **params):
-        return await self._request_margin_api('get', 'margin/asset', data=params)
+        return await self._request_margin_api("get", "margin/asset", data=params)
 
     async def get_margin_symbol(self, **params):
-        return await self._request_margin_api('get', 'margin/pair', data=params)
+        return await self._request_margin_api("get", "margin/pair", data=params)
 
     async def get_margin_all_assets(self, **params):
-        return await self._request_margin_api('get', 'margin/allAssets', data=params)
+        return await self._request_margin_api("get", "margin/allAssets", data=params)
 
     async def get_margin_all_pairs(self, **params):
-        return await self._request_margin_api('get', 'margin/allPairs', data=params)
+        return await self._request_margin_api("get", "margin/allPairs", data=params)
 
     async def create_isolated_margin_account(self, **params):
-        return await self._request_margin_api('post', 'margin/isolated/create', signed=True, data=params)
+        return await self._request_margin_api("post", "margin/isolated/create", signed=True, data=params)
 
     async def get_isolated_margin_symbol(self, **params):
-        return await self._request_margin_api('get', 'margin/isolated/pair', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/isolated/pair", signed=True, data=params)
 
     async def get_all_isolated_margin_symbols(self, **params):
-        return await self._request_margin_api('get', 'margin/isolated/allPairs', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/isolated/allPairs", signed=True, data=params)
 
     async def toggle_bnb_burn_spot_margin(self, **params):
-        return await self._request_margin_api('post', 'bnbBurn', signed=True, data=params)
+        return await self._request_margin_api("post", "bnbBurn", signed=True, data=params)
 
     async def get_bnb_burn_spot_margin(self, **params):
-        return await self._request_margin_api('get', 'bnbBurn', signed=True, data=params)
+        return await self._request_margin_api("get", "bnbBurn", signed=True, data=params)
 
     async def get_margin_price_index(self, **params):
-        return await self._request_margin_api('get', 'margin/priceIndex', data=params)
+        return await self._request_margin_api("get", "margin/priceIndex", data=params)
 
     async def transfer_margin_to_spot(self, **params):
-        params['type'] = 2
-        return await self._request_margin_api('post', 'margin/transfer', signed=True, data=params)
+        params["type"] = 2
+        return await self._request_margin_api("post", "margin/transfer", signed=True, data=params)
 
     async def transfer_spot_to_margin(self, **params):
-        params['type'] = 1
-        return await self._request_margin_api('post', 'margin/transfer', signed=True, data=params)
+        params["type"] = 1
+        return await self._request_margin_api("post", "margin/transfer", signed=True, data=params)
 
     async def transfer_isolated_margin_to_spot(self, **params):
-        params['transFrom'] = "ISOLATED_MARGIN"
-        params['transTo'] = "SPOT"
-        return await self._request_margin_api('post', 'margin/isolated/transfer', signed=True, data=params)
+        params["transFrom"] = "ISOLATED_MARGIN"
+        params["transTo"] = "SPOT"
+        return await self._request_margin_api("post", "margin/isolated/transfer", signed=True, data=params)
 
     async def transfer_spot_to_isolated_margin(self, **params):
-        params['transFrom'] = "SPOT"
-        params['transTo'] = "ISOLATED_MARGIN"
-        return await self._request_margin_api('post', 'margin/isolated/transfer', signed=True, data=params)
+        params["transFrom"] = "SPOT"
+        params["transTo"] = "ISOLATED_MARGIN"
+        return await self._request_margin_api("post", "margin/isolated/transfer", signed=True, data=params)
 
     async def create_margin_loan(self, **params):
-        return await self._request_margin_api('post', 'margin/loan', signed=True, data=params)
+        return await self._request_margin_api("post", "margin/loan", signed=True, data=params)
 
     async def repay_margin_loan(self, **params):
-        return await self._request_margin_api('post', 'margin/repay', signed=True, data=params)
+        return await self._request_margin_api("post", "margin/repay", signed=True, data=params)
 
     async def create_margin_order(self, **params):
-        return await self._request_margin_api('post', 'margin/order', signed=True, data=params)
+        return await self._request_margin_api("post", "margin/order", signed=True, data=params)
 
     async def cancel_margin_order(self, **params):
-        return await self._request_margin_api('delete', 'margin/order', signed=True, data=params)
+        return await self._request_margin_api("delete", "margin/order", signed=True, data=params)
 
     async def get_margin_loan_details(self, **params):
-        return await self._request_margin_api('get', 'margin/loan', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/loan", signed=True, data=params)
 
     async def get_margin_repay_details(self, **params):
-        return await self._request_margin_api('get', 'margin/repay', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/repay", signed=True, data=params)
 
     async def get_margin_interest_history(self, **params):
-        return await self._request_margin_api('get', 'margin/interestHistory', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/interestHistory", signed=True, data=params)
 
     async def get_margin_force_liquidation_rec(self, **params):
-        return await self._request_margin_api('get', 'margin/forceLiquidationRec', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/forceLiquidationRec", signed=True, data=params)
 
     async def get_margin_order(self, **params):
-        return await self._request_margin_api('get', 'margin/order', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/order", signed=True, data=params)
 
     async def get_open_margin_orders(self, **params):
-        return await self._request_margin_api('get', 'margin/openOrders', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/openOrders", signed=True, data=params)
 
     async def get_all_margin_orders(self, **params):
-        return await self._request_margin_api('get', 'margin/allOrders', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/allOrders", signed=True, data=params)
 
     async def get_margin_trades(self, **params):
-        return await self._request_margin_api('get', 'margin/myTrades', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/myTrades", signed=True, data=params)
 
     async def get_max_margin_loan(self, **params):
-        return await self._request_margin_api('get', 'margin/maxBorrowable', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/maxBorrowable", signed=True, data=params)
 
     async def get_max_margin_transfer(self, **params):
-        return await self._request_margin_api('get', 'margin/maxTransferable', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/maxTransferable", signed=True, data=params)
 
     # Margin OCO
 
     async def create_margin_oco_order(self, **params):
-        return await self._request_margin_api('post', 'margin/order/oco', signed=True, data=params)
+        return await self._request_margin_api("post", "margin/order/oco", signed=True, data=params)
 
     async def cancel_margin_oco_order(self, **params):
-        return await self._request_margin_api('delete', 'margin/orderList', signed=True, data=params)
+        return await self._request_margin_api("delete", "margin/orderList", signed=True, data=params)
 
     async def get_margin_oco_order(self, **params):
-        return await self._request_margin_api('get', 'margin/orderList', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/orderList", signed=True, data=params)
 
     async def get_open_margin_oco_orders(self, **params):
-        return await self._request_margin_api('get', 'margin/allOrderList', signed=True, data=params)
+        return await self._request_margin_api("get", "margin/allOrderList", signed=True, data=params)
 
     # Cross-margin
 
     async def margin_stream_get_listen_key(self):
-        res = await self._request_margin_api('post', 'userDataStream', signed=False, data={})
-        return res['listenKey']
+        res = await self._request_margin_api("post", "userDataStream", signed=False, data={})
+        return res["listenKey"]
 
-    async def margin_stream_keepalive(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._request_margin_api('put', 'userDataStream', signed=False, data=params)
+    async def margin_stream_keepalive(self):
+        return await self._request_margin_api("put", "userDataStream", signed=False, data={})
 
-    async def margin_stream_close(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._request_margin_api('delete', 'userDataStream', signed=False, data=params)
+    async def margin_stream_close(self):
+        return await self._request_margin_api("delete", "userDataStream", signed=False, data={})
 
         # Isolated margin
 
     async def isolated_margin_stream_get_listen_key(self, symbol):
-        params = {
-            'symbol': symbol
-        }
-        res = await self._request_margin_api('post', 'userDataStream/isolated', signed=False, data=params)
-        return res['listenKey']
+        params = {"symbol": symbol}
+        res = await self._request_margin_api("post", "userDataStream/isolated", signed=False, data=params)
+        return res["listenKey"]
 
     async def isolated_margin_stream_keepalive(self, symbol, listenKey):
-        params = {
-            'symbol': symbol,
-            'listenKey': listenKey
-        }
-        return await self._request_margin_api('put', 'userDataStream/isolated', signed=False, data=params)
+        params = {"symbol": symbol, "listenKey": listenKey}
+        return await self._request_margin_api("put", "userDataStream/isolated", signed=False, data=params)
 
     async def isolated_margin_stream_close(self, symbol, listenKey):
-        params = {
-            'symbol': symbol,
-            'listenKey': listenKey
-        }
-        return await self._request_margin_api('delete', 'userDataStream/isolated', signed=False, data=params)
+        params = {"symbol": symbol, "listenKey": listenKey}
+        return await self._request_margin_api("delete", "userDataStream/isolated", signed=False, data=params)
 
     # Lending Endpoints
 
     async def get_lending_product_list(self, **params):
-        return await self._request_margin_api('get', 'lending/daily/product/list', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/daily/product/list", signed=True, data=params)
 
     async def get_lending_daily_quota_left(self, **params):
-        return await self._request_margin_api('get', 'lending/daily/userLeftQuota', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/daily/userLeftQuota", signed=True, data=params)
 
     async def purchase_lending_product(self, **params):
-        return await self._request_margin_api('post', 'lending/daily/purchase', signed=True, data=params)
+        return await self._request_margin_api("post", "lending/daily/purchase", signed=True, data=params)
 
     async def get_lending_daily_redemption_quota(self, **params):
-        return await self._request_margin_api('get', 'lending/daily/userRedemptionQuota', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/daily/userRedemptionQuota", signed=True, data=params)
 
     async def redeem_lending_product(self, **params):
-        return await self._request_margin_api('post', 'lending/daily/redeem', signed=True, data=params)
+        return await self._request_margin_api("post", "lending/daily/redeem", signed=True, data=params)
 
     async def get_lending_position(self, **params):
-        return await self._request_margin_api('get', 'lending/daily/token/position', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/daily/token/position", signed=True, data=params)
 
     async def get_fixed_activity_project_list(self, **params):
-        return await self._request_margin_api('get', 'lending/project/list', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/project/list", signed=True, data=params)
 
     async def get_lending_account(self, **params):
-        return await self._request_margin_api('get', 'lending/union/account', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/union/account", signed=True, data=params)
 
     async def get_lending_purchase_history(self, **params):
-        return await self._request_margin_api('get', 'lending/union/purchaseRecord', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/union/purchaseRecord", signed=True, data=params)
 
     async def get_lending_redemption_history(self, **params):
-        return await self._request_margin_api('get', 'lending/union/redemptionRecord', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/union/redemptionRecord", signed=True, data=params)
 
     async def get_lending_interest_history(self, **params):
-        return await self._request_margin_api('get', 'lending/union/interestHistory', signed=True, data=params)
+        return await self._request_margin_api("get", "lending/union/interestHistory", signed=True, data=params)
 
     async def change_fixed_activity_to_daily_position(self, **params):
-        return await self._request_margin_api('post', 'lending/positionChanged', signed=True, data=params)
+        return await self._request_margin_api("post", "lending/positionChanged", signed=True, data=params)
 
     # Sub Accounts
 
     async def get_sub_account_list(self, **params):
-        return await self._request_margin_api('get', 'sub-account/list', True, data=params)
+        return await self._request_margin_api("get", "sub-account/list", True, data=params)
 
     async def get_sub_account_transfer_history(self, **params):
-        return await self._request_margin_api('get', 'sub-account/sub/transfer/history', True, data=params)
+        return await self._request_margin_api("get", "sub-account/sub/transfer/history", True, data=params)
 
     async def get_sub_account_futures_transfer_history(self, **params):
-        return await self._request_margin_api('get', 'sub-account/futures/internalTransfer', True, data=params)
+        return await self._request_margin_api("get", "sub-account/futures/internalTransfer", True, data=params)
 
     async def create_sub_account_futures_transfer(self, **params):
-        return await self._request_margin_api('post', 'sub-account/futures/internalTransfer', True, data=params)
+        return await self._request_margin_api("post", "sub-account/futures/internalTransfer", True, data=params)
 
     async def get_sub_account_assets(self, **params):
-        return await self._request_margin_api('get', 'sub-account/assets', True, data=params)
+        return await self._request_margin_api("get", "sub-account/assets", True, data=params)
 
     async def query_subaccount_spot_summary(self, **params):
-        return await self._request_margin_api('get', 'sub-account/spotSummary', True, data=params)
+        return await self._request_margin_api("get", "sub-account/spotSummary", True, data=params)
 
     async def get_subaccount_deposit_address(self, **params):
-        return await self._request_margin_api('get', 'capital/deposit/subAddress', True, data=params)
+        return await self._request_margin_api("get", "capital/deposit/subAddress", True, data=params)
 
     async def get_subaccount_deposit_history(self, **params):
-        return await self._request_margin_api('get', 'capital/deposit/subHisrec', True, data=params)
+        return await self._request_margin_api("get", "capital/deposit/subHisrec", True, data=params)
 
     async def get_subaccount_futures_margin_status(self, **params):
-        return await self._request_margin_api('get', 'sub-account/status', True, data=params)
+        return await self._request_margin_api("get", "sub-account/status", True, data=params)
 
     async def enable_subaccount_margin(self, **params):
-        return await self._request_margin_api('post', 'sub-account/margin/enable', True, data=params)
+        return await self._request_margin_api("post", "sub-account/margin/enable", True, data=params)
 
     async def get_subaccount_margin_details(self, **params):
-        return await self._request_margin_api('get', 'sub-account/margin/account', True, data=params)
+        return await self._request_margin_api("get", "sub-account/margin/account", True, data=params)
 
     async def get_subaccount_margin_summary(self, **params):
-        return await self._request_margin_api('get', 'sub-account/margin/accountSummary', True, data=params)
+        return await self._request_margin_api("get", "sub-account/margin/accountSummary", True, data=params)
 
     async def enable_subaccount_futures(self, **params):
-        return await self._request_margin_api('post', 'sub-account/futures/enable', True, data=params)
+        return await self._request_margin_api("post", "sub-account/futures/enable", True, data=params)
 
     async def get_subaccount_futures_details(self, **params):
-        return await self._request_margin_api('get', 'sub-account/futures/account', True, data=params)
+        return await self._request_margin_api("get", "sub-account/futures/account", True, data=params)
 
     async def get_subaccount_futures_summary(self, **params):
-        return await self._request_margin_api('get', 'sub-account/futures/accountSummary', True, data=params)
+        return await self._request_margin_api("get", "sub-account/futures/accountSummary", True, data=params)
 
     async def get_subaccount_futures_positionrisk(self, **params):
-        return await self._request_margin_api('get', 'sub-account/futures/positionRisk', True, data=params)
+        return await self._request_margin_api("get", "sub-account/futures/positionRisk", True, data=params)
 
     async def make_subaccount_futures_transfer(self, **params):
-        return await self._request_margin_api('post', 'sub-account/futures/transfer', True, data=params)
+        return await self._request_margin_api("post", "sub-account/futures/transfer", True, data=params)
 
     async def make_subaccount_margin_transfer(self, **params):
-        return await self._request_margin_api('post', 'sub-account/margin/transfer', True, data=params)
+        return await self._request_margin_api("post", "sub-account/margin/transfer", True, data=params)
 
     async def make_subaccount_to_subaccount_transfer(self, **params):
-        return await self._request_margin_api('post', 'sub-account/transfer/subToSub', True, data=params)
+        return await self._request_margin_api("post", "sub-account/transfer/subToSub", True, data=params)
 
     async def make_subaccount_to_master_transfer(self, **params):
-        return await self._request_margin_api('post', 'sub-account/transfer/subToMaster', True, data=params)
+        return await self._request_margin_api("post", "sub-account/transfer/subToMaster", True, data=params)
 
     async def get_subaccount_transfer_history(self, **params):
-        return await self._request_margin_api('get', 'sub-account/transfer/subUserHistory', True, data=params)
+        return await self._request_margin_api("get", "sub-account/transfer/subUserHistory", True, data=params)
 
     async def make_subaccount_universal_transfer(self, **params):
-        return await self._request_margin_api('post', 'sub-account/universalTransfer', True, data=params)
+        return await self._request_margin_api("post", "sub-account/universalTransfer", True, data=params)
 
     async def get_universal_transfer_history(self, **params):
-        return await self._request_margin_api('get', 'sub-account/universalTransfer', True, data=params)
+        return await self._request_margin_api("get", "sub-account/universalTransfer", True, data=params)
 
     # Futures API
 
     async def futures_ping(self):
-        return await self._request_futures_api('get', 'ping')
+        return await self._request_futures_api("get", "ping")
 
     async def futures_time(self):
-        return await self._request_futures_api('get', 'time')
+        return await self._request_futures_api("get", "time")
 
     async def futures_exchange_info(self):
-        return await self._request_futures_api('get', 'exchangeInfo')
+        return await self._request_futures_api("get", "exchangeInfo")
 
     async def futures_order_book(self, **params):
-        return await self._request_futures_api('get', 'depth', data=params)
+        return await self._request_futures_api("get", "depth", data=params)
 
     async def futures_recent_trades(self, **params):
-        return await self._request_futures_api('get', 'trades', data=params)
+        return await self._request_futures_api("get", "trades", data=params)
 
     async def futures_historical_trades(self, **params):
-        return await self._request_futures_api('get', 'historicalTrades', data=params)
+        return await self._request_futures_api("get", "historicalTrades", data=params)
 
     async def futures_aggregate_trades(self, **params):
-        return await self._request_futures_api('get', 'aggTrades', data=params)
+        return await self._request_futures_api("get", "aggTrades", data=params)
 
     async def futures_klines(self, **params):
-        return await self._request_futures_api('get', 'klines', data=params)
+        return await self._request_futures_api("get", "klines", data=params)
 
     async def futures_continuous_klines(self, **params):
-        return await self._request_futures_api('get', 'continuousKlines', data=params)
+        return await self._request_futures_api("get", "continuousKlines", data=params)
 
     async def futures_mark_price(self, **params):
-        return await self._request_futures_api('get', 'premiumIndex', data=params)
+        return await self._request_futures_api("get", "premiumIndex", data=params)
 
     async def futures_funding_rate(self, **params):
-        return await self._request_futures_api('get', 'fundingRate', data=params)
+        return await self._request_futures_api("get", "fundingRate", data=params)
 
     async def futures_ticker(self, **params):
-        return await self._request_futures_api('get', 'ticker/24hr', data=params)
+        return await self._request_futures_api("get", "ticker/24hr", data=params)
 
     async def futures_symbol_ticker(self, **params):
-        return await self._request_futures_api('get', 'ticker/price', data=params)
+        return await self._request_futures_api("get", "ticker/price", data=params)
 
     async def futures_orderbook_ticker(self, **params):
-        return await self._request_futures_api('get', 'ticker/bookTicker', data=params)
+        return await self._request_futures_api("get", "ticker/bookTicker", data=params)
 
     async def futures_liquidation_orders(self, **params):
-        return await self._request_futures_api('get', 'forceOrders', signed=True, data=params)
+        return await self._request_futures_api("get", "forceOrders", signed=True, data=params)
 
     async def futures_adl_quantile_estimate(self, **params):
-        return await self._request_futures_api('get', 'adlQuantile', signed=True, data=params)
+        return await self._request_futures_api("get", "adlQuantile", signed=True, data=params)
 
     async def futures_open_interest(self, **params):
-        return await self._request_futures_api('get', 'openInterest', data=params)
+        return await self._request_futures_api("get", "openInterest", data=params)
 
     async def futures_open_interest_hist(self, **params):
-        return await self._request_futures_data_api('get', 'openInterestHist', data=params)
+        return await self._request_futures_data_api("get", "openInterestHist", data=params)
 
     async def futures_leverage_bracket(self, **params):
-        return await self._request_futures_api('get', 'leverageBracket', True, data=params)
+        return await self._request_futures_api("get", "leverageBracket", True, data=params)
 
     async def futures_account_transfer(self, **params):
-        return await self._request_margin_api('post', 'futures/transfer', True, data=params)
+        return await self._request_margin_api("post", "futures/transfer", True, data=params)
 
     async def transfer_history(self, **params):
-        return await self._request_margin_api('get', 'futures/transfer', True, data=params)
+        return await self._request_margin_api("get", "futures/transfer", True, data=params)
 
     async def futures_create_order(self, **params):
-        return await self._request_futures_api('post', 'order', True, data=params)
+        return await self._request_futures_api("post", "order", True, data=params)
 
     async def futures_create_twap_order(self, **params):
-        return await self._request_margin_api('post', 'algo/futures/newOrderTwap', True, force_params=True, data=params)
+        return await self._request_margin_api("post", "algo/futures/newOrderTwap", True, force_params=True, data=params)
 
     async def futures_create_vp_order(self, **params):
-        return await self._request_margin_api('post', 'algo/futures/newOrderVp', True, force_params=True, data=params)
+        return await self._request_margin_api("post", "algo/futures/newOrderVp", True, force_params=True, data=params)
 
     async def futures_cancel_algo_order(self, **params):
-        return await self._request_margin_api('delete', 'algo/futures/order', True, force_params=True, data=params)
+        return await self._request_margin_api("delete", "algo/futures/order", True, force_params=True, data=params)
 
     async def futures_get_algo_open_orders(self, **params):
-        return await self._request_margin_api('get', 'algo/futures/openOrders', True, data=params)
+        return await self._request_margin_api("get", "algo/futures/openOrders", True, data=params)
 
     async def futures_get_algo_historical_orders(self, **params):
-        return await self._request_margin_api('get', 'algo/futures/historicalOrders', True, data=params)
+        return await self._request_margin_api("get", "algo/futures/historicalOrders", True, data=params)
 
     async def futures_get_algo_suborders(self, **params):
-        return await self._request_margin_api('get', 'algo/futures/subOrders', True, data=params)
+        return await self._request_margin_api("get", "algo/futures/subOrders", True, data=params)
 
     async def get_staking_products(self, **params):
-        return await self._request_margin_api('get', 'staking/productList', True, data=params)
+        return await self._request_margin_api("get", "staking/productList", True, data=params)
 
     async def purchase_staking(self, **params):
-        return await self._request_margin_api('post', 'staking/purchase', True, data=params)
+        return await self._request_margin_api("post", "staking/purchase", True, data=params)
 
     async def redeem_staking(self, **params):
-        return await self._request_margin_api('post', 'staking/redeem', True, data=params)
+        return await self._request_margin_api("post", "staking/redeem", True, data=params)
 
     async def get_staking_position(self, **params):
-        return await self._request_margin_api('get', 'staking/position', True, data=params)
+        return await self._request_margin_api("get", "staking/position", True, data=params)
 
     async def get_staking_purchase_history(self, **params):
-        return self._request_margin_api('get', 'staking/purchaseRecord', True, data=params)
+        return self._request_margin_api("get", "staking/purchaseRecord", True, data=params)
 
     async def set_auto_staking(self, **params):
-        return await self._request_margin_api('post', 'staking/setAutoStaking', True, data=params)
+        return await self._request_margin_api("post", "staking/setAutoStaking", True, data=params)
 
     async def get_personal_left_quota(self, **params):
-        return await self._request_margin_api('get', 'staking/personalLeftQuota', True, data=params)
+        return await self._request_margin_api("get", "staking/personalLeftQuota", True, data=params)
 
     async def futures_place_batch_order(self, **params):
         query_string = urlencode(params)
-        query_string = query_string.replace('%27', '%22')
-        params['batchOrders'] = query_string[12:]
-        return await self._request_futures_api('post', 'batchOrders', True, data=params)
+        query_string = query_string.replace("%27", "%22")
+        params["batchOrders"] = query_string[12:]
+        return await self._request_futures_api("post", "batchOrders", True, data=params)
 
     async def futures_get_order(self, **params):
-        return await self._request_futures_api('get', 'order', True, data=params)
+        return await self._request_futures_api("get", "order", True, data=params)
 
     async def futures_get_open_orders(self, **params):
-        return await self._request_futures_api('get', 'openOrders', True, data=params)
+        return await self._request_futures_api("get", "openOrders", True, data=params)
 
     async def futures_get_all_orders(self, **params):
-        return await self._request_futures_api('get', 'allOrders', True, data=params)
+        return await self._request_futures_api("get", "allOrders", True, data=params)
 
     async def futures_cancel_order(self, **params):
-        return await self._request_futures_api('delete', 'order', True, data=params)
+        return await self._request_futures_api("delete", "order", True, data=params)
 
     async def futures_cancel_all_open_orders(self, **params):
-        return await self._request_futures_api('delete', 'allOpenOrders', True, data=params)
+        return await self._request_futures_api("delete", "allOpenOrders", True, data=params)
 
     async def futures_cancel_orders(self, **params):
-        return await self._request_futures_api('delete', 'batchOrders', True, data=params)
+        return await self._request_futures_api("delete", "batchOrders", True, data=params)
 
     async def futures_account_balance(self, **params):
-        return await self._request_futures_api('get', 'balance', True, data=params)
+        return await self._request_futures_api("get", "balance", True, data=params)
 
     async def futures_account(self, **params):
-        return await self._request_futures_api('get', 'account', True, data=params)
+        return await self._request_futures_api("get", "account", True, data=params, version=2)
 
     async def futures_change_leverage(self, **params):
-        return await self._request_futures_api('post', 'leverage', True, data=params)
+        return await self._request_futures_api("post", "leverage", True, data=params)
 
     async def futures_change_margin_type(self, **params):
-        return await self._request_futures_api('post', 'marginType', True, data=params)
+        return await self._request_futures_api("post", "marginType", True, data=params)
 
     async def futures_change_position_margin(self, **params):
-        return await self._request_futures_api('post', 'positionMargin', True, data=params)
+        return await self._request_futures_api("post", "positionMargin", True, data=params)
 
     async def futures_position_margin_history(self, **params):
-        return await self._request_futures_api('get', 'positionMargin/history', True, data=params)
+        return await self._request_futures_api("get", "positionMargin/history", True, data=params)
 
     async def futures_position_information(self, **params):
-        return await self._request_futures_api('get', 'positionRisk', True, data=params)
+        return await self._request_futures_api("get", "positionRisk", True, data=params)
 
     async def futures_account_trades(self, **params):
-        return await self._request_futures_api('get', 'userTrades', True, data=params)
+        return await self._request_futures_api("get", "userTrades", True, data=params)
 
     async def futures_income_history(self, **params):
-        return await self._request_futures_api('get', 'income', True, data=params)
+        return await self._request_futures_api("get", "income", True, data=params)
 
     async def futures_change_position_mode(self, **params):
-        return await self._request_futures_api('post', 'positionSide/dual', True, data=params)
+        return await self._request_futures_api("post", "positionSide/dual", True, data=params)
 
     async def futures_get_position_mode(self, **params):
-        return await self._request_futures_api('get', 'positionSide/dual', True, data=params)
+        return await self._request_futures_api("get", "positionSide/dual", True, data=params)
 
     async def futures_change_multi_assets_mode(self, multiAssetsMargin: bool):
-        params = {
-            'multiAssetsMargin': 'true' if multiAssetsMargin else 'false'
-        }
-        return await self._request_futures_api('post', 'multiAssetsMargin', True, data=params)
+        params = {"multiAssetsMargin": "true" if multiAssetsMargin else "false"}
+        return await self._request_futures_api("post", "multiAssetsMargin", True, data=params)
 
     async def futures_get_multi_assets_mode(self):
-        return await self._request_futures_api('get', 'multiAssetsMargin', True, data={})
+        return await self._request_futures_api("get", "multiAssetsMargin", True, data={})
 
     async def futures_stream_get_listen_key(self):
-        res = await self._request_futures_api('post', 'listenKey', signed=False, data={})
-        return res['listenKey']
+        res = await self._request_futures_api("post", "listenKey", signed=False, data={})
+        return res["listenKey"]
 
-    async def futures_stream_keepalive(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._request_futures_api('put', 'listenKey', signed=False, data=params)
+    async def futures_stream_keepalive(self):
+        return await self._request_futures_api("put", "listenKey", signed=False, data={})
 
-    async def futures_stream_close(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._request_futures_api('delete', 'listenKey', signed=False, data=params)
+    async def futures_stream_close(self):
+        return await self._request_futures_api("delete", "listenKey", signed=False, data={})
 
     # COIN Futures API
 
     async def futures_coin_ping(self):
         return await self._request_futures_coin_api("get", "ping")
 
     async def futures_coin_time(self):
@@ -1191,18 +1189,18 @@
         return await self._request_margin_api("post", "asset/transfer", signed=True, data=params)
 
     async def futures_coin_create_order(self, **params):
         return await self._request_futures_coin_api("post", "order", True, data=params)
 
     async def futures_coin_place_batch_order(self, **params):
         query_string = urlencode(params)
-        query_string = query_string.replace('%27', '%22')
-        params['batchOrders'] = query_string[12:]
+        query_string = query_string.replace("%27", "%22")
+        params["batchOrders"] = query_string[12:]
 
-        return await self._request_futures_coin_api('post', 'batchOrders', True, data=params)
+        return await self._request_futures_coin_api("post", "batchOrders", True, data=params)
 
     async def futures_coin_get_order(self, **params):
         return await self._request_futures_coin_api("get", "order", True, data=params)
 
     async def futures_coin_get_open_orders(self, **params):
         return await self._request_futures_coin_api("get", "openOrders", True, data=params)
 
@@ -1248,166 +1246,426 @@
     async def futures_coin_change_position_mode(self, **params):
         return await self._request_futures_coin_api("post", "positionSide/dual", True, data=params)
 
     async def futures_coin_get_position_mode(self, **params):
         return await self._request_futures_coin_api("get", "positionSide/dual", True, data=params)
 
     async def futures_coin_stream_get_listen_key(self):
-        res = await self._request_futures_coin_api('post', 'listenKey', signed=False, data={})
-        return res['listenKey']
+        res = await self._request_futures_coin_api("post", "listenKey", signed=False, data={})
+        return res["listenKey"]
 
-    async def futures_coin_stream_keepalive(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._request_futures_coin_api('put', 'listenKey', signed=False, data=params)
+    async def futures_coin_stream_keepalive(self):
+        return await self._request_futures_coin_api("put", "listenKey", signed=False, data={})
 
-    async def futures_coin_stream_close(self, listenKey):
-        params = {
-            'listenKey': listenKey
-        }
-        return await self._request_futures_coin_api('delete', 'listenKey', signed=False, data=params)
+    async def futures_coin_stream_close(self):
+        return await self._request_futures_coin_api("delete", "listenKey", signed=False, data={})
 
     async def get_all_coins_info(self, **params):
-        return await self._request_margin_api('get', 'capital/config/getall', True, data=params)
+        return await self._request_margin_api("get", "capital/config/getall", True, data=params)
 
     async def get_account_snapshot(self, **params):
-        return await self._request_margin_api('get', 'accountSnapshot', True, data=params)
+        return await self._request_margin_api("get", "accountSnapshot", True, data=params)
 
     async def disable_fast_withdraw_switch(self, **params):
-        return await self._request_margin_api('post', 'disableFastWithdrawSwitch', True, data=params)
+        return await self._request_margin_api("post", "disableFastWithdrawSwitch", True, data=params)
 
     async def enable_fast_withdraw_switch(self, **params):
-        return await self._request_margin_api('post', 'enableFastWithdrawSwitch', True, data=params)
+        return await self._request_margin_api("post", "enableFastWithdrawSwitch", True, data=params)
 
     """
     ====================================================================================================================
     Options API
     ====================================================================================================================
     """
 
     # Quoting interface endpoints
 
     async def options_ping(self):
-        return await self._request_options_api('get', 'ping')
+        return await self._request_options_api("get", "ping")
 
     async def options_time(self):
-        return await self._request_options_api('get', 'time')
+        return await self._request_options_api("get", "time")
 
     async def options_info(self):
-        return await self._request_options_api('get', 'optionInfo')
+        return await self._request_options_api("get", "optionInfo")
 
     async def options_exchange_info(self):
-        return await self._request_options_api('get', 'exchangeInfo')
+        return await self._request_options_api("get", "exchangeInfo")
 
     async def options_index_price(self, **params):
-        return await self._request_options_api('get', 'index', data=params)
+        return await self._request_options_api("get", "index", data=params)
 
     async def options_price(self, **params):
-        return await self._request_options_api('get', 'ticker', data=params)
+        return await self._request_options_api("get", "ticker", data=params)
 
     async def options_mark_price(self, **params):
-        return await self._request_options_api('get', 'mark', data=params)
+        return await self._request_options_api("get", "mark", data=params)
 
     async def options_order_book(self, **params):
-        return await self._request_options_api('get', 'depth', data=params)
+        return await self._request_options_api("get", "depth", data=params)
 
     async def options_klines(self, **params):
-        return await self._request_options_api('get', 'klines', data=params)
+        return await self._request_options_api("get", "klines", data=params)
 
     async def options_recent_trades(self, **params):
-        return await self._request_options_api('get', 'trades', data=params)
+        return await self._request_options_api("get", "trades", data=params)
 
     async def options_historical_trades(self, **params):
-        return await self._request_options_api('get', 'historicalTrades', data=params)
+        return await self._request_options_api("get", "historicalTrades", data=params)
 
     # Account and trading interface endpoints
 
     async def options_account_info(self, **params):
-        return await self._request_options_api('get', 'account', signed=True, data=params)
+        return await self._request_options_api("get", "account", signed=True, data=params)
 
     async def options_funds_transfer(self, **params):
-        return await self._request_options_api('post', 'transfer', signed=True, data=params)
+        return await self._request_options_api("post", "transfer", signed=True, data=params)
 
     async def options_positions(self, **params):
-        return await self._request_options_api('get', 'position', signed=True, data=params)
+        return await self._request_options_api("get", "position", signed=True, data=params)
 
     async def options_bill(self, **params):
-        return await self._request_options_api('post', 'bill', signed=True, data=params)
+        return await self._request_options_api("post", "bill", signed=True, data=params)
 
     async def options_place_order(self, **params):
-        return await self._request_options_api('post', 'order', signed=True, data=params)
+        return await self._request_options_api("post", "order", signed=True, data=params)
 
     async def options_place_batch_order(self, **params):
-        return await self._request_options_api('post', 'batchOrders', signed=True, data=params)
+        return await self._request_options_api("post", "batchOrders", signed=True, data=params)
 
     async def options_cancel_order(self, **params):
-        return await self._request_options_api('delete', 'order', signed=True, data=params)
+        return await self._request_options_api("delete", "order", signed=True, data=params)
 
     async def options_cancel_batch_order(self, **params):
-        return await self._request_options_api('delete', 'batchOrders', signed=True, data=params)
+        return await self._request_options_api("delete", "batchOrders", signed=True, data=params)
 
     async def options_cancel_all_orders(self, **params):
-        return await self._request_options_api('delete', 'allOpenOrders', signed=True, data=params)
+        return await self._request_options_api("delete", "allOpenOrders", signed=True, data=params)
 
     async def options_query_order(self, **params):
-        return await self._request_options_api('get', 'order', signed=True, data=params)
+        return await self._request_options_api("get", "order", signed=True, data=params)
 
     async def options_query_pending_orders(self, **params):
-        return await self._request_options_api('get', 'openOrders', signed=True, data=params)
+        return await self._request_options_api("get", "openOrders", signed=True, data=params)
 
     async def options_query_order_history(self, **params):
-        return await self._request_options_api('get', 'historyOrders', signed=True, data=params)
+        return await self._request_options_api("get", "historyOrders", signed=True, data=params)
 
     async def options_user_trades(self, **params):
-        return await self._request_options_api('get', 'userTrades', signed=True, data=params)
+        return await self._request_options_api("get", "userTrades", signed=True, data=params)
 
     # Fiat Endpoints
 
     async def get_fiat_deposit_withdraw_history(self, **params):
-        return await self._request_margin_api('get', 'fiat/orders', signed=True, data=params)
+        return await self._request_margin_api("get", "fiat/orders", signed=True, data=params)
 
     async def get_fiat_payments_history(self, **params):
-        return await self._request_margin_api('get', 'fiat/payments', signed=True, data=params)
+        return await self._request_margin_api("get", "fiat/payments", signed=True, data=params)
+
+    # Portfolio Margin Endpoints
+    async def portfolio_margin_ping(self):
+        return await self._request_portfolio_margin_api("get", "ping")
+
+    async def portfolio_margin_new_um_order(self, **params):
+        return await self._request_portfolio_margin_api("post", "um/order", signed=True, data=params)
+
+    async def portfolio_margin_new_cm_order(self, **params):
+        return await self._request_portfolio_margin_api("post", "cm/order", signed=True, data=params)
+
+    async def portfolio_margin_new_margin_order(self, **params):
+        return await self._request_portfolio_margin_api("post", "margin/order", signed=True, data=params)
+
+    async def portfolio_margin_margin_account_borrow(self, **params):
+        return await self._request_portfolio_margin_api("post", "marginLoan", signed=True, data=params)
+
+    async def portfolio_margin_margin_account_repay(self, **params):
+        return await self._request_portfolio_margin_api("post", "repayLoan", signed=True, data=params)
+
+    async def portfolio_margin_margin_account_new_oco(self, **params):
+        return await self._request_portfolio_margin_api("post", "margin/order/oco", signed=True, data=params)
+
+    async def portfolio_margin_new_um_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("post", "um/conditional/order", signed=True, data=params)
+
+    async def portfolio_margin_new_cm_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("post", "cm/conditional/order", signed=True, data=params)
+
+    async def portfolio_margin_cancel_um_order(self, **params):
+        return await self._request_portfolio_margin_api("delete", "um/order", signed=True, data=params)
+
+    async def portfolio_margin_cancel_all_um_orders(self, **params):
+        return await self._request_portfolio_margin_api("delete", "um/allOpenOrders", signed=True, data=params)
+
+    async def portfolio_margin_cancel_cm_order(self, **params):
+        return await self._request_portfolio_margin_api("delete", "cm/order", signed=True, data=params)
+
+    async def portfolio_margin_cancel_all_cm_orders(self, **params):
+        return await self._request_portfolio_margin_api("delete", "cm/allOpenOrders", signed=True, data=params)
+
+    async def portfolio_margin_cancel_margin_account_order(self, **params):
+        return await self._request_portfolio_margin_api("delete", "margin/order", signed=True, data=params)
+
+    async def portfolio_margin_cancel_margin_account_all_orders(self, **params):
+        return await self._request_portfolio_margin_api("delete", "margin/allOpenOrders", signed=True, data=params)
+
+    async def portfolio_margin_cancel_margin_oco_orders(self, **params):
+        return await self._request_portfolio_margin_api("delete", "margin/orderList", signed=True, data=params)
+
+    async def portfolio_margin_cancel_um_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("delete", "um/conditional/order", signed=True, data=params)
+
+    async def portfolio_margin_cancel_all_um_conditional_orders(self, **params):
+        return await self._request_portfolio_margin_api(
+            "delete", "um/conditional/allOpenOrders", signed=True, data=params
+        )
+
+    async def portfolio_margin_cancel_cm_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("delete", "cm/conditional/order", signed=True, data=params)
+
+    async def portfolio_margin_cancel_all_cm_conditional_orders(self, **params):
+        return await self._request_portfolio_margin_api(
+            "delete", "cm/conditional/allOpenOrders", signed=True, data=params
+        )
+
+    async def portfolio_margin_query_um_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/order", signed=True, data=params)
+
+    async def portfolio_margin_query_current_um_open_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/openOrder", signed=True, data=params)
+
+    async def portfolio_margin_query_all_current_um_open_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/openOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_all_um_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/allOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_cm_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/order", signed=True, data=params)
+
+    async def portfolio_margin_query_current_cm_open_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/openOrder", signed=True, data=params)
+
+    async def portfolio_margin_query_all_current_cm_open_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/openOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_all_cm_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/allOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_current_um_open_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/conditional/openOrder", signed=True, data=params)
+
+    async def portfolio_margin_query_all_current_um_open_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/conditional/openOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_um_conditional_order_history(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/conditional/orderHistory", signed=True, data=params)
+
+    async def portfolio_margin_query_all_um_conditional_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/conditional/allOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_current_cm_open_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/conditional/openOrder", signed=True, data=params)
+
+    async def portfolio_margin_query_all_current_cm_open_conditional_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/conditional/openOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_cm_conditional_order_history(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/conditional/orderHistory", signed=True, data=params)
+
+    async def portfolio_margin_query_all_cm_conditional_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/conditional/allOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_margin_account_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/order", signed=True, data=params)
+
+    async def portfolio_margin_query_current_margin_open_order(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/openOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_all_margin_account_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/allOrders", signed=True, data=params)
+
+    async def portfolio_margin_query_margin_account_oco(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/orderList", signed=True, data=params)
+
+    async def portfolio_margin_query_margin_account_all_oco(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/allOrderList", signed=True, data=params)
+
+    async def portfolio_margin_query_margin_account_open_oco(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/openOrderList", signed=True, data=params)
+
+    async def portfolio_margin_margin_account_trade_list(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/myTrades", signed=True, data=params)
+
+    async def portfolio_margin_balance(self, **params):
+        return await self._request_portfolio_margin_api("get", "balance", signed=True, data=params)
+
+    async def portfolio_margin_account(self, **params):
+        return await self._request_portfolio_margin_api("get", "account", signed=True, data=params)
+
+    async def portfolio_margin_max_borrowable(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/maxBorrowable", signed=True, data=params)
+
+    async def portfolio_margin_max_withdraw(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/maxWithdraw", signed=True, data=params)
+
+    async def portfolio_margin_um_position_information(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/positionRisk", signed=True, data=params)
+
+    async def portfolio_margin_cm_position_information(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/positionRisk", signed=True, data=params)
+
+    async def portfolio_margin_um_leverage(self, **params):
+        return await self._request_portfolio_margin_api("post", "um/leverage", signed=True, data=params)
+
+    async def portfolio_margin_cm_leverage(self, **params):
+        return await self._request_portfolio_margin_api("post", "cm/leverage", signed=True, data=params)
+
+    async def portfolio_margin_change_um_position_mode(self, **params):
+        return await self._request_portfolio_margin_api("post", "um/positionSide/dual", signed=True, data=params)
+
+    async def portfolio_margin_change_cm_position_mode(self, **params):
+        return await self._request_portfolio_margin_api("post", "cm/positionSide/dual", signed=True, data=params)
+
+    async def portfolio_margin_um_position_mode(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/positionSide/dual", signed=True, data=params)
+
+    async def portfolio_margin_cm_position_mode(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/positionSide/dual", signed=True, data=params)
+
+    async def portfolio_margin_um_account_trade_list(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/userTrades", signed=True, data=params)
+
+    async def portfolio_margin_cm_account_trade_list(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/userTrades", signed=True, data=params)
+
+    async def portfolio_margin_um_leverage_bracket(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/leverageBracket", signed=True, data=params)
+
+    async def portfolio_margin_cm_leverage_bracket(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/leverageBracket", signed=True, data=params)
+
+    async def portfolio_margin_user_force_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/forceOrders", signed=True, data=params)
+
+    async def portfolio_margin_um_force_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/forceOrders", signed=True, data=params)
+
+    async def portfolio_margin_cm_force_orders(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/forceOrders", signed=True, data=params)
+
+    async def portfolio_margin_um_trading_quantitative_rules(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/apiTradingStatus", signed=True, data=params)
+
+    async def portfolio_margin_um_commission_rate(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/commissionRate", signed=True, data=params)
+
+    async def portfolio_margin_cm_commission_rate(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/commissionRate", signed=True, data=params)
+
+    async def portfolio_margin_margin_loan_record(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/marginLoan", signed=True, data=params)
+
+    async def portfolio_margin_margin_repay_record(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/repayLoan", signed=True, data=params)
+
+    async def portfolio_margin_margin_interest_history(self, **params):
+        return await self._request_portfolio_margin_api("get", "margin/marginInterestHistory", signed=True, data=params)
+
+    async def portfolio_margin_negative_balance_interest_history(self, **params):
+        return await self._request_portfolio_margin_api("get", "portfolio/interest-history", signed=True, data=params)
+
+    async def portfolio_margin_fund_auto_collection(self, **params):
+        return await self._request_portfolio_margin_api("post", "auto-collection", signed=True, data=params)
+
+    async def portfolio_margin_fund_collection_by_asset(self, **params):
+        return await self._request_portfolio_margin_api("post", "asset-collection", signed=True, data=params)
+
+    async def portfolio_margin_bnb_transfer(self, **params):
+        return await self._request_portfolio_margin_api("post", "bnb-transfer", signed=True, data=params)
+
+    async def portfolio_margin_um_income_history(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/income", signed=True, data=params)
+
+    async def portfolio_margin_cm_income_history(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/income", signed=True, data=params)
+
+    async def portfolio_margin_um_account_detail(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/account", signed=True, data=params)
+
+    async def portfolio_margin_cm_account_detail(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/account", signed=True, data=params)
+
+    async def portfolio_margin_change_auto_repay_futures_status(self, **params):
+        return await self._request_portfolio_margin_api("post", "repay-futures-switch", signed=True, data=params)
+
+    async def portfolio_margin_get_auto_repay_futures_status(self, **params):
+        return await self._request_portfolio_margin_api("get", "repay-futures-switch", signed=True, data=params)
+
+    async def portfolio_margin_repay_futures_negative_balance(self, **params):
+        return await self._request_portfolio_margin_api(
+            "post", "repay-futures-negative-balance", signed=True, data=params
+        )
+
+    async def portfolio_margin_um_position_adl_quantile(self, **params):
+        return await self._request_portfolio_margin_api("get", "um/adlQuantile", signed=True, data=params)
+
+    async def portfolio_margin_cm_position_adl_quantile(self, **params):
+        return await self._request_portfolio_margin_api("get", "cm/adlQuantile", signed=True, data=params)
+
+    async def portfolio_margin_stream_get_listen_key(self) -> str:
+        res = await self._request_portfolio_margin_api("post", "listenKey", signed=False, data={})
+        return res["listenKey"]
+
+    async def portfolio_margin_stream_keepalive(self) -> dict:
+        """
+        @return: empty dict {}
+        """
+        return await self._request_portfolio_margin_api("put", "listenKey", signed=False, data={})
+
+    async def portfolio_margin_stream_close(self) -> dict:
+        """
+        @return: empty dict {}
+        """
+        return await self._request_portfolio_margin_api("delete", "listenKey", signed=False, data={})
 
     # C2C Endpoints
 
     async def get_c2c_trade_history(self, **params):
-        return await self._request_margin_api('get', 'c2c/orderMatch/listUserOrderHistory', signed=True, data=params)
+        return await self._request_margin_api("get", "c2c/orderMatch/listUserOrderHistory", signed=True, data=params)
 
     # Crypto Loans Endpoints
 
     async def get_crypto_loans_income_history(self, **params):
-        return await self._request_margin_api('get', 'loan/income', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/income", signed=True, data=params)
 
     async def borrow_crypto_loans(self, **params):
-        return await self._request_margin_api('post', 'loan/borrow', signed=True, data=params)
+        return await self._request_margin_api("post", "loan/borrow", signed=True, data=params)
 
     async def get_loan_borrow_history(self, **params):
-        return await self._request_margin_api('get', 'loan/borrow/history', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/borrow/history", signed=True, data=params)
 
     async def get_loan_ongoing_orders(self, **params):
-        return await self._request_margin_api('get', 'loan/ongoing/orders', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/ongoing/orders", signed=True, data=params)
 
     async def repay_crypto_loans(self, **params):
-        return await self._request_margin_api('post', 'loan/repay', signed=True, data=params)
+        return await self._request_margin_api("post", "loan/repay", signed=True, data=params)
 
     async def get_loan_repayment_history(self, **params):
-        return await self._request_margin_api('get', 'loan/repay/history', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/repay/history", signed=True, data=params)
 
     async def crypto_loan_adjust_ltv(self, **params):
-        return await self._request_margin_api('post', 'loan/adjust/ltv', signed=True, data=params)
+        return await self._request_margin_api("post", "loan/adjust/ltv", signed=True, data=params)
 
     async def get_loan_ltv_adjustments_history(self, **params):
-        return await self._request_margin_api('get', 'loan/ltv/adjustments/history', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/ltv/adjustments/history", signed=True, data=params)
 
     async def get_loanable_assets_data(self, **params):
-        return await self._request_margin_api('get', 'loan/loanable/data', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/loanable/data", signed=True, data=params)
 
     async def get_collateral_assets_data(self, **params):
-        return await self._request_margin_api('get', 'loan/collateral/data', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/collateral/data", signed=True, data=params)
 
     async def get_collateral_repay_rate(self, **params):
-        return await self._request_margin_api('get', 'loan/repay/collateral/rate', signed=True, data=params)
+        return await self._request_margin_api("get", "loan/repay/collateral/rate", signed=True, data=params)
 
     async def customize_crypto_loan_margin_call(self, **params):
-        return await self._request_margin_api('post', 'loan/customize/margin_call', signed=True, data=params)
+        return await self._request_margin_api("post", "loan/customize/margin_call", signed=True, data=params)
```

### Comparing `trio-binance-0.2.2/trio_binance/enums.py` & `trio_binance-0.3.0/trio_binance/enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 from enum import Enum
 
-SYMBOL_TYPE_SPOT = 'SPOT'
+SYMBOL_TYPE_SPOT = "SPOT"
 
-ORDER_STATUS_NEW = 'NEW'
-ORDER_STATUS_PARTIALLY_FILLED = 'PARTIALLY_FILLED'
-ORDER_STATUS_FILLED = 'FILLED'
-ORDER_STATUS_CANCELED = 'CANCELED'
-ORDER_STATUS_PENDING_CANCEL = 'PENDING_CANCEL'
-ORDER_STATUS_REJECTED = 'REJECTED'
-ORDER_STATUS_EXPIRED = 'EXPIRED'
-
-KLINE_INTERVAL_1MINUTE = '1m'
-KLINE_INTERVAL_3MINUTE = '3m'
-KLINE_INTERVAL_5MINUTE = '5m'
-KLINE_INTERVAL_15MINUTE = '15m'
-KLINE_INTERVAL_30MINUTE = '30m'
-KLINE_INTERVAL_1HOUR = '1h'
-KLINE_INTERVAL_2HOUR = '2h'
-KLINE_INTERVAL_4HOUR = '4h'
-KLINE_INTERVAL_6HOUR = '6h'
-KLINE_INTERVAL_8HOUR = '8h'
-KLINE_INTERVAL_12HOUR = '12h'
-KLINE_INTERVAL_1DAY = '1d'
-KLINE_INTERVAL_3DAY = '3d'
-KLINE_INTERVAL_1WEEK = '1w'
-KLINE_INTERVAL_1MONTH = '1M'
-
-SIDE_BUY = 'BUY'
-SIDE_SELL = 'SELL'
-
-ORDER_TYPE_LIMIT = 'LIMIT'
-ORDER_TYPE_MARKET = 'MARKET'
-ORDER_TYPE_STOP_LOSS = 'STOP_LOSS'
-ORDER_TYPE_STOP_LOSS_LIMIT = 'STOP_LOSS_LIMIT'
-ORDER_TYPE_TAKE_PROFIT = 'TAKE_PROFIT'
-ORDER_TYPE_TAKE_PROFIT_LIMIT = 'TAKE_PROFIT_LIMIT'
-ORDER_TYPE_LIMIT_MAKER = 'LIMIT_MAKER'
-
-FUTURE_ORDER_TYPE_LIMIT = 'LIMIT'
-FUTURE_ORDER_TYPE_MARKET = 'MARKET'
-FUTURE_ORDER_TYPE_STOP = 'STOP'
-FUTURE_ORDER_TYPE_STOP_MARKET = 'STOP_MARKET'
-FUTURE_ORDER_TYPE_TAKE_PROFIT = 'TAKE_PROFIT'
-FUTURE_ORDER_TYPE_TAKE_PROFIT_MARKET = 'TAKE_PROFIT_MARKET'
-FUTURE_ORDER_TYPE_LIMIT_MAKER = 'LIMIT_MAKER'
-
-TIME_IN_FORCE_GTC = 'GTC'  # Good till cancelled
-TIME_IN_FORCE_IOC = 'IOC'  # Immediate or cancel
-TIME_IN_FORCE_FOK = 'FOK'  # Fill or kill
-TIME_IN_FORCE_GTX = 'GTX'  # Post only order
-
-ORDER_RESP_TYPE_ACK = 'ACK'
-ORDER_RESP_TYPE_RESULT = 'RESULT'
-ORDER_RESP_TYPE_FULL = 'FULL'
-
-WEBSOCKET_DEPTH_5 = '5'
-WEBSOCKET_DEPTH_10 = '10'
-WEBSOCKET_DEPTH_20 = '20'
+ORDER_STATUS_NEW = "NEW"
+ORDER_STATUS_PARTIALLY_FILLED = "PARTIALLY_FILLED"
+ORDER_STATUS_FILLED = "FILLED"
+ORDER_STATUS_CANCELED = "CANCELED"
+ORDER_STATUS_PENDING_CANCEL = "PENDING_CANCEL"
+ORDER_STATUS_REJECTED = "REJECTED"
+ORDER_STATUS_EXPIRED = "EXPIRED"
+
+KLINE_INTERVAL_1MINUTE = "1m"
+KLINE_INTERVAL_3MINUTE = "3m"
+KLINE_INTERVAL_5MINUTE = "5m"
+KLINE_INTERVAL_15MINUTE = "15m"
+KLINE_INTERVAL_30MINUTE = "30m"
+KLINE_INTERVAL_1HOUR = "1h"
+KLINE_INTERVAL_2HOUR = "2h"
+KLINE_INTERVAL_4HOUR = "4h"
+KLINE_INTERVAL_6HOUR = "6h"
+KLINE_INTERVAL_8HOUR = "8h"
+KLINE_INTERVAL_12HOUR = "12h"
+KLINE_INTERVAL_1DAY = "1d"
+KLINE_INTERVAL_3DAY = "3d"
+KLINE_INTERVAL_1WEEK = "1w"
+KLINE_INTERVAL_1MONTH = "1M"
+
+SIDE_BUY = "BUY"
+SIDE_SELL = "SELL"
+
+ORDER_TYPE_LIMIT = "LIMIT"
+ORDER_TYPE_MARKET = "MARKET"
+ORDER_TYPE_STOP_LOSS = "STOP_LOSS"
+ORDER_TYPE_STOP_LOSS_LIMIT = "STOP_LOSS_LIMIT"
+ORDER_TYPE_TAKE_PROFIT = "TAKE_PROFIT"
+ORDER_TYPE_TAKE_PROFIT_LIMIT = "TAKE_PROFIT_LIMIT"
+ORDER_TYPE_LIMIT_MAKER = "LIMIT_MAKER"
+
+FUTURE_ORDER_TYPE_LIMIT = "LIMIT"
+FUTURE_ORDER_TYPE_MARKET = "MARKET"
+FUTURE_ORDER_TYPE_STOP = "STOP"
+FUTURE_ORDER_TYPE_STOP_MARKET = "STOP_MARKET"
+FUTURE_ORDER_TYPE_TAKE_PROFIT = "TAKE_PROFIT"
+FUTURE_ORDER_TYPE_TAKE_PROFIT_MARKET = "TAKE_PROFIT_MARKET"
+FUTURE_ORDER_TYPE_LIMIT_MAKER = "LIMIT_MAKER"
+
+TIME_IN_FORCE_GTC = "GTC"  # Good till cancelled
+TIME_IN_FORCE_IOC = "IOC"  # Immediate or cancel
+TIME_IN_FORCE_FOK = "FOK"  # Fill or kill
+TIME_IN_FORCE_GTX = "GTX"  # Post only order
+
+ORDER_RESP_TYPE_ACK = "ACK"
+ORDER_RESP_TYPE_RESULT = "RESULT"
+ORDER_RESP_TYPE_FULL = "FULL"
+
+WEBSOCKET_DEPTH_5 = "5"
+WEBSOCKET_DEPTH_10 = "10"
+WEBSOCKET_DEPTH_20 = "20"
 
 
 class FuturesType(Enum):
     USD_M = 1
     COIN_M = 2
```

### Comparing `trio-binance-0.2.2/trio_binance/exceptions.py` & `trio_binance-0.3.0/trio_binance/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,76 @@
-# coding=utf-8
-import ujson
+import orjson
 
 
 class BinanceAPIException(Exception):
-
     def __init__(self, response, status_code, text):
         self.code = 0
         try:
-            json_res = ujson.loads(text)
+            json_res = orjson.loads(text)
         except ValueError:
-            self.message = 'Invalid JSON error message from Binance: {}'.format(response.text)
+            self.message = "Invalid JSON error message from Binance: {}".format(response.text)
         else:
-            self.code = json_res['code']
-            self.message = json_res['msg']
+            self.code = json_res["code"]
+            self.message = json_res["msg"]
         self.status_code = status_code
         self.response = response
-        self.request = getattr(response, 'request', None)
+        self.request = getattr(response, "request", None)
 
     def __str__(self):  # pragma: no cover
-        return 'APIError(code=%s): %s' % (self.code, self.message)
+        return "APIError(code=%s): %s" % (self.code, self.message)
 
 
 class BinanceRequestException(Exception):
     def __init__(self, message):
         self.message = message
 
     def __str__(self):
-        return 'BinanceRequestException: %s' % self.message
+        return "BinanceRequestException: %s" % self.message
 
 
 class BinanceOrderException(Exception):
-
     def __init__(self, code, message):
         self.code = code
         self.message = message
 
     def __str__(self):
-        return 'BinanceOrderException(code=%s): %s' % (self.code, self.message)
+        return "BinanceOrderException(code=%s): %s" % (self.code, self.message)
 
 
 class BinanceOrderMinAmountException(BinanceOrderException):
-
     def __init__(self, value):
         message = "Amount must be a multiple of %s" % value
         super().__init__(-1013, message)
 
 
 class BinanceOrderMinPriceException(BinanceOrderException):
-
     def __init__(self, value):
         message = "Price must be at least %s" % value
         super().__init__(-1013, message)
 
 
 class BinanceOrderMinTotalException(BinanceOrderException):
-
     def __init__(self, value):
         message = "Total must be at least %s" % value
         super().__init__(-1013, message)
 
 
 class BinanceOrderUnknownSymbolException(BinanceOrderException):
-
     def __init__(self, value):
         message = "Unknown symbol %s" % value
         super().__init__(-1013, message)
 
 
 class BinanceOrderInactiveSymbolException(BinanceOrderException):
-
     def __init__(self, value):
         message = "Attempting to trade an inactive symbol %s" % value
         super().__init__(-1013, message)
 
 
 class BinanceWebsocketUnableToConnect(Exception):
     pass
 
 
 class NotImplementedException(Exception):
     def __init__(self, value):
-        message = f'Not implemented: {value}'
+        message = f"Not implemented: {value}"
         super().__init__(message)
```

### Comparing `trio-binance-0.2.2/trio_binance/helpers.py` & `trio_binance-0.3.0/trio_binance/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     See dateparse docs for formats http://dateparser.readthedocs.io/en/latest/
 
     :param date_str: date in readable format, i.e. "January 01, 2018", "11 hours ago UTC", "now UTC"
     """
     # get epoch value in UTC
     epoch: datetime = datetime.utcfromtimestamp(0).replace(tzinfo=pytz.utc)
     # parse our date string
-    d: Optional[datetime] = dateparser.parse(date_str, settings={'TIMEZONE': "UTC"})
+    d: Optional[datetime] = dateparser.parse(date_str, settings={"TIMEZONE": "UTC"})
     # if the date is not timezone aware apply UTC timezone
     if d.tzinfo is None or d.tzinfo.utcoffset(d) is None:
         d = d.replace(tzinfo=pytz.utc)
 
     # return the difference in time
     return int((d - epoch).total_seconds() * 1000.0)
```

### Comparing `trio-binance-0.2.2/setup.py` & `trio_binance-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,62 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: trio-binance
+Version: 0.3.0
+Summary: trio based asynchronous binance SDK
+Home-page: https://github.com/halfelf/trio-binance
+License: MIT
+Keywords: binance,python-trio
+Author: Shu Wang
+Author-email: halfelf.ronin@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Framework :: Trio
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dateparser (>=1.1.0,<2.0.0)
+Requires-Dist: h2 (>=4.1.0,<5.0.0)
+Requires-Dist: httpx (>0.20.0)
+Requires-Dist: orjson (>=3.6.0,<4.0.0)
+Requires-Dist: pytz (>=2024.1,<2025.0)
+Requires-Dist: trio (>=0.25.0)
+Requires-Dist: trio-websocket (>=0.11.1,<0.12.0)
+Project-URL: Repository, https://github.com/halfelf/trio-binance
+Description-Content-Type: text/x-rst
+
+=================================
+Welcome to trio-binance
+=================================
+
+This is an unofficial Python wrapper for the `Binance exchange REST API v3 <https://binance-docs.github.io/apidocs/spot/en>`_. I am in no way affiliated with Binance, use at your own risk.
+
+And this repository is forked from `python-binance <https://github.com/sammchardy/python-binance>`_, but has only async client, and works **only** with `trio <https://trio.readthedocs.io/en/stable/index.html>`_ or `trio-compatible <https://trio.readthedocs.io/en/stable/awesome-trio-libraries.html#trio-asyncio-interoperability>`_ asynchronous frameworks.
+
+Source code
+  https://github.com/halfelf/trio-binance
+
+Quick Start
+-----------
+
+`Register an account with Binance <https://accounts.binance.com/en/register?ref=10099792>`_.
+
+`Generate an API Key <https://www.binance.com/en/my/settings/api-management>`_ and assign relevant permissions.
+
+.. code:: bash
+
+    pip install trio-binance
+
+
+Example
+-------------
 
-packages = \
-['trio_binance']
+Check pytest file under ``tests``.
 
-package_data = \
-{'': ['*']}
+Donate
+------
 
-install_requires = \
-['dateparser>=1.1.0,<2.0.0',
- 'h2>=4.1.0,<5.0.0',
- 'httpx>0.20.0',
- 'pytz>=2021.3,<2022.0',
- 'trio-websocket>=0.9.2,<0.10.0',
- 'trio>=0.20.0',
- 'ujson>=5.1.0,<6.0.0']
-
-setup_kwargs = {
-    'name': 'trio-binance',
-    'version': '0.2.2',
-    'description': 'trio based asynchronous binance SDK',
-    'long_description': '=================================\nWelcome to trio-binance\n=================================\n\nThis is an unofficial Python wrapper for the `Binance exchange REST API v3 <https://binance-docs.github.io/apidocs/spot/en>`_. I am in no way affiliated with Binance, use at your own risk.\n\nAnd this repository is forked from `python-binance <https://github.com/sammchardy/python-binance>`_, but has only async client, and works **only** with `trio <https://trio.readthedocs.io/en/stable/index.html>`_ or `trio-compatible <https://trio.readthedocs.io/en/stable/awesome-trio-libraries.html#trio-asyncio-interoperability>`_ asynchronous frameworks.\n\nSource code\n  https://github.com/halfelf/trio-binance\n\nQuick Start\n-----------\n\n`Register an account with Binance <https://accounts.binance.com/en/register?ref=10099792>`_.\n\n`Generate an API Key <https://www.binance.com/en/my/settings/api-management>`_ and assign relevant permissions.\n\n.. code:: bash\n\n    pip install trio-binance\n\n\nExample\n-------------\n\nCheck pytest file under ``tests``.\n\nDonate\n------\n\nIf this library helps, feel free to donate.\n\n- ETH: 0xf560e5F7F234307A20670ed8A5778F350a8366d1\n',
-    'author': 'Shu Wang',
-    'author_email': 'halfelf.ronin@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/halfelf/trio-binance',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+If this library helps, feel free to donate.
 
+- ETH: 0xf560e5F7F234307A20670ed8A5778F350a8366d1
 
-setup(**setup_kwargs)
```

