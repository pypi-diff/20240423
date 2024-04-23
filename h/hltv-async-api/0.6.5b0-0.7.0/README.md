# Comparing `tmp/hltv_async_api-0.6.5b0.tar.gz` & `tmp/hltv_async_api-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.6.5b0.tar", max compression
+gzip compressed data, was "hltv_async_api-0.7.0.tar", max compression
```

## Comparing `hltv_async_api-0.6.5b0.tar` & `hltv_async_api-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      125 2024-04-21 22:46:00.384631 hltv_async_api-0.6.5b0/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    41573 2024-04-21 23:03:20.780618 hltv_async_api-0.6.5b0/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.5b0/LICENSE
--rw-r--r--   0        0        0      649 2024-04-21 22:46:00.366896 hltv_async_api-0.6.5b0/pyproject.toml
--rw-r--r--   0        0        0    15522 2024-04-21 23:06:37.312752 hltv_async_api-0.6.5b0/README.md
--rw-r--r--   0        0        0    16030 1970-01-01 00:00:00.000000 hltv_async_api-0.6.5b0/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-23 19:31:20.254506 hltv_async_api-0.7.0/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    42132 2024-04-23 19:29:37.150858 hltv_async_api-0.7.0/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.7.0/LICENSE
+-rw-r--r--   0        0        0      639 2024-04-23 19:31:20.262384 hltv_async_api-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    15333 2024-04-23 18:10:26.740670 hltv_async_api-0.7.0/README.md
+-rw-r--r--   0        0        0    15834 1970-01-01 00:00:00.000000 hltv_async_api-0.7.0/PKG-INFO
```

### Comparing `hltv_async_api-0.6.5b0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.7.0/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,29 @@
+import pytz
+import asyncio
+import re
+import logging
 from typing import Any, List
 from datetime import date, datetime, timedelta
-import pytz
-
 from bs4 import BeautifulSoup
-import asyncio
-from asyncio import get_running_loop
 from functools import partial
-
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientProxyConnectionError, ClientResponseError, ClientOSError, \
     ServerDisconnectedError, ClientHttpProxyError
-import re
-
-import logging
 
 
 class Hltv:
     def __init__(self, max_delay: int = 15,
                  timeout: int = 5,
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
                  debug: bool = False,
                  max_retries: int = 0,
                  proxy_protocol: str | None = None,
-                 proxy_one_time: bool = False,
+                 delete_proxy: bool = False,
                  tz: str = 'Europe/Copenhagen',
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
             "hltvTimeZone": "Europe/Copenhagen"
         }
@@ -41,33 +37,30 @@
 
         self.TIMEZONE = tz
         self._check_tz()
 
         self.PROXY_PATH = proxy_path
         self.PROXY_LIST = proxy_list
         self.PROXY_PROTOCOL = proxy_protocol
-        self.PROXY_ONCE = proxy_one_time
+        self.PROXY_ONCE = delete_proxy
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
         if self.PROXY_PROTOCOL:
             self.PROXY_LIST = [self.PROXY_PROTOCOL + '://' + proxy for i, proxy in enumerate(self.PROXY_LIST, start=0)]
 
         if proxy_path or proxy_list:
             self.USE_PROXY = True
         else:
             self.USE_PROXY = False
 
         self.session = None
-
-    def _configure_logging(self):
-        level = logging.DEBUG if self.DEBUG else logging.INFO
-        logging.basicConfig(level=level, format="%(message)s")
+        self.loop = asyncio.get_running_loop()
 
     async def __aenter__(self):
         await self._create_session()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
@@ -79,39 +72,43 @@
 
     async def close(self):
         if self.session:
             self.logger.debug('Closing Session')
             await self.session.close()
             self.session = None
 
