# Comparing `tmp/embtechx-1.0.3.tar.gz` & `tmp/embtechx-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embtechx-1.0.3.tar", last modified: Mon Apr 22 10:09:22 2024, max compression
+gzip compressed data, was "embtechx-1.0.4.tar", last modified: Tue Apr 23 02:27:31 2024, max compression
```

## Comparing `embtechx-1.0.3.tar` & `embtechx-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:09:22.852511 embtechx-1.0.3/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-22 10:09:22.851713 embtechx-1.0.3/PKG-INFO
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:09:22.845400 embtechx-1.0.3/embtechx/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      862 2024-04-22 10:05:46.000000 embtechx-1.0.3/embtechx/__init__.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-22 10:08:54.000000 embtechx-1.0.3/embtechx/dataframe.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2441 2024-04-22 10:08:55.000000 embtechx-1.0.3/embtechx/domain_emb.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     7472 2024-04-22 10:08:57.000000 embtechx-1.0.3/embtechx/embedding.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-04-22 10:08:56.000000 embtechx-1.0.3/embtechx/evaluate.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     1660 2024-04-22 10:08:57.000000 embtechx-1.0.3/embtechx/search.py
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 10:09:22.850891 embtechx-1.0.3/embtechx.egg-info/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/PKG-INFO
--rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/SOURCES.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/dependency_links.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/requires.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-04-22 10:09:22.000000 embtechx-1.0.3/embtechx.egg-info/top_level.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-22 10:09:22.852594 embtechx-1.0.3/setup.cfg
--rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-04-22 10:08:55.000000 embtechx-1.0.3/setup.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-23 02:27:31.567077 embtechx-1.0.4/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-23 02:27:31.566356 embtechx-1.0.4/PKG-INFO
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-23 02:27:31.563023 embtechx-1.0.4/embtechx/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      863 2024-04-22 16:40:49.000000 embtechx-1.0.4/embtechx/__init__.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-22 10:08:54.000000 embtechx-1.0.4/embtechx/dataframe.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2441 2024-04-22 10:08:55.000000 embtechx-1.0.4/embtechx/domain_emb.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     7472 2024-04-22 16:40:19.000000 embtechx-1.0.4/embtechx/embedding.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     8300 2024-04-22 10:08:56.000000 embtechx-1.0.4/embtechx/evaluate.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     1660 2024-04-22 10:08:57.000000 embtechx-1.0.4/embtechx/search.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-23 02:27:31.565927 embtechx-1.0.4/embtechx.egg-info/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      258 2024-04-23 02:27:31.000000 embtechx-1.0.4/embtechx.egg-info/PKG-INFO
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      295 2024-04-23 02:27:31.000000 embtechx-1.0.4/embtechx.egg-info/SOURCES.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-23 02:27:31.000000 embtechx-1.0.4/embtechx.egg-info/dependency_links.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       86 2024-04-23 02:27:31.000000 embtechx-1.0.4/embtechx.egg-info/requires.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        9 2024-04-23 02:27:31.000000 embtechx-1.0.4/embtechx.egg-info/top_level.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-23 02:27:31.567134 embtechx-1.0.4/setup.cfg
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      364 2024-04-22 16:40:55.000000 embtechx-1.0.4/setup.py
```

### Comparing `embtechx-1.0.3/embtechx/__init__.py` & `embtechx-1.0.4/embtechx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .embedding import emb_train
 embedding = emb_train.sentence_embedding
 create_test_train = emb_train.create_test_train
 train_model = emb_train.train_model
 train_model_customize = emb_train.train_model_customize
 
 train_model_only = emb_train.train_model_only
-train_model_customize_only = emb_train.train_model__only_customize
+train_model__only_customize = emb_train.train_model__only_customize
 
 from .evaluate import eval_model
 evaluate = eval_model.evaluate
 evaluate_svm = eval_model.accuracy_svm
 evaluate_knn = eval_model.accuracy_knn
 evaluate_naive_bayes = eval_model.accuracy_naive_bayes
 evaluate_pca = eval_model.evaluate_pca
```

### Comparing `embtechx-1.0.3/embtechx/dataframe.py` & `embtechx-1.0.4/embtechx/dataframe.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.3/embtechx/domain_emb.py` & `embtechx-1.0.4/embtechx/domain_emb.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.3/embtechx/embedding.py` & `embtechx-1.0.4/embtechx/embedding.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.3/embtechx/evaluate.py` & `embtechx-1.0.4/embtechx/evaluate.py`

 * *Files identical despite different names*

### Comparing `embtechx-1.0.3/embtechx/search.py` & `embtechx-1.0.4/embtechx/search.py`

 * *Files identical despite different names*

