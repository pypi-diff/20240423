# Comparing `tmp/pyqqq-0.8.5.tar.gz` & `tmp/pyqqq-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.8.5.tar", max compression
+gzip compressed data, was "pyqqq-0.8.6.tar", max compression
```

## Comparing `pyqqq-0.8.5.tar` & `pyqqq-0.8.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.8.5/README.md
--rw-r--r--   0        0        0      770 2024-04-22 06:15:24.653248 pyqqq-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      668 2024-04-16 05:13:25.694767 pyqqq-0.8.5/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.8.5/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.8.5/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    41853 2024-04-22 06:13:58.883736 pyqqq-0.8.5/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.8.5/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24284 2024-04-16 05:02:35.915572 pyqqq-0.8.5/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.8.5/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.8.5/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.8.5/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.8.5/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.8.5/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.8.5/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.8.5/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.8.5/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.8.5/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6677 2024-04-22 04:52:35.362423 pyqqq-0.8.5/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.8.5/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.8.5/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4230 2024-04-22 04:52:35.362865 pyqqq-0.8.5/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.8.5/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.8.5/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.8.5/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.8.5/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.8.5/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3205 2024-04-16 02:15:48.378231 pyqqq-0.8.5/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.8.5/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.8.5/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.8.5/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.8.5/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.8.5/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.8.5/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.8.5/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.8.6/README.md
+-rw-r--r--   0        0        0      747 2024-04-23 09:11:06.245136 pyqqq-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-04-16 05:13:25.694767 pyqqq-0.8.6/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.8.6/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.8.6/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    41853 2024-04-22 06:13:58.883736 pyqqq-0.8.6/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.8.6/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24284 2024-04-16 05:02:35.915572 pyqqq-0.8.6/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.8.6/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.8.6/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.8.6/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.8.6/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.8.6/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.8.6/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.8.6/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.8.6/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.8.6/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6717 2024-04-23 09:10:34.476708 pyqqq-0.8.6/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.8.6/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.8.6/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4230 2024-04-22 04:52:35.362865 pyqqq-0.8.6/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.8.6/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.8.6/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.8.6/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.8.6/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.8.6/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3235 2024-04-23 09:07:35.908506 pyqqq-0.8.6/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.8.6/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.8.6/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.8.6/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.8.6/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.8.6/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.8.6/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.8.6/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 pyqqq-0.8.6/PKG-INFO
```

### Comparing `pyqqq-0.8.5/README.md` & `pyqqq-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyproject.toml` & `pyqqq-0.8.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.8.5"
+version = "0.8.6"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 tinydb = "^4.8.0"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
 websockets = "^12.0"
 pandas = "^2.0.3"
 cssutils = "^2.10.2"
 cachetools = "^5.3.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 sphinx = "^7.2.6"
 myst-parser = "^2.0.0"
 sphinx-rtd-theme = "^2.0.0"
-ipykernel = "^6.29.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyqqq-0.8.5/pyqqq/__init__.py` & `pyqqq-0.8.6/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.8.6/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.8.6/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.8.6/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.8.6/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.8.6/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.8.6/pyqqq/brokerage/kis/oauth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyqqq import get_api_key
 from pyqqq.utils.kvstore import KVStore
 from tinydb import TinyDB, Query