+    def _configure_logging(self):
+        level = logging.DEBUG if self.DEBUG else logging.INFO
+        logging.basicConfig(level=level, format="%(message)s")
+
     def config(self, max_delay: int | None = None,
                timeout: int | None = None,
                use_proxy: bool | None = None,
                proxy_file_path: str | None = None,
                proxy_list: list | None = None,
                debug: bool | None = None,
                max_retries: int | None = None,
                proxy_protocol: str | None = None,
-               proxy_one_time: bool | None = None,
+               delete_proxy: bool | None = None,
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
-        if proxy_one_time is not None:
-            self.PROXY_ONCE = proxy_one_time
+        if delete_proxy is not None:
+            self.PROXY_ONCE = delete_proxy
         if tz is not None:
             self.TIMEZONE = tz
             self._check_tz()
         if debug is not None:
             self.DEBUG = debug
             self._configure_logging()
         if proxy_file_path:
@@ -142,16 +139,15 @@
             self.PROXY_LIST = self.PROXY_LIST[1:] + [(self.PROXY_LIST[0])]
             self.logger.info(f"New proxy: {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
 
     @staticmethod
     def _f(result):
         return BeautifulSoup(result, "lxml")
 
-    async def _cloudflare_check(self, result) -> bool:
-        page = self._f(result)
+    def _cloudflare_check(self, page) -> bool:
         challenge_page = page.find(id="challenge-error-title")
         if challenge_page is not None:
             if "Enable JavaScript and cookies to continue" in challenge_page.get_text().strip():
                 self.logger.debug("Got cloudflare challenge page")
                 return True
         return False
 
@@ -169,60 +165,61 @@
 
     async def _parse(self, url, delay):
         proxy = ''
         # setup new proxy, cuz old one was switched
         if self.USE_PROXY:
             proxy = self._get_proxy()
         else:
-            # delay, only for non proxy users. (default = 1-15s)
+            # delay, only for non-proxy users. (default = 1-15s)
             await asyncio.sleep(delay)
         try:
-            async with self.session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout, ) as response:
+            async with self.session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout) as response:
                 self.logger.info(f"Fetching {url}, code: {response.status}")
                 if response.status == 403 or response.status == 404:
                     self.logger.debug("Got 403 forbitten")
-                    return False, self._parse_error_handler(delay)
+                    return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
+                    #return False, self._parse_error_handler(delay)
 
                 # checking for challenge page.
                 result = await response.text()
-                if await self._cloudflare_check(result):
-                    return False, self._parse_error_handler(delay)
+                page = await self.loop.run_in_executor(None, partial(self._f, result))
+                forbitten = await self.loop.run_in_executor(None, partial(self._cloudflare_check, page))
+                #forbitten, parsed = self._cloudflare_check(result)
+                if forbitten:
+                    return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
+                    #return False, self._parse_error_handler(delay)
 
-                return True, result
+                return True, page
         except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
-                ServerDisconnectedError, TimeoutError, ClientHttpProxyError) as e:
+                ServerDisconnectedError, TimeoutError, ClientHttpProxyError, ClientTimeout) as e:
             self.logger.debug(e)
             delay = self._parse_error_handler(delay)
             return False, delay
-        except ClientTimeout:
-            return False, delay
 
     async def _fetch(self, url, delay: int = 0):
         if not self.session:
             await self._create_session()
         status = False
         try_ = 1
         result = None
 
-        # parse until success or not maxretries
+        # parse until success or not max retries
         while (not status) and (try_ != self.max_retries):
             self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
 
             # if status = True, result = page,
             # if status = False, result = delay (default=0)
             status, result = await self._parse(url, delay)
 
             if not status and result:
                 delay = result
             try_ += 1
 
         if status:
