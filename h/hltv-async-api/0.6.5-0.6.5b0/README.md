# Comparing `tmp/hltv_async_api-0.6.5.tar.gz` & `tmp/hltv_async_api-0.6.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.6.5.tar", max compression
+gzip compressed data, was "hltv_async_api-0.6.5b0.tar", max compression
```

## Comparing `hltv_async_api-0.6.5.tar` & `hltv_async_api-0.6.5b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      124 2024-04-22 20:52:31.306195 hltv_async_api-0.6.5/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    41562 2024-04-22 20:54:36.997892 hltv_async_api-0.6.5/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.5/LICENSE
--rw-r--r--   0        0        0      648 2024-04-22 20:52:31.284811 hltv_async_api-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    15491 2024-04-22 20:56:17.073632 hltv_async_api-0.6.5/README.md
--rw-r--r--   0        0        0    15997 1970-01-01 00:00:00.000000 hltv_async_api-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-21 22:46:00.384631 hltv_async_api-0.6.5b0/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    41573 2024-04-21 23:03:20.780618 hltv_async_api-0.6.5b0/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.5b0/LICENSE
+-rw-r--r--   0        0        0      649 2024-04-21 22:46:00.366896 hltv_async_api-0.6.5b0/pyproject.toml
+-rw-r--r--   0        0        0    15522 2024-04-21 23:06:37.312752 hltv_async_api-0.6.5b0/README.md
+-rw-r--r--   0        0        0    16030 1970-01-01 00:00:00.000000 hltv_async_api-0.6.5b0/PKG-INFO
```

### Comparing `hltv_async_api-0.6.5/hltv_async_api/aiohltv.py` & `hltv_async_api-0.6.5b0/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-import pytz
-import asyncio
-import re
-import logging
 from typing import Any, List
 from datetime import date, datetime, timedelta
+import pytz
+
 from bs4 import BeautifulSoup
+import asyncio
+from asyncio import get_running_loop
 from functools import partial
+
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientProxyConnectionError, ClientResponseError, ClientOSError, \
     ServerDisconnectedError, ClientHttpProxyError
+import re
+
+import logging
+
 
 class Hltv:
     def __init__(self, max_delay: int = 15,
                  timeout: int = 5,
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
                  debug: bool = False,
                  max_retries: int = 0,
                  proxy_protocol: str | None = None,
-                 delete_proxy: bool = False,
+                 proxy_one_time: bool = False,
                  tz: str = 'Europe/Copenhagen',
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
             "hltvTimeZone": "Europe/Copenhagen"
         }
@@ -36,15 +41,15 @@
 
         self.TIMEZONE = tz
         self._check_tz()
 
         self.PROXY_PATH = proxy_path
         self.PROXY_LIST = proxy_list
         self.PROXY_PROTOCOL = proxy_protocol
-        self.PROXY_ONCE = delete_proxy
+        self.PROXY_ONCE = proxy_one_time
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
         if self.PROXY_PROTOCOL:
             self.PROXY_LIST = [self.PROXY_PROTOCOL + '://' + proxy for i, proxy in enumerate(self.PROXY_LIST, start=0)]
@@ -82,31 +87,31 @@
                timeout: int | None = None,
                use_proxy: bool | None = None,
                proxy_file_path: str | None = None,
                proxy_list: list | None = None,
                debug: bool | None = None,
                max_retries: int | None = None,
                proxy_protocol: str | None = None,
-               delete_proxy: bool | None = None,
+               proxy_one_time: bool | None = None,
                tz: str = None,
                ):
         if max_delay:
             self.MAX_DELAY = max_delay
         if timeout:
             self.timeout = timeout
         if use_proxy is not None:
             self.USE_PROXY = use_proxy
         if proxy_list:
             self.PROXY_LIST = proxy_list
         if max_retries:
             self.max_retries = max_retries
         if proxy_protocol:
             self.PROXY_PROTOCOL = proxy_protocol
-        if delete_proxy is not None:
-            self.PROXY_ONCE = delete_proxy
+        if proxy_one_time is not None:
+            self.PROXY_ONCE = proxy_one_time
         if tz is not None:
             self.TIMEZONE = tz
             self._check_tz()
         if debug is not None:
             self.DEBUG = debug
             self._configure_logging()
         if proxy_file_path:
@@ -194,28 +199,28 @@
     async def _fetch(self, url, delay: int = 0):
         if not self.session:
             await self._create_session()
         status = False
         try_ = 1
         result = None
 
