# Comparing `tmp/scrapio-0.1.7.tar.gz` & `tmp/scrapio-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/edmundmartin/open-source/Scrapio/dist/tmprbjg4lnl/scrapio-0.1.7.tar", last modified: Sat Jul  9 13:14:23 2022, max compression
+gzip compressed data, was "scrapio-0.1.8.tar", last modified: Tue Apr 23 19:06:13 2024, max compression
```

## Comparing `scrapio-0.1.7.tar` & `scrapio-0.1.8.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.946974 scrapio-0.1.7/
--rw-r--r--   0 edmundmartin   (501) staff       (20)    18092 2022-07-08 17:04:27.000000 scrapio-0.1.7/LICENSE
--rw-r--r--   0 edmundmartin   (501) staff       (20)      574 2022-07-09 13:14:23.946725 scrapio-0.1.7/PKG-INFO
--rw-r--r--   0 edmundmartin   (501) staff       (20)     3442 2022-07-08 17:10:00.000000 scrapio-0.1.7/README.md
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.933727 scrapio-0.1.7/scrapio/
--rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/__init__.py
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.936351 scrapio-0.1.7/scrapio/crawlers/
--rw-r--r--   0 edmundmartin   (501) staff       (20)       62 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/crawlers/__init__.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)     5382 2022-07-08 17:29:21.000000 scrapio-0.1.7/scrapio/crawlers/base_crawler.py
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.937815 scrapio-0.1.7/scrapio/parsing/
--rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/parsing/__init__.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)      726 2022-07-08 17:46:59.000000 scrapio-0.1.7/scrapio/parsing/links.py
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.940780 scrapio-0.1.7/scrapio/requests/
--rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/requests/__init__.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)      295 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/requests/client.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)     2307 2022-07-08 17:43:15.000000 scrapio-0.1.7/scrapio/requests/default_client.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)      900 2022-07-08 17:46:59.000000 scrapio-0.1.7/scrapio/requests/response.py
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.943272 scrapio-0.1.7/scrapio/structures/
--rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/structures/__init__.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)     2192 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/structures/filtering.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)      610 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/structures/proxies.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)     1728 2022-07-08 18:07:31.000000 scrapio-0.1.7/scrapio/structures/queues.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)     1811 2022-07-08 17:19:55.000000 scrapio-0.1.7/scrapio/structures/rate_limiter.py
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.945144 scrapio-0.1.7/scrapio/url_set/
--rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/url_set/__init__.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)      201 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/url_set/abstract_set.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)      314 2022-07-08 17:47:56.000000 scrapio-0.1.7/scrapio/url_set/set_container.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)     1296 2022-07-08 18:08:40.000000 scrapio-0.1.7/scrapio/url_set/trie_container.py
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.946290 scrapio-0.1.7/scrapio/utils/
--rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/utils/__init__.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)     1071 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/utils/helpers.py
--rw-r--r--   0 edmundmartin   (501) staff       (20)      336 2022-07-08 17:04:27.000000 scrapio-0.1.7/scrapio/utils/urls.py
-drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2022-07-09 13:14:23.935284 scrapio-0.1.7/scrapio.egg-info/
--rw-r--r--   0 edmundmartin   (501) staff       (20)      574 2022-07-09 13:14:23.000000 scrapio-0.1.7/scrapio.egg-info/PKG-INFO
--rw-r--r--   0 edmundmartin   (501) staff       (20)      792 2022-07-09 13:14:23.000000 scrapio-0.1.7/scrapio.egg-info/SOURCES.txt
--rw-r--r--   0 edmundmartin   (501) staff       (20)        1 2022-07-09 13:14:23.000000 scrapio-0.1.7/scrapio.egg-info/dependency_links.txt
--rw-r--r--   0 edmundmartin   (501) staff       (20)      133 2022-07-09 13:14:23.000000 scrapio-0.1.7/scrapio.egg-info/requires.txt
--rw-r--r--   0 edmundmartin   (501) staff       (20)        8 2022-07-09 13:14:23.000000 scrapio-0.1.7/scrapio.egg-info/top_level.txt
--rw-r--r--   0 edmundmartin   (501) staff       (20)       38 2022-07-09 13:14:23.947056 scrapio-0.1.7/setup.cfg
--rw-r--r--   0 edmundmartin   (501) staff       (20)     1242 2022-07-09 13:14:17.000000 scrapio-0.1.7/setup.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.038581 scrapio-0.1.8/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)    18092 2024-04-23 18:56:17.000000 scrapio-0.1.8/LICENSE
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      842 2024-04-23 19:06:13.037944 scrapio-0.1.8/PKG-INFO
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     3442 2024-04-23 18:56:17.000000 scrapio-0.1.8/README.md
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.027044 scrapio-0.1.8/scrapio/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/__init__.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.029893 scrapio-0.1.8/scrapio/crawlers/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)       62 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/crawlers/__init__.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     5562 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/crawlers/base_crawler.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.030442 scrapio-0.1.8/scrapio/parsing/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/parsing/__init__.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      726 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/parsing/links.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.032130 scrapio-0.1.8/scrapio/requests/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      121 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/requests/__init__.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      308 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/requests/client.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      539 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/requests/client_configuration.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     1597 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/requests/default_client.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      864 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/requests/response.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.033617 scrapio-0.1.8/scrapio/structures/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/structures/__init__.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     2192 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/structures/filtering.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      610 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/structures/proxies.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     1727 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/structures/queues.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     1811 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/structures/rate_limiter.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.035203 scrapio-0.1.8/scrapio/url_set/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/url_set/__init__.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      201 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/url_set/abstract_set.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      300 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/url_set/set_container.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     1274 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/url_set/trie_container.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.036444 scrapio-0.1.8/scrapio/utils/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)        0 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/utils/__init__.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     1071 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/utils/helpers.py
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      336 2024-04-23 18:56:17.000000 scrapio-0.1.8/scrapio/utils/urls.py
+drwxr-xr-x   0 edmundmartin   (501) staff       (20)        0 2024-04-23 19:06:13.037086 scrapio-0.1.8/scrapio.egg-info/
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      842 2024-04-23 19:06:13.000000 scrapio-0.1.8/scrapio.egg-info/PKG-INFO
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      833 2024-04-23 19:06:13.000000 scrapio-0.1.8/scrapio.egg-info/SOURCES.txt
+-rw-r--r--   0 edmundmartin   (501) staff       (20)        1 2024-04-23 19:06:13.000000 scrapio-0.1.8/scrapio.egg-info/dependency_links.txt
+-rw-r--r--   0 edmundmartin   (501) staff       (20)      133 2024-04-23 19:06:13.000000 scrapio-0.1.8/scrapio.egg-info/requires.txt
+-rw-r--r--   0 edmundmartin   (501) staff       (20)        8 2024-04-23 19:06:13.000000 scrapio-0.1.8/scrapio.egg-info/top_level.txt
+-rw-r--r--   0 edmundmartin   (501) staff       (20)       38 2024-04-23 19:06:13.038736 scrapio-0.1.8/setup.cfg
+-rw-r--r--   0 edmundmartin   (501) staff       (20)     1241 2024-04-23 19:06:08.000000 scrapio-0.1.8/setup.py
```

### Comparing `scrapio-0.1.7/LICENSE` & `scrapio-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapio-0.1.7/README.md` & `scrapio-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `scrapio-0.1.7/scrapio/crawlers/base_crawler.py` & `scrapio-0.1.8/scrapio/crawlers/base_crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 import asyncio
 import logging
-from typing import Union, List, Any
+from typing import Union, List, Any, Optional
 
 
 from aiohttp import ClientTimeout
 
 from scrapio.parsing.links import link_extractor
-from scrapio.requests.default_client import DefaultClient
 from scrapio.requests.response import Response
 from scrapio.structures.queues import WorkQueue
 from scrapio.structures.proxies import AbstractProxyManager
 from scrapio.structures.rate_limiter import RateLimiter
 from scrapio.structures.filtering import URLFilter
+from scrapio.retries.retry import NoOpRetryStrategy
+from scrapio.requests import DefaultClient, AbstractClient
 
 __all__ = ["BaseCrawler"]
 
 
 class BaseCrawler:
     def __init__(
         self,
         start_url: Union[List[str], str],
         max_crawl_size=None,
-        timeout=30,
         verbose=True,
         logger_level=logging.WARN,
+        client: Optional[AbstractClient] = None,
         **kwargs
     ):
         self._start_url = start_url
-        self._client = DefaultClient(timeout, **kwargs)
-        self._client_timeout: Union[None, ClientTimeout] = None
-        self._timeout: Union[int, None] = None
 
+        self._client = client if client else DefaultClient()
         self._proxy_manager: Union[None, AbstractProxyManager] = (
             kwargs.get("proxy_manager")(**kwargs)
             if kwargs.get("proxy_manager")
             else None
         )
         self._url_filter = self._set_url_filter(start_url, **kwargs)
         self._queue = WorkQueue(
             max_crawl_size,
             start_url,
             seen_url_handler=kwargs.get("seen_url_handler", None),
         )
         logging.basicConfig(level=logger_level, format="%(message)s")
         self._logger = kwargs.get("logger", logging.getLogger("Scraper"))
-        self._client_timeout = self._setup_timeout_rules(timeout)
-
         self.verbose = verbose
         self._rate_limiter = (
             RateLimiter(kwargs.get("rate_limit")) if kwargs.get("rate_limit") else None
         )
+        self.retry_handler = kwargs.get("retry_handler", NoOpRetryStrategy())
 
     @staticmethod
     def _set_url_filter(start_url, **kwargs) -> URLFilter:
         custom_filter = kwargs.get("custom_filter")
         if custom_filter and issubclass(custom_filter, URLFilter):
             return custom_filter(
                 start_url,
@@ -92,28 +90,32 @@
     def parse_result(self, response: Response) -> Any:
         raise NotImplementedError
 
     async def save_results(self, result):
         raise NotImplementedError
 
     async def _make_requests(self, consumer: int, url: str):
+        err_raised = False
         try:
             self._logger.info("Coroutine: {}, Requesting URL: {}".format(consumer, url))
             if self._rate_limiter:
                 await self._rate_limiter.limited(url)
             resp = await self._client.get_request(url, self._proxy_manager)
             await asyncio.sleep(0.001)
             await self._parse_response(consumer, resp)
         except Exception as e:
             self._logger.warning(
                 "Coroutine: {}, Encountered exception: {}".format(consumer, e)
             )
+            err_raised = True
             raise e
         finally:
             self._queue.task_done()
+            if err_raised is True and self.retry_handler.should_retry(url):
+                await self._queue.put_url(url)
 
     async def _parse_response(self, consumer: int, response: Response) -> None:
         defrag = self._url_filter.defragment
         try:
             response, links = link_extractor(response, self._url_filter, defrag)
             parsed_data = self.parse_result(response)
             await self.save_results(parsed_data)
@@ -138,15 +140,15 @@
         for worker in workers:
             worker.cancel()
 
     async def _close(self):
         await self._client.close()
 
     def run_crawler(self, workers: int) -> None:
-        loop = asyncio.get_event_loop()
+        loop = self._get_best_event_loop()
         try:
             loop.run_until_complete(self._crawl(workers))
         except KeyboardInterrupt:
             logging.info("Shutting down - received keyboard interrupt")
         finally:
             loop.run_until_complete(self._close())
             loop.close()
```