+from typing import Optional
 import datetime as dtm
 import pyqqq.config as c
 import requests
 
 class KISAuth:
     '''
     한국투자증권 인증 정보를 담고 있는 객체
@@ -87,15 +88,15 @@
 class KISTokenRepository:
     def __init__(self):
         if get_api_key():
             self.repo = _RemoteTokenRepository()
         else:
             self.repo = _LocalTokenRepository()
 
-    def find(self, appkey, appsecret) -> str | None:
+    def find(self, appkey, appsecret) -> Optional[str]:
         """
         앱 키와 앱 시크릿에 해당하는 액세스 토큰을 반환합니다.
 
         Args:
             appkey (str): 앱 키
             appsecret (str): 앱 시크릿
 
@@ -117,15 +118,15 @@
         return self.repo.save(appkey, appsecret, token, expiry)
 
 
 class _LocalTokenRepository:
     def __init__(self):
         self.db = TinyDB(c.get_tiny_db_path())
 
-    def find(self, appkey, appsecret) -> str | None:
+    def find(self, appkey, appsecret) -> Optional[str]:
         TokenCache = Query()
 
         result = self.db.search(TokenCache.appkey == appkey and TokenCache.appsecret == appsecret and TokenCache.expiry > dtm.datetime.now().timestamp())
         if len(result) > 0:
             return result[0]['token']
         else:
             return None
@@ -139,15 +140,15 @@
     def __init__(self):
         self.kvstore = KVStore("kis_token_cache")
         self.cache = {}
 
     def _cache_key(self, appkey, appsecret):
         return f"{appkey}_{appsecret}"
 
-    def find(self, appkey, appsecret) -> str | None:
+    def find(self, appkey, appsecret) -> Optional[str]:
         key = self._cache_key(appkey, appsecret)
 
         # 1st. check local data
         local_data = self.cache.get(key, None)
         if local_data:
             if local_data["expiry"] > dtm.datetime.now().timestamp():
                 return local_data["token"]
```

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.8.6/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.8.6/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.8.6/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/data/domestic.py` & `pyqqq-0.8.6/pyqqq/data/domestic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from pyqqq import get_api_key
 from pyqqq.utils.retry import retry
+from typing import Optional
 import datetime as dtm
 import pandas as pd
 import pyqqq.config as c
 import requests
 
 
-def get_alert_stocks(alert_type: str, date: dtm.date = None) -> pd.DataFrame | None:
+def get_alert_stocks(alert_type: str, date: dtm.date = None) -> Optional[pd.DataFrame]:
     """
     시장 경보 종목을 조회합니다.
 
     Args:
         alert_type (str): 경보종류. caution:투자주의종목 warning:투자경고종목 risk:투자위험종목
         date (dtm.date, optional): 조회할 날짜. 기본값은 None (가장 최근 데이터)
 
@@ -51,15 +52,15 @@
 
         df = pd.DataFrame(r.json())
         if not df.empty:
             df.set_index("code", inplace=True)
         return df
 
 
-def get_management_stocks(date: dtm.date = None) -> pd.DataFrame | None:
+def get_management_stocks(date: dtm.date = None) -> Optional[pd.DataFrame]:
     """
     관리종목을 조회합니다.
 
     Args:
         date (dtm.date, optional): 조회할 날짜(지정일이 아닌 데이터 수집일). 기본값은 None (가장 최근 데이터)
 
     Returns:
@@ -98,15 +99,15 @@
 
         df = pd.DataFrame(r.json())
         if not df.empty:
             df.set_index("code", inplace=True)
         return df
 
 
-def get_ticker_info(code: str) -> pd.DataFrame | None:
+def get_ticker_info(code: str) -> Optional[pd.DataFrame]:
     """
     종목의 기본정보를 조회합니다.
 
     Args:
         code (str): 조회할 종목의 코드
 
     Returns:
@@ -124,15 +125,15 @@
                 isin  name market    type
         code
         005930  KR7005930003  삼성전자  KOSPI  EQUITY
     """
     return _ticker_request('code', code)
 
 
-def find_ticker_info(name: str) -> pd.DataFrame | None:
+def find_ticker_info(name: str) -> Optional[pd.DataFrame]:
     """
     종목명으로 기본정보를 조회합니다.
 
     Args:
         name (str): 조회할 종목의 이름
 
     Returns:
```

### Comparing `pyqqq-0.8.5/pyqqq/data/minutes.py` & `pyqqq-0.8.6/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/data/realtime.py` & `pyqqq-0.8.6/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/data/ticks.py` & `pyqqq-0.8.6/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/datatypes.py` & `pyqqq-0.8.6/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/executors/hook.py` & `pyqqq-0.8.6/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/utils/array.py` & `pyqqq-0.8.6/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/utils/compute.py` & `pyqqq-0.8.6/pyqqq/utils/compute.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from decimal import Decimal, ROUND_CEILING, ROUND_FLOOR, ROUND_HALF_UP
+from typing import Union
 
 
 def quantize_krx_price(
-    price: Decimal | int | float, etf_etn: bool, rounding: str = "floor"
+    price: Union[Decimal, int, float], etf_etn: bool, rounding: str = "floor"
 ) -> int:
     """
     주어진 가격을 한국거래소(KRX)의 틱 사이즈에 따라 지정된 반올림 방식으로 조정합니다.
 
     이 함수는 ETF 또는 ETN 여부에 따라 적절한 틱 사이즈를 계산하고, 주어진 가격을 이 틱 사이즈에 맞추어 반올림합니다.
     사용자는 'round', 'ceil', 'floor' 중에서 반올림 방식을 선택할 수 있습니다.
```

### Comparing `pyqqq-0.8.5/pyqqq/utils/display.py` & `pyqqq-0.8.6/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/utils/kvstore.py` & `pyqqq-0.8.6/pyqqq/utils/kvstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from typing import List
-import json
-import requests
-import os
-import pyqqq.config as c
 from pyqqq import get_api_key
 from pyqqq.utils.retry import retry
+from typing import List, Union
+import json
+import pyqqq.config as c
+import requests
 
 
 class KVStore:
     """
     Simple key-value store
 
     Args:
         context_name (str, optional): 전략 등 DB 구분을 위한 context 식별자. 기본값은 "default".
     """
 
     def __init__(self, context_name: str = "default"):
         self.name = context_name
 
-    def get(self, key: str) -> str | bool | int | float | dict | list | None:
+    def get(self, key: str) -> Union[str, bool, int, float, dict, list, None]:
         """
         KV store 로 부터 key 에 해당하는 값을 가져온다.
 
         Args:
             key (str): key
 
         Returns:
@@ -42,15 +41,15 @@
         data = r.json()
         if data:
             return json.loads(data)
         else:
             return None
 
     def set(
-        self, key: str, value: str | bool | int | float | dict | list | None
+        self, key: str, value: Union[str, bool, int, float, dict, list, None]
     ) -> bool:
         """
         KV store 에 key 에 해당하는 값을 저장한다.
 
         value는 json.dumps로 serialize 가능한 값이어야 한다.
         value가 None이면 key를 삭제한다. (delete 메소드와 동일한 효과)
```

### Comparing `pyqqq-0.8.5/pyqqq/utils/limiter.py` & `pyqqq-0.8.6/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/utils/logger.py` & `pyqqq-0.8.6/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/utils/market_schedule.py` & `pyqqq-0.8.6/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/utils/mock_api.py` & `pyqqq-0.8.6/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/pyqqq/utils/retry.py` & `pyqqq-0.8.6/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.5/PKG-INFO` & `pyqqq-0.8.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.8.5
+Version: 0.8.6
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (>=5.3.3,<6.0.0)
 Requires-Dist: cssutils (>=2.10.2,<3.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
```

