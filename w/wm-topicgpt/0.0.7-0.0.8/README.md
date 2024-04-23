# Comparing `tmp/wm_topicgpt-0.0.7.tar.gz` & `tmp/wm_topicgpt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.0.7.tar", last modified: Tue Apr 23 14:05:44 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.0.8.tar", last modified: Tue Apr 23 14:31:54 2024, max compression
```

## Comparing `wm_topicgpt-0.0.7.tar` & `wm_topicgpt-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.072221 wm_topicgpt-0.0.7/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-23 14:05:44.071162 wm_topicgpt-0.0.7/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2668 2024-04-23 14:04:19.000000 wm_topicgpt-0.0.7/README.md
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-23 14:05:44.072311 wm_topicgpt-0.0.7/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-04-23 13:55:55.000000 wm_topicgpt-0.0.7/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.042559 wm_topicgpt-0.0.7/test/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.0.7/test/test_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.0.7/test/test_functions.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.045387 wm_topicgpt-0.0.7/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-08 17:46:49.000000 wm_topicgpt-0.0.7/topicgpt/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.7/topicgpt/_config.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.0.7/topicgpt/base.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.046967 wm_topicgpt-0.0.7/topicgpt/classification/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       71 2024-04-19 15:12:14.000000 wm_topicgpt-0.0.7/topicgpt/classification/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3753 2024-04-22 21:21:46.000000 wm_topicgpt-0.0.7/topicgpt/classification/_classification.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.048465 wm_topicgpt-0.0.7/topicgpt/embedding/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.0.7/topicgpt/embedding/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-22 21:20:15.000000 wm_topicgpt-0.0.7/topicgpt/embedding/_embed_model.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.051067 wm_topicgpt-0.0.7/topicgpt/feature_extraction/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      110 2024-04-08 21:26:03.000000 wm_topicgpt-0.0.7/topicgpt/feature_extraction/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3384 2024-04-23 05:50:23.000000 wm_topicgpt-0.0.7/topicgpt/feature_extraction/_keywords.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1505 2024-04-08 22:13:17.000000 wm_topicgpt-0.0.7/topicgpt/feature_extraction/_summary.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.052942 wm_topicgpt-0.0.7/topicgpt/pipeline/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       48 2024-04-23 13:07:59.000000 wm_topicgpt-0.0.7/topicgpt/pipeline/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4398 2024-04-23 13:12:27.000000 wm_topicgpt-0.0.7/topicgpt/pipeline/_pipeline.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.054857 wm_topicgpt-0.0.7/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.0.7/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-04-22 21:16:47.000000 wm_topicgpt-0.0.7/topicgpt/preprocessing/_data.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.059237 wm_topicgpt-0.0.7/topicgpt/topic/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      284 2024-04-08 19:59:45.000000 wm_topicgpt-0.0.7/topicgpt/topic/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      431 2024-04-23 04:44:41.000000 wm_topicgpt-0.0.7/topicgpt/topic/_cluster_base.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5205 2024-04-23 13:17:52.000000 wm_topicgpt-0.0.7/topicgpt/topic/_hdbscan_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3997 2024-04-23 05:52:56.000000 wm_topicgpt-0.0.7/topicgpt/topic/_kmeans_appproach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5558 2024-04-23 13:12:05.000000 wm_topicgpt-0.0.7/topicgpt/topic/_topic.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-04-19 14:52:51.000000 wm_topicgpt-0.0.7/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.062894 wm_topicgpt-0.0.7/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-04-12 20:33:35.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/_chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/_embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7000 2024-04-23 05:25:54.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/_llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.069982 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1005 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      251 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.076477 wm_topicgpt-0.0.8/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3439 2024-04-23 14:31:54.075590 wm_topicgpt-0.0.8/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-23 14:31:54.076604 wm_topicgpt-0.0.8/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      526 2024-04-23 14:30:35.000000 wm_topicgpt-0.0.8/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.049486 wm_topicgpt-0.0.8/test/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.0.8/test/test_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.0.8/test/test_functions.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.051872 wm_topicgpt-0.0.8/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-08 17:46:49.000000 wm_topicgpt-0.0.8/topicgpt/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.8/topicgpt/_config.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.0.8/topicgpt/base.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.053400 wm_topicgpt-0.0.8/topicgpt/classification/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       71 2024-04-19 15:12:14.000000 wm_topicgpt-0.0.8/topicgpt/classification/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3753 2024-04-22 21:21:46.000000 wm_topicgpt-0.0.8/topicgpt/classification/_classification.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.054585 wm_topicgpt-0.0.8/topicgpt/embedding/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.0.8/topicgpt/embedding/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-22 21:20:15.000000 wm_topicgpt-0.0.8/topicgpt/embedding/_embed_model.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.056185 wm_topicgpt-0.0.8/topicgpt/feature_extraction/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      110 2024-04-08 21:26:03.000000 wm_topicgpt-0.0.8/topicgpt/feature_extraction/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3384 2024-04-23 05:50:23.000000 wm_topicgpt-0.0.8/topicgpt/feature_extraction/_keywords.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1505 2024-04-08 22:13:17.000000 wm_topicgpt-0.0.8/topicgpt/feature_extraction/_summary.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.057590 wm_topicgpt-0.0.8/topicgpt/pipeline/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       48 2024-04-23 13:07:59.000000 wm_topicgpt-0.0.8/topicgpt/pipeline/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4398 2024-04-23 13:12:27.000000 wm_topicgpt-0.0.8/topicgpt/pipeline/_pipeline.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.059391 wm_topicgpt-0.0.8/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.0.8/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-04-22 21:16:47.000000 wm_topicgpt-0.0.8/topicgpt/preprocessing/_data.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.063345 wm_topicgpt-0.0.8/topicgpt/topic/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      284 2024-04-08 19:59:45.000000 wm_topicgpt-0.0.8/topicgpt/topic/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      431 2024-04-23 04:44:41.000000 wm_topicgpt-0.0.8/topicgpt/topic/_cluster_base.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5205 2024-04-23 13:17:52.000000 wm_topicgpt-0.0.8/topicgpt/topic/_hdbscan_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3997 2024-04-23 05:52:56.000000 wm_topicgpt-0.0.8/topicgpt/topic/_kmeans_appproach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5558 2024-04-23 13:12:05.000000 wm_topicgpt-0.0.8/topicgpt/topic/_topic.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-04-19 14:52:51.000000 wm_topicgpt-0.0.8/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.066404 wm_topicgpt-0.0.8/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-04-12 20:33:35.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/_chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/_embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7000 2024-04-23 05:25:54.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/_llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.074921 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3439 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      995 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      267 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.0.7/README.md` & `wm_topicgpt-0.0.8/wm_topicgpt.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: wm-topicgpt
+Version: 0.0.8
+Summary: This is a package to generate topics for the text corpus.
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: numpy==1.26.4
+Requires-Dist: pandas==2.2.1
+Requires-Dist: tqdm==4.66.2
+Requires-Dist: azure-ai-textanalytics==5.3.0
+Requires-Dist: aiohttp==3.9.3
+Requires-Dist: langchain==0.1.14
+Requires-Dist: langchain_community==0.0.31
+Requires-Dist: pycryptodome==3.10.1
+Requires-Dist: tiktoken==0.6.0
+Requires-Dist: openai==1.16.0
+Requires-Dist: scikit_learn==1.4.0
+Requires-Dist: umap_learn==0.5.5
+Requires-Dist: sentence_transformers==2.6.1
+Requires-Dist: pydantic==2.7.1
+
 # TopicGPT package
 
 ## How to install this package?
 ```python
-pip install wm_topicgpt==0.0.7
+pip install wm_topicgpt==0.0.8
 ```
 
 ## How to use this package?
 
 ### Step 1: Set up global parameters
 ```python
 from topicgpt import config
@@ -28,14 +49,18 @@
 
 data_df = pd.read_csv("dataset.csv")
 ```
 
 ### Step 3: Run the code
 
 ```python
+# If using jupyter notebook, you should includes those two lines.
+import nest_asyncio
+nest_asyncio.apply()
+
 
 # Setting up some params for this approach. If you don't need some parts, just drop that part.
 params = {
     # preprocessing part
     'preprocessing': {'words_range': (1, 500)},
     # name filter part
     'name_filter': {},
```

