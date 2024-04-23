# Comparing `tmp/gobnb-0.0.6.tar.gz` & `tmp/gobnb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gobnb-0.0.6.tar", last modified: Wed Mar 27 08:57:37 2024, max compression
+gzip compressed data, was "gobnb-0.0.7.tar", last modified: Tue Apr 23 03:30:05 2024, max compression
```

## Comparing `gobnb-0.0.6.tar` & `gobnb-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-27 08:57:37.008468 gobnb-0.0.6/
--rw-rw-r--   0 user      (1000) user      (1000)     1060 2024-03-27 06:52:07.000000 gobnb-0.0.6/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2239 2024-03-27 08:57:37.004468 gobnb-0.0.6/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1830 2024-03-27 06:52:07.000000 gobnb-0.0.6/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      315 2024-03-27 08:57:16.000000 gobnb-0.0.6/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-27 08:57:37.008468 gobnb-0.0.6/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      480 2024-03-27 07:16:39.000000 gobnb-0.0.6/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-27 08:57:37.000468 gobnb-0.0.6/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-27 08:57:37.004468 gobnb-0.0.6/src/gobnb/
--rw-rw-r--   0 user      (1000) user      (1000)      219 2024-03-27 06:52:07.000000 gobnb-0.0.6/src/gobnb/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1328 2024-03-27 06:52:07.000000 gobnb-0.0.6/src/gobnb/api.py
--rw-rw-r--   0 user      (1000) user      (1000)     2822 2024-03-27 06:58:14.000000 gobnb-0.0.6/src/gobnb/details.py
--rw-rw-r--   0 user      (1000) user      (1000)     1289 2024-03-27 07:10:44.000000 gobnb-0.0.6/src/gobnb/parse.py
--rw-rw-r--   0 user      (1000) user      (1000)     4363 2024-03-27 06:52:07.000000 gobnb-0.0.6/src/gobnb/price.py
--rw-rw-r--   0 user      (1000) user      (1000)     6127 2024-03-27 06:52:07.000000 gobnb-0.0.6/src/gobnb/search.py
--rw-rw-r--   0 user      (1000) user      (1000)    11241 2024-03-27 06:52:07.000000 gobnb-0.0.6/src/gobnb/standardize.py
--rw-rw-r--   0 user      (1000) user      (1000)      921 2024-03-27 06:52:07.000000 gobnb-0.0.6/src/gobnb/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-27 08:57:37.004468 gobnb-0.0.6/src/gobnb.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2239 2024-03-27 08:57:36.000000 gobnb-0.0.6/src/gobnb.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      367 2024-03-27 08:57:36.000000 gobnb-0.0.6/src/gobnb.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-27 08:57:36.000000 gobnb-0.0.6/src/gobnb.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       14 2024-03-27 08:57:36.000000 gobnb-0.0.6/src/gobnb.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2024-03-27 08:57:36.000000 gobnb-0.0.6/src/gobnb.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/
+-rw-rw-r--   0 user      (1000) user      (1000)     1060 2024-03-27 06:52:07.000000 gobnb-0.0.7/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2239 2024-04-23 03:30:05.101741 gobnb-0.0.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1830 2024-03-27 06:52:07.000000 gobnb-0.0.7/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      315 2024-04-23 03:29:32.000000 gobnb-0.0.7/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-23 03:30:05.105741 gobnb-0.0.7/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      480 2024-03-27 07:16:39.000000 gobnb-0.0.7/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/src/gobnb/
+-rw-rw-r--   0 user      (1000) user      (1000)      219 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1356 2024-04-23 03:27:28.000000 gobnb-0.0.7/src/gobnb/api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2822 2024-03-27 06:58:14.000000 gobnb-0.0.7/src/gobnb/details.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1289 2024-03-27 07:10:44.000000 gobnb-0.0.7/src/gobnb/parse.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4363 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/price.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6127 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/search.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11241 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/standardize.py
+-rw-rw-r--   0 user      (1000) user      (1000)      921 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/src/gobnb.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2239 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      367 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/top_level.txt
```

### Comparing `gobnb-0.0.6/LICENSE` & `gobnb-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/PKG-INFO` & `gobnb-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gobnb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Airbnb scraper in Python
 Home-page: https://github.com/johnbalvin/pybnb
 Author: John (John Balvin)
 Author-email: John Balvin <johnchristian@hotmail.es>
 Project-URL: Homepage, https://github.com/johnbalvin/pybnb
 Keywords: airbnb,scraper,crawler
 Description-Content-Type: text/markdown
```

### Comparing `gobnb-0.0.6/README.md` & `gobnb-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/src/gobnb/api.py` & `gobnb-0.0.7/src/gobnb/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from curl_cffi import requests
 import re
 
 ep = "https://www.airbnb.com"
 
-regx_api_key = re.compile(r'"key":".+?"')
+regx_api_key = re.compile(r'"api_config":{"key":".+?"')
 
 def get(proxy_url: str) -> str:
     headers = {
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         "Accept-Language": "en",
         "Cache-Control": "no-cache",
         "Pragma": "no-cache",
@@ -27,10 +27,10 @@
         session.proxies.update({'http': proxy_url, 'https': proxy_url})
 
     response = session.get(ep, timeout=60)  
     response.raise_for_status() 
 
     body = response.text
     api_key = regx_api_key.search(body).group()
-    api_key = api_key.replace('"key":"', '')
+    api_key = api_key.replace('"api_config":{"key":"', '')
     api_key = api_key.replace('"', "")
     return api_key
```

### Comparing `gobnb-0.0.6/src/gobnb/details.py` & `gobnb-0.0.7/src/gobnb/details.py`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/src/gobnb/parse.py` & `gobnb-0.0.7/src/gobnb/parse.py`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/src/gobnb/price.py` & `gobnb-0.0.7/src/gobnb/price.py`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/src/gobnb/search.py` & `gobnb-0.0.7/src/gobnb/search.py`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/src/gobnb/standardize.py` & `gobnb-0.0.7/src/gobnb/standardize.py`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/src/gobnb/utils.py` & `gobnb-0.0.7/src/gobnb/utils.py`

 * *Files identical despite different names*

### Comparing `gobnb-0.0.6/src/gobnb.egg-info/PKG-INFO` & `gobnb-0.0.7/src/gobnb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gobnb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Airbnb scraper in Python
 Home-page: https://github.com/johnbalvin/pybnb
 Author: John (John Balvin)
 Author-email: John Balvin <johnchristian@hotmail.es>
 Project-URL: Homepage, https://github.com/johnbalvin/pybnb
 Keywords: airbnb,scraper,crawler
 Description-Content-Type: text/markdown
```