-            loop = get_running_loop()
-            parsed = await loop.run_in_executor(None, partial(self._f, result))
-            return parsed
+            return result
         else:
             self.logger.error('Connection failed')
             return None
 
     @staticmethod
     def _normalize_date(parts) -> str:
         month_abbreviations = {
@@ -246,15 +243,15 @@
         if self.TIMEZONE == 'Europe/Copenhagen':
             return date_
         if date_str:
             date_ = datetime.strptime(date_str, '%d-%m-%Y')
         if date_.tzinfo:
             return date_.astimezone(pytz.timezone(self.TIMEZONE))
         else:
-            return date_.replace(tzinfo=pytz.timezone('Europe/Copenhagen')).astimezone(pytz.timezone(self.TIMEZONE))
+            return pytz.timezone('Europe/Copenhagen').localize(date_).astimezone(pytz.timezone(self.TIMEZONE))
 
     async def get(self, type: str, id: int | str | None = None,
                   title: str | None = None,
                   team1: str | None = None,
                   team2: str | None = None):
         if type == 'events':
             if id:
@@ -356,15 +353,15 @@
                                     event = match.find('span', {'class': 'line-clamp-3'}).text
                                 except AttributeError:
                                     event = ''
 
                             matches.append({
                                 'id': id_,
                                 'date': dtime.strftime('%d-%m-%Y'),
-                                'time': dtime.strftime('%d-%m-%Y'),
+                                'time': dtime.strftime('%H:%M'),
                                 'team1': team1,
                                 'team2': team2,
                                 't1_id': t1_id,
                                 't2_id': t2_id,
                                 'maps': maps,
                                 'rating': rating,
                                 'event': event
@@ -459,28 +456,34 @@
                         'kd': kd,
                         'adr': adr,
                         'rating': rating
                     })
 
         if status_int == 1:
             for map in maps:
-                len_ = len(map)
-                if map["r_team1"] == '13':
-                    if len_ != 1:
-                        score1 += 1
-                    else:
-                        score1 = 13
-                        score2 = int(map["r_team2"])
-
-                elif map["r_team1"] == '13':
-                    if len_ != 1:
-                        score2 += 1
-                    else:
-                        score2 = 13
-                        score1 = int(map["r_team1"])
+                try:
+                    if map["r_team1"].isdigit() and map["r_team2"].isdigit():
+                        len_ = len(map)
+                        s1, s2 = int(map["r_team1"]), int(map["r_team2"])
+                        if s1 > 12 and s1 > s2:
+                            if len_ != 1:
+                                score1 += 1
+                            else:
+                                score1 = s1
+                                score2 = s2
+
+                        elif s2 > 12 and s2 > s1:
+                            if len_ != 1:
+                                score2 += 1
+                            else:
+                                score2 = s2
+                                score1 = s1
+
+                except ValueError:
+                    pass
 
         return {'id': match_id, 'score1': score1, 'score2': score2, 'status': status, 'maps': maps, 'stats': stats_}
 
     async def get_results(self, days: int = 1,
                           min_rating: int = 1,
                           max: int = 30,
                           featured: bool = True,
@@ -589,14 +592,15 @@
                 break
             date_ = self.__normalize_date(result.find("span", class_="standard-headline").text.strip())
             date = self._localize_datetime_to_timezone(date_str=date_).strftime("%d-%m-%Y")
 
             for match in result.find_all("a", class_="a-reset"):
                 if n > max_:
                     break
+
                 id_ = match['href'].split('/')[2]
                 teams = match.find_all("div", class_="team")
                 team1 = teams[0].text.strip()
                 team2 = teams[1].text.strip()
 
                 scores = match.find("td", class_="result-score").text.strip().split('-')
                 score_t1 = scores[0].strip()
@@ -619,15 +623,15 @@
         if not r:
             return
 
         live_matches: List | Any
         matches = []
         try:
             live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div",
-                                                                                   {'class', 'liveMatch-container'})
+                                                     {'class', 'liveMatch-container'})
         except AttributeError:
             live_matches = []
         for live in live_matches:
             id_ = live.find('a', {'class': 'match a-reset'})['href'].split('/')[2]
             teams = live.find_all("div", class_="matchTeamName text-ellipsis")
             team1 = teams[0].text.strip()
             team2 = teams[1].text.strip()
@@ -649,15 +653,16 @@
                 'team1': team1,
                 'team2': team2,
                 't1_id': t1_id,
                 't2_id': t2_id
             })
 
         for date_sect in r.find_all('div', {'class': 'upcomingMatchesSection'}):
-            date_ = datetime.strptime(date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1], "%Y-%m-%d")
+            date_ = datetime.strptime(date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1],
+                                      "%Y-%m-%d")
             for match in date_sect.find_all('div', {'class': 'upcomingMatch'}):
                 teams_ = match.find_all("div", class_="matchTeamName text-ellipsis")
                 id_ = match.find('a')['href'].split('/')[2]
                 t1_id = 0
                 t2_id = 0
                 time_ = match.find('div', {'class', 'matchTime'}).text
                 team1_ = 'TBD'
@@ -1025,12 +1030,12 @@
             if only_today:
                 break
 
         return news
 
 
 async def main():
-    hltv = Hltv(tz='UT234C')
-    print(await hltv.get_match_info(2371594, '3DMAX', 'Guild-Eagles', 'YaLLa-Compass-Spring-2024'))
+    async with Hltv(proxy_path='proxies.txt', proxy_protocol='http', debug=True) as hltv:
+        print(await hltv.get_matches())
 
 if __name__ == '__main__':
     asyncio.run(main())
