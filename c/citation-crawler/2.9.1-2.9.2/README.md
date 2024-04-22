# Comparing `tmp/citation_crawler-2.9.1.tar.gz` & `tmp/citation_crawler-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.9.1.tar", last modified: Mon Apr 22 22:42:53 2024, max compression
+gzip compressed data, was "citation_crawler-2.9.2.tar", last modified: Mon Apr 22 23:07:56 2024, max compression
```

## Comparing `citation_crawler-2.9.1.tar` & `citation_crawler-2.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.788264 citation_crawler-2.9.2/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 23:07:56.000000 citation_crawler-2.9.2/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:07:56.792264 citation_crawler-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 23:07:49.000000 citation_crawler-2.9.2/setup.py
```

### Comparing `citation_crawler-2.9.1/LICENSE` & `citation_crawler-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/PKG-INFO` & `citation_crawler-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation_crawler
-Version: 2.9.1
+Version: 2.9.2
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.1/README.md` & `citation_crawler-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/__main__.py` & `citation_crawler-2.9.2/citation_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/arg.py` & `citation_crawler-2.9.2/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/crawlers/ss.py` & `citation_crawler-2.9.2/citation_crawler/crawlers/ss.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/graph.py` & `citation_crawler-2.9.2/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/init/neo4j.py` & `citation_crawler-2.9.2/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/items.py` & `citation_crawler-2.9.2/citation_crawler/items.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.9.2/citation_crawler/summarizers/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler/summarizers/nx.py` & `citation_crawler-2.9.2/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.9.2/citation_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-crawler
-Version: 2.9.1
+Version: 2.9.2
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.9.1/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.9.2/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9.1/setup.py` & `citation_crawler-2.9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.9.1',
+    version='2.9.2',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

