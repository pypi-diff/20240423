# Comparing `tmp/nlpknife-0.0.2.tar.gz` & `tmp/nlpknife-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpknife-0.0.2.tar", last modified: Fri Jan 12 06:06:08 2024, max compression
+gzip compressed data, was "nlpknife-0.0.3.tar", last modified: Tue Apr 23 02:18:53 2024, max compression
```

## Comparing `nlpknife-0.0.2.tar` & `nlpknife-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.397902 nlpknife-0.0.2/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1211 2024-01-03 15:59:34.000000 nlpknife-0.0.2/LICENSE
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      776 2024-01-12 06:06:08.397598 nlpknife-0.0.2/PKG-INFO
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      495 2024-01-05 09:58:15.000000 nlpknife-0.0.2/README.md
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.390653 nlpknife-0.0.2/nlpknife/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      466 2024-01-12 06:03:28.000000 nlpknife-0.0.2/nlpknife/__init__.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.394124 nlpknife-0.0.2/nlpknife/db/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      157 2024-01-04 14:22:41.000000 nlpknife-0.0.2/nlpknife/db/__init__.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-01-04 03:41:14.000000 nlpknife-0.0.2/nlpknife/db/es_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-01-04 06:05:34.000000 nlpknife-0.0.2/nlpknife/db/minio_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1362 2024-01-10 06:48:08.000000 nlpknife-0.0.2/nlpknife/db/mysql_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      560 2024-01-04 03:25:12.000000 nlpknife-0.0.2/nlpknife/db/neo4j_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      643 2024-01-04 03:27:37.000000 nlpknife-0.0.2/nlpknife/db/redis_helper.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.395388 nlpknife-0.0.2/nlpknife/evaluation/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      203 2024-01-10 15:00:49.000000 nlpknife-0.0.2/nlpknife/evaluation/__init__.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.395990 nlpknife-0.0.2/nlpknife/evaluation/ner_eval_core/
--rw-rw-r--   0 zhpmatrix   (501) staff       (20)        0 2024-01-10 15:01:18.000000 nlpknife-0.0.2/nlpknife/evaluation/ner_eval_core/__init__.py
--rw-rw-r--   0 zhpmatrix   (501) staff       (20)    23342 2024-01-10 10:20:05.000000 nlpknife-0.0.2/nlpknife/evaluation/ner_eval_core/ner_eval.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     5005 2024-01-10 15:02:43.000000 nlpknife-0.0.2/nlpknife/evaluation/ner_evaluation.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     3766 2024-01-12 05:40:32.000000 nlpknife-0.0.2/nlpknife/evaluation/rag_evaluation.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.396756 nlpknife-0.0.2/nlpknife/extractor/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      155 2024-01-10 10:37:03.000000 nlpknife-0.0.2/nlpknife/extractor/__init__.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1014 2024-01-09 14:58:29.000000 nlpknife-0.0.2/nlpknife/extractor/json_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1973 2024-01-04 02:44:53.000000 nlpknife-0.0.2/nlpknife/logger.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.397153 nlpknife-0.0.2/nlpknife/message/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      269 2024-01-10 15:06:34.000000 nlpknife-0.0.2/nlpknife/message/__init__.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1890 2024-01-12 06:05:20.000000 nlpknife-0.0.2/nlpknife/search.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      548 2024-01-07 06:08:45.000000 nlpknife-0.0.2/nlpknife/timer.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-01-12 06:06:08.392122 nlpknife-0.0.2/nlpknife.egg-info/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      776 2024-01-12 06:06:08.000000 nlpknife-0.0.2/nlpknife.egg-info/PKG-INFO
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      717 2024-01-12 06:06:08.000000 nlpknife-0.0.2/nlpknife.egg-info/SOURCES.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        1 2024-01-12 06:06:08.000000 nlpknife-0.0.2/nlpknife.egg-info/dependency_links.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)       64 2024-01-12 06:06:08.000000 nlpknife-0.0.2/nlpknife.egg-info/requires.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        9 2024-01-12 06:06:08.000000 nlpknife-0.0.2/nlpknife.egg-info/top_level.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)       38 2024-01-12 06:06:08.397947 nlpknife-0.0.2/setup.cfg
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      867 2024-01-12 06:03:19.000000 nlpknife-0.0.2/setup.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.322530 nlpknife-0.0.3/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1211 2024-04-23 01:35:20.000000 nlpknife-0.0.3/LICENSE
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      773 2024-04-23 02:18:53.322240 nlpknife-0.0.3/PKG-INFO
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      455 2024-04-23 01:52:42.000000 nlpknife-0.0.3/README.md
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.316477 nlpknife-0.0.3/nlpknife/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      319 2024-04-23 02:18:36.000000 nlpknife-0.0.3/nlpknife/__init__.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.319368 nlpknife-0.0.3/nlpknife/db/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      157 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/db/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/db/es_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/db/minio_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1362 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/db/mysql_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      560 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/db/neo4j_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      643 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/db/redis_helper.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.320515 nlpknife-0.0.3/nlpknife/evaluation/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      203 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/evaluation/__init__.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.320932 nlpknife-0.0.3/nlpknife/evaluation/ner_eval_core/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/evaluation/ner_eval_core/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)    23342 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/evaluation/ner_eval_core/ner_eval.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     5005 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/evaluation/ner_evaluation.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     3733 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/evaluation/rag_evaluation.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.321547 nlpknife-0.0.3/nlpknife/extractor/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      155 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/extractor/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1014 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/extractor/json_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1973 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/logger.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.321928 nlpknife-0.0.3/nlpknife/message/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      269 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/message/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1750 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/search.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      449 2024-04-23 01:35:20.000000 nlpknife-0.0.3/nlpknife/timer.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-23 02:18:53.317646 nlpknife-0.0.3/nlpknife.egg-info/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      773 2024-04-23 02:18:53.000000 nlpknife-0.0.3/nlpknife.egg-info/PKG-INFO
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      717 2024-04-23 02:18:53.000000 nlpknife-0.0.3/nlpknife.egg-info/SOURCES.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        1 2024-04-23 02:18:53.000000 nlpknife-0.0.3/nlpknife.egg-info/dependency_links.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)       75 2024-04-23 02:18:53.000000 nlpknife-0.0.3/nlpknife.egg-info/requires.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        9 2024-04-23 02:18:53.000000 nlpknife-0.0.3/nlpknife.egg-info/top_level.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)       38 2024-04-23 02:18:53.322580 nlpknife-0.0.3/setup.cfg
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      964 2024-04-23 02:18:32.000000 nlpknife-0.0.3/setup.py
```

### Comparing `nlpknife-0.0.2/LICENSE` & `nlpknife-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/db/mysql_helper.py` & `nlpknife-0.0.3/nlpknife/db/mysql_helper.py`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/db/neo4j_helper.py` & `nlpknife-0.0.3/nlpknife/db/neo4j_helper.py`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/db/redis_helper.py` & `nlpknife-0.0.3/nlpknife/db/redis_helper.py`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/evaluation/ner_eval_core/ner_eval.py` & `nlpknife-0.0.3/nlpknife/evaluation/ner_eval_core/ner_eval.py`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/evaluation/ner_evaluation.py` & `nlpknife-0.0.3/nlpknife/evaluation/ner_evaluation.py`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/evaluation/rag_evaluation.py` & `nlpknife-0.0.3/nlpknife/evaluation/rag_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 '''
 Description: aka.zhp
 Version: 0.0.1
 Author: aka.zhp
 Date: 2024-01-08 22:25:37
-LastEditTime: 2024-01-12 13:40:32
+LastEditTime: 2024-01-10 22:52:45
 '''
-import sys
-sys.path.append("./")
 
 import yaml
 from pprint import pprint
 from datasets import Dataset
 from ragas import evaluate
 from ragas.llms import LangchainLLM
 from langchain_community.embeddings import AzureOpenAIEmbeddings
```

