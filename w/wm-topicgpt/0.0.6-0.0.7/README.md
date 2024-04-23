# Comparing `tmp/wm_topicgpt-0.0.6.tar.gz` & `tmp/wm_topicgpt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.0.6.tar", last modified: Mon Apr  8 17:48:18 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.0.7.tar", last modified: Tue Apr 23 14:05:44 2024, max compression
```

## Comparing `wm_topicgpt-0.0.6.tar` & `wm_topicgpt-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.070455 wm_topicgpt-0.0.6/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-08 17:48:18.069891 wm_topicgpt-0.0.6/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1976 2024-04-08 17:47:17.000000 wm_topicgpt-0.0.6/README.md
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-08 17:48:18.070515 wm_topicgpt-0.0.6/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-04-08 17:48:01.000000 wm_topicgpt-0.0.6/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.045661 wm_topicgpt-0.0.6/test/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.0.6/test/test_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.0.6/test/test_functions.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.048735 wm_topicgpt-0.0.6/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-08 17:46:49.000000 wm_topicgpt-0.0.6/topicgpt/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.6/topicgpt/_config.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.0.6/topicgpt/base.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.050546 wm_topicgpt-0.0.6/topicgpt/embedding/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.0.6/topicgpt/embedding/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-08 03:42:15.000000 wm_topicgpt-0.0.6/topicgpt/embedding/_embed_model.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.054511 wm_topicgpt-0.0.6/topicgpt/feature_extraction/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      103 2024-04-05 20:30:29.000000 wm_topicgpt-0.0.6/topicgpt/feature_extraction/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1854 2024-04-08 03:38:13.000000 wm_topicgpt-0.0.6/topicgpt/feature_extraction/_keywords.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1967 2024-04-08 06:13:40.000000 wm_topicgpt-0.0.6/topicgpt/feature_extraction/_topic.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.056154 wm_topicgpt-0.0.6/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.0.6/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2240 2024-04-08 05:28:02.000000 wm_topicgpt-0.0.6/topicgpt/preprocessing/_data.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.060771 wm_topicgpt-0.0.6/topicgpt/topic/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      147 2024-04-05 20:39:25.000000 wm_topicgpt-0.0.6/topicgpt/topic/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      444 2024-04-05 20:42:20.000000 wm_topicgpt-0.0.6/topicgpt/topic/_cluster_base.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4313 2024-04-08 15:07:32.000000 wm_topicgpt-0.0.6/topicgpt/topic/_hdbscan_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)        0 2024-04-08 16:33:42.000000 wm_topicgpt-0.0.6/topicgpt/topic/_kmeans_appproach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-03-28 20:09:22.000000 wm_topicgpt-0.0.6/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.064333 wm_topicgpt-0.0.6/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.0.6/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9096 2024-04-04 05:06:04.000000 wm_topicgpt-0.0.6/topicgpt/walmart_llm/_chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.6/topicgpt/walmart_llm/_embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     6969 2024-04-08 05:14:18.000000 wm_topicgpt-0.0.6/topicgpt/walmart_llm/_llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-08 17:48:18.069009 wm_topicgpt-0.0.6/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-08 17:48:17.000000 wm_topicgpt-0.0.6/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)      838 2024-04-08 17:48:18.000000 wm_topicgpt-0.0.6/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-08 17:48:17.000000 wm_topicgpt-0.0.6/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      251 2024-04-08 17:48:17.000000 wm_topicgpt-0.0.6/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-08 17:48:17.000000 wm_topicgpt-0.0.6/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.072221 wm_topicgpt-0.0.7/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-23 14:05:44.071162 wm_topicgpt-0.0.7/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2668 2024-04-23 14:04:19.000000 wm_topicgpt-0.0.7/README.md
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-23 14:05:44.072311 wm_topicgpt-0.0.7/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-04-23 13:55:55.000000 wm_topicgpt-0.0.7/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.042559 wm_topicgpt-0.0.7/test/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.0.7/test/test_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.0.7/test/test_functions.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.045387 wm_topicgpt-0.0.7/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-08 17:46:49.000000 wm_topicgpt-0.0.7/topicgpt/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.7/topicgpt/_config.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.0.7/topicgpt/base.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.046967 wm_topicgpt-0.0.7/topicgpt/classification/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       71 2024-04-19 15:12:14.000000 wm_topicgpt-0.0.7/topicgpt/classification/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3753 2024-04-22 21:21:46.000000 wm_topicgpt-0.0.7/topicgpt/classification/_classification.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.048465 wm_topicgpt-0.0.7/topicgpt/embedding/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.0.7/topicgpt/embedding/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-22 21:20:15.000000 wm_topicgpt-0.0.7/topicgpt/embedding/_embed_model.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.051067 wm_topicgpt-0.0.7/topicgpt/feature_extraction/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      110 2024-04-08 21:26:03.000000 wm_topicgpt-0.0.7/topicgpt/feature_extraction/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3384 2024-04-23 05:50:23.000000 wm_topicgpt-0.0.7/topicgpt/feature_extraction/_keywords.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1505 2024-04-08 22:13:17.000000 wm_topicgpt-0.0.7/topicgpt/feature_extraction/_summary.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.052942 wm_topicgpt-0.0.7/topicgpt/pipeline/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       48 2024-04-23 13:07:59.000000 wm_topicgpt-0.0.7/topicgpt/pipeline/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4398 2024-04-23 13:12:27.000000 wm_topicgpt-0.0.7/topicgpt/pipeline/_pipeline.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.054857 wm_topicgpt-0.0.7/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.0.7/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-04-22 21:16:47.000000 wm_topicgpt-0.0.7/topicgpt/preprocessing/_data.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.059237 wm_topicgpt-0.0.7/topicgpt/topic/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      284 2024-04-08 19:59:45.000000 wm_topicgpt-0.0.7/topicgpt/topic/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      431 2024-04-23 04:44:41.000000 wm_topicgpt-0.0.7/topicgpt/topic/_cluster_base.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5205 2024-04-23 13:17:52.000000 wm_topicgpt-0.0.7/topicgpt/topic/_hdbscan_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3997 2024-04-23 05:52:56.000000 wm_topicgpt-0.0.7/topicgpt/topic/_kmeans_appproach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5558 2024-04-23 13:12:05.000000 wm_topicgpt-0.0.7/topicgpt/topic/_topic.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-04-19 14:52:51.000000 wm_topicgpt-0.0.7/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.062894 wm_topicgpt-0.0.7/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-04-12 20:33:35.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/_chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/_embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7000 2024-04-23 05:25:54.000000 wm_topicgpt-0.0.7/topicgpt/walmart_llm/_llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:05:44.069982 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      591 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1005 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      251 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-23 14:05:43.000000 wm_topicgpt-0.0.7/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.0.6/PKG-INFO` & `wm_topicgpt-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wm_topicgpt
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `wm_topicgpt-0.0.6/test/test_approach.py` & `wm_topicgpt-0.0.7/test/test_approach.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.6/test/test_functions.py` & `wm_topicgpt-0.0.7/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.6/topicgpt/embedding/_embed_model.py` & `wm_topicgpt-0.0.7/topicgpt/embedding/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.6/topicgpt/preprocessing/_data.py` & `wm_topicgpt-0.0.7/topicgpt/preprocessing/_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,75 @@
 import re
 import sys
 import math
 import asyncio
+import pandas as pd
 from tqdm import tqdm
 from azure.ai.textanalytics.aio import TextAnalyticsClient
 from azure.ai.textanalytics import PiiEntityCategory
 from azure.core.credentials import AzureKeyCredential
 from .. import config
 from ..base import TransformerMixin
 
 
 class MinMaxLengthFilter(TransformerMixin):
 
     def __init__(self, words_range=(0, -1)):
         self.words_range = words_range
         
-    def transform(self, texts, labels=None):
+    def transform(self, data):
         min_words = self.words_range[0]
         max_words = self.words_range[1] if self.words_range[1] != -1 else sys.maxsize
-        texts_tr, labels_tr = [], []
-        for idx in range(len(texts)):
-            words = str(texts[idx]).strip().split()
-            if min_words <= len(words) <= max_words:
-                texts_tr.append(texts[idx])
-                if labels:
-                    labels_tr.append(labels[idx])
-        if labels:
-            return texts_tr, labels_tr
+
+        if isinstance(data, list):
+            rt_data = []
+            for idx in range(len(data)):
+                words = str(data[idx]).strip().split()
+                if min_words <= len(words) <= max_words:
+                    rt_data.append(data[idx])
+                return rt_data
+        elif isinstance(data, pd.DataFrame):
+            if 'input' not in data.columns:
+                raise ValueError(f"Must include `input` column in data.")
+            def select_row(row):
+                length = len(str(row['input']).strip().split())
+                return (length >= min_words) and (length <= max_words)
+            rt_data = data[data.apply(select_row, axis=1)]
+            rt_data = rt_data.reset_index(drop=True)
+            return rt_data
         else:
-            return texts_tr
-        
+            raise ValueError("data should be in the type of `list` or `pd.DataFrame`")
+
 
 class NameFilter(TransformerMixin):
 
     batch_size = 5
 
     def __init__(self):
-        self._test_config()
-
-    def _test_config(self):
         if config.azure_key is None:
             raise ValueError("Please set up `config.azure_key`!")
         if config.azure_endpoint is None:
             raise ValueError("Please set up `config.azure_endpoint`!")
 
     async def _name_filter(self, texts):
         client = TextAnalyticsClient(
             endpoint=config.azure_endpoint,
             credential=AzureKeyCredential(config.azure_key),
         )
         async with client:
             response = await client.recognize_pii_entities(documents=texts, language="en", categories_filter = [PiiEntityCategory.PERSON], verify_ssl=False)
-            filtered_texts = [re.sub(r'[*]+', 'PersonName', doc.redacted_text) for doc in response if not doc.is_error]
+            filtered_texts = [re.sub(r'[*]+', 'PersonName', doc.redacted_text) if not doc.is_error else "" for doc in response]
         await client.close()
         return filtered_texts
 
-    def transform(self, texts):
-        texts_tr = []
+    def transform(self, data):
+        if 'input' not in data.columns:
+            raise ValueError(f"Must include `input` column in data.")
+        texts = data['input'].tolist()
+
+        rt_texts = []
         num_batch = math.ceil(len(texts) / self.batch_size)
         for idx in tqdm(range(0, len(texts), self.batch_size), total=num_batch):
-            texts_tr.extend(asyncio.run(self._name_filter(texts[idx: idx+self.batch_size])))
-        return texts_tr
+            rt_texts.extend(asyncio.run(self._name_filter(texts[idx: idx+self.batch_size])))
+    
+        data['input'] = rt_texts
+        return data[data['input'] != ""]
```