-        # parse until success or not max retries
+        # parse until success or not maxretries
         while (not status) and (try_ != self.max_retries):
             self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
 
             # if status = True, result = page,
             # if status = False, result = delay (default=0)
             status, result = await self._parse(url, delay)
 
             if not status and result:
                 delay = result
             try_ += 1
 
         if status:
-            loop = asyncio.get_running_loop()
+            loop = get_running_loop()
             parsed = await loop.run_in_executor(None, partial(self._f, result))
             return parsed
         else:
             self.logger.error('Connection failed')
             return None
 
     @staticmethod
@@ -351,15 +356,15 @@
                                     event = match.find('span', {'class': 'line-clamp-3'}).text
                                 except AttributeError:
                                     event = ''
 
                             matches.append({
                                 'id': id_,
                                 'date': dtime.strftime('%d-%m-%Y'),
-                                'time': dtime.strftime('%H:%M'),
+                                'time': dtime.strftime('%d-%m-%Y'),
                                 'team1': team1,
                                 'team2': team2,
                                 't1_id': t1_id,
                                 't2_id': t2_id,
                                 'maps': maps,
                                 'rating': rating,
                                 'event': event
@@ -644,16 +649,15 @@
                 'team1': team1,
                 'team2': team2,
                 't1_id': t1_id,
                 't2_id': t2_id
             })
 
         for date_sect in r.find_all('div', {'class': 'upcomingMatchesSection'}):
-            date_ = datetime.strptime(date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1],
-                                      "%Y-%m-%d")
+            date_ = datetime.strptime(date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1], "%Y-%m-%d")
             for match in date_sect.find_all('div', {'class': 'upcomingMatch'}):
                 teams_ = match.find_all("div", class_="matchTeamName text-ellipsis")
                 id_ = match.find('a')['href'].split('/')[2]
                 t1_id = 0
                 t2_id = 0
                 time_ = match.find('div', {'class', 'matchTime'}).text
                 team1_ = 'TBD'
```

### Comparing `hltv_async_api-0.6.5/LICENSE` & `hltv_async_api-0.6.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.5/pyproject.toml` & `hltv_async_api-0.6.5b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.6.5"
+version = "0.6.5b"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.6.5/README.md` & `hltv_async_api-0.6.5b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 
-**This page is not completed, not all methods and configs are written**
+**This page not completed, not all methods and configs are written**
 
 
 # Features
 
 
-* **Simple Usage** (its really simple)
+* **Simple Usage** (its realy simple)
 
 
 * **New and modern fully async library**
 
 
 * **Huge amount of options**
 
@@ -48,15 +48,15 @@
 
     ```
 
     from hltv_async_api import Hltv
     
     hltv = Hltv()
     print(await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024'))
-    await hltv.close()
+    await hltv.close_session()
 
     ```
 
 ---
 
 # Proxy Usage
 
@@ -72,20 +72,20 @@
 **Load Proxies from file**
 
     ```
     hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT')
     ```
 
 
-**Delete proxy**
+**One-time proxy**
 
-    Removes bad proxies
+    removes bad proxies from list
     
     ```
-    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', delete_proxy=True)
+    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', proxy_one_time=True)
     ```
 
 **Protocol usage**
 
     ```
     proxy_list = ['120.234.203.171:9002', '110.38.68.38:80']
     
@@ -253,17 +253,17 @@
 
     Path to your proxy (proxy_list will be ignored). If your proxies doesnt have any protocol you can use proxy_protocol
 
 * proxy_protocol: str | None = None,
 
     Proxy protocol. Your proxies ```hltv = Hltv(proxy_protocol='http' ...) -> '11.11.11.11:1111' -> 'http://11.11.11.11:1111'
 
-* delete_proxy: bool = False
+* proxy_one_time: bool = False
 
-    Removes proxy from list (proxy_path included) if connection unsuccessfully
+    Removes proxy from list (proxy_path included) if connection unsuccessfull
 
 * timeout: int = 5
 
     Max time to close connection. Recommended to use timeout=1 if you are using random proxies.
 
 * debug: bool = False
 
@@ -296,15 +296,15 @@
 
 ```
 from hltv_async_api import Hltv
 
 
 async def test():
 
-    hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, delete_proxy=True, proxy_protocol='http')
+    hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, proxy_one_time=True, proxy_protocol='http')
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
 ```
 
