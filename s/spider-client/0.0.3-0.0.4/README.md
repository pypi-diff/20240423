# Comparing `tmp/spider-client-0.0.3.tar.gz` & `tmp/spider-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-client-0.0.3.tar", last modified: Mon Apr 22 22:16:43 2024, max compression
+gzip compressed data, was "spider-client-0.0.4.tar", last modified: Tue Apr 23 09:10:05 2024, max compression
```

## Comparing `spider-client-0.0.3.tar` & `spider-client-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 22:16:43.345197 spider-client-0.0.3/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.3/LICENSE
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 22:16:43.345065 spider-client-0.0.3/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     3527 2024-04-22 13:06:28.000000 spider-client-0.0.3/README.md
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-22 22:16:43.345246 spider-client-0.0.3/setup.cfg
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-22 22:16:40.000000 spider-client-0.0.3/setup.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 22:16:43.344595 spider-client-0.0.3/spider_client.egg-info/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)      256 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/requires.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       12 2024-04-22 22:16:43.000000 spider-client-0.0.3/spider_client.egg-info/top_level.txt
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-22 22:16:43.344842 spider-client-0.0.3/spiderwebai/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.3/spiderwebai/__init__.py
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     6205 2024-04-22 22:16:22.000000 spider-client-0.0.3/spiderwebai/spider.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-23 09:10:05.932887 spider-client-0.0.4/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spider-client-0.0.4/LICENSE
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-23 09:10:05.932743 spider-client-0.0.4/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     3527 2024-04-22 13:06:28.000000 spider-client-0.0.4/README.md
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-23 09:10:05.932956 spider-client-0.0.4/setup.cfg
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     1060 2024-04-23 09:09:59.000000 spider-client-0.0.4/setup.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-23 09:10:05.931797 spider-client-0.0.4/spider/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       26 2024-04-22 13:01:33.000000 spider-client-0.0.4/spider/__init__.py
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     6205 2024-04-22 22:16:22.000000 spider-client-0.0.4/spider/spider.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-23 09:10:05.932528 spider-client-0.0.4/spider_client.egg-info/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     4268 2024-04-23 09:10:05.000000 spider-client-0.0.4/spider_client.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)      246 2024-04-23 09:10:05.000000 spider-client-0.0.4/spider_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-23 09:10:05.000000 spider-client-0.0.4/spider_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-23 09:10:05.000000 spider-client-0.0.4/spider_client.egg-info/requires.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        7 2024-04-23 09:10:05.000000 spider-client-0.0.4/spider_client.egg-info/top_level.txt
```

### Comparing `spider-client-0.0.3/PKG-INFO` & `spider-client-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.3/README.md` & `spider-client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spider-client-0.0.3/setup.py` & `spider-client-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8").read()
 
 
 setup(
     name="spider-client",
-    version="0.0.3",
+    version="0.0.4",
     url="https://github.com/spider-rs/spider-clients/tree/main/python",
     author="Spider",
     author_email="jeff@a11ywatch.com",
     description="Python SDK for Spider Cloud API",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `spider-client-0.0.3/spider_client.egg-info/PKG-INFO` & `spider-client-0.0.4/spider_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python SDK for Spider Cloud API
 Home-page: https://github.com/spider-rs/spider-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spider-client-0.0.3/spiderwebai/spider.py` & `spider-client-0.0.4/spider/spider.py`

 * *Files identical despite different names*