```

### Comparing `hltv_async_api-0.6.5b0/LICENSE` & `hltv_async_api-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.5b0/pyproject.toml` & `hltv_async_api-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.6.5b"
+version = "0.7.0"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
-description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
+description = "An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `hltv_async_api-0.6.5b0/README.md` & `hltv_async_api-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 
-**This page not completed, not all methods and configs are written**
+**This page is not completed, not all methods and configs are written**
 
 
 # Features
 
 
-* **Simple Usage** (its realy simple)
+* **Simple Usage** (its really simple)
 
 
 * **New and modern fully async library**
 
 
 * **Huge amount of options**
 
@@ -48,15 +48,15 @@
 
     ```
 
     from hltv_async_api import Hltv
     
     hltv = Hltv()
     print(await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024'))
-    await hltv.close_session()
+    await hltv.close()
 
     ```
 
 ---
 
 # Proxy Usage
 
@@ -72,20 +72,20 @@
 **Load Proxies from file**
 
     ```
     hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT')
     ```
 
 
-**One-time proxy**
+**Delete proxy**
 
-    removes bad proxies from list
+    Removes bad proxies
     
     ```
-    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', proxy_one_time=True)
+    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', delete_proxy=True)
     ```
 
 **Protocol usage**
 
     ```
     proxy_list = ['120.234.203.171:9002', '110.38.68.38:80']
     
@@ -212,15 +212,15 @@
 # Configs
 
 * max_delay: int = 15
 
     We automaticly increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s)
 
     ```
-    hltv = Hltv(max_delay=5, use_proxy=False)
+    hltv = Hltv(max_delay=5)
     
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 4s
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 5s
@@ -236,34 +236,30 @@
     
     Creating Session
     Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 1/2
     Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 2/2
     Connection failed
     ```
 
-* use_proxy: bool = False
-
-    Proxy Usage. No compatibility with max_delay (max_delay will be ignored)
-
 * proxy_list: list | None = None
 
     list of your proxies, if your proxies doesnt have any protocol you can use proxy_protocol.
     Note: To add nonproxy to list just put '' to it, you can find example with ar
 
 * proxy_path: str | None = None
 
     Path to your proxy (proxy_list will be ignored). If your proxies doesnt have any protocol you can use proxy_protocol
 
 * proxy_protocol: str | None = None,
 
     Proxy protocol. Your proxies ```hltv = Hltv(proxy_protocol='http' ...) -> '11.11.11.11:1111' -> 'http://11.11.11.11:1111'
 
-* proxy_one_time: bool = False
+* delete_proxy: bool = False
 
-    Removes proxy from list (proxy_path included) if connection unsuccessfull
+    Removes proxy from list (proxy_path included) if connection unsuccessfully
 
 * timeout: int = 5
 
     Max time to close connection. Recommended to use timeout=1 if you are using random proxies.
 
 * debug: bool = False
 
@@ -296,15 +292,15 @@
 
 ```
 from hltv_async_api import Hltv
 
 
 async def test():
 
-    hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, proxy_one_time=True, proxy_protocol='http')
+    hltv = Hltv(debug=True, proxy_path='proxy_test.txt', timeout=1, delete_proxy=True, proxy_protocol='http')
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
 ```
 
@@ -319,23 +315,23 @@
     from redis.asyncio import Redis, ConnectionPool
     
     from hltv_async_api import Hltv
     
     
     
     async def startup(ctx):
-        ctx["hltv"] = Hltv(max_delay=5, use_proxy=True, proxy_path='proxies.txt', debug=True)
+        async with Hltv(max_delay=5, proxy_path='proxies.txt', debug=True) as hltv:
+              ctx["hltv"] = hltv
+  
         ctx["redis"] = redis_client = Redis(
-            connection_pool=ConnectionPool.from_url(settings.redis_url),
-        )
+            connection_pool=ConnectionPool.from_url(settings.redis_url))
         logger.success(f"Scheduler started. UTC time {datetime.utcnow()}")
     
     
     async def shutdown(ctx):
-        await ctx["hltv"].close_session()
         await ctx["redis"].close()
     
     
     async def parse_matches(ctx):
         hltv = ctx["hltv"]
         redis = ctx["redis"]
         matches = await hltv.get_upcoming_matches(1, 1)