### Comparing `wm_topicgpt-0.0.7/test/test_approach.py` & `wm_topicgpt-0.0.8/test/test_approach.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/test/test_functions.py` & `wm_topicgpt-0.0.8/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/classification/_classification.py` & `wm_topicgpt-0.0.8/topicgpt/classification/_classification.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/embedding/_embed_model.py` & `wm_topicgpt-0.0.8/topicgpt/embedding/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/feature_extraction/_keywords.py` & `wm_topicgpt-0.0.8/topicgpt/feature_extraction/_keywords.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/feature_extraction/_summary.py` & `wm_topicgpt-0.0.8/topicgpt/feature_extraction/_summary.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/pipeline/_pipeline.py` & `wm_topicgpt-0.0.8/topicgpt/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/preprocessing/_data.py` & `wm_topicgpt-0.0.8/topicgpt/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/topic/_hdbscan_approach.py` & `wm_topicgpt-0.0.8/topicgpt/topic/_hdbscan_approach.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/topic/_kmeans_appproach.py` & `wm_topicgpt-0.0.8/topicgpt/topic/_kmeans_appproach.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/topic/_topic.py` & `wm_topicgpt-0.0.8/topicgpt/topic/_topic.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/walmart_llm/_chat_model.py` & `wm_topicgpt-0.0.8/topicgpt/walmart_llm/_chat_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/walmart_llm/_embed_model.py` & `wm_topicgpt-0.0.8/topicgpt/walmart_llm/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/topicgpt/walmart_llm/_llm_client.py` & `wm_topicgpt-0.0.8/topicgpt/walmart_llm/_llm_client.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.7/wm_topicgpt.egg-info/SOURCES.txt` & `wm_topicgpt-0.0.8/wm_topicgpt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 setup.py
 test/test_approach.py
 test/test_functions.py
 topicgpt/__init__.py
 topicgpt/_config.py
 topicgpt/base.py
 topicgpt/utils.py
```