### Comparing `scrapio-0.1.7/scrapio/parsing/links.py` & `scrapio-0.1.8/scrapio/parsing/links.py`

 * *Files identical despite different names*

### Comparing `scrapio-0.1.7/scrapio/requests/response.py` & `scrapio-0.1.8/scrapio/requests/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from typing import Dict, Optional, Any
 
 from aiohttp import ClientResponse
 
 
 class Response:
 
-    __slots__ = [
-        'url',
-        'status',
-        'headers',
-        'body',
-        'raw_response'
-    ]
+    __slots__ = ["url", "status", "headers", "body", "raw_response"]
 
     def __init__(self):
         self.url: Optional[str] = None
         self.status: Optional[int] = None
         self.headers: Optional[Dict] = None
         self.body: Optional[str] = None
         self.raw_response: Optional[Any] = None
@@ -25,11 +19,11 @@
 
 
 async def from_aiohttp_response(client_response: ClientResponse) -> Response:
     resp = Response()
     resp.url = client_response.url
     resp.status = client_response.status
     resp.headers = client_response.headers
-    bytes = await client_response.read()
-    resp.body = bytes.decode("utf-8", errors='ignore')
+    resp_bytes = await client_response.read()
+    resp.body = resp_bytes.decode("utf-8", errors="ignore")
     resp.raw_response = client_response
     return resp