### Comparing `wm_topicgpt-0.0.6/topicgpt/walmart_llm/_chat_model.py` & `wm_topicgpt-0.0.7/topicgpt/walmart_llm/_chat_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,14 @@
         def _make_rest_call(endpoint: str, headers: dict, payload: dict):
             try:
                 response = requests.post(endpoint, headers=headers, json=payload, verify=False)
             except requests.exceptions.RequestException as e:
                 raise ValueError(f"Error raised by inference endpoint: {e}")
 
             if response.status_code != 200:
-                print(response.status_code)
                 raise ValueError(f"Error raised by inference API: {response.content}")
             return response.json()
 
         # send request
         generated_text = _make_rest_call(gateway_endpoint, headers, payload)
         return generated_text
```

### Comparing `wm_topicgpt-0.0.6/topicgpt/walmart_llm/_embed_model.py` & `wm_topicgpt-0.0.7/topicgpt/walmart_llm/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.6/topicgpt/walmart_llm/_llm_client.py` & `wm_topicgpt-0.0.7/topicgpt/walmart_llm/_llm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     }
     embedding_client = WalmartAzureOpenaiEmbeddings(vendor="azure-openai", model_name=model_version, **consumer_params)
     return embedding_client
 
 
 class ChatModel:
 
-    def __init__(self, model_name="gpt-35-turbo", temperature=0., batch_size=500):
+    def __init__(self, model_name="gpt-35-turbo", temperature=0.5, batch_size=300):
         self.temperature = temperature
         self.model = instantiate_walmart_chat_completion(model_version=model_name, temperature=temperature)
         self.batch_size = batch_size
 
     def completion(self, message):
         message = [[HumanMessage(content=message)]]
         response = self.model.generate(message).generations[0][0].text