@@ -319,23 +319,23 @@
     from redis.asyncio import Redis, ConnectionPool
     
     from hltv_async_api import Hltv
     
     
     
     async def startup(ctx):
-        async with Hltv(max_delay=5, use_proxy=True, proxy_path='proxies.txt', debug=True) as hltv:
-              ctx["hltv"] = hltv
-  
+        ctx["hltv"] = Hltv(max_delay=5, use_proxy=True, proxy_path='proxies.txt', debug=True)
         ctx["redis"] = redis_client = Redis(
-            connection_pool=ConnectionPool.from_url(settings.redis_url))
+            connection_pool=ConnectionPool.from_url(settings.redis_url),
+        )
         logger.success(f"Scheduler started. UTC time {datetime.utcnow()}")
     
     
     async def shutdown(ctx):
+        await ctx["hltv"].close_session()
         await ctx["redis"].close()
     
     
     async def parse_matches(ctx):
         hltv = ctx["hltv"]
         redis = ctx["redis"]
         matches = await hltv.get_upcoming_matches(1, 1)
```

### Comparing `hltv_async_api-0.6.5/PKG-INFO` & `hltv_async_api-0.6.5b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.6.5
+Version: 0.6.5b0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -20,21 +20,21 @@
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Description-Content-Type: text/markdown
 
 # hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 
-**This page is not completed, not all methods and configs are written**
+**This page not completed, not all methods and configs are written**
 
 
 # Features
 
 
-* **Simple Usage** (its really simple)
+* **Simple Usage** (its realy simple)
 
 
 * **New and modern fully async library**
 
 
 * **Huge amount of options**
 
@@ -71,15 +71,15 @@
 
     ```
 
     from hltv_async_api import Hltv
     
     hltv = Hltv()
     print(await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024'))
-    await hltv.close()
+    await hltv.close_session()
 
     ```
 
 ---
 
 # Proxy Usage
 
@@ -95,20 +95,20 @@
 **Load Proxies from file**
 
     ```
     hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT')
     ```
 
 
-**Delete proxy**
+**One-time proxy**
 
-    Removes bad proxies
+    removes bad proxies from list
     
     ```
-    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', delete_proxy=True)
+    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', proxy_one_time=True)
     ```
 
 **Protocol usage**
 
     ```
     proxy_list = ['120.234.203.171:9002', '110.38.68.38:80']
     
@@ -276,17 +276,17 @@
 
     Path to your proxy (proxy_list will be ignored). If your proxies doesnt have any protocol you can use proxy_protocol
 
 * proxy_protocol: str | None = None,
 
     Proxy protocol. Your proxies ```hltv = Hltv(proxy_protocol='http' ...) -> '11.11.11.11:1111' -> 'http://11.11.11.11:1111'
 
-* delete_proxy: bool = False
+* proxy_one_time: bool = False
 
-    Removes proxy from list (proxy_path included) if connection unsuccessfully
+    Removes proxy from list (proxy_path included) if connection unsuccessfull
 
 * timeout: int = 5
 
     Max time to close connection. Recommended to use timeout=1 if you are using random proxies.
 
 * debug: bool = False
 
@@ -319,15 +319,15 @@
 
 ```
 from hltv_async_api import Hltv
 
 
 async def test():
 
-    hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, delete_proxy=True, proxy_protocol='http')
+    hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, proxy_one_time=True, proxy_protocol='http')
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
 ```
 
@@ -342,23 +342,23 @@
     from redis.asyncio import Redis, ConnectionPool
     
     from hltv_async_api import Hltv
     
     
     
     async def startup(ctx):
-        async with Hltv(max_delay=5, use_proxy=True, proxy_path='proxies.txt', debug=True) as hltv:
-              ctx["hltv"] = hltv
-  
+        ctx["hltv"] = Hltv(max_delay=5, use_proxy=True, proxy_path='proxies.txt', debug=True)
         ctx["redis"] = redis_client = Redis(
-            connection_pool=ConnectionPool.from_url(settings.redis_url))
+            connection_pool=ConnectionPool.from_url(settings.redis_url),
+        )
         logger.success(f"Scheduler started. UTC time {datetime.utcnow()}")
     
     
     async def shutdown(ctx):
+        await ctx["hltv"].close_session()
         await ctx["redis"].close()
     
     
     async def parse_matches(ctx):
         hltv = ctx["hltv"]
         redis = ctx["redis"]
         matches = await hltv.get_upcoming_matches(1, 1)
```

