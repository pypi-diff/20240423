# Comparing `tmp/citation_crawler-2.9.2.tar.gz` & `tmp/citation_crawler-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.9.2.tar", last modified: Mon Apr 22 23:07:56 2024, max compression
+gzip compressed data, was "citation_crawler-2.9.3.tar", last modified: Mon Apr 22 23:16:55 2024, max compression
```

## Comparing `citation_crawler-2.9.2.tar` & `citation_crawler-2.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.788264 citation_crawler-2.9.2/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.575324 citation_crawler-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:16:55.575324 citation_crawler-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:16:55.575324 citation_crawler-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/setup.py
```

### Comparing `citation_crawler-2.9.2/LICENSE` & `citation_crawler-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/PKG-INFO` & `citation_crawler-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation_crawler
-Version: 2.9.2
+Version: 2.9.3
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.2/README.md` & `citation_crawler-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/__main__.py` & `citation_crawler-2.9.3/citation_crawler/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,28 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('citation_crawler')
 
 parser = argparse.ArgumentParser()
 
 parser.add_argument("-y", "--year", type=int, help="Only crawl the paper after the specified year.", default=2000)
 parser.add_argument("-l", "--limit", type=int, help="Limitation of BFS depth.", default=-1)
+parser.add_argument(
+    '-v', '--verbose',
+    help="Print lots of debugging statements",
+    action="store_const", dest="loglevel", const=logging.DEBUG,
+    default=logging.INFO,
+)
 add_argument_kw(parser)
 add_argument_pid(parser)
 add_argument_aid(parser)
 
 
 def func_parser(parser):
     args = parser.parse_args()
+    logging.basicConfig(level=args.loglevel)
     year = args.year
     limit = args.limit
     keywords = parse_args_kw(parser)
     pid_list, aid_list = parse_args_pid_author(parser)
     logger.info(f"Specified keyword rules: {keywords.rules}")
     logger.info(f"Specified paperId list for init: {pid_list}")
     logger.info(f"Specified authorId list for init: {aid_list}")
@@ -108,15 +115,16 @@
             yield paper
 
 
 parser_n4j = subparsers.add_parser('neo4j', help='Write result to neo4j database')
 parser_n4j.add_argument("--username", type=str, default=None, help=f'Auth username to neo4j database.')
 parser_n4j.add_argument("--password", type=str, default=None, help=f'Auth password to neo4j database.')
 parser_n4j.add_argument("--uri", type=str, required=True, help=f'URI to neo4j database.')
-parser_n4j.add_argument("--no-skip-exists", action="store_true", help=f'Do not skip exists references. Use it when you want to rewrite all papers.')
+parser_n4j.add_argument("--no-skip-exists", action="store_true",
+                        help=f'Do not skip exists references. Use it when you want to rewrite all papers.')
 
 
 async def func_parser_n4j_async(parser):
     from neo4j import AsyncGraphDatabase
     year, keywords, pid_list, aid_list, limit = func_parser(parser)
     args = parser.parse_args()
     logger.info(f"Specified uri and auth: {args.uri} {args.username} {'******' if args.password else 'none'}")
```

### Comparing `citation_crawler-2.9.2/citation_crawler/arg.py` & `citation_crawler-2.9.3/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/crawlers/common.py` & `citation_crawler-2.9.3/citation_crawler/crawlers/common.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/crawlers/ss.py` & `citation_crawler-2.9.3/citation_crawler/crawlers/ss.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/graph.py` & `citation_crawler-2.9.3/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/init/neo4j.py` & `citation_crawler-2.9.3/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/items.py` & `citation_crawler-2.9.3/citation_crawler/items.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.9.3/citation_crawler/summarizers/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler/summarizers/nx.py` & `citation_crawler-2.9.3/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.9.3/citation_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-crawler
-Version: 2.9.2
+Version: 2.9.3
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.2/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.9.3/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.2/setup.py` & `citation_crawler-2.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.9.2',
+    version='2.9.3',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

