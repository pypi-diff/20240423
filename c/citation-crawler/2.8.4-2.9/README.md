# Comparing `tmp/citation_crawler-2.8.4.tar.gz` & `tmp/citation_crawler-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.8.4.tar", last modified: Mon Apr 22 07:04:00 2024, max compression
+gzip compressed data, was "citation_crawler-2.9.tar", last modified: Mon Apr 22 22:27:52 2024, max compression
```

## Comparing `citation_crawler-2.8.4.tar` & `citation_crawler-2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 22:27:44.000000 citation_crawler-2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-22 22:27:52.251619 citation_crawler-2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-22 22:27:44.000000 citation_crawler-2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.247619 citation_crawler-2.9/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.247619 citation_crawler-2.9/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:27:52.251619 citation_crawler-2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-22 22:27:44.000000 citation_crawler-2.9/setup.py
```

### Comparing `citation_crawler-2.8.4/LICENSE` & `citation_crawler-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/PKG-INFO` & `citation_crawler-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation_crawler
-Version: 2.8.4
+Version: 2.9
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -101,14 +101,17 @@
 * `HTTP_PROXY`
   * Set it `http://your_user:your_password@your_proxy_url:your_proxy_port` if you want to use proxy
 * `HTTP_TIMEOUT`
   * Timeout for each http request, in seconds
 * `HTTP_CONCORRENT`
   * Concurrent HTTP requests
   * default: `8`
+* `HTTP_HEADERS`
+  * Headers for HTTP requests
+  * default: None
 
 ### Write to a JSON file
 
 e.g. write to `summary.json`:
 
 ```sh
 python -m citation_crawler -k video -k edge -p 27d5dc70280c8628f181a7f8881912025f808256 -a 1681457 networkx --dest summary.json
```

### Comparing `citation_crawler-2.8.4/README.md` & `citation_crawler-2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,17 @@
 * `HTTP_PROXY`
   * Set it `http://your_user:your_password@your_proxy_url:your_proxy_port` if you want to use proxy
 * `HTTP_TIMEOUT`
   * Timeout for each http request, in seconds
 * `HTTP_CONCORRENT`
   * Concurrent HTTP requests
   * default: `8`
+* `HTTP_HEADERS`
+  * Headers for HTTP requests
+  * default: None
 
 ### Write to a JSON file
 
 e.g. write to `summary.json`:
 
 ```sh
 python -m citation_crawler -k video -k edge -p 27d5dc70280c8628f181a7f8881912025f808256 -a 1681457 networkx --dest summary.json
```

#### html2text {}

```diff
@@ -38,16 +38,17 @@
 (to get details of a paper) for how many days * default: `-1` (cache forever,
 since detailed information of a published paper are not likely to change) *
 `CITATION_CRAWLER_MAX_CACHE_DAYS_INIT_AUTHOR` * save cache for an author page
 (to init papers from specified author by `-a`) for how many days * default: `7`
 (author may publish frequently) * `HTTP_PROXY` * Set it `http://your_user:
 your_password@your_proxy_url:your_proxy_port` if you want to use proxy *
 `HTTP_TIMEOUT` * Timeout for each http request, in seconds * `HTTP_CONCORRENT`
-* Concurrent HTTP requests * default: `8` ### Write to a JSON file e.g. write
-to `summary.json`: ```sh python -m citation_crawler -k video -k edge -
+* Concurrent HTTP requests * default: `8` * `HTTP_HEADERS` * Headers for HTTP
+requests * default: None ### Write to a JSON file e.g. write to `summary.json`:
+```sh python -m citation_crawler -k video -k edge -
 p 27d5dc70280c8628f181a7f8881912025f808256 -a 1681457 networkx --dest
 summary.json ``` #### JSON format ```json { "nodes": { "": { "paperId": "",
 "dblp_key": "", "title": "
  ", "doi": "", "authors": [ { "authorId": "", "name": "", "dblp_name": [ "",
 "", "", "......" ] }, { ...... }, { ...... }, ...... ] }, "": { ...... }, "":
 { ...... }, ...... }, "edges": [ [ "", "" ], [ ...... ], [ ...... ], ...... ]
 ``` ### Write to a Neo4J database ```sh docker pull neo4j docker run --rm -it -
```

### Comparing `citation_crawler-2.8.4/citation_crawler/__main__.py` & `citation_crawler-2.9/citation_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler/arg.py` & `citation_crawler-2.9/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler/crawlers/common.py` & `citation_crawler-2.9/citation_crawler/crawlers/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Dict, Callable
 import os
+import json
 from datetime import datetime, timedelta
 
 import aiohttp
 import logging
 from aiofile import async_open
 from asyncio import Semaphore
 
@@ -16,17 +17,28 @@
         try:
             return int(cache_days)
         except:
             pass
     return None
 
 
+def getenv_headers(key) -> Dict:
+    headers = os.getenv(key)
+    if headers is not None:
+        try:
+            return json.loads(headers)
+        except:
+            pass
+    return None
+
+
 http_concorent = getenv_int('HTTP_CONCORRENT')
 http_sem = Semaphore(http_concorent if http_concorent is not None else 8)
 file_sem = Semaphore(512)
+http_headers = getenv_headers('HTTP_HEADERS')
 
 
 def get_cache_datetime(path) -> datetime:
     return datetime.fromtimestamp(os.path.getmtime(path))
 
 
 async def download_item(url: str, path: str, cache_days: int, is_valid: Callable[[str], None]) -> Optional[Dict]:
@@ -49,15 +61,15 @@
                         except Exception as e:
                             logger.info(" rm cache: %s" % e)
         else:
             logger.info("old cache: %s" % save_path)
 
     async with http_sem:
         try:
-            async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(verify_ssl=False)) as session:
+            async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(verify_ssl=False), headers=http_headers) as session:
                 async with session.get(url,
                                        proxy=os.getenv("HTTP_PROXY"),
                                        timeout=os.getenv("HTTP_TIMEOUT") or 30) as response:
                     logger.debug(" download: %s <- %s" % (path, url))
                     text = await response.text()
                     assert is_valid(text)
                     os.makedirs(os.path.dirname(save_path), exist_ok=True)
```

### Comparing `citation_crawler-2.8.4/citation_crawler/crawlers/ss.py` & `citation_crawler-2.9/citation_crawler/crawlers/ss.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler/graph.py` & `citation_crawler-2.9/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler/init/neo4j.py` & `citation_crawler-2.9/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler/items.py` & `citation_crawler-2.9/citation_crawler/items.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.9/citation_crawler/summarizers/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler/summarizers/nx.py` & `citation_crawler-2.9/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.9/citation_crawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-crawler
-Version: 2.8.4
+Version: 2.9
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -101,14 +101,17 @@
 * `HTTP_PROXY`
   * Set it `http://your_user:your_password@your_proxy_url:your_proxy_port` if you want to use proxy
 * `HTTP_TIMEOUT`
   * Timeout for each http request, in seconds
 * `HTTP_CONCORRENT`
   * Concurrent HTTP requests
   * default: `8`
+* `HTTP_HEADERS`
+  * Headers for HTTP requests
+  * default: None
 
 ### Write to a JSON file
 
 e.g. write to `summary.json`:
 
 ```sh
 python -m citation_crawler -k video -k edge -p 27d5dc70280c8628f181a7f8881912025f808256 -a 1681457 networkx --dest summary.json
```

### Comparing `citation_crawler-2.8.4/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.9/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.4/setup.py` & `citation_crawler-2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.8.4',
+    version='2.9',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