```

### Comparing `hltv_async_api-0.6.5b0/PKG-INFO` & `hltv_async_api-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.6.5b0
-Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
+Version: 0.7.0
+Summary: An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -20,21 +20,21 @@
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Description-Content-Type: text/markdown
 
 # hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 
-**This page not completed, not all methods and configs are written**
+**This page is not completed, not all methods and configs are written**
 
 
 # Features
 
 
-* **Simple Usage** (its realy simple)
+* **Simple Usage** (its really simple)
 
 
 * **New and modern fully async library**
 
 
 * **Huge amount of options**
 
@@ -71,15 +71,15 @@
 
     ```
 
     from hltv_async_api import Hltv
     
     hltv = Hltv()
     print(await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024'))
-    await hltv.close_session()
+    await hltv.close()
 
     ```
 
 ---
 
 # Proxy Usage
 
@@ -95,20 +95,20 @@
 **Load Proxies from file**
 
     ```
     hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT')
     ```
 
 
-**One-time proxy**
+**Delete proxy**
 
-    removes bad proxies from list
+    Removes bad proxies
     
     ```
-    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', proxy_one_time=True)
+    hltv = Hltv(proxy_path='PATH_TO_PROXY.TXT', delete_proxy=True)
     ```
 
 **Protocol usage**
 
     ```
     proxy_list = ['120.234.203.171:9002', '110.38.68.38:80']
     
@@ -235,15 +235,15 @@
 # Configs
 
 * max_delay: int = 15
 
     We automaticly increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s)
 
     ```
-    hltv = Hltv(max_delay=5, use_proxy=False)
+    hltv = Hltv(max_delay=5)
     
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 4s
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 5s
@@ -259,34 +259,30 @@
     
     Creating Session
     Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 1/2
     Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 2/2
     Connection failed
     ```
 
-* use_proxy: bool = False
-
-    Proxy Usage. No compatibility with max_delay (max_delay will be ignored)
-
 * proxy_list: list | None = None
 
     list of your proxies, if your proxies doesnt have any protocol you can use proxy_protocol.
     Note: To add nonproxy to list just put '' to it, you can find example with ar
 
 * proxy_path: str | None = None
 
     Path to your proxy (proxy_list will be ignored). If your proxies doesnt have any protocol you can use proxy_protocol
 
 * proxy_protocol: str | None = None,
 
     Proxy protocol. Your proxies ```hltv = Hltv(proxy_protocol='http' ...) -> '11.11.11.11:1111' -> 'http://11.11.11.11:1111'
 
-* proxy_one_time: bool = False
+* delete_proxy: bool = False
 
-    Removes proxy from list (proxy_path included) if connection unsuccessfull
+    Removes proxy from list (proxy_path included) if connection unsuccessfully
 
 * timeout: int = 5
 
     Max time to close connection. Recommended to use timeout=1 if you are using random proxies.
 
 * debug: bool = False
 
@@ -319,15 +315,15 @@
 
 ```
 from hltv_async_api import Hltv
 
 
 async def test():
 
-    hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, proxy_one_time=True, proxy_protocol='http')
+    hltv = Hltv(debug=True, proxy_path='proxy_test.txt', timeout=1, delete_proxy=True, proxy_protocol='http')
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
 ```
 
@@ -342,23 +338,23 @@
     from redis.asyncio import Redis, ConnectionPool
     
     from hltv_async_api import Hltv
     
     
     
     async def startup(ctx):
-        ctx["hltv"] = Hltv(max_delay=5, use_proxy=True, proxy_path='proxies.txt', debug=True)
+        async with Hltv(max_delay=5, proxy_path='proxies.txt', debug=True) as hltv:
+              ctx["hltv"] = hltv
+  
         ctx["redis"] = redis_client = Redis(
-            connection_pool=ConnectionPool.from_url(settings.redis_url),
-        )
+            connection_pool=ConnectionPool.from_url(settings.redis_url))
         logger.success(f"Scheduler started. UTC time {datetime.utcnow()}")
     
     
     async def shutdown(ctx):
-        await ctx["hltv"].close_session()
         await ctx["redis"].close()
     
     
     async def parse_matches(ctx):
         hltv = ctx["hltv"]
         redis = ctx["redis"]
         matches = await hltv.get_upcoming_matches(1, 1)
```

