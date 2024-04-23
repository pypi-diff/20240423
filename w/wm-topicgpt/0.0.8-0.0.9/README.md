# Comparing `tmp/wm_topicgpt-0.0.8.tar.gz` & `tmp/wm_topicgpt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.0.8.tar", last modified: Tue Apr 23 14:31:54 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.0.9.tar", last modified: Tue Apr 23 15:27:26 2024, max compression
```

## Comparing `wm_topicgpt-0.0.8.tar` & `wm_topicgpt-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.076477 wm_topicgpt-0.0.8/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3439 2024-04-23 14:31:54.075590 wm_topicgpt-0.0.8/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-23 14:31:54.076604 wm_topicgpt-0.0.8/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      526 2024-04-23 14:30:35.000000 wm_topicgpt-0.0.8/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.049486 wm_topicgpt-0.0.8/test/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.0.8/test/test_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.0.8/test/test_functions.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.051872 wm_topicgpt-0.0.8/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-08 17:46:49.000000 wm_topicgpt-0.0.8/topicgpt/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.8/topicgpt/_config.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.0.8/topicgpt/base.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.053400 wm_topicgpt-0.0.8/topicgpt/classification/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       71 2024-04-19 15:12:14.000000 wm_topicgpt-0.0.8/topicgpt/classification/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3753 2024-04-22 21:21:46.000000 wm_topicgpt-0.0.8/topicgpt/classification/_classification.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.054585 wm_topicgpt-0.0.8/topicgpt/embedding/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.0.8/topicgpt/embedding/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-22 21:20:15.000000 wm_topicgpt-0.0.8/topicgpt/embedding/_embed_model.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.056185 wm_topicgpt-0.0.8/topicgpt/feature_extraction/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      110 2024-04-08 21:26:03.000000 wm_topicgpt-0.0.8/topicgpt/feature_extraction/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3384 2024-04-23 05:50:23.000000 wm_topicgpt-0.0.8/topicgpt/feature_extraction/_keywords.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1505 2024-04-08 22:13:17.000000 wm_topicgpt-0.0.8/topicgpt/feature_extraction/_summary.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.057590 wm_topicgpt-0.0.8/topicgpt/pipeline/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       48 2024-04-23 13:07:59.000000 wm_topicgpt-0.0.8/topicgpt/pipeline/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4398 2024-04-23 13:12:27.000000 wm_topicgpt-0.0.8/topicgpt/pipeline/_pipeline.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.059391 wm_topicgpt-0.0.8/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.0.8/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-04-22 21:16:47.000000 wm_topicgpt-0.0.8/topicgpt/preprocessing/_data.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.063345 wm_topicgpt-0.0.8/topicgpt/topic/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      284 2024-04-08 19:59:45.000000 wm_topicgpt-0.0.8/topicgpt/topic/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      431 2024-04-23 04:44:41.000000 wm_topicgpt-0.0.8/topicgpt/topic/_cluster_base.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5205 2024-04-23 13:17:52.000000 wm_topicgpt-0.0.8/topicgpt/topic/_hdbscan_approach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3997 2024-04-23 05:52:56.000000 wm_topicgpt-0.0.8/topicgpt/topic/_kmeans_appproach.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5558 2024-04-23 13:12:05.000000 wm_topicgpt-0.0.8/topicgpt/topic/_topic.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-04-19 14:52:51.000000 wm_topicgpt-0.0.8/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.066404 wm_topicgpt-0.0.8/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-04-12 20:33:35.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/_chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/_embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7000 2024-04-23 05:25:54.000000 wm_topicgpt-0.0.8/topicgpt/walmart_llm/_llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 14:31:54.074921 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3439 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)      995 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      267 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-23 14:31:53.000000 wm_topicgpt-0.0.8/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.807134 wm_topicgpt-0.0.9/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4753 2024-04-23 15:27:26.806451 wm_topicgpt-0.0.9/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-23 15:27:26.807195 wm_topicgpt-0.0.9/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      601 2024-04-23 15:27:18.000000 wm_topicgpt-0.0.9/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.769239 wm_topicgpt-0.0.9/test/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1523 2024-04-08 01:24:06.000000 wm_topicgpt-0.0.9/test/test_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2315 2024-04-05 21:17:40.000000 wm_topicgpt-0.0.9/test/test_functions.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.771817 wm_topicgpt-0.0.9/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      194 2024-04-08 17:46:49.000000 wm_topicgpt-0.0.9/topicgpt/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.9/topicgpt/_config.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-04-05 18:53:52.000000 wm_topicgpt-0.0.9/topicgpt/base.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.773447 wm_topicgpt-0.0.9/topicgpt/classification/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       71 2024-04-19 15:12:14.000000 wm_topicgpt-0.0.9/topicgpt/classification/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3753 2024-04-22 21:21:46.000000 wm_topicgpt-0.0.9/topicgpt/classification/_classification.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.775283 wm_topicgpt-0.0.9/topicgpt/embedding/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-05 15:01:57.000000 wm_topicgpt-0.0.9/topicgpt/embedding/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      944 2024-04-22 21:20:15.000000 wm_topicgpt-0.0.9/topicgpt/embedding/_embed_model.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.778088 wm_topicgpt-0.0.9/topicgpt/feature_extraction/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      110 2024-04-08 21:26:03.000000 wm_topicgpt-0.0.9/topicgpt/feature_extraction/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3384 2024-04-23 15:24:16.000000 wm_topicgpt-0.0.9/topicgpt/feature_extraction/_keywords.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1505 2024-04-08 22:13:17.000000 wm_topicgpt-0.0.9/topicgpt/feature_extraction/_summary.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.780301 wm_topicgpt-0.0.9/topicgpt/pipeline/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       74 2024-04-23 15:10:49.000000 wm_topicgpt-0.0.9/topicgpt/pipeline/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8595 2024-04-23 15:24:15.000000 wm_topicgpt-0.0.9/topicgpt/pipeline/_pipeline.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.782413 wm_topicgpt-0.0.9/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-04-04 04:34:46.000000 wm_topicgpt-0.0.9/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-04-22 21:16:47.000000 wm_topicgpt-0.0.9/topicgpt/preprocessing/_data.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.789188 wm_topicgpt-0.0.9/topicgpt/topic/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      284 2024-04-08 19:59:45.000000 wm_topicgpt-0.0.9/topicgpt/topic/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      431 2024-04-23 04:44:41.000000 wm_topicgpt-0.0.9/topicgpt/topic/_cluster_base.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5205 2024-04-23 13:17:52.000000 wm_topicgpt-0.0.9/topicgpt/topic/_hdbscan_approach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3981 2024-04-23 15:05:47.000000 wm_topicgpt-0.0.9/topicgpt/topic/_kmeans_appproach.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5558 2024-04-23 13:12:05.000000 wm_topicgpt-0.0.9/topicgpt/topic/_topic.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-04-19 14:52:51.000000 wm_topicgpt-0.0.9/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.797095 wm_topicgpt-0.0.9/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      115 2024-04-05 21:44:12.000000 wm_topicgpt-0.0.9/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-04-12 20:33:35.000000 wm_topicgpt-0.0.9/topicgpt/walmart_llm/_chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.9/topicgpt/walmart_llm/_embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7000 2024-04-23 05:25:54.000000 wm_topicgpt-0.0.9/topicgpt/walmart_llm/_llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-23 15:27:26.805108 wm_topicgpt-0.0.9/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4753 2024-04-23 15:27:26.000000 wm_topicgpt-0.0.9/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      995 2024-04-23 15:27:26.000000 wm_topicgpt-0.0.9/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-23 15:27:26.000000 wm_topicgpt-0.0.9/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      267 2024-04-23 15:27:26.000000 wm_topicgpt-0.0.9/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-23 15:27:26.000000 wm_topicgpt-0.0.9/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.0.8/setup.py` & `wm_topicgpt-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,19 @@
     install_requires = f.read().splitlines()
 
 with open("topicgpt/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='wm_topicgpt',
-    version='0.0.8',
+    version='0.0.9',
     description='This is a package to generate topics for the text corpus.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=install_requires,
     python_requires='>=3.9',
-)
+)
+
+# upload codes
+# python3 setup.py sdist bdist_wheel
+# twine upload dist/*
```

### Comparing `wm_topicgpt-0.0.8/test/test_approach.py` & `wm_topicgpt-0.0.9/test/test_approach.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/test/test_functions.py` & `wm_topicgpt-0.0.9/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/classification/_classification.py` & `wm_topicgpt-0.0.9/topicgpt/classification/_classification.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/embedding/_embed_model.py` & `wm_topicgpt-0.0.9/topicgpt/embedding/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/feature_extraction/_keywords.py` & `wm_topicgpt-0.0.9/topicgpt/feature_extraction/_keywords.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/feature_extraction/_summary.py` & `wm_topicgpt-0.0.9/topicgpt/feature_extraction/_summary.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/preprocessing/_data.py` & `wm_topicgpt-0.0.9/topicgpt/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/topic/_hdbscan_approach.py` & `wm_topicgpt-0.0.9/topicgpt/topic/_hdbscan_approach.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/topic/_kmeans_appproach.py` & `wm_topicgpt-0.0.9/topicgpt/topic/_kmeans_appproach.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from ..walmart_llm import AdaEmbedModel
 from ..embedding import BGEEmbedModel
 
 
 class KmeansTopicGenerator(GeneratorMixin):
 
     def __init__(self, n_clusters_list = [], topk=5, batch_size=100, model_name="gpt-35-turbo", 
-                 temperature=0.5, embed_model="bge-small", device="mps", embed_batch_size=300):
+                 temperature=0.5, embed_model="bge", device="mps", embed_batch_size=300):
         self.n_clusters_list = n_clusters_list
         self.topk = topk
         self.batch_size = batch_size,
         self.topic_generator = TopicGenerator(model_name, temperature, batch_size=batch_size)
