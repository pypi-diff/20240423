# Comparing `tmp/spider-client-0.0.2.tar.gz` & `tmp/spider-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-client-0.0.2.tar", last modified: Mon Apr 22 16:25:37 2024, max compression
+gzip compressed data, was "spider-client-0.0.3.tar", last modified: Mon Apr 22 22:16:43 2024, max compression
```

## Comparing `spider-client-0.0.2.tar` & `spider-client-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 16:25:37.394457 spider-client-0.0.2/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.2/LICENSE
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 16:25:37.394321 spider-client-0.0.2/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     3527 2024-04-22 13:06:28.000000 spider-client-0.0.2/README.md
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-22 16:25:37.394505 spider-client-0.0.2/setup.cfg
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-22 16:25:16.000000 spider-client-0.0.2/setup.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 16:25:37.393791 spider-client-0.0.2/spider_client.egg-info/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)      256 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/requires.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       12 2024-04-22 16:25:37.000000 spider-client-0.0.2/spider_client.egg-info/top_level.txt
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 16:25:37.394045 spider-client-0.0.2/spiderwebai/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.2/spiderwebai/__init__.py
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     6205 2024-04-22 16:25:11.000000 spider-client-0.0.2/spiderwebai/spider.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 22:16:43.345197 spider-client-0.0.3/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.3/LICENSE
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 22:16:43.345065 spider-client-0.0.3/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     3527 2024-04-22 13:06:28.000000 spider-client-0.0.3/README.md
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-22 22:16:43.345246 spider-client-0.0.3/setup.cfg
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-22 22:16:40.000000 spider-client-0.0.3/setup.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 22:16:43.344595 spider-client-0.0.3/spider_client.egg-info/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)      256 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/requires.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       12 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/top_level.txt
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 22:16:43.344842 spider-client-0.0.3/spiderwebai/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.3/spiderwebai/__init__.py
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     6205 2024-04-22 22:16:22.000000 spider-client-0.0.3/spiderwebai/spider.py
```

### Comparing `spider-client-0.0.2/PKG-INFO` & `spider-client-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.2/README.md` & `spider-client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spider-client-0.0.2/setup.py` & `spider-client-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8").read()
 
 
 setup(
     name="spider-client",
-    version="0.0.2",
+    version="0.0.3",
     url="https://github.com/spider-rs/spider-clients/tree/main/python",
     author="Spider",
     author_email="jeff@a11ywatch.com",
     description="Python SDK for Spider Cloud API",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `spider-client-0.0.2/spider_client.egg-info/PKG-INFO` & `spider-client-0.0.3/spider_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.2/spiderwebai/spider.py` & `spider-client-0.0.3/spiderwebai/spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         :param endpoint: The API endpoint to which the POST request is sent.
         :param data: The data (dictionary) to be sent in the POST request.
         :param stream: Boolean indicating if the response should be streamed.
         :return: The JSON response or the raw response stream if stream is True.
         """
         headers = self._prepare_headers(content_type)
         response = self._post_request(
-            f"https://spider.a11ywatch.com/v1/{endpoint}", data, headers, stream
+            f"https://https://spider.cloud/v1/{endpoint}", data, headers, stream
         )
         if stream:
             return response
         elif response.status_code == 200:
             return response.json()
         else:
             self._handle_error(response, f"post to {endpoint}")
@@ -39,15 +39,15 @@
         Send a GET request to the specified endpoint.
 
         :param endpoint: The API endpoint from which to retrieve data.
         :return: The JSON decoded response.
         """
         headers = self._prepare_headers(content_type)
         response = self._get_request(
-            f"https://spider.a11ywatch.com/v1/{endpoint}", headers, stream
+            f"https://https://spider.cloud/v1/{endpoint}", headers, stream
         )
         if response.status_code == 200:
             return response.json()
         else:
             self._handle_error(response, f"get from {endpoint}")
 
     def scrape_url(
```

