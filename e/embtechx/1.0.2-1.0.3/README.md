# Comparing `tmp/embtechx-1.0.2.tar.gz` & `tmp/embtechx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embtechx-1.0.2.tar", last modified: Mon Apr 22 10:05:57 2024, max compression
+gzip compressed data, was "embtechx-1.0.3.tar", last modified: Mon Apr 22 10:09:22 2024, max compression
```

## Comparing `embtechx-1.0.2.tar` & `embtechx-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:05:57.564267 embtechx-1.0.2/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-22 10:05:57.563420 embtechx-1.0.2/PKG-INFO
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:05:57.560046 embtechx-1.0.2/embtechx/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      862 2024-04-22 10:05:46.000000 embtechx-1.0.2/embtechx/__init__.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-22 10:05:44.000000 embtechx-1.0.2/embtechx/dataframe.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2441 2024-04-22 10:05:44.000000 embtechx-1.0.2/embtechx/domain_emb.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     7471 2024-04-22 09:25:08.000000 embtechx-1.0.2/embtechx/embedding.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-04-22 10:05:43.000000 embtechx-1.0.2/embtechx/evaluate.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     1660 2024-04-22 10:05:42.000000 embtechx-1.0.2/embtechx/search.py
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:05:57.562930 embtechx-1.0.2/embtechx.egg-info/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-22 10:05:57.000000 embtechx-1.0.2/embtechx.egg-info/PKG-INFO
--rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-04-22 10:05:57.000000 embtechx-1.0.2/embtechx.egg-info/SOURCES.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-22 10:05:57.000000 embtechx-1.0.2/embtechx.egg-info/dependency_links.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-04-22 10:05:57.000000 embtechx-1.0.2/embtechx.egg-info/requires.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-04-22 10:05:57.000000 embtechx-1.0.2/embtechx.egg-info/top_level.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-22 10:05:57.564430 embtechx-1.0.2/setup.cfg
--rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-04-22 10:05:49.000000 embtechx-1.0.2/setup.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:09:22.852511 embtechx-1.0.3/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-22 10:09:22.851713 embtechx-1.0.3/PKG-INFO
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:09:22.845400 embtechx-1.0.3/embtechx/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      862 2024-04-22 10:05:46.000000 embtechx-1.0.3/embtechx/__init__.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-22 10:08:54.000000 embtechx-1.0.3/embtechx/dataframe.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2441 2024-04-22 10:08:55.000000 embtechx-1.0.3/embtechx/domain_emb.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     7472 2024-04-22 10:08:57.000000 embtechx-1.0.3/embtechx/embedding.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-04-22 10:08:56.000000 embtechx-1.0.3/embtechx/evaluate.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     1660 2024-04-22 10:08:57.000000 embtechx-1.0.3/embtechx/search.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:09:22.850891 embtechx-1.0.3/embtechx.egg-info/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/PKG-INFO
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/SOURCES.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/dependency_links.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/requires.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/top_level.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-22 10:09:22.852594 embtechx-1.0.3/setup.cfg
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-04-22 10:08:55.000000 embtechx-1.0.3/setup.py
```

### Comparing `embtechx-1.0.2/embtechx/__init__.py` & `embtechx-1.0.3/embtechx/__init__.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.2/embtechx/dataframe.py` & `embtechx-1.0.3/embtechx/dataframe.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.2/embtechx/domain_emb.py` & `embtechx-1.0.3/embtechx/domain_emb.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.2/embtechx/embedding.py` & `embtechx-1.0.3/embtechx/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from sentence_transformers.evaluation import TripletEvaluator
 from torch.utils.data import DataLoader
 
 import time
 import pandas as pd
 from langdetect import *
 
-from dataframe import emb_dataframe
+from .dataframe import emb_dataframe
 concat_df = emb_dataframe.concat_df
 
 model_en = SentenceTransformer("sentence-transformers/all-MiniLM-L6-v2")
 model_th = SentenceTransformer("mrp/simcse-model-m-bert-thai-cased")
 
 class emb_train:
     def detect_df_language(dataframe):
```

### Comparing `embtechx-1.0.2/embtechx/evaluate.py` & `embtechx-1.0.3/embtechx/evaluate.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.2/embtechx/search.py` & `embtechx-1.0.3/embtechx/search.py`

 * *Files identical despite different names*