-        if embed_model == "ada-002":
+        if embed_model == "ada":
             self.embed_model = AdaEmbedModel(batch_size=embed_batch_size)
-        elif embed_model == "bge-small":
+        elif embed_model == "bge":
             self.embed_model = BGEEmbedModel(batch_size=embed_batch_size, device=device)
         
     def generate_micro_clusters(self, data): 
         kmeans = KMeans(n_clusters=self.n_clusters_list[0], random_state=42, n_init="auto")
         kmeans.fit(np.array(data['embeddings'].tolist(), dtype=np.float32))
         data['label'] = kmeans.labels_
         # generate micro clusters
```

### Comparing `wm_topicgpt-0.0.8/topicgpt/topic/_topic.py` & `wm_topicgpt-0.0.9/topicgpt/topic/_topic.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/walmart_llm/_chat_model.py` & `wm_topicgpt-0.0.9/topicgpt/walmart_llm/_chat_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/walmart_llm/_embed_model.py` & `wm_topicgpt-0.0.9/topicgpt/walmart_llm/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/topicgpt/walmart_llm/_llm_client.py` & `wm_topicgpt-0.0.9/topicgpt/walmart_llm/_llm_client.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.8/wm_topicgpt.egg-info/SOURCES.txt` & `wm_topicgpt-0.0.9/wm_topicgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

