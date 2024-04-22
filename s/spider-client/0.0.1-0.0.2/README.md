# Comparing `tmp/spider-client-0.0.1.tar.gz` & `tmp/spider-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-client-0.0.1.tar", last modified: Mon Apr 22 13:06:43 2024, max compression
+gzip compressed data, was "spider-client-0.0.2.tar", last modified: Mon Apr 22 16:25:37 2024, max compression
```

## Comparing `spider-client-0.0.1.tar` & `spider-client-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 13:06:43.268489 spider-client-0.0.1/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.1/LICENSE
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 13:06:43.268360 spider-client-0.0.1/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     3527 2024-04-22 13:06:28.000000 spider-client-0.0.1/README.md
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-22 13:06:43.268535 spider-client-0.0.1/setup.cfg
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-22 13:06:33.000000 spider-client-0.0.1/setup.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 13:06:43.267790 spider-client-0.0.1/spider_client.egg-info/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 13:06:43.000000 spider-client-0.0.1/spider_client.egg-info/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)      256 2024-04-22 13:06:43.000000 spider-client-0.0.1/spider_client.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-22 13:06:43.000000 spider-client-0.0.1/spider_client.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-22 13:06:43.000000 spider-client-0.0.1/spider_client.egg-info/requires.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       12 2024-04-22 13:06:43.000000 spider-client-0.0.1/spider_client.egg-info/top_level.txt
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 13:06:43.268071 spider-client-0.0.1/spiderwebai/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.1/spiderwebai/__init__.py
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     6172 2024-04-22 13:01:11.000000 spider-client-0.0.1/spiderwebai/spider.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 16:25:37.394457 spider-client-0.0.2/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.2/LICENSE
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 16:25:37.394321 spider-client-0.0.2/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     3527 2024-04-22 13:06:28.000000 spider-client-0.0.2/README.md
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-22 16:25:37.394505 spider-client-0.0.2/setup.cfg
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-22 16:25:16.000000 spider-client-0.0.2/setup.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 16:25:37.393791 spider-client-0.0.2/spider_client.egg-info/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)      256 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/requires.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       12 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/top_level.txt
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 16:25:37.394045 spider-client-0.0.2/spiderwebai/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.2/spiderwebai/__init__.py
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     6205 2024-04-22 16:25:11.000000 spider-client-0.0.2/spiderwebai/spider.py
```

### Comparing `spider-client-0.0.1/PKG-INFO` & `spider-client-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.1/README.md` & `spider-client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spider-client-0.0.1/setup.py` & `spider-client-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8").read()
 
 
 setup(
     name="spider-client",
-    version="0.0.1",
+    version="0.0.2",
     url="https://github.com/spider-rs/spider-clients/tree/main/python",
     author="Spider",
     author_email="jeff@a11ywatch.com",
     description="Python SDK for Spider Cloud API",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `spider-client-0.0.1/spider_client.egg-info/PKG-INFO` & `spider-client-0.0.2/spider_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.1/spiderwebai/spider.py` & `spider-client-0.0.2/spiderwebai/spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         :param params: Optional dictionary of additional parameters for the scrape request.
         :return: JSON response containing the scraping results.
         """
         return self.api_post(
             "crawl", {"url": url, "limit": 1, **(params or {})}, stream, content_type
         )
 
-    def crawl_url(self, url, params=None, stream=False):
+    def crawl_url(self, url, params=None, stream=False, content_type="application/json"):
         """
         Start crawling at the specified URL.
 
         :param url: The URL to begin crawling.
         :param params: Optional dictionary with additional parameters to customize the crawl.
         :param stream: Boolean indicating if the response should be streamed. Defaults to False.
         :return: JSON response or the raw response stream if streaming enabled.
```