@@ -143,20 +143,20 @@
         try:
             message = [[HumanMessage(content=message)]]
             response = self.model.generate(message).generations[0][0].text
             json_response = eval(response)
             for key in keys:
                 if key not in json_response:
                     raise ValueError(f"Response doesn't include {key}")
-            return json_response
+            return response
         except Exception as e:
             raise ValueError(f"{e} - Response: {json_response}")
     
     def batch_completion(self, messages):
-        
+        @retry(stop=stop_after_attempt(10))
         async def agenerate(model, messages):
             responses = await model.agenerate(messages)
             return responses.generations
 
         responses = []
         num_batch = math.ceil(len(messages) / self.batch_size)
         for idx in tqdm(range(0, len(messages), self.batch_size), total=num_batch):
@@ -164,15 +164,15 @@
             batch_responses = asyncio.run(agenerate(self.model, batch_messages))
             responses.extend([response[0].text for response in batch_responses])
         return responses
 
 
 class AdaEmbedModel:
 
-    def __init__(self, batch_size=500, model_name="text-embedding-ada-002"):
+    def __init__(self, batch_size=300, model_name="text-embedding-ada-002"):
         self.model = instantiate_walmart_embedding(model_version=model_name)
         self.batch_size = batch_size
 
     @retry(wait=wait_exponential(multiplier=1, min=2, max=60))
     def retry_embed_documents(self, documents):
         return self.model.embed_documents(documents)
```

### Comparing `wm_topicgpt-0.0.6/wm_topicgpt.egg-info/PKG-INFO` & `wm_topicgpt-0.0.7/wm_topicgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wm-topicgpt
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
 Requires-Dist: aiohttp==3.9.3
```

