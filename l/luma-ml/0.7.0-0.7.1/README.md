# Comparing `tmp/luma-ml-0.7.0.tar.gz` & `tmp/luma-ml-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.7.0.tar", last modified: Fri Apr 19 13:30:16 2024, max compression
+gzip compressed data, was "luma-ml-0.7.1.tar", last modified: Tue Apr 23 16:20:04 2024, max compression
```

## Comparing `luma-ml-0.7.0.tar` & `luma-ml-0.7.1.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.188654 luma-ml-0.7.0/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.0/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-19 13:30:16.188345 luma-ml-0.7.0/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-04-19 13:29:32.000000 luma-ml-0.7.0/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.165301 luma-ml-0.7.0/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    10173 2024-04-18 20:22:41.000000 luma-ml-0.7.0/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.0/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.168248 luma-ml-0.7.0/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12269 2024-04-04 10:30:54.000000 luma-ml-0.7.0/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7627 2024-04-04 10:35:57.000000 luma-ml-0.7.0/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5539 2024-04-04 10:36:09.000000 luma-ml-0.7.0/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8951 2024-04-04 10:36:38.000000 luma-ml-0.7.0/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8854 2024-04-04 18:17:19.000000 luma-ml-0.7.0/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9534 2024-04-04 10:37:54.000000 luma-ml-0.7.0/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.170910 luma-ml-0.7.0/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17258 2024-04-04 10:38:24.000000 luma-ml-0.7.0/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17399 2024-04-04 10:39:29.000000 luma-ml-0.7.0/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7670 2024-04-04 10:39:48.000000 luma-ml-0.7.0/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17693 2024-04-04 10:41:26.000000 luma-ml-0.7.0/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8017 2024-04-04 11:10:57.000000 luma-ml-0.7.0/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11402 2024-04-04 11:13:10.000000 luma-ml-0.7.0/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.171949 luma-ml-0.7.0/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5248 2024-04-14 08:02:38.000000 luma-ml-0.7.0/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-04-18 09:50:34.000000 luma-ml-0.7.0/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11480 2024-04-18 20:49:42.000000 luma-ml-0.7.0/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.174458 luma-ml-0.7.0/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9715 2024-04-04 11:13:31.000000 luma-ml-0.7.0/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19224 2024-04-04 11:16:30.000000 luma-ml-0.7.0/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9631 2024-04-04 11:17:33.000000 luma-ml-0.7.0/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13548 2024-04-04 11:17:49.000000 luma-ml-0.7.0/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6479 2024-04-04 11:18:40.000000 luma-ml-0.7.0/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.175138 luma-ml-0.7.0/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.0/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17510 2024-04-19 13:20:09.000000 luma-ml-0.7.0/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.175994 luma-ml-0.7.0/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1471 2024-03-17 17:44:55.000000 luma-ml-0.7.0/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5709 2024-03-17 18:40:44.000000 luma-ml-0.7.0/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1551 2024-03-19 13:36:06.000000 luma-ml-0.7.0/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1646 2024-03-19 16:59:18.000000 luma-ml-0.7.0/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.176172 luma-ml-0.7.0/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.0/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.178227 luma-ml-0.7.0/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3267 2024-04-04 17:34:24.000000 luma-ml-0.7.0/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7679 2024-04-04 17:35:02.000000 luma-ml-0.7.0/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11844 2024-04-11 14:17:07.000000 luma-ml-0.7.0/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5219 2024-04-18 21:02:26.000000 luma-ml-0.7.0/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.179628 luma-ml-0.7.0/luma/neural/
--rw-r--r--   0 chanlee    (501) staff       (20)     1387 2024-04-18 21:57:58.000000 luma-ml-0.7.0/luma/neural/activation.py
--rw-r--r--   0 chanlee    (501) staff       (20)    20652 2024-04-19 13:30:12.000000 luma-ml-0.7.0/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)      669 2024-04-18 23:27:35.000000 luma-ml-0.7.0/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16728 2024-04-18 19:59:40.000000 luma-ml-0.7.0/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    20833 2024-04-18 21:58:02.000000 luma-ml-0.7.0/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8208 2024-04-11 14:52:27.000000 luma-ml-0.7.0/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.179840 luma-ml-0.7.0/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7217 2024-04-11 12:45:03.000000 luma-ml-0.7.0/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.180544 luma-ml-0.7.0/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5293 2024-04-10 12:13:12.000000 luma-ml-0.7.0/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5531 2024-04-10 12:30:21.000000 luma-ml-0.7.0/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3600 2024-04-10 19:13:28.000000 luma-ml-0.7.0/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2553 2024-04-18 16:23:01.000000 luma-ml-0.7.0/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.181791 luma-ml-0.7.0/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18446 2024-04-04 11:25:12.000000 luma-ml-0.7.0/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39139 2024-04-04 15:10:56.000000 luma-ml-0.7.0/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16170 2024-04-05 18:23:54.000000 luma-ml-0.7.0/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.183678 luma-ml-0.7.0/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19091 2024-04-06 10:17:17.000000 luma-ml-0.7.0/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12178 2024-04-07 16:01:11.000000 luma-ml-0.7.0/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6636 2024-04-07 19:41:56.000000 luma-ml-0.7.0/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2960 2024-04-07 20:18:45.000000 luma-ml-0.7.0/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10678 2024-04-08 19:03:59.000000 luma-ml-0.7.0/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7486 2024-04-10 11:10:31.000000 luma-ml-0.7.0/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7187 2024-04-10 11:41:01.000000 luma-ml-0.7.0/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.184321 luma-ml-0.7.0/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.0/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24471 2024-04-13 15:18:20.000000 luma-ml-0.7.0/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.186155 luma-ml-0.7.0/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1636 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-19 13:30:16.188716 luma-ml-0.7.0/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-19 13:29:14.000000 luma-ml-0.7.0/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.187665 luma-ml-0.7.0/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-03-30 12:09:50.000000 luma-ml-0.7.0/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2005 2024-04-19 13:25:48.000000 luma-ml-0.7.0/test/__test.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2059 2024-04-18 22:07:38.000000 luma-ml-0.7.0/test/_mlp.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.247055 luma-ml-0.7.1/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.1/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-23 16:20:04.246658 luma-ml-0.7.1/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-04-23 15:45:00.000000 luma-ml-0.7.1/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.230214 luma-ml-0.7.1/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10349 2024-04-23 15:02:10.000000 luma-ml-0.7.1/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.1/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.231884 luma-ml-0.7.1/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-21 11:35:44.000000 luma-ml-0.7.1/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.1/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.1/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.1/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.1/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.1/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.232982 luma-ml-0.7.1/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.1/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.1/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.1/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.1/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.1/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.1/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.233887 luma-ml-0.7.1/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5248 2024-04-14 08:02:38.000000 luma-ml-0.7.1/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-04-18 09:50:34.000000 luma-ml-0.7.1/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11480 2024-04-18 20:49:42.000000 luma-ml-0.7.1/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.235090 luma-ml-0.7.1/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.1/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.1/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.1/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.1/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.1/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.235964 luma-ml-0.7.1/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.1/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2696 2024-04-21 13:53:19.000000 luma-ml-0.7.1/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14826 2024-04-23 15:24:58.000000 luma-ml-0.7.1/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.236723 luma-ml-0.7.1/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1473 2024-04-21 11:35:58.000000 luma-ml-0.7.1/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5742 2024-04-21 11:35:59.000000 luma-ml-0.7.1/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1553 2024-04-21 11:36:01.000000 luma-ml-0.7.1/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1648 2024-04-21 11:36:02.000000 luma-ml-0.7.1/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.237181 luma-ml-0.7.1/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.1/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.237908 luma-ml-0.7.1/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.1/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.1/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.1/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-04-21 11:36:06.000000 luma-ml-0.7.1/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.239811 luma-ml-0.7.1/luma/neural/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1154 2024-04-23 15:01:38.000000 luma-ml-0.7.1/luma/neural/activation.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4350 2024-04-23 16:17:50.000000 luma-ml-0.7.1/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1673 2024-04-23 16:10:06.000000 luma-ml-0.7.1/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    22320 2024-04-23 16:19:59.000000 luma-ml-0.7.1/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2681 2024-04-23 14:55:20.000000 luma-ml-0.7.1/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16804 2024-04-23 15:06:00.000000 luma-ml-0.7.1/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    20835 2024-04-21 11:36:11.000000 luma-ml-0.7.1/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.1/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.240030 luma-ml-0.7.1/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.1/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.240733 luma-ml-0.7.1/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.1/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.1/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.1/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.1/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.241576 luma-ml-0.7.1/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.1/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.1/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.1/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.243482 luma-ml-0.7.1/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.1/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.1/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.1/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.1/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.1/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.1/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.1/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.243921 luma-ml-0.7.1/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.1/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.1/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.244981 luma-ml-0.7.1/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1701 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-23 16:20:04.000000 luma-ml-0.7.1/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-23 16:20:04.247154 luma-ml-0.7.1/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-23 15:45:10.000000 luma-ml-0.7.1/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-23 16:20:04.245998 luma-ml-0.7.1/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.1/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2108 2024-04-23 16:13:28.000000 luma-ml-0.7.1/test/__test.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2059 2024-04-21 12:40:24.000000 luma-ml-0.7.1/test/_mlp.py
```

### Comparing `luma-ml-0.7.0/LICENSE` & `luma-ml-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.0/PKG-INFO` & `luma-ml-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.01k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.07k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.0</td>
+                    <td>0.7.1</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~17.4K</td>
+                    <td>~17.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.0 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.1 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.01k-red][GitHub code size in bytes][Code Style]
+5.07k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.0
-Lines of Code  ~17.4K
+Latest Version 0.7.1
+Lines of Code  ~17.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.0/README.md` & `luma-ml-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.01k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.07k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.0</td>
+                    <td>0.7.1</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~17.4K</td>
+                    <td>~17.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.01k-red][GitHub code size in bytes][Code Style]
+5.07k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.0
-Lines of Code  ~17.4K
+Latest Version 0.7.1
+Lines of Code  ~17.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.0/luma/__import__.py` & `luma-ml-0.7.1/luma/__import__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from luma.core.main import Luma
 from luma.core.base import ModelBase, ParadigmBase, MetricBase, VisualBase
 from luma.core.super import Estimator, Transformer, Optimizer, Evaluator, Visualizer
 from luma.core.super import Supervised, Unsupervised, Distance
 