```

### Comparing `scrapio-0.1.7/scrapio/structures/filtering.py` & `scrapio-0.1.8/scrapio/structures/filtering.py`

 * *Files identical despite different names*

### Comparing `scrapio-0.1.7/scrapio/structures/proxies.py` & `scrapio-0.1.8/scrapio/structures/proxies.py`

 * *Files identical despite different names*

### Comparing `scrapio-0.1.7/scrapio/structures/queues.py` & `scrapio-0.1.8/scrapio/structures/queues.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def __init__(
         self,
         max_crawl_size: Union[int, None],
         seed_urls: Union[List[str], str],
         seen_url_handler: AbstractUrlSet = None,
     ):
-        self._seen_urls: AbstractUrlSet = seen_url_handler or TrieContainer()
+        self._seen_urls: AbstractUrlSet = seen_url_handler or SetContainer()
         self._active_jobs = 0
         self._max_crawl_size = max_crawl_size
         self._page_count = 0
         self._queue = asyncio.Queue()
         self.seed_queue(seed_urls)
 
     def seed_queue(self, seed_urls: Union[List[str], str]):
```

### Comparing `scrapio-0.1.7/scrapio/structures/rate_limiter.py` & `scrapio-0.1.8/scrapio/structures/rate_limiter.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     @abstractmethod
     async def limited(self, url: str) -> None:
         pass
 
 
 class RateLimiter(AbstractLimiter):
 
