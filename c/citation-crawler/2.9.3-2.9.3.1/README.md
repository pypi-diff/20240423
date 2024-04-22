# Comparing `tmp/citation_crawler-2.9.3.tar.gz` & `tmp/citation_crawler-2.9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.9.3.tar", last modified: Mon Apr 22 23:16:55 2024, max compression
+gzip compressed data, was "citation_crawler-2.9.3.1.tar", last modified: Mon Apr 22 23:22:31 2024, max compression
```

## Comparing `citation_crawler-2.9.3.tar` & `citation_crawler-2.9.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.575324 citation_crawler-2.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:16:55.575324 citation_crawler-2.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:55.571324 citation_crawler-2.9.3/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:16:55.000000 citation_crawler-2.9.3/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:16:55.575324 citation_crawler-2.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 23:16:44.000000 citation_crawler-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:22:31.813577 citation_crawler-2.9.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-22 23:22:31.813577 citation_crawler-2.9.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:22:31.809577 citation_crawler-2.9.3.1/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:22:31.813577 citation_crawler-2.9.3.1/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:22:31.813577 citation_crawler-2.9.3.1/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:22:31.813577 citation_crawler-2.9.3.1/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:22:31.813577 citation_crawler-2.9.3.1/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-22 23:22:31.000000 citation_crawler-2.9.3.1/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:22:31.000000 citation_crawler-2.9.3.1/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:22:31.000000 citation_crawler-2.9.3.1/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 23:22:31.000000 citation_crawler-2.9.3.1/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:22:31.000000 citation_crawler-2.9.3.1/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:22:31.813577 citation_crawler-2.9.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-22 23:22:25.000000 citation_crawler-2.9.3.1/setup.py
```

### Comparing `citation_crawler-2.9.3/LICENSE` & `citation_crawler-2.9.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/PKG-INFO` & `citation_crawler-2.9.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation_crawler
-Version: 2.9.3
+Version: 2.9.3.1
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.3/README.md` & `citation_crawler-2.9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/__main__.py` & `citation_crawler-2.9.3.1/citation_crawler/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 
 from dblp_crawler.keyword.arg import add_argument as add_argument_kw, parse_args as parse_args_kw
 from citation_crawler.arg import add_argument_pid, add_argument_aid, parse_args_pid_author
 from citation_crawler.crawlers import SemanticScholarCrawler
 from citation_crawler.summarizers import NetworkxSummarizer, Neo4jSummarizer
 
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('citation_crawler')
 
 parser = argparse.ArgumentParser()
 
 parser.add_argument("-y", "--year", type=int, help="Only crawl the paper after the specified year.", default=2000)
 parser.add_argument("-l", "--limit", type=int, help="Limitation of BFS depth.", default=-1)
 parser.add_argument(
```

### Comparing `citation_crawler-2.9.3/citation_crawler/arg.py` & `citation_crawler-2.9.3.1/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/crawlers/common.py` & `citation_crawler-2.9.3.1/citation_crawler/crawlers/common.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/crawlers/ss.py` & `citation_crawler-2.9.3.1/citation_crawler/crawlers/ss.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/graph.py` & `citation_crawler-2.9.3.1/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/init/neo4j.py` & `citation_crawler-2.9.3.1/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/items.py` & `citation_crawler-2.9.3.1/citation_crawler/items.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.9.3.1/citation_crawler/summarizers/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler/summarizers/nx.py` & `citation_crawler-2.9.3.1/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.9.3.1/citation_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-crawler
-Version: 2.9.3
+Version: 2.9.3.1
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.3/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.9.3.1/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.3/setup.py` & `citation_crawler-2.9.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.9.3',
+    version='2.9.3.1',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