-from luma.interface.exception import NotFittedError, NotConvergedError
 from luma.interface.exception import (
+    NotFittedError,
+    NotConvergedError,
     UnsupportedParameterError,
     ModelExtensionError,
     InvalidRangeError,
 )
-from luma.interface.util import (
+from luma.interface.typing import (
+    TensorLike,
     Matrix,
     Vector,
     Tensor,
     Scalar,
+)
+from luma.interface.util import (
     DecisionTreeNode,
     NearestNeighbors,
+    SilhouetteUtil,
+    DBUtil,
+    KernelUtil,
+    ActivationUtil,
+    InitUtil,
+    Clone,
+    ParamRange,
 )
-from luma.interface.util import SilhouetteUtil, DBUtil, KernelUtil, ActivationUtil
-from luma.interface.util import Clone, ParamRange, Layer, Loss
 
 from luma.classifier.discriminant import (
     LDAClassifier,
     QDAClassifier,
     RDAClassifier,
     KDAClassifier,
 )
@@ -57,30 +66,32 @@
 from luma.ensemble.forest import RandomForestClassifier, RandomForestRegressor
 from luma.ensemble.vote import VotingClassifier, VotingRegressor
 from luma.ensemble.bagging import BaggingClassifier, BaggingRegressor
 from luma.ensemble.boost import AdaBoostClassifier, AdaBoostRegressor
 from luma.ensemble.boost import GradientBoostingClassifier, GradientBoostingRegressor
 from luma.ensemble.stack import StackingClassifier, StackingRegressor
 
-from luma.neural.activation import ReLU, LeakyReLU, ELU, Tanh, Sigmoid, Softmax
+from luma.neural.activation import ReLU, LeakyReLU, ELU, Tanh, Sigmoid
 from luma.neural.optimizer import (
     SGDOptimizer,
     MomentumOptimizer,
     RMSPropOptimizer,
     AdamOptimizer,
     AdaGradOptimizer,
     AdaDeltaOptimizer,
     AdaMaxOptimizer,
     AdamWOptimizer,
     NAdamOptimizer,
 )
 from luma.neural.single import PerceptronClassifier, PerceptronRegressor
 from luma.neural.network import MLPClassifier, MLPRegressor
+from luma.neural.base import Layer, Loss, Initializer
 from luma.neural.layer import Convolution, Pooling, Dense, Dropout, Flatten, Sequential
-from luma.neural.loss import CategoricalCrossEntropy
+from luma.neural.loss import SoftmaxLoss, CrossEntropyLoss, MSELoss
+from luma.neural.init import KaimingInit, XavierInit
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
     MeanAbsolutePercentageError,
@@ -162,18 +173,19 @@
     Supervised, Unsupervised, Distance
 
     # ----------------- [ luma.interface ] ---------------------
     NotFittedError, NotConvergedError,
     UnsupportedParameterError, ModelExtensionError,
     InvalidRangeError
 
-    Matrix, Vector, Tensor, Scalar,
+    TensorLike, Matrix, Vector, Tensor, Scalar
+
     DecisionTreeNode, NearestNeighbors,
     SilhouetteUtil, DBUtil, KernelUtil, ActivationUtil,
-    Clone, ParamRange, Layer, Loss
+    InitUtil, Clone, ParamRange
 
     # ----------------- [ luma.classifier ] --------------------
     LDAClassifier, QDAClassifier, RDAClassifier, KDAClassifier
 
     LogisticRegressor, SoftmaxRegressor
 
     GaussianNaiveBayes, BernoulliNaiveBayes
@@ -214,23 +226,27 @@
     StackingClassifier, StackingRegressor
 
     # ------------------- [ luma.neural ] ----------------------
     PerceptronClassifier, PerceptronRegressor
 
     MLPClassifier, MLPRegressor
 
-    ReLU, LeakyReLU, ELU, Tanh, Sigmoid, Softmax
+    ReLU, LeakyReLU, ELU, Tanh, Sigmoid
 
     SGDOptimizer, MomentumOptimizer, RMSPropOptimizer,
     AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
     AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
+    Layer, Loss, Initializer
+
     Convolution, Pooling, Dense, Dropout, Flatten, Sequential
 
-    CategoricalCrossEntropy
+    SoftmaxLoss, CrossEntropyLoss, MSELoss
+
+    KaimingInit, XavierInit
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
     MeanAbsolutePercentageError, RSquaredScore,
     AdjustedRSquaredScore
```

### Comparing `luma-ml-0.7.0/luma/__init__.py` & `luma-ml-0.7.1/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.0/luma/classifier/discriminant.py` & `luma-ml-0.7.1/luma/classifier/discriminant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Self
 from scipy.special import softmax
 from scipy.stats import multivariate_normal
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
-from luma.interface.util import Matrix, Scalar, Vector, KernelUtil
+from luma.interface.typing import Matrix, Scalar, Vector
+from luma.interface.util import KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.metric.classification import Accuracy
 
 
 __all__ = ("LDAClassifier", "QDAClassifier", "RDAClassifier", "KDAClassifier")
```

### Comparing `luma-ml-0.7.0/luma/classifier/logistic.py` & `luma-ml-0.7.1/luma/classifier/logistic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Literal, Self
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.metric.classification import Accuracy
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 
 
 __all__ = ("LogisticRegressor", "SoftmaxRegressor")
```

### Comparing `luma-ml-0.7.0/luma/classifier/naive_bayes.py` & `luma-ml-0.7.1/luma/classifier/naive_bayes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Self
 import numpy as np
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.classification import Accuracy
 
 
 __all__ = ("GaussianNaiveBayes", "BernoulliNaiveBayes")
```

### Comparing `luma-ml-0.7.0/luma/classifier/neighbors.py` & `luma-ml-0.7.1/luma/classifier/neighbors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Self
 from scipy.spatial import distance_matrix
 import numpy as np
 
-from luma.interface.util import Matrix
 from luma.core.super import Estimator, Supervised, Evaluator
+from luma.interface.typing import Matrix
 from luma.interface.util import NearestNeighbors
 from luma.interface.exception import NotFittedError
 from luma.metric.classification import Accuracy
 
 
 __all__ = ("KNNClassifier", "AdaptiveKNNClassifier", "WeightedKNNClassifier")
```

### Comparing `luma-ml-0.7.0/luma/classifier/svm.py` & `luma-ml-0.7.1/luma/classifier/svm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Self
 import numpy as np
 
-from luma.interface.util import Matrix, KernelUtil
+from luma.interface.typing import Matrix
+from luma.interface.util import KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.classification import Accuracy
 
 
 __all__ = ("SVC", "KernelSVC")
```

### Comparing `luma-ml-0.7.0/luma/classifier/tree.py` & `luma-ml-0.7.1/luma/classifier/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Literal, Self, Tuple
 import numpy as np
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import DecisionTreeNode
 from luma.metric.classification import Accuracy
 
 
 __all__ = "DecisionTreeClassifier"
```

### Comparing `luma-ml-0.7.0/luma/clustering/affinity.py` & `luma-ml-0.7.1/luma/clustering/affinity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Literal, Self
 import numpy as np
 
-from luma.interface.util import Matrix, Vector, Scalar, KernelUtil
+from luma.interface.typing import Matrix, Vector, Scalar
+from luma.interface.util import KernelUtil
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.clustering import SilhouetteCoefficient
 
 
 __all__ = (
     "AffinityPropagation",
```

### Comparing `luma-ml-0.7.0/luma/clustering/density.py` & `luma-ml-0.7.1/luma/clustering/density.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal, Optional, Self, Tuple, List
 from matplotlib import pyplot as plt
 from scipy.spatial.distance import cdist
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Unsupervised
-from luma.interface.util import Matrix, Vector, Scalar
+from luma.interface.typing import Matrix, Vector, Scalar
 from luma.interface.exception import NotFittedError, NotConvergedError
 from luma.interface.exception import UnsupportedParameterError
 
 from luma.metric.distance import Euclidean, Minkowski
 from luma.metric.clustering import SilhouetteCoefficient
```

### Comparing `luma-ml-0.7.0/luma/clustering/hierarchy.py` & `luma-ml-0.7.1/luma/clustering/hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal, Optional, Self, Tuple
 from scipy.spatial.distance import pdist, squareform
 from scipy.cluster.hierarchy import linkage, dendrogram
 import matplotlib.pyplot as plt
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.clustering.kmeans import KMeansClusteringPlus
 from luma.metric.clustering import SilhouetteCoefficient
 
 
 __all__ = ("AgglomerativeClustering", "DivisiveClustering")
```

### Comparing `luma-ml-0.7.0/luma/clustering/kmeans.py` & `luma-ml-0.7.1/luma/clustering/kmeans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Self
 import numpy as np
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.metric.clustering import SilhouetteCoefficient
 
 
 __all__ = (
     "KMeansClustering",
```

### Comparing `luma-ml-0.7.0/luma/clustering/mixture.py` & `luma-ml-0.7.1/luma/clustering/mixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Unsupervised
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.metric.clustering import SilhouetteCoefficient
 from luma.interface.exception import NotFittedError
 
 
 __all__ = ("GaussianMixture", "MultinomialMixture")
```

### Comparing `luma-ml-0.7.0/luma/clustering/spectral.py` & `luma-ml-0.7.1/luma/clustering/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from scipy.spatial.distance import pdist, squareform
 from scipy.linalg import eigh
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.clustering.kmeans import KMeansClusteringPlus
 from luma.clustering.hierarchy import AgglomerativeClustering, DivisiveClustering
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.clustering import SilhouetteCoefficient
 
 
 __all__ = (
     "SpectralClustering",
```

### Comparing `luma-ml-0.7.0/luma/core/base.py` & `luma-ml-0.7.1/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.0/luma/core/super.py` & `luma-ml-0.7.1/luma/core/super.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.0/luma/ensemble/bagging.py` & `luma-ml-0.7.1/luma/ensemble/bagging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Any, Dict, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
-from luma.interface.util import Matrix, Vector, Clone
+from luma.interface.typing import Matrix, Vector
+from luma.interface.util import Clone
 from luma.interface.exception import NotFittedError
+
 from luma.classifier.tree import DecisionTreeClassifier
 from luma.regressor.tree import DecisionTreeRegressor
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = ("BaggingClassifier", "BaggingRegressor")
```

### Comparing `luma-ml-0.7.0/luma/ensemble/boost.py` & `luma-ml-0.7.1/luma/ensemble/boost.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any, Dict, List, Literal, Self, Tuple
 from scipy.special import softmax
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
-from luma.interface.util import Matrix, Vector, Clone
+from luma.interface.typing import Matrix, Vector
+from luma.interface.util import Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
+
 from luma.classifier.tree import DecisionTreeClassifier
 from luma.regressor.tree import DecisionTreeRegressor
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
```

### Comparing `luma-ml-0.7.0/luma/ensemble/forest.py` & `luma-ml-0.7.1/luma/ensemble/forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal, Self
 from scipy.stats import mode
 import numpy as np
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.classifier.tree import DecisionTreeClassifier
 from luma.regressor.tree import DecisionTreeRegressor
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
```

### Comparing `luma-ml-0.7.0/luma/ensemble/stack.py` & `luma-ml-0.7.1/luma/ensemble/stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, List, Dict, Literal, Self
 import numpy as np
 
 from luma.core.super import Estimator, Transformer, Evaluator, Supervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.classifier.logistic import SoftmaxRegressor
 from luma.regressor.linear import LinearRegressor
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 from luma.model_selection.fold import FoldType, KFold
```

### Comparing `luma-ml-0.7.0/luma/ensemble/vote.py` & `luma-ml-0.7.1/luma/ensemble/vote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List, Literal, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
-from luma.interface.util import Matrix, Vector, Scalar, Clone
+from luma.interface.typing import Matrix, Vector, Scalar
+from luma.interface.util import Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
+
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 from luma.preprocessing.encoder import LabelEncoder
 
 
 __all__ = ("VotingClassifier", "VotingRegressor")
```

### Comparing `luma-ml-0.7.0/luma/interface/exception.py` & `luma-ml-0.7.1/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.0/luma/interface/util.py` & `luma-ml-0.7.1/luma/interface/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,110 +1,28 @@
-from typing import Any, AnyStr, Callable, Literal, Self, Tuple, Type, TypeGuard
+from typing import Any, AnyStr, Callable, Literal, Optional, Type, TypeGuard
 import numpy as np
 
 from luma.interface.exception import UnsupportedParameterError, InvalidRangeError
-from luma.neural import activation
+from luma.interface.typing import Matrix, Scalar
+from luma.neural import activation, init
 
 
 __all__ = (
-    "Matrix",
-    "Vector",
-    "Tensor",
-    "Scalar",
     "DecisionTreeNode",
     "NearestNeighbors",
     "SilhouetteUtil",
     "DBUtil",
     "KernelUtil",
     "ActivationUtil",
+    "InitUtil",
     "Clone",
     "ParamRange",
-    "Layer",
-    "Loss",
 )
 
 
-type TensorLike = Matrix | Tensor | Vector
-
-
-class Matrix(np.ndarray):
-    """
-    Internal class for matrices(2D-array) that extends `numpy.ndarray`.
-
-    This class provides a way to create matrix objects that have
-    all the capabilities of numpy arrays with the potential for
-    additional functionalities and readability.
-
-    Example
-    -------
-    >>> m = Matrix([1, 2, 3])
-    >>> isinstance(m, numpy.ndarray) # True
-
-    """
-
-    def __new__(cls, array_like: Any) -> Self:
-        if isinstance(array_like, (list, np.matrix)):
-            obj = np.array(array_like)
-        else:
-            obj = array_like
-        return obj
-
-    def __array_finalize__(self, obj: np.ndarray | None) -> None:
-        if obj is None:
-            return
-
-
-class Vector(Matrix):
-    """
-    Internal class for vectors(1D-array) that extends `Matrix`.
-
-    This class represents a single row/column vector with its
-    type of `numpy.ndarray` or `Matrix`.
-
-    """
-
-    def __new__(cls, array_like: Any) -> Self:
-        if isinstance(array_like, list):
-            obj = Matrix(array_like)
-        else:
-            obj = array_like
-        return obj
-
-
-class Tensor(Matrix):
-    """
-    Internal class for tensors(>=3D-arrray) that extends `Matrix`.
-
-    This class provides a way to create tensor objects that have
-    all the capabilities of numpy arrays with the potential for
-    additional functionalities and readability.
-    """
-
-    type Tensor_3D = "Tensor"
-    type Tensor_4D = "Tensor"
-
-    def __new__(cls, array_like: Any) -> Self:
-        if isinstance(array_like, list):
-            obj = Matrix(array_like)
-        else:
-            obj = array_like
-        return obj
-
-
-class Scalar:
-    """
-    A placeholder class for scalar type.
-
-    This class encompasses `int` and `float`.
-    """
-
-    def __new__(cls, value: int | float) -> Self:
-        return float(value)
-
-
 class DecisionTreeNode:
     """
     Internal class for node used in tree-based models.
 
     Parameters
     ----------
     `feature_index` : Feature of node
@@ -349,57 +267,76 @@
 class ActivationUtil:
     """
     Internal class for activaiton functions used in neural networks.
 
     Properties
     ----------
     For getting an activation function class:
-        ```py
-        @property
-        def activation_type(self) -> type
-        ```
+    ```py
+    @property
+    def activation_type(self) -> type
+    ```
+
+    Notes
+    -----
+    When the passed activation is `None`, an identity activation is
+    returned, with its function and gradient being identity functions.
 
     Examples
     --------
     >>> act = ActivationUtil(activation='relu')
     >>> relu = act.activation_type
     ReLU()
 
     """
 
-    FuncType = Literal[
-        "relu",
-        "ReLU",
-        "leaky-relu",
-        "leaky-ReLU",
-        "elu",
-        "ELU",
-        "tanh",
-        "sigmoid",
-        "sig",
-        "softmax",
+    FuncType = Optional[
+        Literal[
+            "relu",
+            "ReLU",
+            "leaky-relu",
+            "leaky-ReLU",
+            "elu",
+            "ELU",
+            "tanh",
+            "sigmoid",
+            "sig",
+        ]
     ]
 
     def __init__(self, activation: str) -> None:
         self.activation = activation
 
     @property
     def activation_type(self) -> type:
+        if self.activation is None:
+            return self._return_identity()
+
         if self.activation in ("relu", "ReLU"):
             return activation.ReLU
         elif self.activation in ("leaky-relu", "leaky-ReLU"):
             return activation.LeakyReLU
         elif self.activation in ("elu", "ELU"):
             return activation.ELU
         elif self.activation in ("tanh"):
             return activation.Tanh
         elif self.activation in ("sigmoid", "sig"):
             return activation.Sigmoid
-        elif self.activation in ("softmax"):
-            return activation.Softmax
+        else:
+            raise UnsupportedParameterError(self.activation)
+
+    def _return_identity(self) -> type:
+        class _Identity:
+            def func(self, X: Matrix) -> Matrix:
+                return X
+
+            def grad(self, X: Matrix) -> Matrix:
+                return X
+
+        return _Identity
 
 
 class Clone:
     """
     A utility class for cloning LUMA models.
 
     This class creates a copy of a given LUMA model,
@@ -539,97 +476,54 @@
             return lambda x: lower <= x < upper
         elif not lower_open and not upper_open:
             return lambda x: lower <= x <= upper
         else:
             NotImplemented
 
 
-class Layer:
+class InitUtil:
     """
-    An internal class for layers in neural networks.
-
-    Neural network layers are composed of interconnected nodes,
-    each performing computations on input data. Common types include
-    fully connected, convolutional, and recurrent layers, each
-    serving distinct roles in learning from data.
+    An utility class for weight initializers used in neural networks.
 
-    Attributes
+    Parameters
     ----------
-    - `weights_` : Weight tensor
-    - `biases_` : Bias tensor
-    - `dX` : Gradient w.r.t. the input
-    - `dW` : Gradient w.r.t. the weights
-    - `dB` : Gradient w.r.t. the biases
-    - `optimizer` : Optimizer for certain layer
-    - `out_shape` : Shape of the output when forwarding
+    `initializer` : Name of an initializer (`InitType`)
+    `activation` : Name of an activation function (`FuncType`)
 
     Properties
     ----------
-    To get its parameter size (weights, biases):
+    To get the corresponding initializer type:
     ```py
-    (property) param_size: Tuple[int, int]
+    @property
+    def initializer_type(self) -> type | None
+    # `None` for random init
     ```
     """
 
-    def __init__(self) -> None:
-        self.input_: Tensor = None
-        self.weights_: Tensor = None
-        self.biases_: Vector = None
-
-        self.dX: Tensor = None
-        self.dW: Tensor = None
-        self.dB: Tensor = None
-
-        self.optimizer: object = None
-        self.out_shape: tuple = None
+    InitType = Literal["he", "kaiming", "xavier", "auto", "random"]
 
-    def forward(self) -> Tensor: ...
-
-    def backward(self) -> Tensor: ...
-
-    def update(self) -> None:
-        if self.optimizer is None:
-            return
-        weights_, biases_ = self.optimizer.update(
-            self.weights_, self.biases_, self.dW, self.dB
-        )
-        self.weights_ = Tensor(weights_)
-        self.biases_ = Tensor(biases_)
+    def __init__(
+        self,
+        initializer: InitType,
+        activation: ActivationUtil.FuncType,
+    ) -> None:
+        self.initializer = initializer
+        self.activation = activation
 
     @property
-    def param_size(self) -> Tuple[int, int]:
-        w_size, b_size = 0, 0
-        if self.weights_ is not None:
-            w_size += len(self.weights_.flatten())
-        if self.biases_ is not None:
-            b_size += len(self.biases_.flatten())
-
-        return w_size, b_size
-
-    def __str__(self) -> str:
-        return type(self).__name__
-
-    def __repr__(self) -> str:
-        w_size, b_size = self.param_size
-        return (
-            f"{type(self).__name__}: "
-            + f"({w_size:,} weights, {b_size:,} biases)"
-            + f" -> {w_size + b_size:,} params"
-        )
-
-
-class Loss:
-    """
-    An internal class for loss functions used in neural networks.
-
-    Loss functions, integral to the training process of machine
-    learning models, serve as crucial metrics assessing the disparity
-    between predicted outcomes and ground truth labels. They play a
-    pivotal role in optimization algorithms, guiding parameter updates
-    towards minimizing the discrepancy between predictions and true values.
-    """
-
-    def __init__(self) -> None: ...
+    def initializer_type(self) -> type | None:
+        if self.initializer == "auto":
+            return self._auto_init()
+        else:
+            return self._manual_init()
 
-    def loss(self) -> float: ...
+    def _manual_init(self) -> type | None:
+        if self.initializer in ("he", "kaiming"):
+            return init.KaimingInit
+        elif self.initializer in ("xavier"):
+            return init.XavierInit
 
-    def grad(self) -> Matrix: ...
+    def _auto_init(self) -> type | None:
+        if self.activation in ("relu", "ReLU"):
+            return init.KaimingInit
+        elif self.activation in ("tanh", "sigmoid", "sig"):
+            return init.XavierInit
```

### Comparing `luma-ml-0.7.0/luma/metric/classification.py` & `luma-ml-0.7.1/luma/metric/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.core.super import Evaluator
 
 
 __all__ = ("Accuracy", "Precision", "Recall", "F1Score", "Specificity")
 
 
 class Accuracy(Evaluator):
```

### Comparing `luma-ml-0.7.0/luma/metric/clustering.py` & `luma-ml-0.7.1/luma/metric/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 from scipy.spatial.distance import pdist, squareform
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.core.super import Evaluator, Visualizer
-from luma.interface.util import Matrix, SilhouetteUtil, DBUtil
+from luma.interface.util import SilhouetteUtil, DBUtil
+from luma.interface.typing import Matrix
 
 
 __all__ = ("SilhouetteCoefficient", "DaviesBouldin", "Inertia")
 
 
 class SilhouetteCoefficient(Evaluator, Visualizer):
     """
```

### Comparing `luma-ml-0.7.0/luma/metric/distance.py` & `luma-ml-0.7.1/luma/metric/distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.core.super import Distance
 
 
 __all__ = (
     "Euclidean",
     "Manhattan",
     "Chebyshev",
```

### Comparing `luma-ml-0.7.0/luma/metric/regression.py` & `luma-ml-0.7.1/luma/metric/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import *
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.core.super import Evaluator
 
 
 __all__ = (
     "MeanAbsoluteError",
     "MeanSquaredError",
     "RootMeanSquaredError",
```

### Comparing `luma-ml-0.7.0/luma/migrate/port.py` & `luma-ml-0.7.1/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.0/luma/model_selection/cv.py` & `luma-ml-0.7.1/luma/model_selection/cv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.model_selection.fold import FoldType, KFold
 
 
 __all__ = "CrossValidator"
 
 
 class CrossValidator(Evaluator):
```

### Comparing `luma-ml-0.7.0/luma/model_selection/fold.py` & `luma-ml-0.7.1/luma/model_selection/fold.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import Counter, defaultdict
 from itertools import chain
 from typing import Generator, Tuple, Union
 import numpy as np
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 
 FoldType = Union["KFold", "StratifiedKFold", "GroupKFold"]
 
 
 __all__ = ("KFold", "StratifiedKFold", "GroupKFold")
```

### Comparing `luma-ml-0.7.0/luma/model_selection/search.py` & `luma-ml-0.7.1/luma/model_selection/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, TypeVar
 from scipy.stats import rv_continuous, rv_discrete
 import numpy as np
 import random
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.core.super import Estimator, Evaluator, Optimizer
 from luma.interface.exception import NotFittedError
 from luma.model_selection.cv import CrossValidator
 from luma.model_selection.fold import FoldType, KFold
 
 DT = TypeVar("DT", bound=rv_continuous | rv_discrete)
```

### Comparing `luma-ml-0.7.0/luma/model_selection/split.py` & `luma-ml-0.7.1/luma/model_selection/split.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Iterator, Tuple
 import numpy as np
 
-from luma.interface.util import Matrix, Vector, TensorLike
+from luma.interface.typing import Matrix, Vector, TensorLike
 
 
 __all__ = ("TrainTestSplit", "BatchGenerator")
 
 
 class TrainTestSplit:
     """
```

### Comparing `luma-ml-0.7.0/luma/neural/activation.py` & `luma-ml-0.7.1/luma/neural/activation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 
+from luma.interface.typing import Matrix
 
-__all__ = ("ReLU", "LeakyReLU", "ELU", "Tanh", "Sigmoid", "Softmax")
 
-
-type Matrix = Matrix
+__all__ = ("ReLU", "LeakyReLU", "ELU", "Tanh", "Sigmoid")
 
 
 class ReLU:
     def func(self, X: Matrix) -> Matrix:
         return np.maximum(0, X)
 
     def grad(self, X: Matrix) -> Matrix:
@@ -47,16 +46,7 @@
 
 class Sigmoid:
     def func(self, X: Matrix) -> Matrix:
         return 1 / (1 + np.exp(-X))
 
     def grad(self, X: Matrix) -> Matrix:
         return X * (1 - X)
-
-
-class Softmax:
-    def func(self, X: Matrix) -> Matrix:
-        exps = np.exp(X - np.max(X, axis=1, keepdims=True))
-        return exps / np.sum(exps, axis=1, keepdims=True)
-
-    def grad(self, _: Matrix) -> Matrix:
-        NotImplemented
```

### Comparing `luma-ml-0.7.0/luma/neural/layer.py` & `luma-ml-0.7.1/luma/neural/layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 from typing import Any, List, Literal, Self, Tuple
 import numpy as np
 
 from luma.core.super import Optimizer
-from luma.interface.util import Layer, Matrix, Tensor, ActivationUtil, Loss, Clone
+from luma.interface.typing import Matrix, Tensor
+from luma.interface.util import ActivationUtil, InitUtil, Clone
 from luma.interface.exception import UnsupportedParameterError
-from luma.neural.activation import Softmax
+from luma.neural.base import Layer, Loss
 
 
-__all__ = ("Convolution", "Pooling", "Dense", "Dropout", "Flatten", "Sequential")
+__all__ = (
+    "Convolution",
+    "Pooling",
+    "Dense",
+    "Dropout",
+    "Flatten",
+    "Sequential",
+)
 
 
 class Convolution(Layer):
     """
     A convolutional layer in a neural network convolves learnable filters
     across input data, detecting patterns like edges or textures, producing
     feature maps essential for tasks such as image recognition within CNNs.
     By sharing parameters, it efficiently extracts hierarchical representations,
     enabling the network to learn complex visual features.
 
     Parameters
     ----------
-    `n_filters` : Number of filters(kernels) to use
-    `size`: Size of each filter
+    `in_channels` : Number of input channels
+    `out_channels` : Number of output channels(filters)
+    `filter_size`: Size of each filter
     `stride` : Step size for filters during convolution
     `padding` : Padding stratagies
     (`valid` for no padding, `same` for typical 0-padding)
     `activation` : Type of activation function
+    `initializer` : Type of weight initializer (default 'auto')
     `optimizer` : Optimizer for weight update (default `SGDOptimizer`)
     `lambda_` : L2-regularization strength
     `random_state` : Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 4D-array(`Tensor`).
@@ -37,139 +47,173 @@
         ```py
         X.shape = (batch_size, channels, height, width)
         ```
     """
 
     def __init__(
         self,
-        n_filters: int,
-        size: int,
+        in_channels: int,
+        out_channels: int,
+        filter_size: int,
         stride: int = 1,
         padding: Literal["valid", "same"] = "same",
         activation: ActivationUtil.FuncType = "relu",
+        initializer: InitUtil.InitType = "auto",
         optimizer: Optimizer = None,
         lambda_: float = 0.0,
         random_state: int = None,
     ) -> None:
         super().__init__()
-        self.n_filters = n_filters
-        self.size = size
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
         self.activation = activation
+        self.initializer = initializer
         self.optimizer = optimizer
         self.lambda_ = lambda_
+        self.random_state = random_state
 
         act = ActivationUtil(self.activation)
         self.act_ = act.activation_type()
-        self.rs_ = np.random.RandomState(random_state)
+        self.rs_ = np.random.RandomState(self.random_state)
 
-        self.biases_: Matrix = np.zeros((1, self.n_filters))
+        self.init_params(
+            w_shape=(
+                self.out_channels,
+                self.in_channels,
+                self.filter_size,
+                self.filter_size,
+            ),
+            b_shape=(1, self.out_channels),
+        )
+        self.set_param_ranges(
+            {
+                "in_channels": ("0<,+inf", int),
+                "out_channels": ("0<,+inf", int),
+                "filter_size": ("0<,+inf", int),
+                "stride": ("0<,+inf", int),
+                "lambda_": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
 
     def forward(self, X: Tensor) -> Tensor:
         self.input_ = X
         batch_size, channels, height, width = X.shape
-
-        if self.weights_ is None:
-            self.weights_ = 0.01 * self.rs_.randn(
-                self.n_filters, channels, self.size, self.size
+        if self.in_channels != channels:
+            raise ValueError(
+                f"channels of 'X' does not match with 'in_channels'! "
+                + f"({self.in_channels}!={channels})"
             )
 
-        pad_h, pad_w, padded_height, padded_width = self._get_padding_dim(height, width)
+        pad_h, pad_w, padded_h, padded_w = self._get_padding_dim(height, width)
 
-        out_height = ((padded_height - self.size) // self.stride) + 1
-        out_width = ((padded_width - self.size) // self.stride) + 1
+        out_height = ((padded_h - self.filter_size) // self.stride) + 1
+        out_width = ((padded_w - self.filter_size) // self.stride) + 1
 
-        out: Tensor = np.zeros((batch_size, self.n_filters, out_height, out_width))
+        out: Tensor = np.zeros(
+            (
+                batch_size,
+                self.out_channels,
+                out_height,
+                out_width,
+            )
+        )
         self.out_shape = out.shape
 
         X_padded = np.pad(
             X, ((0, 0), (0, 0), (pad_h, pad_h), (pad_w, pad_w)), mode="constant"
         )
-        X_fft = np.fft.rfftn(X_padded, s=(padded_height, padded_width), axes=[2, 3])
+        X_fft = np.fft.rfftn(X_padded, s=(padded_h, padded_w), axes=[2, 3])
         filter_fft = np.fft.rfftn(
-            self.weights_, s=(padded_height, padded_width), axes=[2, 3]
+            self.weights_,
+            s=(padded_h, padded_w),
+            axes=[2, 3],
         )
 
         for i in range(batch_size):
-            for f in range(self.n_filters):
+            for f in range(self.out_channels):
                 result_fft = np.sum(X_fft[i] * filter_fft[f], axis=0)
-                result = np.fft.irfftn(result_fft, s=(padded_height, padded_width))
+                result = np.fft.irfftn(result_fft, s=(padded_h, padded_w))
 
                 sampled_result = result[
-                    pad_h : padded_height - pad_h : self.stride,
-                    pad_w : padded_width - pad_w : self.stride,
+                    pad_h : padded_h - pad_h : self.stride,
+                    pad_w : padded_w - pad_w : self.stride,
                 ]
                 out[i, f] = sampled_result[:out_height, :out_width]
 
         out += self.biases_[:, :, np.newaxis, np.newaxis]
         out = self.act_.func(out)
         return out
 
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         batch_size, channels, height, width = X.shape
-        pad_h, pad_w, padded_height, padded_width = self._get_padding_dim(height, width)
+        pad_h, pad_w, padded_h, padded_w = self._get_padding_dim(height, width)
 
-        dX_padded = np.zeros((batch_size, channels, padded_height, padded_width))
+        dX_padded = np.zeros((batch_size, channels, padded_h, padded_w))
         self.dW = np.zeros_like(self.weights_)
         self.dB = np.zeros_like(self.biases_)
 
         X_padded = np.pad(
             X, ((0, 0), (0, 0), (pad_h, pad_h), (pad_w, pad_w)), mode="constant"
         )
-        X_fft = np.fft.rfftn(X_padded, s=(padded_height, padded_width), axes=[2, 3])
-        d_out_fft = np.fft.rfftn(d_out, s=(padded_height, padded_width), axes=[2, 3])
+        X_fft = np.fft.rfftn(X_padded, s=(padded_h, padded_w), axes=[2, 3])
+        d_out_fft = np.fft.rfftn(d_out, s=(padded_h, padded_w), axes=[2, 3])
 
-        for f in range(self.n_filters):
+        for f in range(self.out_channels):
             self.dB[:, f] = np.sum(d_out[:, f, :, :])
 
-        for f in range(self.n_filters):
+        for f in range(self.out_channels):
             for c in range(channels):
-                filter_d_out_fft = np.sum(X_fft[:, c] * d_out_fft[:, f].conj(), axis=0)
+                filter_d_out_fft = np.sum(
+                    X_fft[:, c] * d_out_fft[:, f].conj(),
+                    axis=0,
+                )
                 self.dW[f, c] = np.fft.irfftn(
-                    filter_d_out_fft, s=(padded_height, padded_width)
-                )[pad_h : pad_h + self.size, pad_w : pad_w + self.size]
+                    filter_d_out_fft,
+                    s=(padded_h, padded_w),
+                )[pad_h : pad_h + self.filter_size, pad_w : pad_w + self.filter_size]
 
         self.dW += 2 * self.lambda_ * self.weights_
 
         for i in range(batch_size):
             for c in range(channels):
-                temp = np.zeros(
-                    (padded_height, padded_width // 2 + 1), dtype=np.complex128
-                )
-                for f in range(self.n_filters):
+                temp = np.zeros((padded_h, padded_w // 2 + 1), dtype=np.complex128)
+                for f in range(self.out_channels):
                     filter_fft = np.fft.rfftn(
-                        self.weights_[f, c], s=(padded_height, padded_width)
+                        self.weights_[f, c], s=(padded_h, padded_w)
                     )
                     temp += filter_fft * d_out_fft[i, f]
-                dX_padded[i, c] = np.fft.irfftn(temp, s=(padded_height, padded_width))
+                dX_padded[i, c] = np.fft.irfftn(temp, s=(padded_h, padded_w))
 
         self.dX = (
             dX_padded[:, :, pad_h:-pad_h, pad_w:-pad_w]
             if pad_h > 0 or pad_w > 0
             else dX_padded
         )
         self.dX = self.act_.grad(self.dX)
         return self.dX
 
     def _get_padding_dim(self, height: int, width: int) -> Tuple[int, int, int, int]:
         if self.padding == "same":
-            pad_h = pad_w = (self.size - 1) // 2
-            padded_height = height + 2 * pad_h
-            padded_width = width + 2 * pad_w
+            pad_h = pad_w = (self.filter_size - 1) // 2
+            padded_h = height + 2 * pad_h
+            padded_w = width + 2 * pad_w
 
         elif self.padding == "valid":
             pad_h = pad_w = 0
-            padded_height = height
-            padded_width = width
+            padded_h = height
+            padded_w = width
         else:
             raise UnsupportedParameterError(self.padding)
 
-        return pad_h, pad_w, padded_height, padded_width
+        return pad_h, pad_w, padded_h, padded_w
 
 
 class Pooling(Layer):
     """
     A pooling layer in a neural network reduces the spatial dimensions of
     feature maps, reducing computational complexity. It aggregates neighboring
     values, typically through operations like max pooling or average pooling,
@@ -190,26 +234,37 @@
 
         ```py
         X.shape = (batch_size, channels, height, width)
         ```
     """
 
     def __init__(
-        self, size: int = 2, stride: int = 2, mode: Literal["max", "avg"] = "max"
+        self,
+        filter_size: int = 2,
+        stride: int = 2,
+        mode: Literal["max", "avg"] = "max",
     ) -> None:
         super().__init__()
-        self.size = size
+        self.filter_size = filter_size
         self.stride = stride
         self.mode = mode
 
+        self.set_param_ranges(
+            {
+                "filter_size": ("0<,+inf", int),
+                "stride": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
     def forward(self, X: Tensor) -> Tensor:
         self.input_ = X
         batch_size, channels, height, width = X.shape
-        out_height = 1 + (height - self.size) // self.stride
-        out_width = 1 + (width - self.size) // self.stride
+        out_height = 1 + (height - self.filter_size) // self.stride
+        out_width = 1 + (width - self.filter_size) // self.stride
 
         out: Tensor = np.zeros((batch_size, channels, out_height, out_width))
         self.out_shape = out.shape
 
         for i in range(out_height):
             for j in range(out_width):
                 h_start, h_end, w_start, w_end = self._get_height_width(i, j)
@@ -239,23 +294,23 @@
                     mask_ = window == max_vals
                     self.dX[:, :, h_start:h_end, w_start:w_end] += (
                         mask_ * d_out[:, :, i : i + 1, j : j + 1]
                     )
                 elif self.mode == "avg":
                     self.dX[:, :, h_start:h_end, w_start:w_end] += d_out[
                         :, :, i : i + 1, j : j + 1
-                    ] / (self.size**2)
+                    ] / (self.filter_size**2)
 
         return self.dX
 
     def _get_height_width(self, cur_h: int, cur_w: int) -> Tuple[int, int, int, int]:
         h_start = cur_h * self.stride
         w_start = cur_w * self.stride
-        h_end = h_start + self.size
-        w_end = w_start + self.size
+        h_end = h_start + self.filter_size
+        w_end = w_start + self.filter_size
 
         return h_start, h_end, w_start, w_end
 
 
 class Dense(Layer):
     """
     A dense layer, also known as a fully connected layer, connects each
@@ -264,17 +319,18 @@
     enabling complex relationships between input and output. Dense layers
     are fundamental in deep learning models for learning representations from
     data. They play a crucial role in capturing intricate patterns and
     features during the training process.
 
     Parameters
     ----------
-    `input_size` : Number of input neurons
-    `output_size`:  Number of output neurons
+    `in_features` : Number of input features
+    `out_features`:  Number of output features
     `activation` : Activation function (Use `Sigmoid` for final dense layer)
+    `initializer` : Type of weight initializer (default `auto`)
     `optimizer` : Optimizer for weight update (default `SGDOptimizer`)
     `lambda_` : L2-regularization strength
     `random_state` : Seed for various random sampling processes
 
     Notes
     -----
     - The input `X` must have the form of 2D-array(`Matrix`).
@@ -282,50 +338,59 @@
         ```py
         X.shape = (batch_size, n_features)
         ```
     """
 
     def __init__(
         self,
-        input_size: int,
-        output_size: int,
+        in_features: int,
+        out_features: int,
         activation: ActivationUtil.FuncType = "relu",
+        initializer: InitUtil.InitType = "auto",
         optimizer: Optimizer = None,
         lambda_: float = 0.0,
         random_state: int = None,
     ) -> None:
         super().__init__()
-        self.input_size = input_size
-        self.output_size = output_size
+        self.in_features = in_features
+        self.out_features = out_features
         self.activation = activation
+        self.initializer = initializer
         self.optimizer = optimizer
         self.lambda_ = lambda_
         self.random_state = random_state
 
         act = ActivationUtil(self.activation)
         self.act_ = act.activation_type()
         self.rs_ = np.random.RandomState(self.random_state)
 
-        self.weights_: Matrix = 0.01 * self.rs_.randn(self.input_size, self.output_size)
-        self.biases_: Matrix = np.zeros((1, self.output_size))
+        self.init_params(
+            w_shape=(self.in_features, self.out_features),
+            b_shape=(1, self.out_features),
+        )
+        self.set_param_ranges(
+            {
+                "in_features": ("0<,+inf", int),
+                "out_features": ("0<,+inf", int),
+                "lambda_": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
 
     def forward(self, X: Matrix) -> Matrix:
         self.input_ = X
 
         out = np.dot(X, self.weights_) + self.biases_
         out = self.act_.func(out)
         self.out_shape = out.shape
         return out
 
     def backward(self, d_out: Matrix) -> Matrix:
         X = self.input_
-        if isinstance(self.act_, Softmax):
-            pass
-        else:
-            d_out = self.act_.grad(d_out)
+        d_out = self.act_.grad(d_out)
 
         self.dX = np.dot(d_out, self.weights_.T)
         self.dW = np.dot(X.T, d_out)
         self.dW += 2 * self.lambda_ * self.weights_
         self.dB = np.sum(d_out, axis=0, keepdims=True)
 
         return self.dX
@@ -346,22 +411,25 @@
     Notes
     -----
     - During inference, dropout is typically turned off, and the layer behaves
       as the identity function.
 
     """
 
-    def __init__(self, dropout_rate: float = 0.1, random_state: int = None) -> None:
+    def __init__(self, dropout_rate: float = 0.5, random_state: int = None) -> None:
         super().__init__()
         self.dropout_rate = dropout_rate
         self.random_state = random_state
 
         self.mask_: Tensor = None
         self.rs_ = np.random.RandomState(self.random_state)
 
+        self.set_param_ranges({"dropout_rate": ("0,1", None)})
+        self.check_param_ranges()
+
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         self.input_ = X
         self.out_shape = self.input_.shape
 
         if is_train:
             self.mask_ = (
                 self.rs_.rand(*X.shape) < self.dropout_rate
@@ -433,33 +501,30 @@
     def get_loss(y: Matrix, out: Matrix) -> float
     ```
     Specials
     --------
     - You can use `+` operator to add a layer or another instance of `Sequential`.
 
     - By calling its instance, `forward`, `backward`, and `update`
-        is automatically called (single cycle).
+        is automatically called (single cycle) and the loss is returned.
 
     - Use `repr()` to print out its structural configuration.
 
     Notes
     -----
     - Before any execution, an optimizer and a loss function must be assigned.
 
-    - Use `param_size` after at least one forwarding to get the proper
-        size of its parameter.
-
     - For multi-class classification, the target variable `y`
         must be one-hot encoded.
 
     Examples
     --------
     ```py
     model = Sequential(
-        ("conv_1", Convolution(6, 3, activation="relu")),
+        ("conv_1", Convolution(3, 6, 3, activation="relu")),
         ("pool_1", Pooling(2, 2, mode="max")),
         ...,
         ("drop", Dropout(0.1)),
         ("flat", Flatten()),
         ("dense_1", Dense(384, 32, activation="relu")),
         ("dense_2", Dense(32, 10, activation="softmax")),
     )
@@ -597,17 +662,17 @@
         return self
 
     def __str__(self) -> str:
         return super().__str__()
 
     def __repr__(self) -> str:
         rep = f"{type(self).__name__} Configuration\n"
-        rep += "-" * 60 + "\n"
+        rep += "-" * 70 + "\n"
         for name, layer in self.layers:
             rep += f"({name}) {repr(layer)}\n"
 
         w_size, b_size = self.param_size
         rep += f"\nTotal Layers: {len(self.layers)}"
         rep += f"\nTotal Params: ({w_size:,} weights, {b_size:,} biases)"
         rep += f" -> {w_size + b_size:,}\n"
-        rep += "-" * 60
+        rep += "-" * 70
         return rep
```

### Comparing `luma-ml-0.7.0/luma/neural/network.py` & `luma-ml-0.7.1/luma/neural/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from typing import Any, Dict, List, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
-from luma.interface.util import Matrix, Vector, ActivationUtil
+from luma.interface.typing import Matrix, Vector
+from luma.interface.util import ActivationUtil
 from luma.interface.exception import NotFittedError
+
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
-from luma.neural.activation import Softmax
 from luma.neural.optimizer import SGDOptimizer
 
 
 __all__ = ("MLPClassifier", "MLPRegressor")
 
 
+# TODO: Possibly change MLPs into a single DNN with `Sequential`
+
+
 class MLPClassifier(Estimator, Estimator.NeuralNet, Supervised):
     """
     An MLP (Multilayer Perceptron) is a type of neural network composed
     of one input layer, one or more hidden layers, and one output layer,
     with fully connected neurons. Each neuron uses a nonlinear activation
     function to allow the network to capture complex patterns in the data.
     MLPs are trained using backpropagation, where the network learns by
@@ -116,15 +120,15 @@
         self.layer_sizes = [self.input_size, *self.hidden_sizes, self.output_size]
         self.n_layers = len(self.layer_sizes) - 1
         self.weights = []
         self.biases = []
 
         act = ActivationUtil(self.activation)
         self.act_ = act.activation_type()
-        self.softmax_ = Softmax()
+        # self.softmax_ = Softmax() # NOTE: Removed
         self.rs_ = np.random.RandomState(self.random_state)
 
         self.optimizer.set_params(
             **self.optimizer_params,
             learning_rate=self.learning_rate,
             ignore_missing=True,
         )
```

### Comparing `luma-ml-0.7.0/luma/neural/optimizer.py` & `luma-ml-0.7.1/luma/neural/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple
 import numpy as np
 
 from luma.core.super import Optimizer
-from luma.interface.util import Tensor
+from luma.interface.typing import Tensor
 
 
 __all__ = (
     "SGDOptimizer",
     "MomentumOptimizer",
     "RMSPropOptimizer",
     "AdamOptimizer",
```

### Comparing `luma-ml-0.7.0/luma/neural/single.py` & `luma-ml-0.7.1/luma/neural/single.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = ("PerceptronClassifier", "PerceptronRegressor")
```

### Comparing `luma-ml-0.7.0/luma/pipe/pipeline.py` & `luma-ml-0.7.1/luma/pipe/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Literal, Self, Tuple, List, Any
 
 from luma.core.super import Estimator, Transformer, Evaluator
 from luma.core.super import Supervised
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
 type Model = Estimator | Transformer
```

### Comparing `luma-ml-0.7.0/luma/preprocessing/encoder.py` & `luma-ml-0.7.1/luma/preprocessing/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal, Self
 import numpy as np
 
 from luma.core.super import Transformer
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 
 
 __all__ = ("OneHotEncoder", "LabelEncoder", "OrdinalEncoder", "LabelBinarizer")
 
 
 class OneHotEncoder(Transformer, Transformer.Feature):
```

### Comparing `luma-ml-0.7.0/luma/preprocessing/imputer.py` & `luma-ml-0.7.1/luma/preprocessing/imputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal, Self
 from scipy.spatial.distance import cdist
 from scipy.stats import mode
 import numpy as np
 import pandas as pd
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.core.super import Transformer
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 
 
 __all__ = ("SimpleImputer", "KNNImputer", "HotDeckImputer")
```

### Comparing `luma-ml-0.7.0/luma/preprocessing/outlier.py` & `luma-ml-0.7.1/luma/preprocessing/outlier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Self, Tuple
 from scipy.spatial.distance import cdist
 import numpy as np
 
 from luma.core.super import Transformer
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.interface.exception import NotFittedError
 
 
 __all__ = "LocalOutlierFactor"
 
 
 class LocalOutlierFactor(Transformer, Transformer.Both):
```

### Comparing `luma-ml-0.7.0/luma/preprocessing/scaler.py` & `luma-ml-0.7.1/luma/preprocessing/scaler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Self
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.core.super import Transformer
 from luma.interface.exception import NotFittedError
 
 
 __all__ = ("StandardScaler", "MinMaxScaler")
```

### Comparing `luma-ml-0.7.0/luma/reduction/linear.py` & `luma-ml-0.7.1/luma/reduction/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Self, Tuple
 from scipy.linalg import svd, eigh
 import numpy as np
 
-from luma.interface.util import Matrix, Vector, KernelUtil
+from luma.interface.typing import Matrix, Vector
+from luma.interface.util import KernelUtil
 from luma.core.super import Transformer, Unsupervised, Supervised
 from luma.interface.exception import (
     NotFittedError,
     NotConvergedError,
     UnsupportedParameterError,
 )
```

### Comparing `luma-ml-0.7.0/luma/reduction/manifold.py` & `luma-ml-0.7.1/luma/reduction/manifold.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from scipy.spatial.distance import pdist, cdist, squareform
 from scipy.sparse.csgraph import shortest_path
 from scipy.spatial import KDTree
 from scipy.linalg import eigh, svd
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.reduction.linear import PCA
 from luma.core.super import Transformer, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.clustering.kmeans import *
 from luma.metric.distance import *
```

### Comparing `luma-ml-0.7.0/luma/reduction/selection.py` & `luma-ml-0.7.1/luma/reduction/selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from itertools import combinations
 from typing import Tuple
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Transformer, Supervised
-from luma.interface.util import Matrix, Vector, Clone
+from luma.interface.typing import Matrix, Vector
+from luma.interface.util import Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
+
 from luma.model_selection.split import TrainTestSplit
 from luma.model_selection.cv import CrossValidator
 from luma.model_selection.fold import FoldType, KFold
 
 
 __all__ = ("SBS", "SFS", "RFE")
```

### Comparing `luma-ml-0.7.0/luma/regressor/general.py` & `luma-ml-0.7.1/luma/regressor/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal, Self
 from scipy.special import psi
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = (
     "PoissonRegressor",
```

### Comparing `luma-ml-0.7.0/luma/regressor/linear.py` & `luma-ml-0.7.1/luma/regressor/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Self
 import numpy as np
 
-from luma.interface.util import Matrix, Vector, KernelUtil
+from luma.interface.typing import Matrix, Vector
+from luma.interface.util import KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = (
     "LinearRegressor",
```

### Comparing `luma-ml-0.7.0/luma/regressor/neighbors.py` & `luma-ml-0.7.1/luma/regressor/neighbors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Self
 from scipy.spatial import distance_matrix
 import numpy as np
 
-from luma.interface.util import Matrix
 from luma.core.super import Estimator, Supervised, Evaluator
+from luma.interface.typing import Matrix
 from luma.interface.util import NearestNeighbors
 from luma.interface.exception import NotFittedError
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = ("KNNRegressor", "AdaptiveKNNRegressor", "WeightedKNNRegressor")
```

### Comparing `luma-ml-0.7.0/luma/regressor/poly.py` & `luma-ml-0.7.1/luma/regressor/poly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Literal, Self
 import numpy as np
 
-from luma.interface.util import Matrix
+from luma.interface.typing import Matrix
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = "PolynomialRegressor"
```

### Comparing `luma-ml-0.7.0/luma/regressor/robust.py` & `luma-ml-0.7.1/luma/regressor/robust.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Self, Tuple
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.metric.regression import MeanSquaredError
 from luma.regressor.linear import LinearRegressor
 
 
 __all__ = ("RANSAC", "MLESAC")
```

### Comparing `luma-ml-0.7.0/luma/regressor/svm.py` & `luma-ml-0.7.1/luma/regressor/svm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Self
 import numpy as np
 
-from luma.interface.util import Matrix, KernelUtil
+from luma.interface.typing import Matrix
+from luma.interface.util import KernelUtil
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = ("SVR", "KernelSVR")
```

### Comparing `luma-ml-0.7.0/luma/regressor/tree.py` & `luma-ml-0.7.1/luma/regressor/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Self, Tuple
 import numpy as np
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import DecisionTreeNode
 from luma.metric.regression import MeanSquaredError
 
 
 __all__ = ("DecisionTreeRegressor",)
```

### Comparing `luma-ml-0.7.0/luma/visual/eda.py` & `luma-ml-0.7.1/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.0/luma/visual/evaluation.py` & `luma-ml-0.7.1/luma/visual/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Literal, Optional, Tuple
 from matplotlib.colors import ListedColormap
 import matplotlib.pyplot as plt
 import numpy as np
 
-from luma.interface.util import Matrix, Vector
+from luma.interface.typing import Matrix, Vector
 from luma.core.super import Evaluator, Visualizer, Estimator
 from luma.model_selection.split import TrainTestSplit
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.metric.classification import Accuracy, Precision, Recall, Specificity
 from luma.model_selection.cv import CrossValidator
 from luma.model_selection.fold import FoldType, KFold
```

### Comparing `luma-ml-0.7.0/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.7.1/luma_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.01k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.07k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.0</td>
+                    <td>0.7.1</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~17.4K</td>
+                    <td>~17.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.0 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.1 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.01k-red][GitHub code size in bytes][Code Style]
+5.07k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.0
-Lines of Code  ~17.4K
+Latest Version 0.7.1
+Lines of Code  ~17.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.0/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.7.1/luma_ml.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,28 @@
 luma/core/super.py
 luma/ensemble/bagging.py
 luma/ensemble/boost.py
 luma/ensemble/forest.py
 luma/ensemble/stack.py
 luma/ensemble/vote.py
 luma/interface/exception.py
+luma/interface/typing.py
 luma/interface/util.py
 luma/metric/classification.py
 luma/metric/clustering.py
 luma/metric/distance.py
 luma/metric/regression.py
 luma/migrate/port.py
 luma/model_selection/cv.py
 luma/model_selection/fold.py
 luma/model_selection/search.py
 luma/model_selection/split.py
 luma/neural/activation.py
+luma/neural/base.py
+luma/neural/init.py
 luma/neural/layer.py
 luma/neural/loss.py
 luma/neural/network.py
 luma/neural/optimizer.py
 luma/neural/single.py
 luma/pipe/pipeline.py
 luma/preprocessing/encoder.py
```

### Comparing `luma-ml-0.7.0/setup.py` & `luma-ml-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.7.0",
+    version="0.7.1",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/LUMA",
     packages=setuptools.find_namespace_packages(),
```

### Comparing `luma-ml-0.7.0/test/__test.py` & `luma-ml-0.7.1/test/__test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import __local__
 from luma.preprocessing.scaler import StandardScaler
 from luma.preprocessing.encoder import OneHotEncoder
 from luma.model_selection.split import TrainTestSplit, BatchGenerator
 from luma.metric.classification import Accuracy
 
-from luma.neural.layer import Sequential
-from luma.neural.layer import Convolution, Pooling, Flatten, Dense
-from luma.neural.loss import CategoricalCrossEntropy
+from luma.neural.layer import Convolution, Flatten, Dense, Sequential
+from luma.neural.loss import SoftmaxLoss
 from luma.neural.optimizer import AdamOptimizer
 
 from sklearn.datasets import load_digits
 import matplotlib.pyplot as plt
 import numpy as np
 
 
@@ -31,37 +30,39 @@
 
 X_train = X_train.reshape(-1, 1, 8, 8)
 X_test = X_test.reshape(-1, 1, 8, 8)
 
 epochs = 100
 batch_size = 100
 
+# -----------------------------------------------------------#
 model = Sequential(
-    Convolution(6, 3, activation="relu"),
-    Pooling(2, 2, mode="avg"),
+    Convolution(1, 6, 3, padding="same", activation="relu"),
+    Convolution(6, 12, 3, padding="same", activation="relu"),
     Flatten(),
-    Dense(96, 10, activation="softmax"),
+    Dense(768, 10, activation=None),
 )
+
 model.set_optimizer(AdamOptimizer(), learning_rate=0.001)
-model.set_loss(CategoricalCrossEntropy())
+model.set_loss(SoftmaxLoss())
+print(repr(model))
+# -----------------------------------------------------------#
 
 losses = []
 for i in range(1, epochs + 1):
     epoch_loss = []
     for j, (X_batch, y_batch) in enumerate(
         BatchGenerator(X_train, y_train, batch_size=batch_size), start=1
     ):
         loss = model(X_batch, y_batch, is_train=True)
         losses.append(loss)
         epoch_loss.append(loss)
 
     print(f"Epoch {i}/{epochs} - Avg. Loss: {np.average(epoch_loss)}")
 
-print("\n" + repr(model))
-
 score = Accuracy.score(
     y_true=y_test.argmax(axis=1), y_pred=model.forward(X_test).argmax(axis=1)
 )
 
 plt.plot(losses, lw=1, label=type(model.optimizer).__name__)
 plt.xlabel("Total Batches")
 plt.ylabel("Loss")
```

### Comparing `luma-ml-0.7.0/test/_mlp.py` & `luma-ml-0.7.1/test/_mlp.py`

 * *Files identical despite different names*