### Comparing `nlpknife-0.0.2/nlpknife/extractor/json_helper.py` & `nlpknife-0.0.3/nlpknife/extractor/json_helper.py`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/logger.py` & `nlpknife-0.0.3/nlpknife/logger.py`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/nlpknife/search.py` & `nlpknife-0.0.3/nlpknife/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 '''
 Description: 搜索类
 Version: 0.0.1
 Author: aka.zhp
 Date: 2023-12-27 15:21:14
-LastEditTime: 2024-01-12 14:04:27
+LastEditTime: 2024-01-04 11:36:11
 '''
 import requests
 from pprint import pprint
 from baidusearch.baidusearch import search
 
-import os
-import yaml
-CONFIG = yaml.safe_load(open("config/config.yaml", "r"))
-
-bing_search_url = CONFIG["BING_SERARCH_URL"]
-bing_subscription_key = CONFIG["BING_SUBSCRIPTION_KEY"]
 class SearchAPIUtils:
     def __init__(self,
-                 bing_search_url=bing_search_url,
-                 bing_subscription_key=bing_subscription_key):
+                 bing_search_url="https://api.bing.microsoft.com/v7.0/search",
+                 bing_subscription_key="2ec8bf74c0104ee69b2951e35653f89d"):
         self.BING_SEARCH_URL = bing_search_url
         self.BING_SUBSCRIPTION_KEY = bing_subscription_key
     
     def search(self, keyword, num_results, search_engine):
         return search_engine(keyword,num_results)
     
     def _baidu_search(self,keyword,num_results=10):
@@ -51,8 +45,8 @@
                     result.append({
                         "title":each["name"],
                         "abstract":each["snippet"],
                         "url":each["url"],
                         "rank":None
                                    })
         return result
-  
+
```

### Comparing `nlpknife-0.0.2/nlpknife.egg-info/SOURCES.txt` & `nlpknife-0.0.3/nlpknife.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlpknife-0.0.2/setup.py` & `nlpknife-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 '''
 Description: aka.zhp
 Version: 0.0.1
 Author: aka.zhp
 Date: 2024-01-04 21:12:45
-LastEditTime: 2024-01-12 13:33:09
+LastEditTime: 2024-04-23 10:16:11
 '''
-
+import setuptools
 import os, shutil
 from distutils.core import setup
 from nlpknife import __version__ as version
-from setuptools import setup, find_packages
 
 with open("./requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 print(install_requires)
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="nlpknife",
     version=version,
     author="zhpmatrix",
     description="my nlpknife",
     long_description=read("README.md"),
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     url="https://github.com/zhpmatrix/nlpknife",
-    packages=find_packages(),
+    packages=setuptools.find_packages(exclude=["test"]),
     download_url="https://pypi.tuna.tsinghua.edu.cn/simple",
     python_requires=">=3.7",
-    install_requires=install_requires
+    install_requires=install_requires,
+    package_data={
+        '': ['*.yaml', '*.json', "*.csv", "*.txt", "*.json", "*.pkl"],
+    }
 )
```