-    __slots__ = ['_rate_limit', '_start_time', '_url_count']
+    __slots__ = ["_rate_limit", "_start_time", "_url_count"]
 
     def __init__(self, reqs_per_second: int):
         self._rate_limit = reqs_per_second
         self._start_time: time.time = time.time()
         self._url_count: int = 0
 
     async def limited(self, url: str) -> None:
```

### Comparing `scrapio-0.1.7/scrapio/url_set/trie_container.py` & `scrapio-0.1.8/scrapio/url_set/trie_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 from typing import List
 
 from scrapio.url_set.abstract_set import AbstractUrlSet
 
 
 class TrieContainer(AbstractUrlSet):
 
-    __slots__ = (
-        'trie',
-        '_end_symbol'
-    )
+    __slots__ = ("trie", "_end_symbol")
 
     def __init__(self):
         self.trie = dict()
         self._end_symbol = "END"
 
     def make_parts(self, url: str) -> List[str]:
         parsed = urlparse(url)
         parts = [parsed.scheme, parsed.netloc]
-        for item in parsed.path.split('/'):
+        for item in parsed.path.split("/"):
             parts.append(item)
         return parts
 
     def __contains__(self, item):
         sub_trie = self.trie
         parts = self.make_parts(item)
         for char in parts:
```

### Comparing `scrapio-0.1.7/scrapio/utils/helpers.py` & `scrapio-0.1.8/scrapio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `scrapio-0.1.7/scrapio.egg-info/SOURCES.txt` & `scrapio-0.1.8/scrapio.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 scrapio.egg-info/top_level.txt
 scrapio/crawlers/__init__.py
 scrapio/crawlers/base_crawler.py
 scrapio/parsing/__init__.py
 scrapio/parsing/links.py
 scrapio/requests/__init__.py
 scrapio/requests/client.py
+scrapio/requests/client_configuration.py
 scrapio/requests/default_client.py
 scrapio/requests/response.py
 scrapio/structures/__init__.py
 scrapio/structures/filtering.py
 scrapio/structures/proxies.py
 scrapio/structures/queues.py
 scrapio/structures/rate_limiter.py
```

