# Comparing `tmp/freerec-0.7.5.tar.gz` & `tmp/freerec-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freerec-0.7.5.tar", last modified: Sun Mar 31 12:54:09 2024, max compression
+gzip compressed data, was "freerec-0.8.1.tar", last modified: Tue Apr 23 11:27:49 2024, max compression
```

## Comparing `freerec-0.7.5.tar` & `freerec-0.8.1.tar`

### file list

```diff
@@ -1,76 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.716142 freerec-0.7.5/
--rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.7.5/LICENSE
--rw-rw-rw-   0        0        0     2292 2024-03-31 12:54:09.715142 freerec-0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     1664 2024-03-31 12:53:13.000000 freerec-0.7.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.654756 freerec-0.7.5/freerec/
--rw-rw-rw-   0        0        0      554 2024-03-31 12:52:35.000000 freerec-0.7.5/freerec/__init__.py
--rw-rw-rw-   0        0        0     6698 2024-03-18 08:00:27.000000 freerec-0.7.5/freerec/__main__.py
--rw-rw-rw-   0        0        0     6274 2023-12-13 06:06:13.000000 freerec-0.7.5/freerec/criterions.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.673917 freerec-0.7.5/freerec/data/
--rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.7.5/freerec/data/__init__.py
--rw-rw-rw-   0        0        0    12386 2023-12-22 12:34:35.000000 freerec-0.7.5/freerec/data/dataloader.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.674916 freerec-0.7.5/freerec/data/datasets/
--rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.7.5/freerec/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    23639 2024-03-31 09:22:21.000000 freerec-0.7.5/freerec/data/datasets/base.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.686176 freerec-0.7.5/freerec/data/datasets/context/
--rw-rw-rw-   0        0        0       69 2024-03-23 09:23:20.000000 freerec-0.7.5/freerec/data/datasets/context/__init__.py
--rw-rw-rw-   0        0        0    13778 2024-03-20 08:21:25.000000 freerec-0.7.5/freerec/data/datasets/context/amazon.py
--rw-rw-rw-   0        0        0     3229 2024-03-23 09:22:46.000000 freerec-0.7.5/freerec/data/datasets/context/base.py
--rw-rw-rw-   0        0        0     5394 2024-03-25 12:22:04.000000 freerec-0.7.5/freerec/data/datasets/context/mmrec.py
--rw-rw-rw-   0        0        0     3467 2024-03-25 12:20:58.000000 freerec-0.7.5/freerec/data/datasets/context/mmssl.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.693205 freerec-0.7.5/freerec/data/datasets/general/
--rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.7.5/freerec/data/datasets/general/__init__.py
--rw-rw-rw-   0        0        0    13580 2023-04-26 06:46:20.000000 freerec-0.7.5/freerec/data/datasets/general/amazon.py
--rw-rw-rw-   0        0        0     3876 2024-01-16 12:41:53.000000 freerec-0.7.5/freerec/data/datasets/general/base.py
--rw-rw-rw-   0        0        0     2825 2023-04-26 06:46:27.000000 freerec-0.7.5/freerec/data/datasets/general/gowalla.py
--rw-rw-rw-   0        0        0     4657 2023-04-26 06:54:50.000000 freerec-0.7.5/freerec/data/datasets/general/movielens.py
--rw-rw-rw-   0        0        0     2809 2023-04-26 06:52:08.000000 freerec-0.7.5/freerec/data/datasets/general/yelp.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.694203 freerec-0.7.5/freerec/data/datasets/knowledge/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.7.5/freerec/data/datasets/knowledge/__init__.py
--rw-rw-rw-   0        0        0      215 2024-01-16 12:41:48.000000 freerec-0.7.5/freerec/data/datasets/knowledge/base.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.698221 freerec-0.7.5/freerec/data/datasets/sequential/
--rw-rw-rw-   0        0        0       89 2023-09-07 08:34:27.000000 freerec-0.7.5/freerec/data/datasets/sequential/__init__.py
--rw-rw-rw-   0        0        0    10771 2023-04-26 07:43:46.000000 freerec-0.7.5/freerec/data/datasets/sequential/amazon.py
--rw-rw-rw-   0        0        0     2888 2024-01-16 12:41:12.000000 freerec-0.7.5/freerec/data/datasets/sequential/base.py
--rw-rw-rw-   0        0        0     5035 2024-01-13 06:02:57.000000 freerec-0.7.5/freerec/data/datasets/sequential/movielens.py
--rw-rw-rw-   0        0        0     1751 2023-04-26 07:33:37.000000 freerec-0.7.5/freerec/data/datasets/sequential/steam.py
--rw-rw-rw-   0        0        0     1220 2024-01-16 12:41:38.000000 freerec-0.7.5/freerec/data/datasets/sequential/yelp.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.700400 freerec-0.7.5/freerec/data/datasets/session/
--rw-rw-rw-   0        0        0       55 2023-05-31 03:03:02.000000 freerec-0.7.5/freerec/data/datasets/session/__init__.py
--rw-rw-rw-   0        0        0     3444 2024-01-16 13:28:35.000000 freerec-0.7.5/freerec/data/datasets/session/base.py
--rw-rw-rw-   0        0        0     3175 2023-06-21 06:31:56.000000 freerec-0.7.5/freerec/data/datasets/session/diginetica.py
--rw-rw-rw-   0        0        0     6539 2023-06-21 06:44:03.000000 freerec-0.7.5/freerec/data/datasets/session/yoochoose.py
--rw-rw-rw-   0        0        0    35651 2024-03-20 08:36:23.000000 freerec-0.7.5/freerec/data/fields.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.704401 freerec-0.7.5/freerec/data/postprocessing/
--rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.7.5/freerec/data/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.7.5/freerec/data/postprocessing/base.py
--rw-rw-rw-   0        0        0     9262 2023-12-03 07:31:10.000000 freerec-0.7.5/freerec/data/postprocessing/column.py
--rw-rw-rw-   0        0        0    12158 2023-11-27 02:54:19.000000 freerec-0.7.5/freerec/data/postprocessing/row.py
--rw-rw-rw-   0        0        0    24276 2023-11-30 05:35:42.000000 freerec-0.7.5/freerec/data/postprocessing/sampler.py
--rw-rw-rw-   0        0        0     3492 2024-01-21 06:35:34.000000 freerec-0.7.5/freerec/data/postprocessing/source.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.713141 freerec-0.7.5/freerec/data/preprocessing/
--rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.7.5/freerec/data/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    31563 2024-03-18 07:44:12.000000 freerec-0.7.5/freerec/data/preprocessing/base.py
--rw-rw-rw-   0        0        0    17822 2024-03-17 09:12:37.000000 freerec-0.7.5/freerec/data/preprocessing/datasets.py
--rw-rw-rw-   0        0        0      929 2024-03-18 01:05:27.000000 freerec-0.7.5/freerec/data/tags.py
--rw-rw-rw-   0        0        0     5969 2023-06-18 13:30:46.000000 freerec-0.7.5/freerec/data/transformation.py
--rw-rw-rw-   0        0        0     9632 2024-03-25 12:31:05.000000 freerec-0.7.5/freerec/data/utils.py
--rw-rw-rw-   0        0        0     9147 2023-12-25 08:54:45.000000 freerec-0.7.5/freerec/ddp.py
--rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.7.5/freerec/dict2obj.py
--rw-rw-rw-   0        0        0     4762 2024-03-31 09:09:13.000000 freerec-0.7.5/freerec/graph.py
--rw-rw-rw-   0        0        0    38909 2024-03-31 12:51:13.000000 freerec-0.7.5/freerec/launcher.py
--rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.7.5/freerec/metrics.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.715142 freerec-0.7.5/freerec/models/
--rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.7.5/freerec/models/__init__.py
--rw-rw-rw-   0        0        0     6978 2024-03-31 07:38:41.000000 freerec-0.7.5/freerec/models/base.py
--rw-rw-rw-   0        0        0    16393 2024-01-21 06:14:20.000000 freerec-0.7.5/freerec/parser.py
--rw-rw-rw-   0        0        0    15070 2023-12-29 12:17:22.000000 freerec-0.7.5/freerec/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 12:54:09.669915 freerec-0.7.5/freerec.egg-info/
--rw-rw-rw-   0        0        0     2292 2024-03-31 12:54:09.000000 freerec-0.7.5/freerec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2024-03-31 12:54:09.000000 freerec-0.7.5/freerec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 12:54:09.000000 freerec-0.7.5/freerec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-03-31 12:54:09.000000 freerec-0.7.5/freerec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2024-03-31 12:54:09.000000 freerec-0.7.5/freerec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-31 12:54:09.000000 freerec-0.7.5/freerec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 12:54:09.716142 freerec-0.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1160 2024-01-23 02:00:40.000000 freerec-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.096286 freerec-0.8.1/
+-rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     2348 2024-04-23 11:27:49.095037 freerec-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1782 2024-04-22 01:25:03.000000 freerec-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.050667 freerec-0.8.1/freerec/
+-rw-rw-rw-   0        0        0      554 2024-04-23 07:10:43.000000 freerec-0.8.1/freerec/__init__.py
+-rw-rw-rw-   0        0        0     4116 2024-04-14 08:06:45.000000 freerec-0.8.1/freerec/__main__.py
+-rw-rw-rw-   0        0        0     6270 2024-04-17 09:20:21.000000 freerec-0.8.1/freerec/criterions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.079465 freerec-0.8.1/freerec/data/
+-rw-rw-rw-   0        0        0       78 2024-04-22 08:24:53.000000 freerec-0.8.1/freerec/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.084968 freerec-0.8.1/freerec/data/datasets/
+-rw-rw-rw-   0        0        0     2297 2024-04-21 05:44:43.000000 freerec-0.8.1/freerec/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0      848 2024-04-21 03:05:02.000000 freerec-0.8.1/freerec/data/datasets/allrecipes.py
+-rw-rw-rw-   0        0        0    18450 2024-04-21 05:33:17.000000 freerec-0.8.1/freerec/data/datasets/amazon2014.py
+-rw-rw-rw-   0        0        0     6405 2024-04-21 06:09:58.000000 freerec-0.8.1/freerec/data/datasets/amazon2018.py
+-rw-rw-rw-   0        0        0    25273 2024-04-23 02:45:52.000000 freerec-0.8.1/freerec/data/datasets/base.py
+-rw-rw-rw-   0        0        0     1436 2024-04-21 02:32:56.000000 freerec-0.8.1/freerec/data/datasets/gowalla.py
+-rw-rw-rw-   0        0        0    11008 2024-04-21 02:34:07.000000 freerec-0.8.1/freerec/data/datasets/movielens.py
+-rw-rw-rw-   0        0        0      831 2024-04-21 03:02:57.000000 freerec-0.8.1/freerec/data/datasets/tiktok.py
+-rw-rw-rw-   0        0        0     6649 2024-04-21 02:37:51.000000 freerec-0.8.1/freerec/data/datasets/yelp.py
+-rw-rw-rw-   0        0        0    13268 2024-04-17 06:58:28.000000 freerec-0.8.1/freerec/data/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.090975 freerec-0.8.1/freerec/data/postprocessing/
+-rw-rw-rw-   0        0        0      956 2024-04-16 11:37:36.000000 freerec-0.8.1/freerec/data/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2919 2024-04-23 03:23:48.000000 freerec-0.8.1/freerec/data/postprocessing/base.py
+-rw-rw-rw-   0        0        0    24772 2024-04-23 03:09:55.000000 freerec-0.8.1/freerec/data/postprocessing/base.pyi
+-rw-rw-rw-   0        0        0     1825 2024-04-23 07:56:44.000000 freerec-0.8.1/freerec/data/postprocessing/column.py
+-rw-rw-rw-   0        0        0     9732 2024-04-22 05:44:09.000000 freerec-0.8.1/freerec/data/postprocessing/row.py
+-rw-rw-rw-   0        0        0    19109 2024-04-23 07:48:46.000000 freerec-0.8.1/freerec/data/postprocessing/sampler.py
+-rw-rw-rw-   0        0        0     2807 2024-04-23 03:21:07.000000 freerec-0.8.1/freerec/data/postprocessing/source.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.091975 freerec-0.8.1/freerec/data/preprocessing/
+-rw-rw-rw-   0        0        0       37 2024-04-14 08:01:15.000000 freerec-0.8.1/freerec/data/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    28235 2024-04-20 06:56:44.000000 freerec-0.8.1/freerec/data/preprocessing/base.py
+-rw-rw-rw-   0        0        0      789 2024-04-20 07:59:27.000000 freerec-0.8.1/freerec/data/tags.py
+-rw-rw-rw-   0        0        0     9778 2024-04-22 07:01:44.000000 freerec-0.8.1/freerec/data/utils.py
+-rw-rw-rw-   0        0        0     9147 2023-12-25 08:54:45.000000 freerec-0.8.1/freerec/ddp.py
+-rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.8.1/freerec/dict2obj.py
+-rw-rw-rw-   0        0        0     4806 2024-04-14 12:22:40.000000 freerec-0.8.1/freerec/graph.py
+-rw-rw-rw-   0        0        0    34594 2024-04-23 07:34:48.000000 freerec-0.8.1/freerec/launcher.py
+-rw-rw-rw-   0        0        0    23293 2023-04-30 11:44:17.000000 freerec-0.8.1/freerec/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.094532 freerec-0.8.1/freerec/models/
+-rw-rw-rw-   0        0        0       66 2024-04-23 06:25:12.000000 freerec-0.8.1/freerec/models/__init__.py
+-rw-rw-rw-   0        0        0     6997 2024-04-23 06:37:08.000000 freerec-0.8.1/freerec/models/base.py
+-rw-rw-rw-   0        0        0    16893 2024-04-22 08:21:05.000000 freerec-0.8.1/freerec/parser.py
+-rw-rw-rw-   0        0        0    16048 2024-04-17 03:34:43.000000 freerec-0.8.1/freerec/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:27:49.076458 freerec-0.8.1/freerec.egg-info/
+-rw-rw-rw-   0        0        0     2348 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 11:27:48.000000 freerec-0.8.1/freerec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 11:27:49.097048 freerec-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2024-04-23 06:22:49.000000 freerec-0.8.1/setup.py
```

### Comparing `freerec-0.7.5/LICENSE` & `freerec-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freerec-0.7.5/PKG-INFO` & `freerec-0.8.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2066 7265  : 2.1..Name: fre
 00000020: 6572 6563 0d0a 5665 7273 696f 6e3a 2030  erec..Version: 0
-00000030: 2e37 2e35 0d0a 5375 6d6d 6172 793a 2050  .7.5..Summary: P
+00000030: 2e38 2e31 0d0a 5375 6d6d 6172 793a 2050  .8.1..Summary: P
 00000040: 7954 6f72 6368 206c 6962 7261 7279 2066  yTorch library f
 00000050: 6f72 2072 6563 6f6d 6d65 6e64 6572 2073  or recommender s
 00000060: 7973 7465 6d73 0d0a 486f 6d65 2d70 6167  ystems..Home-pag
 00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000080: 622e 636f 6d2f 4d54 616e 6448 4a2f 6672  b.com/MTandHJ/fr
 00000090: 6565 7265 630d 0a41 7574 686f 723a 204d  eerec..Author: M
 000000a0: 5461 6e64 484a 0d0a 4175 7468 6f72 2d65  TandHJ..Author-e
@@ -23,122 +23,125 @@
 00000160: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
 00000170: 6e64 656e 740d 0a52 6571 7569 7265 732d  ndent..Requires-
 00000180: 5079 7468 6f6e 3a20 3e3d 332e 390d 0a44  Python: >=3.9..D
 00000190: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
 000001a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
 000001b0: 726b 646f 776e 0d0a 4c69 6365 6e73 652d  rkdown..License-
 000001c0: 4669 6c65 3a20 4c49 4345 4e53 450d 0a52  File: LICENSE..R
-000001d0: 6571 7569 7265 732d 4469 7374 3a20 6672  equires-Dist: fr
-000001e0: 6565 706c 6f74 3e3d 302e 342e 350d 0a52  eeplot>=0.4.5..R
-000001f0: 6571 7569 7265 732d 4469 7374 3a20 5079  equires-Dist: Py
-00000200: 5941 4d4c 3e3d 362e 300d 0a52 6571 7569  YAML>=6.0..Requi
-00000210: 7265 732d 4469 7374 3a20 7465 6e73 6f72  res-Dist: tensor
-00000220: 626f 6172 643e 3d32 2e31 302e 300d 0a52  board>=2.10.0..R
-00000230: 6571 7569 7265 732d 4469 7374 3a20 7073  equires-Dist: ps
-00000240: 7574 696c 3e3d 352e 392e 300d 0a52 6571  util>=5.9.0..Req
-00000250: 7569 7265 732d 4469 7374 3a20 7072 6574  uires-Dist: pret
-00000260: 7479 7461 626c 653e 3d33 2e34 2e31 0d0a  tytable>=3.4.1..
-00000270: 0d0a 0d0a 0d0a 215b 5d28 646f 6373 2f73  ......![](docs/s
-00000280: 7263 2f6c 6f67 6f2e 706e 6729 0d0a 0d0a  rc/logo.png)....
-00000290: 4672 6565 5265 6320 6973 2061 2072 6570  FreeRec is a rep
-000002a0: 6f73 6974 6f72 7920 6465 7369 676e 6564  ository designed
-000002b0: 2066 6f72 2065 6173 7920 2872 6563 6f6d   for easy (recom
-000002c0: 6d65 6e64 6174 696f 6e29 2064 6174 6120  mendation) data 
-000002d0: 7072 652d 7072 6f63 6573 7369 6e67 2061  pre-processing a
-000002e0: 6e64 206d 6f64 656c 2074 7261 696e 696e  nd model trainin
-000002f0: 672e 0d0a 4920 616d 2061 2062 6567 696e  g...I am a begin
-00000300: 6e65 7220 696e 2074 6865 2066 6965 6c64  ner in the field
-00000310: 206f 6620 7265 636f 6d6d 656e 6465 7220   of recommender 
-00000320: 7379 7374 656d 732c 2073 6f20 6d75 6368  systems, so much
-00000330: 206f 6620 4672 6565 5265 6327 7320 6465   of FreeRec's de
-00000340: 7369 676e 7320 6d61 7920 6e6f 7420 6265  signs may not be
-00000350: 2061 7320 6566 6665 6374 6976 652e 2049   as effective. I
-00000360: 6e20 6164 6469 7469 6f6e 2c20 796f 7520  n addition, you 
-00000370: 6172 6520 6672 6565 2074 6f20 7370 6563  are free to spec
-00000380: 6966 7920 796f 7572 206f 776e 2066 7261  ify your own fra
-00000390: 6d65 776f 726b 2062 6173 6564 206f 6e20  mework based on 
-000003a0: 4672 6565 5265 632e 0d0a 0d0a 0d0a 2323  FreeRec.......##
-000003b0: 2052 6571 7569 7265 6d65 6e74 733a 200d   Requirements: .
-000003c0: 0a0d 0a50 7974 686f 6e20 3e3d 2033 2e39  ...Python >= 3.9
-000003d0: 207c 205b 5079 546f 7263 6820 3e3d 322e   | [PyTorch >=2.
-000003e0: 305d 2868 7474 7073 3a2f 2f70 7974 6f72  0](https://pytor
-000003f0: 6368 2e6f 7267 2f29 207c 205b 546f 7263  ch.org/) | [Torc
-00000400: 6844 6174 6120 3e3d 302e 362e 305d 2868  hData >=0.6.0](h
-00000410: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000420: 6d2f 7079 746f 7263 682f 6461 7461 2920  m/pytorch/data) 
-00000430: 7c20 5b50 7947 203e 3d32 2e33 5d28 6874  | [PyG >=2.3](ht
-00000440: 7470 733a 2f2f 7079 746f 7263 682d 6765  tps://pytorch-ge
-00000450: 6f6d 6574 7269 632e 7265 6164 7468 6564  ometric.readthed
-00000460: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000470: 2f6e 6f74 6573 2f69 6e73 7461 6c6c 6174  /notes/installat
-00000480: 696f 6e2e 6874 6d6c 2329 0d0a 0d0a 0d0a  ion.html#)......
-00000490: 6060 600d 0a63 6f6e 6461 2063 7265 6174  ```..conda creat
-000004a0: 6520 2d2d 6e61 6d65 3d46 7265 6552 6563  e --name=FreeRec
-000004b0: 2070 7974 686f 6e3d 332e 390d 0a63 6f6e   python=3.9..con
-000004c0: 6461 2061 6374 6976 6174 6520 4672 6565  da activate Free
-000004d0: 5265 630d 0a60 6060 0d0a 0d0a 0d0a 2a2a  Rec..```......**
-000004e0: 4e6f 7465 3a2a 2a20 4166 7465 7220 5079  Note:** After Py
-000004f0: 546f 7263 6820 322e 302c 2060 546f 7263  Torch 2.0, `Torc
-00000500: 6844 6174 6160 2073 6565 6d73 2074 6f20  hData` seems to 
-00000510: 6861 7665 2073 746f 7070 6564 2062 6569  have stopped bei
-00000520: 6e67 2075 7064 6174 6564 2c20 616e 6420  ng updated, and 
-00000530: 796f 7520 6361 6e20 696e 7374 616c 6c20  you can install 
-00000540: 6974 2077 6974 6820 602d 2d6e 6f2d 6465  it with `--no-de
-00000550: 7073 6020 746f 2061 766f 6964 2069 6e73  ps` to avoid ins
-00000560: 7461 6c6c 696e 6720 6465 7065 6e64 656e  talling dependen
-00000570: 6369 6573 2e0d 0a0d 0a60 6060 0d0a 7069  cies.....```..pi
-00000580: 7020 696e 7374 616c 6c20 2d2d 6e6f 2d64  p install --no-d
-00000590: 6570 7320 746f 7263 6864 6174 610d 0a60  eps torchdata..`
-000005a0: 6060 0d0a 0d0a 0d0a 2323 2049 6e73 7461  ``......## Insta
-000005b0: 6c6c 6174 696f 6e0d 0a0d 0a20 2020 2070  llation....    p
-000005c0: 6970 2069 6e73 7461 6c6c 2066 7265 6572  ip install freer
-000005d0: 6563 0d0a 0d0a 6f72 2028 666f 7220 6c61  ec....or (for la
-000005e0: 7465 7374 290d 0a0d 0a20 2020 2070 6970  test)....    pip
-000005f0: 2069 6e73 7461 6c6c 2067 6974 2b68 7474   install git+htt
-00000600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000610: 4d54 616e 6448 4a2f 6672 6565 7265 632e  MTandHJ/freerec.
-00000620: 6769 740d 0a0d 0a0d 0a0d 0a23 2320 4461  git........## Da
-00000630: 7461 2050 6970 656c 696e 650d 0a0d 0a21  ta Pipeline....!
-00000640: 5b5d 2864 6f63 732f 7372 632f 7069 7065  [](docs/src/pipe
-00000650: 6c69 6e65 2e70 6e67 290d 0a0d 0a2a 2a4e  line.png)....**N
-00000660: 6f74 653a 2a2a 2054 6f20 6d61 6b65 2064  ote:** To make d
-00000670: 6174 6173 6574 2c20 706c 6561 7365 2064  ataset, please d
-00000680: 6f77 6e6c 6f61 6420 636f 7272 6573 706f  ownload correspo
-00000690: 6e64 696e 6720 4174 6f6d 6963 2066 696c  nding Atomic fil
-000006a0: 6573 2066 726f 6d20 5b5b 5265 6342 6f6c  es from [[RecBol
-000006b0: 655d 2868 7474 7073 3a2f 2f64 7269 7665  e](https://drive
-000006c0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
-000006d0: 652f 666f 6c64 6572 732f 3173 6f30 6c63  e/folders/1so0lc
-000006e0: 6b49 364e 365f 6e69 5645 5961 4275 2d4c  kI6N6_niVEYaBu-L
-000006f0: 4963 704f 645a 6639 396b 6a29 5d2e 200d  IcpOdZf99kj)]. .
-00000700: 0a54 6865 6e2c 2072 756e 2060 6672 6565  .Then, run `free
-00000710: 7265 6320 6d61 6b65 202d 2d68 656c 7060  rec make --help`
-00000720: 2e0d 0a0d 0a23 2320 5472 6169 6e69 6e67  .....## Training
-00000730: 2046 6c6f 770d 0a0d 0a0d 0a21 5b5d 2864   Flow......![](d
-00000740: 6f63 732f 7372 632f 666c 6f77 2e70 6e67  ocs/src/flow.png
-00000750: 290d 0a0d 0a0d 0a23 2320 5265 6665 7265  )......## Refere
-00000760: 6e63 6520 436f 6465 0d0a 0d0a 2d20 546f  nce Code....- To
-00000770: 7263 6852 6563 3a20 6874 7470 733a 2f2f  rchRec: https://
-00000780: 6769 7468 7562 2e63 6f6d 2f70 7974 6f72  github.com/pytor
-00000790: 6368 2f74 6f72 6368 7265 6320 0d0a 2d20  ch/torchrec ..- 
-000007a0: 4465 6570 4354 522d 546f 7263 683a 2068  DeepCTR-Torch: h
-000007b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000007c0: 6d2f 7368 656e 7765 6963 6865 6e2f 4465  m/shenweichen/De
-000007d0: 6570 4354 522d 546f 7263 680d 0a2d 2046  epCTR-Torch..- F
-000007e0: 7578 6943 5452 3a20 6874 7470 733a 2f2f  uxiCTR: https://
-000007f0: 6769 7468 7562 2e63 6f6d 2f78 7565 2d70  github.com/xue-p
-00000800: 6169 2f46 7578 6943 5452 0d0a 2d20 4241  ai/FuxiCTR..- BA
-00000810: 5253 3a20 6874 7470 733a 2f2f 6769 7468  RS: https://gith
-00000820: 7562 2e63 6f6d 2f6f 7065 6e62 656e 6368  ub.com/openbench
-00000830: 6d61 726b 2f42 4152 530d 0a2d 2052 6563  mark/BARS..- Rec
-00000840: 426f 6c65 3a20 6874 7470 733a 2f2f 6769  Bole: https://gi
-00000850: 7468 7562 2e63 6f6d 2f52 5543 4149 426f  thub.com/RUCAIBo
-00000860: 782f 5265 6342 6f6c 650d 0a0d 0a0d 0a0d  x/RecBole.......
-00000870: 0a23 2320 4163 6b6e 6f77 6c65 6467 656d  .## Acknowledgem
-00000880: 656e 7473 0d0a 0d0a 5468 616e 6b73 2074  ents....Thanks t
-00000890: 6f20 4368 6174 4750 5420 666f 7220 7468  o ChatGPT for th
-000008a0: 6520 616e 6e6f 7461 7469 6f6e 206f 6620  e annotation of 
-000008b0: 736f 6d65 2063 6f64 652e 2046 6f72 2074  some code. For t
-000008c0: 6869 7320 7265 6173 6f6e 2c20 736f 6d65  his reason, some
-000008d0: 206f 6620 7468 6520 636f 6d6d 656e 7473   of the comments
-000008e0: 206d 6179 2062 6520 696c 6c6f 6769 6361   may be illogica
-000008f0: 6c2e 0d0a                                l...
+000001d0: 6571 7569 7265 732d 4469 7374 3a20 5079  equires-Dist: Py
+000001e0: 5941 4d4c 3e3d 362e 300d 0a52 6571 7569  YAML>=6.0..Requi
+000001f0: 7265 732d 4469 7374 3a20 7465 6e73 6f72  res-Dist: tensor
+00000200: 626f 6172 643e 3d32 2e31 302e 300d 0a52  board>=2.10.0..R
+00000210: 6571 7569 7265 732d 4469 7374 3a20 7072  equires-Dist: pr
+00000220: 6574 7479 7461 626c 653e 3d33 2e34 2e31  ettytable>=3.4.1
+00000230: 0d0a 0d0a 0d0a 0d0a 215b 5d28 646f 6373  ........![](docs
+00000240: 2f73 7263 2f6c 6f67 6f2e 706e 6729 0d0a  /src/logo.png)..
+00000250: 0d0a 3c68 3420 616c 6967 6e3d 2263 656e  ..<h4 align="cen
+00000260: 7465 7222 3e0d 0a20 2020 203c 703e 0d0a  ter">..    <p>..
+00000270: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
+00000280: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000290: 636f 6d2f 4d54 616e 6448 4a2f 6672 6565  com/MTandHJ/free
+000002a0: 7265 632f 626c 6f62 2f6d 6173 7465 722f  rec/blob/master/
+000002b0: 6461 7461 7365 7425 3230 7072 6f63 6573  dataset%20proces
+000002c0: 7369 6e67 2e6d 6422 3e44 6174 6173 6574  sing.md">Dataset
+000002d0: 2070 726f 6365 7373 696e 673c 2f61 3e20   processing</a> 
+000002e0: 7c0d 0a20 2020 2020 2020 203c 6120 6872  |..        <a hr
+000002f0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000300: 7562 2e63 6f6d 2f4d 5461 6e64 484a 2f66  ub.com/MTandHJ/f
+00000310: 7265 6572 6563 2f62 6c6f 622f 6d61 7374  reerec/blob/mast
+00000320: 6572 2f74 7261 696e 696e 6725 3230 616e  er/training%20an
+00000330: 6425 3230 7475 6e69 6e67 2e6d 6422 3e54  d%20tuning.md">T
+00000340: 7261 696e 696e 6720 616e 6420 5475 6e69  raining and Tuni
+00000350: 6e67 3c2f 613e 207c 0d0a 2020 2020 2020  ng</a> |..      
+00000360: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000370: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d54  ://github.com/MT
+00000380: 616e 6448 4a2f 5265 6342 6f61 7264 223e  andHJ/RecBoard">
+00000390: 5265 6342 6f61 7264 3c2f 613e 0d0a 2020  RecBoard</a>..  
+000003a0: 2020 3c2f 703e 0d0a 3c2f 6834 3e0d 0a0d    </p>..</h4>...
+000003b0: 0a46 7265 6552 6563 2069 7320 6120 7265  .FreeRec is a re
+000003c0: 706f 7369 746f 7279 2064 6573 6967 6e65  pository designe
+000003d0: 6420 666f 7220 6561 7379 2028 7265 636f  d for easy (reco
+000003e0: 6d6d 656e 6461 7469 6f6e 2920 6461 7461  mmendation) data
+000003f0: 2070 7265 2d70 726f 6365 7373 696e 6720   pre-processing 
+00000400: 616e 6420 6d6f 6465 6c20 7472 6169 6e69  and model traini
+00000410: 6e67 2e20 596f 7520 6172 6520 6672 6565  ng. You are free
+00000420: 2074 6f20 7370 6563 6966 7920 796f 7572   to specify your
+00000430: 206f 776e 2066 7261 6d65 776f 726b 2062   own framework b
+00000440: 6173 6564 206f 6e20 4672 6565 5265 632e  ased on FreeRec.
+00000450: 0d0a 0d0a 0d0a 2323 2052 6571 7569 7265  ......## Require
+00000460: 6d65 6e74 733a 200d 0a0d 0a50 7974 686f  ments: ....Pytho
+00000470: 6e20 3e3d 2033 2e39 207c 205b 5079 546f  n >= 3.9 | [PyTo
+00000480: 7263 6820 3e3d 322e 305d 2868 7474 7073  rch >=2.0](https
+00000490: 3a2f 2f70 7974 6f72 6368 2e6f 7267 2f29  ://pytorch.org/)
+000004a0: 207c 205b 546f 7263 6844 6174 6120 3e3d   | [TorchData >=
+000004b0: 302e 362e 305d 2868 7474 7073 3a2f 2f67  0.6.0](https://g
+000004c0: 6974 6875 622e 636f 6d2f 7079 746f 7263  ithub.com/pytorc
+000004d0: 682f 6461 7461 2920 7c20 5b50 7947 203e  h/data) | [PyG >
+000004e0: 3d32 2e33 5d28 6874 7470 733a 2f2f 7079  =2.3](https://py
+000004f0: 746f 7263 682d 6765 6f6d 6574 7269 632e  torch-geometric.
+00000500: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000510: 6e2f 6c61 7465 7374 2f6e 6f74 6573 2f69  n/latest/notes/i
+00000520: 6e73 7461 6c6c 6174 696f 6e2e 6874 6d6c  nstallation.html
+00000530: 2329 0d0a 0d0a 0d0a 6060 600d 0a63 6f6e  #)......```..con
+00000540: 6461 2063 7265 6174 6520 2d2d 6e61 6d65  da create --name
+00000550: 3d46 7265 6552 6563 2070 7974 686f 6e3d  =FreeRec python=
+00000560: 332e 390d 0a63 6f6e 6461 2061 6374 6976  3.9..conda activ
+00000570: 6174 6520 4672 6565 5265 630d 0a60 6060  ate FreeRec..```
+00000580: 0d0a 0d0a 0d0a 2a2a 4e6f 7465 3a2a 2a20  ......**Note:** 
+00000590: 4166 7465 7220 5079 546f 7263 6820 322e  After PyTorch 2.
+000005a0: 302c 2060 546f 7263 6844 6174 6160 2073  0, `TorchData` s
+000005b0: 6565 6d73 2074 6f20 6861 7665 2073 746f  eems to have sto
+000005c0: 7070 6564 2062 6569 6e67 2075 7064 6174  pped being updat
+000005d0: 6564 2c20 616e 6420 796f 7520 6361 6e20  ed, and you can 
+000005e0: 696e 7374 616c 6c20 6974 2077 6974 6820  install it with 
+000005f0: 602d 2d6e 6f2d 6465 7073 6020 746f 2061  `--no-deps` to a
+00000600: 766f 6964 2069 6e73 7461 6c6c 696e 6720  void installing 
+00000610: 6465 7065 6e64 656e 6369 6573 2e0d 0a0d  dependencies....
+00000620: 0a60 6060 0d0a 7069 7020 696e 7374 616c  .```..pip instal
+00000630: 6c20 2d2d 6e6f 2d64 6570 7320 746f 7263  l --no-deps torc
+00000640: 6864 6174 610d 0a60 6060 0d0a 0d0a 0d0a  hdata..```......
+00000650: 2323 2049 6e73 7461 6c6c 6174 696f 6e0d  ## Installation.
+00000660: 0a0d 0a20 2020 2070 6970 2069 6e73 7461  ...    pip insta
+00000670: 6c6c 2066 7265 6572 6563 0d0a 0d0a 6f72  ll freerec....or
+00000680: 2028 666f 7220 6c61 7465 7374 290d 0a0d   (for latest)...
+00000690: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+000006a0: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
+000006b0: 6875 622e 636f 6d2f 4d54 616e 6448 4a2f  hub.com/MTandHJ/
+000006c0: 6672 6565 7265 632e 6769 740d 0a0d 0a0d  freerec.git.....
+000006d0: 0a0d 0a23 2320 4461 7461 2050 6970 656c  ...## Data Pipel
+000006e0: 696e 650d 0a0d 0a3e 2052 6566 6572 2074  ine....> Refer t
+000006f0: 6f20 5b68 6572 655d 282e 2f64 6174 6173  o [here](./datas
+00000700: 6574 2532 3070 726f 6365 7373 696e 672e  et%20processing.
+00000710: 6d64 2920 666f 7220 6461 7461 7365 7420  md) for dataset 
+00000720: 7072 6f63 6573 7369 6e67 2061 6e64 2073  processing and s
+00000730: 706c 6974 7469 6e67 2e0d 0a0d 0a21 5b5d  plitting.....![]
+00000740: 2864 6f63 732f 7372 632f 7069 7065 6c69  (docs/src/pipeli
+00000750: 6e65 2e70 6e67 290d 0a0d 0a0d 0a23 2320  ne.png)......## 
+00000760: 5472 6169 6e69 6e67 2046 6c6f 770d 0a0d  Training Flow...
+00000770: 0a0d 0a21 5b5d 2864 6f63 732f 7372 632f  ...![](docs/src/
+00000780: 666c 6f77 2e70 6e67 290d 0a0d 0a0d 0a23  flow.png)......#
+00000790: 2320 5265 6665 7265 6e63 6520 436f 6465  # Reference Code
+000007a0: 0d0a 0d0a 2d20 546f 7263 6852 6563 3a20  ....- TorchRec: 
+000007b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007c0: 6f6d 2f70 7974 6f72 6368 2f74 6f72 6368  om/pytorch/torch
+000007d0: 7265 6320 0d0a 2d20 4465 6570 4354 522d  rec ..- DeepCTR-
+000007e0: 546f 7263 683a 2068 7474 7073 3a2f 2f67  Torch: https://g
+000007f0: 6974 6875 622e 636f 6d2f 7368 656e 7765  ithub.com/shenwe
+00000800: 6963 6865 6e2f 4465 6570 4354 522d 546f  ichen/DeepCTR-To
+00000810: 7263 680d 0a2d 2046 7578 6943 5452 3a20  rch..- FuxiCTR: 
+00000820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000830: 6f6d 2f78 7565 2d70 6169 2f46 7578 6943  om/xue-pai/FuxiC
+00000840: 5452 0d0a 2d20 4241 5253 3a20 6874 7470  TR..- BARS: http
+00000850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000860: 7065 6e62 656e 6368 6d61 726b 2f42 4152  penbenchmark/BAR
+00000870: 530d 0a2d 2052 6563 426f 6c65 3a20 6874  S..- RecBole: ht
+00000880: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000890: 2f52 5543 4149 426f 782f 5265 6342 6f6c  /RUCAIBox/RecBol
+000008a0: 650d 0a0d 0a0d 0a0d 0a23 2320 4163 6b6e  e........## Ackn
+000008b0: 6f77 6c65 6467 656d 656e 7473 0d0a 0d0a  owledgements....
+000008c0: 5468 616e 6b73 2074 6f20 4368 6174 4750  Thanks to ChatGP
+000008d0: 5420 666f 7220 7468 6520 616e 6e6f 7461  T for the annota
+000008e0: 7469 6f6e 206f 6620 736f 6d65 2063 6f64  tion of some cod
+000008f0: 652e 2046 6f72 2074 6869 7320 7265 6173  e. For this reas
+00000900: 6f6e 2c20 736f 6d65 206f 6620 7468 6520  on, some of the 
+00000910: 636f 6d6d 656e 7473 206d 6179 2062 6520  comments may be 
+00000920: 696c 6c6f 6769 6361 6c2e 0d0a            illogical...
```

### Comparing `freerec-0.7.5/README.md` & `freerec-0.8.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,112 @@
 00000000: 0d0a 0d0a 215b 5d28 646f 6373 2f73 7263  ....![](docs/src
-00000010: 2f6c 6f67 6f2e 706e 6729 0d0a 0d0a 4672  /logo.png)....Fr
-00000020: 6565 5265 6320 6973 2061 2072 6570 6f73  eeRec is a repos
-00000030: 6974 6f72 7920 6465 7369 676e 6564 2066  itory designed f
-00000040: 6f72 2065 6173 7920 2872 6563 6f6d 6d65  or easy (recomme
-00000050: 6e64 6174 696f 6e29 2064 6174 6120 7072  ndation) data pr
-00000060: 652d 7072 6f63 6573 7369 6e67 2061 6e64  e-processing and
-00000070: 206d 6f64 656c 2074 7261 696e 696e 672e   model training.
-00000080: 0d0a 4920 616d 2061 2062 6567 696e 6e65  ..I am a beginne
-00000090: 7220 696e 2074 6865 2066 6965 6c64 206f  r in the field o
-000000a0: 6620 7265 636f 6d6d 656e 6465 7220 7379  f recommender sy
-000000b0: 7374 656d 732c 2073 6f20 6d75 6368 206f  stems, so much o
-000000c0: 6620 4672 6565 5265 6327 7320 6465 7369  f FreeRec's desi
-000000d0: 676e 7320 6d61 7920 6e6f 7420 6265 2061  gns may not be a
-000000e0: 7320 6566 6665 6374 6976 652e 2049 6e20  s effective. In 
-000000f0: 6164 6469 7469 6f6e 2c20 796f 7520 6172  addition, you ar
-00000100: 6520 6672 6565 2074 6f20 7370 6563 6966  e free to specif
-00000110: 7920 796f 7572 206f 776e 2066 7261 6d65  y your own frame
-00000120: 776f 726b 2062 6173 6564 206f 6e20 4672  work based on Fr
-00000130: 6565 5265 632e 0d0a 0d0a 0d0a 2323 2052  eeRec.......## R
-00000140: 6571 7569 7265 6d65 6e74 733a 200d 0a0d  equirements: ...
-00000150: 0a50 7974 686f 6e20 3e3d 2033 2e39 207c  .Python >= 3.9 |
-00000160: 205b 5079 546f 7263 6820 3e3d 322e 305d   [PyTorch >=2.0]
-00000170: 2868 7474 7073 3a2f 2f70 7974 6f72 6368  (https://pytorch
-00000180: 2e6f 7267 2f29 207c 205b 546f 7263 6844  .org/) | [TorchD
-00000190: 6174 6120 3e3d 302e 362e 305d 2868 7474  ata >=0.6.0](htt
-000001a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000001b0: 7079 746f 7263 682f 6461 7461 2920 7c20  pytorch/data) | 
-000001c0: 5b50 7947 203e 3d32 2e33 5d28 6874 7470  [PyG >=2.3](http
-000001d0: 733a 2f2f 7079 746f 7263 682d 6765 6f6d  s://pytorch-geom
-000001e0: 6574 7269 632e 7265 6164 7468 6564 6f63  etric.readthedoc
-000001f0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6e  s.io/en/latest/n
-00000200: 6f74 6573 2f69 6e73 7461 6c6c 6174 696f  otes/installatio
-00000210: 6e2e 6874 6d6c 2329 0d0a 0d0a 0d0a 6060  n.html#)......``
-00000220: 600d 0a63 6f6e 6461 2063 7265 6174 6520  `..conda create 
-00000230: 2d2d 6e61 6d65 3d46 7265 6552 6563 2070  --name=FreeRec p
-00000240: 7974 686f 6e3d 332e 390d 0a63 6f6e 6461  ython=3.9..conda
-00000250: 2061 6374 6976 6174 6520 4672 6565 5265   activate FreeRe
-00000260: 630d 0a60 6060 0d0a 0d0a 0d0a 2a2a 4e6f  c..```......**No
-00000270: 7465 3a2a 2a20 4166 7465 7220 5079 546f  te:** After PyTo
-00000280: 7263 6820 322e 302c 2060 546f 7263 6844  rch 2.0, `TorchD
-00000290: 6174 6160 2073 6565 6d73 2074 6f20 6861  ata` seems to ha
-000002a0: 7665 2073 746f 7070 6564 2062 6569 6e67  ve stopped being
-000002b0: 2075 7064 6174 6564 2c20 616e 6420 796f   updated, and yo
-000002c0: 7520 6361 6e20 696e 7374 616c 6c20 6974  u can install it
-000002d0: 2077 6974 6820 602d 2d6e 6f2d 6465 7073   with `--no-deps
-000002e0: 6020 746f 2061 766f 6964 2069 6e73 7461  ` to avoid insta
-000002f0: 6c6c 696e 6720 6465 7065 6e64 656e 6369  lling dependenci
-00000300: 6573 2e0d 0a0d 0a60 6060 0d0a 7069 7020  es.....```..pip 
-00000310: 696e 7374 616c 6c20 2d2d 6e6f 2d64 6570  install --no-dep
-00000320: 7320 746f 7263 6864 6174 610d 0a60 6060  s torchdata..```
-00000330: 0d0a 0d0a 0d0a 2323 2049 6e73 7461 6c6c  ......## Install
-00000340: 6174 696f 6e0d 0a0d 0a20 2020 2070 6970  ation....    pip
-00000350: 2069 6e73 7461 6c6c 2066 7265 6572 6563   install freerec
-00000360: 0d0a 0d0a 6f72 2028 666f 7220 6c61 7465  ....or (for late
-00000370: 7374 290d 0a0d 0a20 2020 2070 6970 2069  st)....    pip i
-00000380: 6e73 7461 6c6c 2067 6974 2b68 7474 7073  nstall git+https
-00000390: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d54  ://github.com/MT
-000003a0: 616e 6448 4a2f 6672 6565 7265 632e 6769  andHJ/freerec.gi
-000003b0: 740d 0a0d 0a0d 0a0d 0a23 2320 4461 7461  t........## Data
-000003c0: 2050 6970 656c 696e 650d 0a0d 0a21 5b5d   Pipeline....![]
-000003d0: 2864 6f63 732f 7372 632f 7069 7065 6c69  (docs/src/pipeli
-000003e0: 6e65 2e70 6e67 290d 0a0d 0a2a 2a4e 6f74  ne.png)....**Not
-000003f0: 653a 2a2a 2054 6f20 6d61 6b65 2064 6174  e:** To make dat
-00000400: 6173 6574 2c20 706c 6561 7365 2064 6f77  aset, please dow
-00000410: 6e6c 6f61 6420 636f 7272 6573 706f 6e64  nload correspond
-00000420: 696e 6720 4174 6f6d 6963 2066 696c 6573  ing Atomic files
-00000430: 2066 726f 6d20 5b5b 5265 6342 6f6c 655d   from [[RecBole]
-00000440: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
-00000450: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
-00000460: 666f 6c64 6572 732f 3173 6f30 6c63 6b49  folders/1so0lckI
-00000470: 364e 365f 6e69 5645 5961 4275 2d4c 4963  6N6_niVEYaBu-LIc
-00000480: 704f 645a 6639 396b 6a29 5d2e 200d 0a54  pOdZf99kj)]. ..T
-00000490: 6865 6e2c 2072 756e 2060 6672 6565 7265  hen, run `freere
-000004a0: 6320 6d61 6b65 202d 2d68 656c 7060 2e0d  c make --help`..
-000004b0: 0a0d 0a23 2320 5472 6169 6e69 6e67 2046  ...## Training F
-000004c0: 6c6f 770d 0a0d 0a0d 0a21 5b5d 2864 6f63  low......![](doc
-000004d0: 732f 7372 632f 666c 6f77 2e70 6e67 290d  s/src/flow.png).
-000004e0: 0a0d 0a0d 0a23 2320 5265 6665 7265 6e63  .....## Referenc
-000004f0: 6520 436f 6465 0d0a 0d0a 2d20 546f 7263  e Code....- Torc
-00000500: 6852 6563 3a20 6874 7470 733a 2f2f 6769  hRec: https://gi
-00000510: 7468 7562 2e63 6f6d 2f70 7974 6f72 6368  thub.com/pytorch
-00000520: 2f74 6f72 6368 7265 6320 0d0a 2d20 4465  /torchrec ..- De
-00000530: 6570 4354 522d 546f 7263 683a 2068 7474  epCTR-Torch: htt
-00000540: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000550: 7368 656e 7765 6963 6865 6e2f 4465 6570  shenweichen/Deep
-00000560: 4354 522d 546f 7263 680d 0a2d 2046 7578  CTR-Torch..- Fux
-00000570: 6943 5452 3a20 6874 7470 733a 2f2f 6769  iCTR: https://gi
-00000580: 7468 7562 2e63 6f6d 2f78 7565 2d70 6169  thub.com/xue-pai
-00000590: 2f46 7578 6943 5452 0d0a 2d20 4241 5253  /FuxiCTR..- BARS
-000005a0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-000005b0: 2e63 6f6d 2f6f 7065 6e62 656e 6368 6d61  .com/openbenchma
-000005c0: 726b 2f42 4152 530d 0a2d 2052 6563 426f  rk/BARS..- RecBo
-000005d0: 6c65 3a20 6874 7470 733a 2f2f 6769 7468  le: https://gith
-000005e0: 7562 2e63 6f6d 2f52 5543 4149 426f 782f  ub.com/RUCAIBox/
-000005f0: 5265 6342 6f6c 650d 0a0d 0a0d 0a0d 0a23  RecBole........#
-00000600: 2320 4163 6b6e 6f77 6c65 6467 656d 656e  # Acknowledgemen
-00000610: 7473 0d0a 0d0a 5468 616e 6b73 2074 6f20  ts....Thanks to 
-00000620: 4368 6174 4750 5420 666f 7220 7468 6520  ChatGPT for the 
-00000630: 616e 6e6f 7461 7469 6f6e 206f 6620 736f  annotation of so
-00000640: 6d65 2063 6f64 652e 2046 6f72 2074 6869  me code. For thi
-00000650: 7320 7265 6173 6f6e 2c20 736f 6d65 206f  s reason, some o
-00000660: 6620 7468 6520 636f 6d6d 656e 7473 206d  f the comments m
-00000670: 6179 2062 6520 696c 6c6f 6769 6361 6c2e  ay be illogical.
+00000010: 2f6c 6f67 6f2e 706e 6729 0d0a 0d0a 3c68  /logo.png)....<h
+00000020: 3420 616c 6967 6e3d 2263 656e 7465 7222  4 align="center"
+00000030: 3e0d 0a20 2020 203c 703e 0d0a 2020 2020  >..    <p>..    
+00000040: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000050: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000060: 4d54 616e 6448 4a2f 6672 6565 7265 632f  MTandHJ/freerec/
+00000070: 626c 6f62 2f6d 6173 7465 722f 6461 7461  blob/master/data
+00000080: 7365 7425 3230 7072 6f63 6573 7369 6e67  set%20processing
+00000090: 2e6d 6422 3e44 6174 6173 6574 2070 726f  .md">Dataset pro
+000000a0: 6365 7373 696e 673c 2f61 3e20 7c0d 0a20  cessing</a> |.. 
+000000b0: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
+000000c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000d0: 6f6d 2f4d 5461 6e64 484a 2f66 7265 6572  om/MTandHJ/freer
+000000e0: 6563 2f62 6c6f 622f 6d61 7374 6572 2f74  ec/blob/master/t
+000000f0: 7261 696e 696e 6725 3230 616e 6425 3230  raining%20and%20
+00000100: 7475 6e69 6e67 2e6d 6422 3e54 7261 696e  tuning.md">Train
+00000110: 696e 6720 616e 6420 5475 6e69 6e67 3c2f  ing and Tuning</
+00000120: 613e 207c 0d0a 2020 2020 2020 2020 3c61  a> |..        <a
+00000130: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000140: 6974 6875 622e 636f 6d2f 4d54 616e 6448  ithub.com/MTandH
+00000150: 4a2f 5265 6342 6f61 7264 223e 5265 6342  J/RecBoard">RecB
+00000160: 6f61 7264 3c2f 613e 0d0a 2020 2020 3c2f  oard</a>..    </
+00000170: 703e 0d0a 3c2f 6834 3e0d 0a0d 0a46 7265  p>..</h4>....Fre
+00000180: 6552 6563 2069 7320 6120 7265 706f 7369  eRec is a reposi
+00000190: 746f 7279 2064 6573 6967 6e65 6420 666f  tory designed fo
+000001a0: 7220 6561 7379 2028 7265 636f 6d6d 656e  r easy (recommen
+000001b0: 6461 7469 6f6e 2920 6461 7461 2070 7265  dation) data pre
+000001c0: 2d70 726f 6365 7373 696e 6720 616e 6420  -processing and 
+000001d0: 6d6f 6465 6c20 7472 6169 6e69 6e67 2e20  model training. 
+000001e0: 596f 7520 6172 6520 6672 6565 2074 6f20  You are free to 
+000001f0: 7370 6563 6966 7920 796f 7572 206f 776e  specify your own
+00000200: 2066 7261 6d65 776f 726b 2062 6173 6564   framework based
+00000210: 206f 6e20 4672 6565 5265 632e 0d0a 0d0a   on FreeRec.....
+00000220: 0d0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
+00000230: 733a 200d 0a0d 0a50 7974 686f 6e20 3e3d  s: ....Python >=
+00000240: 2033 2e39 207c 205b 5079 546f 7263 6820   3.9 | [PyTorch 
+00000250: 3e3d 322e 305d 2868 7474 7073 3a2f 2f70  >=2.0](https://p
+00000260: 7974 6f72 6368 2e6f 7267 2f29 207c 205b  ytorch.org/) | [
+00000270: 546f 7263 6844 6174 6120 3e3d 302e 362e  TorchData >=0.6.
+00000280: 305d 2868 7474 7073 3a2f 2f67 6974 6875  0](https://githu
+00000290: 622e 636f 6d2f 7079 746f 7263 682f 6461  b.com/pytorch/da
+000002a0: 7461 2920 7c20 5b50 7947 203e 3d32 2e33  ta) | [PyG >=2.3
+000002b0: 5d28 6874 7470 733a 2f2f 7079 746f 7263  ](https://pytorc
+000002c0: 682d 6765 6f6d 6574 7269 632e 7265 6164  h-geometric.read
+000002d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000002e0: 7465 7374 2f6e 6f74 6573 2f69 6e73 7461  test/notes/insta
+000002f0: 6c6c 6174 696f 6e2e 6874 6d6c 2329 0d0a  llation.html#)..
+00000300: 0d0a 0d0a 6060 600d 0a63 6f6e 6461 2063  ....```..conda c
+00000310: 7265 6174 6520 2d2d 6e61 6d65 3d46 7265  reate --name=Fre
+00000320: 6552 6563 2070 7974 686f 6e3d 332e 390d  eRec python=3.9.
+00000330: 0a63 6f6e 6461 2061 6374 6976 6174 6520  .conda activate 
+00000340: 4672 6565 5265 630d 0a60 6060 0d0a 0d0a  FreeRec..```....
+00000350: 0d0a 2a2a 4e6f 7465 3a2a 2a20 4166 7465  ..**Note:** Afte
+00000360: 7220 5079 546f 7263 6820 322e 302c 2060  r PyTorch 2.0, `
+00000370: 546f 7263 6844 6174 6160 2073 6565 6d73  TorchData` seems
+00000380: 2074 6f20 6861 7665 2073 746f 7070 6564   to have stopped
+00000390: 2062 6569 6e67 2075 7064 6174 6564 2c20   being updated, 
+000003a0: 616e 6420 796f 7520 6361 6e20 696e 7374  and you can inst
+000003b0: 616c 6c20 6974 2077 6974 6820 602d 2d6e  all it with `--n
+000003c0: 6f2d 6465 7073 6020 746f 2061 766f 6964  o-deps` to avoid
+000003d0: 2069 6e73 7461 6c6c 696e 6720 6465 7065   installing depe
+000003e0: 6e64 656e 6369 6573 2e0d 0a0d 0a60 6060  ndencies.....```
+000003f0: 0d0a 7069 7020 696e 7374 616c 6c20 2d2d  ..pip install --
+00000400: 6e6f 2d64 6570 7320 746f 7263 6864 6174  no-deps torchdat
+00000410: 610d 0a60 6060 0d0a 0d0a 0d0a 2323 2049  a..```......## I
+00000420: 6e73 7461 6c6c 6174 696f 6e0d 0a0d 0a20  nstallation.... 
+00000430: 2020 2070 6970 2069 6e73 7461 6c6c 2066     pip install f
+00000440: 7265 6572 6563 0d0a 0d0a 6f72 2028 666f  reerec....or (fo
+00000450: 7220 6c61 7465 7374 290d 0a0d 0a20 2020  r latest)....   
+00000460: 2070 6970 2069 6e73 7461 6c6c 2067 6974   pip install git
+00000470: 2b68 7474 7073 3a2f 2f67 6974 6875 622e  +https://github.
+00000480: 636f 6d2f 4d54 616e 6448 4a2f 6672 6565  com/MTandHJ/free
+00000490: 7265 632e 6769 740d 0a0d 0a0d 0a0d 0a23  rec.git........#
+000004a0: 2320 4461 7461 2050 6970 656c 696e 650d  # Data Pipeline.
+000004b0: 0a0d 0a3e 2052 6566 6572 2074 6f20 5b68  ...> Refer to [h
+000004c0: 6572 655d 282e 2f64 6174 6173 6574 2532  ere](./dataset%2
+000004d0: 3070 726f 6365 7373 696e 672e 6d64 2920  0processing.md) 
+000004e0: 666f 7220 6461 7461 7365 7420 7072 6f63  for dataset proc
+000004f0: 6573 7369 6e67 2061 6e64 2073 706c 6974  essing and split
+00000500: 7469 6e67 2e0d 0a0d 0a21 5b5d 2864 6f63  ting.....![](doc
+00000510: 732f 7372 632f 7069 7065 6c69 6e65 2e70  s/src/pipeline.p
+00000520: 6e67 290d 0a0d 0a0d 0a23 2320 5472 6169  ng)......## Trai
+00000530: 6e69 6e67 2046 6c6f 770d 0a0d 0a0d 0a21  ning Flow......!
+00000540: 5b5d 2864 6f63 732f 7372 632f 666c 6f77  [](docs/src/flow
+00000550: 2e70 6e67 290d 0a0d 0a0d 0a23 2320 5265  .png)......## Re
+00000560: 6665 7265 6e63 6520 436f 6465 0d0a 0d0a  ference Code....
+00000570: 2d20 546f 7263 6852 6563 3a20 6874 7470  - TorchRec: http
+00000580: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00000590: 7974 6f72 6368 2f74 6f72 6368 7265 6320  ytorch/torchrec 
+000005a0: 0d0a 2d20 4465 6570 4354 522d 546f 7263  ..- DeepCTR-Torc
+000005b0: 683a 2068 7474 7073 3a2f 2f67 6974 6875  h: https://githu
+000005c0: 622e 636f 6d2f 7368 656e 7765 6963 6865  b.com/shenweiche
+000005d0: 6e2f 4465 6570 4354 522d 546f 7263 680d  n/DeepCTR-Torch.
+000005e0: 0a2d 2046 7578 6943 5452 3a20 6874 7470  .- FuxiCTR: http
+000005f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f78  s://github.com/x
+00000600: 7565 2d70 6169 2f46 7578 6943 5452 0d0a  ue-pai/FuxiCTR..
+00000610: 2d20 4241 5253 3a20 6874 7470 733a 2f2f  - BARS: https://
+00000620: 6769 7468 7562 2e63 6f6d 2f6f 7065 6e62  github.com/openb
+00000630: 656e 6368 6d61 726b 2f42 4152 530d 0a2d  enchmark/BARS..-
+00000640: 2052 6563 426f 6c65 3a20 6874 7470 733a   RecBole: https:
+00000650: 2f2f 6769 7468 7562 2e63 6f6d 2f52 5543  //github.com/RUC
+00000660: 4149 426f 782f 5265 6342 6f6c 650d 0a0d  AIBox/RecBole...
+00000670: 0a0d 0a0d 0a23 2320 4163 6b6e 6f77 6c65  .....## Acknowle
+00000680: 6467 656d 656e 7473 0d0a 0d0a 5468 616e  dgements....Than
+00000690: 6b73 2074 6f20 4368 6174 4750 5420 666f  ks to ChatGPT fo
+000006a0: 7220 7468 6520 616e 6e6f 7461 7469 6f6e  r the annotation
+000006b0: 206f 6620 736f 6d65 2063 6f64 652e 2046   of some code. F
+000006c0: 6f72 2074 6869 7320 7265 6173 6f6e 2c20  or this reason, 
+000006d0: 736f 6d65 206f 6620 7468 6520 636f 6d6d  some of the comm
+000006e0: 656e 7473 206d 6179 2062 6520 696c 6c6f  ents may be illo
+000006f0: 6769 6361 6c2e                           gical.
```

### Comparing `freerec-0.7.5/freerec/__init__.py` & `freerec-0.8.1/freerec/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7.5'
+__version__ = '0.8.1'
 
 from . import data, models, criterions, ddp, graph, launcher, metrics, parser, utils
 from .utils import infoLogger
 from freerec.dict2obj import Config
 
 
 def declare(*, version: str):
```

### Comparing `freerec-0.7.5/freerec/criterions.py` & `freerec-0.8.1/freerec/criterions.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,16 +131,14 @@
         reduction: Optional[str] = None
     ):
         reduction = reduction if reduction is not None else self.reduction
         return F.l1_loss(inputs, targets, reduction=reduction)
 
 
 
-
-
 def cross_entropy_with_logits(
     logits: torch.Tensor, targets: torch.Tensor,
     reduction: str = "mean"
 ) -> torch.Tensor:
     r"""
     Cross-entropy loss with logits.
```

### Comparing `freerec-0.7.5/freerec/data/datasets/base.py` & `freerec-0.8.1/freerec/data/datasets/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 
 
-from typing import Iterator, Optional, TypeVar, Tuple, List
+from typing import Any, TypeVar, Literal, Union, Optional, Callable, Iterator, Iterable, Dict, Tuple, List
 
 import torch, os, abc
 import numpy as np
+import pandas as pd
 import torchdata.datapipes as dp
+from copy import copy
 from functools import lru_cache
-from freeplot.utils import import_pickle, export_pickle
 
-from ..tags import FieldTags, SPARSE, USER, SESSION, ITEM, ID
-from ..fields import Field, BufferField, FieldList, FieldTuple
+from ..tags import FieldTags, TaskTags, USER, ITEM, ID, RATING, TIMESTAMP, FEATURE, SEQUENCE
+from ..fields import Field, FieldTuple
 from ..utils import download_from_url, extract_archive
-from ...utils import timemeter, infoLogger, mkdirs, warnLogger
+from ...utils import timemeter, infoLogger, warnLogger
+from ...dict2obj import Config
 
 
 __all__ = ['BaseSet', 'RecDataSet']
 
 
-DEFAULT_PICKLE_FMT = "{0}_from_pickle"
-DEFAULT_TRANSFORM_FILENAME = "transforms.pickle"
-DEFAULT_CHUNK_FMT = "chunk{0}.pickle"
+T = TypeVar('T')
 
 
-T = TypeVar('T')
+def safe_mode(*modes):
+    def decorator(func):
+        def wrapper(self, *args, **kwargs):
+            if self.mode not in modes:
+                fname = f"\033[0m\033[0;31;47m{func.__name__}\033[0m\033[1;31m"
+                mode = f"\033[0m\033[0;31;47m{self.mode}\033[0m\033[1;31m"
+                warnLogger(f"{fname} runs in {mode} mode. Make sure that this is intentional ...")
+            return func(self, *args, **kwargs)
+        wrapper.__name__ == func.__name__
+        wrapper.__doc__ = func.__doc__
+        return wrapper
+    return decorator
 
 
 #===============================Basic Class===============================
 
 class RecSetBuildingError(Exception): ...
 
 
@@ -34,97 +45,75 @@
     r""" 
     Base class for data pipes. Defines basic functionality and methods for 
     pre-processing the data for the learning models.
 
     Parameters:
     -----------
     root: str
-        The path storing datasets.
-    filename: str, optional 
-        The dirname of the dataset. If `None`, sets the classname as the filename.
+        The root path storing datasets.
+    filefir: str, optional 
+        The dirname of the dataset. If `None`, set the classname as the filedir.
     download: bool 
         Download the dataset from a URL.
-
-    Attributes:
-    -----------
-    _cfg: Config[str, Field] 
-        Includes fields of each column.
-    DEFAULT_CHUNK_SIZE: int, default 51200 
-        Chunk size for saving.
-    DATATYPE: str
-        Dataset type.
-        - `General': for general recommendation.
-        - `Sequential': for sequential recommendation.
-        - `Session': for session-based recommendation.
-        - `Context': for context-aware recommendation.
-        - `Knowledge': for knowledge-based recommendation.
-    VALID_IS_TEST: bool 
-        The validset and testset are the same one sometimes.
-
-    Notes:
-    ------
-    All datasets that inherit RecDataSet should define the class variable `_cfg` before instantiation.
-    Generally speaking, the dataset will be split into:
-        - trainset
-        - validset
-        - testset
     """
 
-    DEFAULT_CHUNK_SIZE = 51200 # chunk size
-    URL: str
-    DATATYPE: str
-    VALID_IS_TEST: bool
-
-    def __new__(cls, *args, **kwargs):
-        for attr in ('_cfg', 'DATATYPE', 'VALID_IS_TEST'):
-            if not hasattr(cls, attr):
-                raise RecSetBuildingError(f"'{attr}' should be defined before instantiation ...")
-        assert 'fields' in cls._cfg, "the config of fields should be defined in '_cfg' ..."
-        return super().__new__(cls)
+    _field_builder = {
+        USER.name: Field(USER.name, USER, ID),
+        ITEM.name: Field(ITEM.name, ITEM, ID),
+        RATING.name: Field(RATING.name, RATING),
+        TIMESTAMP.name: Field(TIMESTAMP.name, TIMESTAMP)
+    }
+
+    _open_kwargs = Config(
+        trainfile='train.txt', validfile='valid.txt', testfile='test.txt',
+        userfile='user.txt', itemfile='item.txt',
+        sep='\t'
+    )
 
-    def __init__(self, root: str, filename: Optional[str] = None, download: bool = True) -> None:
-        super().__init__()
+    TASK: TaskTags
+    URL: Optional[str] = None
 
-        self.trainsize: int = 0
-        self.validsize: int = 0
-        self.testsize: int = 0
+    def __init__(
+        self, 
+        root: str, 
+        filedir: Optional[str] = None, 
+        download: bool = True,
+        tasktag: Optional[TaskTags] = None
+    ) -> None:
+        super().__init__()
 
-        fields = []
-        for field_type, cfg in self._cfg['fields']:
-            fields.append(field_type(**cfg))
-        self.fields = fields
-        self.__mode = 'train'
+        self.fields = []
+        self.__mode: Literal['train', 'valid', 'test'] = 'train'
+        if tasktag is not None:
+            self.TASK = tasktag
 
-        filename = filename if filename else self.__class__.__name__
-        self.path = os.path.join(root, self.DATATYPE, filename)
+        filedir = filedir if filedir else self.__class__.__name__
+        self.path = os.path.join(root, 'Processed', filedir)
         if not os.path.exists(self.path) or not any(True for _ in os.scandir(self.path)):
-            if download:
+            if download and self.URL is not None:
                 extract_archive(
                     download_from_url(self.URL, root, overwrite=False),
                     self.path
                 )
             else:
-                raise FileNotFoundError(f"No such file of {self.path}, or this dir is empty ...")
+                raise FileNotFoundError(
+                    f"No such file of {self.path}, or this dir is empty. \n"
+                    f"Please use `freerec make` to prepare the dataset with the following setting: \n {self.__class__.__doc__}"
+                )
 
         self.compile()
         self.check()
 
     def check(self):
         """Self-check program should be placed here."""
         ...
         
     @property
-    def mode(self) -> str:
-        r"""
-        Return the mode in which the dataset is currently being used.
-
-        Returns:
-            str: The mode in which the dataset is currently being used.
-        """
-
+    def mode(self) -> Literal['train', 'test', 'valid']:
+        """Return the current mode."""
         return self.__mode
 
     def train(self: T) -> T:
         """Switch the dataset mode to 'train'."""
         self.__mode = 'train'
         return self
 
@@ -135,60 +124,355 @@
 
     def test(self: T) -> T:
         """Switch the dataset mode to 'test'."""
         self.__mode = 'test'
         return self
 
     @property
-    def fields(self):
-        return self.__fields
-
-    @fields.setter
-    def fields(self, vals) -> FieldTuple[Field]:
-        """Return: Tuple of Field."""
-        self.__fields = FieldTuple(vals)
+    def datasize(self):
+        """Return the size of dataset according to the current mode."""
+        if self.mode == 'train':
+            return self.trainsize
+        elif self.mode == 'valid':
+            return self.validsize
+        else:
+            return self.testsize
 
-    @abc.abstractmethod
-    def raw2data(self) -> dp.iter.IterableWrapper:
+    @property
+    def interdata(self) -> Dict[Field, Tuple]:
         r"""
-        Process raw data.
+        Get interaction data.
 
-        Returns:
-        --------
-        A processed data.
+        Examples:
+        ---------
+        >>> dataset: BaseSet
+        >>> dataset.train().interdata == dataset.valid().interdata
+        False
+        """
+        return self.__interdata[self.mode]
+
+    @property
+    def userdata(self) -> Dict[Field, Tuple]:
+        try:
+            return self.__userdata
+        except AttributeError:
+            self.load_user()
+            return self.__userdata
 
-        Raises:
-        -------
-        NotImplementedError: Subclasses should implement this method.
+    @property
+    def itemdata(self) -> Dict[Field, Tuple]:
+        try:
+            return self.__itemdata
+        except AttributeError:
+            self.load_item()
+            return self.__itemdata
+
+    @property
+    def fields(self) -> FieldTuple[Field]:
+        """Return a tuple of Field."""
+        return self.__fields
+
+    @fields.setter
+    def fields(self, fields: Iterable[Field]):
+        r"""
+        Set fields.
 
         Notes:
         ------
-        This method should be implemented by subclasses.
+        Set fields will change the saved interaction data.
         """
-        raise NotImplementedError(f"{self.__class__.__name__}.raw2data() method should be implemented ...")
+        self.__fields = FieldTuple(fields)
+        traindata = dict()
+        validdata = dict()
+        testdata = dict()
+        for field in self.fields:
+            try:
+                traindata[field] = self.train().interdata[field]
+                validdata[field] = self.valid().interdata[field]
+                testdata[field] = self.test().interdata[field]
+            except KeyError:
+                raise ValueError(
+                    f"Setting a {field} not in `self.fields` ..."
+                )
+        self.__interdata = {
+            'train': traindata, 'valid': validdata, 'test': testdata
+        }
 
-    @abc.abstractmethod
-    def pickle2data(self):
-        raise NotImplementedError(
-                f"{self.__class__.__name__}.pickle2data should be implemented before using ..."
-        )
-
-    def __iter__(self) -> Iterator[FieldList[BufferField]]:
-        for cols in self.pickle2data():
-            yield FieldList(map(
-                lambda field, col: field.buffer(col),
-                self.fields,
-                cols
-            ))
+    @classmethod
+    def build_fields(cls, columns: Iterable[str], *tags: FieldTags) -> FieldTuple[Field]:
+        fields = []
+        for colname in columns:
+            field = cls._field_builder.get(
+                colname,
+                Field(colname, FEATURE)
+            ).fork(*tags)
+            fields.append(field)
+        return FieldTuple(fields)
+
+    def load_inter(self):
+        r"""
+        Load interaction data.
+
+        Flows:
+        ------
+        1. Read dataframe according `_open_kwargs`.
+        2. Record datasize.
+        3. Build fields.
+        4. Transform each field data.
+        """
+        train_df = pd.read_csv(
+            os.path.join(self.path, self._open_kwargs.trainfile),
+            sep=self._open_kwargs.sep
+        )
+        valid_df = pd.read_csv(
+            os.path.join(self.path, self._open_kwargs.validfile),
+            sep=self._open_kwargs.sep
+        )
+        test_df = pd.read_csv(
+            os.path.join(self.path, self._open_kwargs.testfile),
+            sep=self._open_kwargs.sep
+        )
+
+        self.trainsize = len(train_df)
+        self.validsize = len(valid_df)
+        self.testsize = len(test_df)
+
+        self.__fields = self.build_fields(train_df.columns)
+
+        self.__interdata = {
+            'train': dict(), 'valid': dict(), 'test': dict()
+        }
+        for field in self.fields:
+            colname = field.name
+            traindata = field.try_to_numeric(train_df[colname])
+            validdata = field.try_to_numeric(valid_df[colname])
+            testdata = field.try_to_numeric(test_df[colname])
+
+            field.count = len(
+                set(traindata) | set(validdata) | set(testdata)
+            )
+
+            self.__interdata['train'][field] = traindata
+            self.__interdata['valid'][field] = validdata
+            self.__interdata['test'][field] = testdata
+
+    def load_user(self):
+        user_df = pd.read_csv(
+            os.path.join(self.path, self._open_kwargs.userfile),
+            sep=self._open_kwargs.sep
+        )
+        fields = self.build_fields(user_df.columns, USER)
+        self.__userdata = {}
+        for field in fields:
+            colname = field.name
+            data = field.try_to_numeric(user_df[colname])
+            field.count = len(set(data))
+            self.__userdata[field] = data
+
+    def load_item(self):
+        item_df = pd.read_csv(
+            os.path.join(self.path, self._open_kwargs.itemfile),
+            sep=self._open_kwargs.sep
+        )
+        fields = self.build_fields(item_df.columns, ITEM)
+        self.__itemdata = {}
+        for field in fields:
+            colname = field.name
+            data = field.try_to_numeric(item_df[colname])
+            field.count = len(set(data))
+            self.__itemdata[field] = data
 
     def summary(self):
         """Print a summary of the dataset."""
         infoLogger(str(self))
 
     @timemeter
+    def compile(self):
+        self.load_inter()
+        self.summary()
+        self.train()
+
+    def match_all(self: T, *tags: FieldTags) -> T:
+        r"""
+        Return a copy of dataset with fields matching all given tags.
+
+        Examples:
+        ---------
+        >>> dataset: BaseSet
+        RecDataSet(USER:ID,USER|ITEM:ID,ITEM|RATING:RATING|TIMESTAMP:TIMESTAMP)
+        >>> dataset.match_all(ID)
+        RecDataSet(USER:ID,USER|ITEM:ID,ITEM)
+        >>> dataset.match_all()
+        RecDataSet(USER:ID,USER|ITEM:ID,ITEM|RATING:RATING|TIMESTAMP:TIMESTAMP)
+        """
+        dataset = copy(self)
+        dataset.fields = self.fields.match_all(*tags)
+        return dataset
+
+    def match_any(self: T, *tags: FieldTags) -> T:
+        r"""
+        Return a copy of dataset with fields matching any given tags.
+
+        Examples:
+        ---------
+        >>> dataset: BaseSet
+        RecDataSet(USER:ID,USER|ITEM:ID,ITEM|RATING:RATING|TIMESTAMP:TIMESTAMP)
+        >>> dataset.match_any(ID, TIMESTAMP)
+        RecDataSet(USER:ID,USER|ITEM:ID,ITEM|TIMESTAMP:TIMESTAMP)
+        >>> dataset.match_any()
+        RecDataSet()
+        """
+        dataset = copy(self)
+        dataset.fields = self.fields.match_any(*tags)
+        return dataset
+
+    @staticmethod
+    def listmap(func: Callable, *iterables) -> List:
+        r"""
+        Apply a function to multiple iterables and return a list.
+
+        Parameters:
+        -----------
+        func (Callable): The function to be applied.
+        *iterables: Multiple iterables to be processed.
+
+        Returns:
+        --------
+        List: The results after applying the function to the iterables.
+        """
+        return list(map(func, *iterables))
+
+    @classmethod
+    def to_rows(cls, field_dict: Dict[Field, Iterable[T]]) -> List[Dict[Field, T]]:
+        fields = field_dict.keys()
+        return cls.listmap(
+            lambda values: dict(zip(fields, values)),
+            zip(*field_dict.values())
+        )
+
+    def __repr__(self) -> str:
+        cfg = '|'.join(map(str, self.fields))
+        return f"{self.__class__.__name__}({cfg})"
+
+    def __str__(self) -> str:
+        cfg = ' | '.join(map(str, self.fields))
+        return f"[{self.__class__.__name__}] >>> " + cfg
+
+    def __iter__(self) -> Iterator[Dict[Field, Any]]:
+        yield from iter(
+            self.to_rows(self.interdata)
+        )
+
+
+class RecDataSet(BaseSet):
+    """RecDataSet provides a template for specific datasets."""
+
+    def to_pairs(self) -> List[Dict[Field, int]]:
+        """Return (User, Item) in pairs."""
+        User = self.fields[USER, ID]
+        Item = self.fields[ITEM, ID]
+        users, items = self.interdata[User], self.interdata[Item]
+        return self.to_rows({User: users, Item:items})
+
+    def to_seqs(self, maxlen: Optional[int] = None) -> List[Dict[Field, Union[int, Tuple[int]]]]:
+        r"""
+        Return dataset in sequence.
+
+        Parameters:
+        -----------
+        maxlen: int, optional
+            Maximum length
+            `None`: return the whole sequence
+            `int`: return the recent `maxlen` items
+        """
+        User = self.fields[USER, ID]
+        Item = self.fields[ITEM, ID]
+        seqs = [[] for id_ in range(User.count)]
+
+        self.listmap(
+            lambda data: seqs[data[User]].append(data[Item]),
+            self.to_pairs()
+        )
+        users = list(range(User.count))
+        if maxlen is not None:
+            seqs = [tuple(items[-maxlen:]) for items in seqs]
+        else:
+            seqs = [tuple(items) for items in seqs]
+
+        return self.to_rows({User: users, Item.fork(SEQUENCE): seqs})
+
+    def to_roll_seqs(
+        self, minlen: int = 2, maxlen: Optional[int] = None,
+        keep_at_least_itself: bool = True
+    ) -> List[Dict[Field, Union[int, Tuple[int]]]]:
+        r"""
+        Rolling dataset in sequence.
+
+        Parameters:
+        -----------
+        minlen: int
+            Shorest sequence
+        maxlen: int, optional
+            Maximum length
+            `None`: Roll throughout the whole sequence
+        keep_at_least_itself: bool, default to `True`
+            `True`: Keep the sequence with items less than `minlen`
+        """
+        User = self.fields[USER, ID]
+        ISeq = self.fields[ITEM, ID].fork(SEQUENCE)
+        data = self.to_seqs(maxlen)
+
+        roll_seqs = []
+        for row in data:
+            user, seq = row[User], row[ISeq]
+            if len(seq) <= minlen and keep_at_least_itself:
+                roll_seqs.append(
+                    {User: user, ISeq: seq}
+                )
+                continue
+            for k in range(minlen, len(seq) + 1):
+                roll_seqs.append(
+                    {User: user, ISeq: seq[:k]}
+                )
+
+        return roll_seqs
+
+    def seqlens(self) -> List[int]:
+        ISeq = self.fields[ITEM, ID].fork(SEQUENCE)
+        seqlens = [len(row[ISeq]) for row in self.to_seqs()]
+        return list(filter(lambda x: x > 0, seqlens))
+
+    @property
+    def maxlen(self) -> int:
+        return np.max(self.seqlens()).item()
+
+    @property
+    def minlen(self) -> int:
+        return np.min(self.seqlens()).item()
+
+    @property
+    def meanlen(self) -> int:
+        return np.mean(self.seqlens()).item()
+
+    @lru_cache()
+    def has_duplicates(self) -> bool:
+        """Check whether the dataset has repeated interactions."""
+        ISeq = self.fields[ITEM, ID].fork(SEQUENCE)
+        traindata = self.train().to_seqs()
+        validdata = self.valid().to_seqs()
+        testdata = self.test().to_seqs()
+
+        for triplet in zip(traindata, validdata, testdata):
+            seq = triplet[0][ISeq] + triplet[1][ISeq] + triplet[2][ISeq]
+            if len(seq) != len(set(seq)):
+                return True
+        return False
+
+    @timemeter
+    @safe_mode('train')
     def to_heterograph(self, *edge_types: Tuple[Tuple[FieldTags], Optional[str], Tuple[FieldTags]]):
         r"""
         Convert datapipe to a heterograph.
 
         Parameters:
         -----------
         *edge_types: Tuple[Tuple[str, str], Optional[str], Tuple[str, str]]
@@ -205,50 +489,40 @@
 
         Notes:
         ------
         A warning will be raised if the current mode is not 'train'!
 
         Examples:
         ---------
-        >>> from freerec.data.datasets import Gowalla_m1
-        >>> from freerec.data.tags import USER, ITEM, ID
-        >>> basepipe = Gowalla_m1("../data")
-        >>> fields = basepipe.fields
-        >>> graph = basepipe.to_heterograph(
+        >>> dataset: RecDataSet
+        >>> graph = dataset.to_heterograph(
         ...    ((USER, ID), None, (ITEM, ID)),
         ...    ((ITEM, ID), None, (USER, ID))
         ... )
         >>> graph
         HeteroData(
-            UserID={ x=[29858, 0] },
-            ItemID={ x=[40981, 0] },
-            (UserID, UserID2ItemID, ItemID)={ edge_index=[2, 810128] },
-            (ItemID, ItemID2UserID, UserID)={ edge_index=[2, 810128] }
+            USER={ x=[22363, 0] },
+            ITEM={ x=[12101, 0] },
+            (USER, USER2ITEM, ITEM)={ edge_index=[2, 153776] },
+            (ITEM, ITEM2USER, USER)={ edge_index=[2, 153776] }
         )
         """
         from torch_geometric.data import HeteroData
 
-        # check mode and raise warning if not in 'train' mode
-        if self.mode != 'train':
-            warnLogger(f"Convert the {self.mode} datapipe to graph. Make sure that this is intentional ...")
-
         srcs, edges, dsts = zip(*edge_types)
         srcs = [self.fields[src] for src in srcs]
         dsts = [self.fields[dst] for dst in dsts]
         nodes = set(srcs + dsts)
         edges = list(map(
             lambda src, edge, dst: edge if edge else f"{src.name}2{dst.name}",
             srcs, edges, dsts
         ))
-        data = {node.name: [] for node in nodes}
-        for chunk in self:
-            for node in nodes:
-                data[node.name].append(np.ravel(chunk[node.tags].data))
+        data = {node.name: self.interdata[node] for node in nodes}
         for key in data:
-            data[key] = torch.tensor(np.concatenate(data[key], axis=0), dtype=torch.long)
+            data[key] = torch.tensor(data[key], dtype=torch.long)
 
         graph = HeteroData()
         for node in srcs:
             graph[node.name].x = torch.empty((node.count, 0), dtype=torch.long)
         for node in dsts:
             if node not in srcs:
                 graph[node.name].x = torch.empty((node.count, 0), dtype=torch.long)
@@ -282,26 +556,23 @@
 
         Notes:
         ------
         A warning will be raised if the current mode is not 'train'!
 
         Examples:
         ---------
-        >>> from freerec.data.datasets import Gowalla_m1
-        >>> from freerec.data.tags import USER, ITEM, ID
-        >>> basepipe = Gowalla_m1("../data")
-        >>> fields = basepipe.fields
-        >>> graph = basepipe.to_bigraph(
+        >>> dataset: RecDataSet
+        >>> graph = dataset.to_bigraph(
         ...    (USER, ID), (ITEM, ID)
         ... )
         >>> graph
         HeteroData(
-            UserID={ x=[29858, 0] },
-            ItemID={ x=[40981, 0] },
-            (UserID, UserID2ItemID, ItemID)={ edge_index=[2, 810128] }
+            USER={ x=[22363, 0] },
+            ITEM={ x=[12101, 0] },
+            (USER, USER2ITEM, ITEM)={ edge_index=[2, 153776] }
         )
         """
         return self.to_heterograph((src, edge_type, dst))
    
     def to_graph(
         self, 
         src: Tuple[FieldTags] = (USER, ID), 
@@ -324,23 +595,20 @@
 
         Notes:
         ------
         A warning will be raised if current mode is not 'train' !
 
         Examples:
         --------
-        >>> from freerec.data.datasets import Gowalla_m1
-        >>> from freerec.data.tags import USER, ITEM, ID
-        >>> basepipe = Gowalla_m1("../data")
-        >>> fields = basepipe.fields
+        >>> dataset: RecDataSet
         >>> graph = basepipe.to_graph(
         ...    fields[USER, ID], fields[ITEM, ID],
         ... )
         >>> graph
-        Data(edge_index=[2, 1620256], x=[70839, 0])
+        Data(edge_index=[2, 307552], x=[34464, 0], node_type=[34464], edge_type=[153776])
         """
         from torch_geometric.utils import to_undirected
         graph = self.to_heterograph((src, None, dst)).to_homogeneous()
         graph.edge_index = to_undirected(graph.edge_index)
         return graph
 
     def to_normalized_adj(
@@ -377,358 +645,126 @@
             self.to_graph(src, dst).edge_index, normalization=normalization
         )
         return to_adjacency(
             edge_index, edge_weight,
             num_nodes=User.count + Item.count
         )
 
-
-class RecDataSet(BaseSet):
-    """RecDataSet provides a template for specific datasets."""
-
-    def check_transforms(self) -> None:
-        """Check if the transformations exist."""
-        file_ = os.path.join(
-            self.path,
-            DEFAULT_PICKLE_FMT.format(self.__class__.__name__), 
-            DEFAULT_TRANSFORM_FILENAME
-        )
-        if os.path.isfile(file_):
-            return True
-        else:
-            mkdirs(os.path.join(
-                self.path,
-                DEFAULT_PICKLE_FMT.format(self.__class__.__name__)
-            ))
-            return False
-
-    def save_transforms(self) -> None:
-        """Save transformers in a pickle format."""
-        infoLogger(f"[{self.__class__.__name__}] >>> Save transformers ...")
-        state_dict = self.fields.state_dict()
-        state_dict['trainsize'] = self.trainsize
-        state_dict['validsize'] = self.validsize
-        state_dict['testsize'] = self.testsize
-        file_ = os.path.join(
-            self.path, 
-            DEFAULT_PICKLE_FMT.format(self.__class__.__name__), 
-            DEFAULT_TRANSFORM_FILENAME
-        )
-        export_pickle(state_dict, file_)
-
-    def load_transforms(self) -> None:
-        """Load transformers from a pickle file."""
-        file_ = os.path.join(
-            self.path, 
-            DEFAULT_PICKLE_FMT.format(self.__class__.__name__), 
-            DEFAULT_TRANSFORM_FILENAME
-        )
-        state_dict = import_pickle(file_)
-        self.trainsize = state_dict['trainsize']
-        self.validsize = state_dict['validsize']
-        self.testsize = state_dict['testsize']
-        self.fields.load_state_dict(state_dict, strict=False)
-
-    def check_pickle(self) -> bool:
-        """Check if the dataset has been converted into pickle format."""
-        path = os.path.join(
-            self.path,
-            DEFAULT_PICKLE_FMT.format(self.__class__.__name__), 
-            self.mode
-        )
-        if os.path.exists(path):
-            return any(True for _ in os.scandir(path))
-        else:
-            os.makedirs(path)
-            return False
-
-    def write_pickle(self, data, count: int) -> None:
-        r"""
-        Save pickle format data.
-
-        Parameters:
-        -----------
-        data: Any
-            The data to be saved in pickle format.
-        count: int
-            The count of the data chunks.
-
-        Returns:
-        --------
-        None
-        """
-        file_ = os.path.join(
-            self.path,
-            DEFAULT_PICKLE_FMT.format(self.__class__.__name__),
-            self.mode, DEFAULT_CHUNK_FMT.format(count)
-        )
-        export_pickle(data, file_)
-
-    def read_pickle(self, file_: str):
-        r"""
-        Load pickle format data.
-
-        Parameters:
-        -----------
-        file_: str 
-            The file path to load the pickle format data.
-
-        Returns:
-        --------
-        The loaded pickle format data.
-        """
-        return import_pickle(file_)
-
-    def row_processer(self, row):
-        r"""
-        Process a row of raw data.
-
-        Parameters:
-        -----------
-        row: Any
-            A row of raw data.
-
-        Returns:
-        --------
-        A processed row of data.
-        """
-        return [field.caster(val) for val, field in zip(row, self.fields)]
-
-    def raw2pickle(self):
-        """Convert raw data into pickle format."""
-        infoLogger(f"[{self.__class__.__name__}] >>> Convert raw data ({self.mode}) to chunks in pickle format")
-        datapipe = self.raw2data()
-        count = 0
-        for chunk in datapipe.batch(batch_size=self.DEFAULT_CHUNK_SIZE).column_():
-            for j, field in enumerate(self.fields):
-                chunk[j] = field.transform(chunk[j])
-            self.write_pickle(chunk, count)
-            count += 1
-        infoLogger(f"[{self.__class__.__name__}] >>> {count} chunks done")
-
-    def pickle2data(self):
-        r"""
-        Read the pickle data and return it as a generator.
-
-        Yields:
-        -------
-        A chunk of the pickle data.
-        """
-        datapipe = dp.iter.FileLister(
-            os.path.join(
-                self.path,
-                DEFAULT_PICKLE_FMT.format(self.__class__.__name__),
-                self.mode
-            ),
-            non_deterministic=False # return sorted chunks
-        )
-        for file_ in datapipe:
-            yield self.read_pickle(file_)
-
-    @timemeter
-    def compile(self):
+    @safe_mode('valid', 'test')
+    def ordered_user_ids_source(self):
         r"""
-        Check current dataset and transformations.
-
-        Flows:
-        ------
-        1. Check whether the transformation has been fitted:
-            - `True`: Skip.
-            - `False`: Fit the total trainset and the `SPARSE` fields in valid|testset
-                to avoid unseen features. This operation will not cause information leakage.
-            
-        2. Convert each set into pickle format for fast loading.
-        """
-
-        def fit_transform(*tags):
-            """Function to fit and transform data for pickle conversion."""
-            datapipe = self.raw2data().batch(self.DEFAULT_CHUNK_SIZE).column_()
-            datasize = 0
-            fields = self.fields.groupby(*tags)
-            for chunk in datapipe:
-                datasize += len(chunk[0])
-                for field in fields:
-                    index = self.fields.index(*field.tags)
-                    field.partial_fit(chunk[index])
-            return datasize
-
-        if self.check_transforms():
-            self.load_transforms()
-        else:
-            self.train()
-            self.trainsize = fit_transform()
-
-            # avoid unseen IDs not included in trainset
-            self.valid()
-            self.validsize = fit_transform(SPARSE)
-            self.test()
-            self.testsize = fit_transform(SPARSE)
-
-            self.save_transforms()
-            
-        # raw2pickle
-        self.train()
-        if not self.check_pickle():
-            self.raw2pickle()
-        self.valid()
-        if not self.check_pickle():
-            self.raw2pickle()
-        self.test()
-        if not self.check_pickle():
-            self.raw2pickle()
-        self.train()
+        To ordered User ID source.
 
-        self.summary()
-
-    @property
-    def datasize(self):
-        """Return the size of dataset according to the current mode."""
-        if self.mode == 'train':
-            return self.trainsize
-        elif self.mode == 'valid':
-            return self.validsize
-        else:
-            return self.testsize
+        Examples:
+        ---------
+        >>> dataset: RecDataSet
+        >>> datapipe = dataset.valid().to_ordered_user_ids()
+        >>> len(datapipe) == dataset.fields[USER, ID].count
+        True
+        """
+        from ..postprocessing.source import OrderedSource
+        User = self.fields[USER, ID]
+        source = self.to_rows({User: list(range(User.count))})
+        return OrderedSource(self, source)
 
-    def to_pairs(self, master: Tuple = (USER, ID)) -> List:
+    @safe_mode('train')
+    def choiced_user_ids_source(self):
         r"""
-        Return dataset in pairs.
-
-        Parameters:
-        -----------
-        master: Tuple
-            Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
-        
-        Returns:
-        --------
-        List
-        """
-        Master = self.fields[master]
-        assert Master is not None, f"{Master} is not in fields ..."
-        pairs = []
+        To random choiced User ID source.
+        The datasize equals the current dataset's datasize.
 
-        for chunk in self:
-            pairs.extend(list(zip(chunk[master], chunk[ITEM, ID])))
-        return pairs
+        Examples:
+        ---------
+        >>> dataset: RecDataSet
+        >>> datapipe = dataset.train().to_choiced_user_ids()
+        >>> len(datapipe) == dataset.trainsize
+        True
+        """
+        from ..postprocessing.source import RandomChoicedSource
+        User = self.fields[USER, ID]
+        source = self.to_rows({User: list(range(User.count))})
+        return RandomChoicedSource(self, source)
 
-    def to_seqs(self, master: Tuple = (USER, ID), keepid: bool = False) -> List:
+    @safe_mode('train')
+    def shuffled_pairs_source(self):
         r"""
-        Return dataset in sequence.
+        To random shuffled (User, Item) pairs source.
+        The datasize equals the current dataset's datasize.
 
-        Parameters:
-        -----------
-        master: Tuple
-            Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
-        keepid: bool, default to False
-            `True`: return list of (id, items)
-            `False`: return list of items
-        
-        Returns:
-        --------
-        List
+        Examples:
+        ---------
+        >>> dataset: RecDataSet
+        >>> datapipe = dataset.train().to_shuffled_pairs()
+        >>> len(datapipe) == dataset.trainsize
+        True
+        >>> list(datapipe)[0].keys()
+        dict_keys([Field(USER:ID,USER), Field(ITEM:ID,ITEM)])
         """
-        Master = self.fields[master]
-        assert Master is not None, f"{Master} is not in fields ..."
-        seqs = [[] for id_ in range(Master.count)]
-
-        for chunk in self:
-            list(map(
-                lambda id_, item: seqs[id_].append(item),
-                chunk[master], chunk[ITEM, ID]
-            ))
-
-        if keepid:
-            seqs = [(id_, tuple(items)) for id_, items in enumerate(seqs)]
-        else:
-            seqs = [tuple(items) for items in seqs]
-
-        return seqs
+        from ..postprocessing.source import RandomShuffledSource
+        return RandomShuffledSource(self, self.to_pairs())
 
-    def to_roll_seqs(
-        self, master: Tuple = (USER, ID), 
-        minlen: int = 2, maxlen: Optional[int] = None,
-        keep_at_least_itself: bool = True
-    ) -> List:
+    @safe_mode('train')
+    def shuffled_seqs_source(self, maxlen: Optional[int] = None):
         r"""
-        Rolling dataset in sequence.
+        To random shuffled (User, ISeq) source.
 
         Parameters:
         -----------
-        master: Tuple
-            Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
-        minlen: int
-            Shorest sequence
         maxlen: int, optional
             Maximum length
-            `None`: Roll throughout the whole sequence
-        keep_at_least_itself: bool, default to `True`
-            `True`: Keep the sequence with items less than `minlen`
-       
-        Returns:
-        --------
-        List
-        """
-        seqs = self.to_seqs(master=master, keepid=True)
-
-        roll_seqs = []
-        for id_, items in seqs:
-            if maxlen is not None:
-                items = items[-maxlen:]
-            if len(items) <= minlen and keep_at_least_itself:
-                roll_seqs.append(
-                    (id_, items)
-                )
-                continue
-            for k in range(minlen, len(items) + 1):
-                roll_seqs.append(
-                    (id_, items[:k])
-                )
+            `None`: return the whole sequence
+            `int`: return the recent `maxlen` items
 
-        return roll_seqs
+        Examples:
+        ---------
+        >>> dataset: RecDataSet
+        >>> datapipe = dataset.train().to_shuffled_seqs()
+        >>> len(datapipe) == dataset[USER, ID].count
+        True
+        >>> list(datapipe)[0].keys()
+        dict_keys([Field(USER:ID,USER), Field(ITEM:ID,ITEM,SEQUENCE)])
+        """
+        from ..postprocessing.source import RandomShuffledSource
+        return RandomShuffledSource(self, self.to_seqs(maxlen))
+
+    @safe_mode('train')
+    def shuffled_roll_seqs_source(
+        self, minlen: int = 2, maxlen: Optional[int] = None,
+        keep_at_least_itself: bool = True
+    ):
+        r"""
+        To random shuffled (User, ISeq) rolling source.
 
-    def seqlens(self, master: Tuple = (USER, ID)) -> List:
-        seqs = self.to_seqs(master, keepid=False)
-        return list(filter(lambda x: x > 0, [len(items) for items in seqs]))
+        Examples:
+        ---------
+        >>> dataset: RecDataSet
+        >>> datapipe = dataset.train().to_shuffled_roll_seqs()
+        >>> list(datapipe)[0].keys()
+        dict_keys([Field(USER:ID,USER), Field(ITEM:ID,ITEM,SEQUENCE)])
+        """
+        from ..postprocessing.source import RandomShuffledSource
+        return RandomShuffledSource(
+            self, self.to_roll_seqs(minlen, maxlen, keep_at_least_itself)
+        )
 
-    @lru_cache()
-    def has_duplicates(self, master: Tuple = (USER, ID)) -> bool:
-        r"""
-        Check whether the dataset has repeated interactions.
+    def summary(self):
+        super().summary()
+        from prettytable import PrettyTable
+        User, Item = self.fields[USER, ID], self.fields[ITEM, ID]
 
-        Parameters:
-        -----------
-        master: Tuple
-            Tuple of tags to spefic a field, e.g., (USER, ID), (SESSION, ID)
+        table = PrettyTable(['#Users', '#Items', 'Avg.Len', '#Interactions', '#Train', '#Valid', '#Test', 'Density'])
+        table.add_row([
+            User.count, Item.count, self.train().meanlen + 2,
+            self.trainsize + self.validsize + self.testsize,
+            self.trainsize, self.validsize, self.testsize,
+            (self.trainsize + self.validsize + self.testsize) / (User.count * Item.count)
+        ])
 
-        Returns:
-        --------
-        bool
-        """
-        from itertools import chain
-        train_seqs = self.train().to_seqs(master, keepid=False)
-        valid_seqs = self.valid().to_seqs(master, keepid=False)
-        test_seqs = self.test().to_seqs(master, keepid=False)
-        seqs = map(
-            lambda triple: chain(*triple),
-            zip(train_seqs, valid_seqs, test_seqs)
-        )
-        for seq in seqs:
-            seq = list(seq)
-            if len(seq) != len(set(seq)):
-                return True
-        return False
+        infoLogger(table)
 
-    @property
-    def maxlen(self) -> int:
-        return np.max(self.seqlens()).item()
 
-    @property
-    def minlen(self) -> int:
-        return np.min(self.seqlens()).item()
+class MatchingRecDataSet(RecDataSet):
+    TASK = TaskTags.MATCHING
 
-    @property
-    def meanlen(self) -> int:
-        return np.mean(self.seqlens()).item()
 
-    def __str__(self) -> str:
-        cfg = '\n'.join(map(str, self.fields))
-        return f"[{self.__class__.__name__}] >>> \n" + cfg
+class NextItemRecDataSet(RecDataSet):
+    TASK = TaskTags.NEXTITEM
```

### Comparing `freerec-0.7.5/freerec/data/datasets/sequential/steam.py` & `freerec-0.8.1/freerec/data/datasets/gowalla.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,43 @@
 
 
-from .base import UserItemTimeTriplet
+from .base import MatchingRecDataSet
 
 
-__all__ = [
-    'Steam',
-    'Steam_550_Chron',
-    'Steam_500_Chron'
-]
-
-
-class Steam(UserItemTimeTriplet): ...
-
-
-class Steam_550_Chron(UserItemTimeTriplet):
+class Gowalla2010_10100811_ROU(MatchingRecDataSet):
     r"""
-    Chronologically-ordered MovieLens1M dataset.
-
-    Config:
-    -------
-    filename: steam
-    dataset: Steam
-    kcore4user: 5
-    kcore4item: 5
+    Settings:
+    ---------
+    kcore4user: 10
+    kcore4item: 10
     star4pos: 0
+    ratios: 8,1,1
+    splitting: ROU
 
     Statistics:
     -----------
-    +-------+-------+---------------+--------+--------+-------+----------------------+
-    | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
-    +-------+-------+---------------+--------+--------+-------+----------------------+
-    | 25389 |  4089 |     328278    | 277500 | 25389  | 25389 | 0.003162125283631449 |
-    +-------+-------+---------------+--------+--------+-------+----------------------+
+    +-------+--------+---------------+---------+--------+--------+-----------------------+
+    | #User | #Item  | #Interactions |  #Train | #Valid | #Test  |        Density        |
+    +-------+--------+---------------+---------+--------+--------+-----------------------+
+    | 52985 | 121866 |    3301571    | 2620128 | 326791 | 354652 | 0.0005113110117881469 |
+    +-------+--------+---------------+---------+--------+--------+-----------------------+
     """
-    URL = "https://zenodo.org/record/7866203/files/Steam_550_Chron.zip"
 
 
-class Steam_500_Chron(UserItemTimeTriplet):
+class Gowalla2010_10100712_ROU(MatchingRecDataSet):
     r"""
-    Chronologically-ordered MovieLens1M dataset.
-
-    Config:
-    -------
-    filename: steam
-    dataset: Steam
-    kcore4user: 5
-    kcore4item: 0
+    Settings:
+    ---------
+    kcore4user: 10
+    kcore4item: 10
     star4pos: 0
+    ratios: 7,1,2
+    splitting: ROU
 
     Statistics:
     -----------
-    +-------+-------+---------------+--------+--------+-------+----------------------+
-    | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
-    +-------+-------+---------------+--------+--------+-------+----------------------+
-    | 26247 |  9327 |     341270    | 288776 | 26247  | 26247 | 0.001394043945100003 |
-    +-------+-------+---------------+--------+--------+-------+----------------------+
-    """
-    URL = "https://zenodo.org/record/7866203/files/Steam_500_Chron.zip"
-
+    +-------+--------+---------------+---------+--------+--------+-----------------------+
+    | #User | #Item  | #Interactions |  #Train | #Valid | #Test  |        Density        |
+    +-------+--------+---------------+---------+--------+--------+-----------------------+
+    | 52985 | 121866 |    3301571    | 2287870 | 332258 | 681443 | 0.0005113110117881469 |
+    +-------+--------+---------------+---------+--------+--------+-----------------------+
+    """
```

### Comparing `freerec-0.7.5/freerec/data/datasets/session/yoochoose.py` & `freerec-0.8.1/freerec/data/datasets/amazon2018.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,163 +1,180 @@
 
 
-from .base import SessionItemTimeTriplet
+from .base import NextItemRecDataSet
 
 
-__all__ = [
-    'YooChooseBuys', 'YooChooseClicks',
-    'YooChooseClicks14_250811_Chron', 'YooChooseClicks164_250811_Chron',
-    'YooChooseClicks14_250712_Chron', 'YooChooseClicks164_250712_Chron',
-    'YooChooseClicks14_2501_Chron', 'YooChooseClicks164_2501_Chron'
-]
+#===================================MatchingRecDataSset===================================
 
 
-class YooChooseBuys(SessionItemTimeTriplet):
-    ...
+#===================================NextItemRecDataSset===================================
 
 
-class YooChooseClicks(SessionItemTimeTriplet):
-    ...
+class Amazon2018Books_550_LOU(NextItemRecDataSet):
+    r"""
+    Settings:
+    ---------
+    kcore4user: 5
+    kcore4item: 5
+    star4pos: 0
+    splitting: LOU
 
+    Statistics:
+    -----------
+    +---------+--------+---------------+----------+---------+---------+-----------------------+
+    |  #User  | #Item  | #Interactions |  #Train  |  #Valid |  #Test  |        Density        |
+    +---------+--------+---------------+----------+---------+---------+-----------------------+
+    | 1855553 | 702955 |    27157802   | 23446696 | 1855553 | 1855553 | 2.082062344661726e-05 |
+    +---------+--------+---------------+----------+---------+---------+-----------------------+
+    """
 
-class YooChooseClicks14_250811_Chron(SessionItemTimeTriplet):
-    r"""
-    Chronologically-ordered YooChooseClickss1/4 dataset.
 
-    Config:
-    -------
-    filename: yoochoose-clicks
-    dataset: YooChooseClicks14
-    kcore4user: 2
+class Amazon2018CDs_550_LOU(NextItemRecDataSet):
+    r"""
+    Settings:
+    ---------
+    kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    ratios: (8, 1, 1)
+    splitting: LOU
 
     Statistics:
     -----------
-    +-----------+--------+-------------------+---------------+---------+--------+--------+------------------------+
-    | #Sessions | #Items |      Avg.Len      | #Interactions |  #Train | #Valid | #Test  |        Density         |
-    +-----------+--------+-------------------+---------------+---------+--------+--------+------------------------+
-    |  1995340  | 30576  | 4.090095923501759 |    8161132    | 6524270 | 803053 | 833809 | 0.00013376818169485083 |
-    +-----------+--------+-------------------+---------------+---------+--------+--------+------------------------+
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | #User  | #Item | #Interactions |  #Train | #Valid | #Test  |        Density         |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | 112134 | 73303 |    1441330    | 1217062 | 112134 | 112134 | 0.00017534943175208346 |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
     """
-    URL = "https://zenodo.org/record/8062815/files/YooChooseClicks14_250811_Chron.zip"
 
 
-class YooChooseClicks164_250811_Chron(SessionItemTimeTriplet):
+class Amazon2018Clothing_550_LOU(NextItemRecDataSet):
     r"""
-    Chronologically-ordered YooChooseClickss1/64 dataset.
-
-    Config:
-    -------
-    filename: yoochoose-clicks
-    dataset: YooChooseClicks164
-    kcore4user: 2
+    Settings:
+    ---------
+    kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    ratios: (8, 1, 1)
+    splitting: LOU
 
     Statistics:
     -----------
-    +-----------+--------+-------------------+---------------+--------+--------+-------+------------------------+
-    | #Sessions | #Items |      Avg.Len      | #Interactions | #Train | #Valid | #Test |        Density         |
-    +-----------+--------+-------------------+---------------+--------+--------+-------+------------------------+
-    |   124709  | 17567  | 4.243655229373982 |     529222    | 411917 | 57912  | 59393 | 0.00024156971761678047 |
-    +-----------+--------+-------------------+---------------+--------+--------+-------+------------------------+
+    +---------+--------+---------------+---------+---------+---------+------------------------+
+    |  #User  | #Item  | #Interactions |  #Train |  #Valid |  #Test  |        Density         |
+    +---------+--------+---------------+---------+---------+---------+------------------------+
+    | 1219337 | 376378 |    11282445   | 8843771 | 1219337 | 1219337 | 2.4584152571414375e-05 |
+    +---------+--------+---------------+---------+---------+---------+------------------------+
     """
-    URL = "https://zenodo.org/record/8062815/files/YooChooseClicks164_250811_Chron.zip"
 
 
-class YooChooseClicks14_250712_Chron(SessionItemTimeTriplet):
+class Amazon2018Electronics_550_LOU(NextItemRecDataSet):
     r"""
-    Chronologically-ordered YooChooseClickss1/4 dataset.
-
-    Config:
-    -------
-    filename: yoochoose-clicks
-    dataset: YooChooseClicks14
-    kcore4user: 2
+    Settings:
+    ---------
+    kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    ratios: (7, 1, 2)
+    splitting: LOU
 
     Statistics:
     -----------
-    +-----------+--------+-------------------+---------------+---------+--------+---------+------------------------+
-    | #Sessions | #Items |      Avg.Len      | #Interactions |  #Train | #Valid |  #Test  |        Density         |
-    +-----------+--------+-------------------+---------------+---------+--------+---------+------------------------+
-    |  1995340  | 30576  | 4.090095923501759 |    8161132    | 5722495 | 801775 | 1636862 | 0.00013376818169485083 |
-    +-----------+--------+-------------------+---------------+---------+--------+---------+------------------------+
+    +--------+--------+---------------+---------+--------+--------+-----------------------+
+    | #User  | #Item  | #Interactions |  #Train | #Valid | #Test  |        Density        |
+    +--------+--------+---------------+---------+--------+--------+-----------------------+
+    | 728489 | 159729 |    6737580    | 5280602 | 728489 | 728489 | 5.790247980421062e-05 |
+    +--------+--------+---------------+---------+--------+--------+-----------------------+
     """
-    URL = "https://zenodo.org/record/8062815/files/YooChooseClicks14_250712_Chron.zip"
 
 
-class YooChooseClicks164_250712_Chron(SessionItemTimeTriplet):
+class Amazon2018Movies_550_LOU(NextItemRecDataSet):
     r"""
-    Chronologically-ordered YooChooseClickss1/64 dataset.
-
-    Config:
-    -------
-    filename: yoochoose-clicks
-    dataset: YooChooseClicks164
-    kcore4user: 2
+    Settings:
+    ---------
+    kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    ratios: (7, 1, 2)
+    splitting: LOU
 
     Statistics:
     -----------
-    +-----------+--------+-------------------+---------------+--------+--------+--------+------------------------+
-    | #Sessions | #Items |      Avg.Len      | #Interactions | #Train | #Valid | #Test  |        Density         |
-    +-----------+--------+-------------------+---------------+--------+--------+--------+------------------------+
-    |   124709  | 17567  | 4.243655229373982 |     529222    | 350663 | 61254  | 117305 | 0.00024156971761678047 |
-    +-----------+--------+-------------------+---------------+--------+--------+--------+------------------------+
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | #User  | #Item | #Interactions |  #Train | #Valid | #Test  |        Density         |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | 297377 | 59925 |    3408612    | 2813858 | 297377 | 297377 | 0.00019127673500988237 |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
     """
-    URL = "https://zenodo.org/record/8062815/files/YooChooseClicks164_250712_Chron.zip"
 
 
-class YooChooseClicks14_2501_Chron(SessionItemTimeTriplet):
+class Amazon2018Office_550_LOU(NextItemRecDataSet):
     r"""
-    Chronologically-ordered YooChooseClickss1/4 dataset.
-
-    Config:
-    -------
-    filename: yoochoose-clicks
-    dataset: YooChooseClicks14
-    kcore4user: 2
+    Settings:
+    ---------
+    kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    days: 1
+    splitting: LOU
 
     Statistics:
     -----------
-    +-----------+--------+-------------------+---------------+---------+--------+-------+------------------------+
-    | #Sessions | #Items |      Avg.Len      | #Interactions |  #Train | #Valid | #Test |        Density         |
-    +-----------+--------+-------------------+---------------+---------+--------+-------+------------------------+
-    |  1995340  | 30576  | 4.090095923501759 |    8161132    | 8031636 | 58233  | 71263 | 0.00013376818169485083 |
-    +-----------+--------+-------------------+---------------+---------+--------+-------+------------------------+
+    +--------+-------+---------------+--------+--------+--------+------------------------+
+    | #User  | #Item | #Interactions | #Train | #Valid | #Test  |        Density         |
+    +--------+-------+---------------+--------+--------+--------+------------------------+
+    | 101133 | 27500 |     797563    | 595297 | 101133 | 101133 | 0.00028677376236333255 |
+    +--------+-------+---------------+--------+--------+--------+------------------------+
     """
-    URL = "https://zenodo.org/record/8062815/files/YooChooseClicks14_2501_Chron.zip"
 
 
-class YooChooseClicks164_2501_Chron(SessionItemTimeTriplet):
+class Amazon2018Sports_550_LOU(NextItemRecDataSet):
     r"""
-    Chronologically-ordered YooChooseClickss1/64 dataset.
+    Settings:
+    ---------
+    kcore4user: 5
+    kcore4item: 5
+    star4pos: 0
+    splitting: LOU
 
-    Config:
-    -------
-    filename: yoochoose-clicks
-    dataset: YooChooseClicks164
-    kcore4user: 2
+    Statistics:
+    -----------
+    +--------+--------+---------------+---------+--------+--------+-----------------------+
+    | #User  | #Item  | #Interactions |  #Train | #Valid | #Test  |        Density        |
+    +--------+--------+---------------+---------+--------+--------+-----------------------+
+    | 331844 | 103911 |    2835125    | 2171437 | 331844 | 331844 | 8.221985709448659e-05 |
+    +--------+--------+---------------+---------+--------+--------+-----------------------+
+    """
+
+
+class Amazon2018Tools_550_LOU(NextItemRecDataSet):
+    r"""
+    Settings:
+    ---------
+    kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    days: 1
+    splitting: LOU
 
     Statistics:
     -----------
-    +-----------+--------+-------------------+---------------+--------+--------+-------+------------------------+
-    | #Sessions | #Items |      Avg.Len      | #Interactions | #Train | #Valid | #Test |        Density         |
-    +-----------+--------+-------------------+---------------+--------+--------+-------+------------------------+
-    |   124709  | 17567  | 4.243655229373982 |     529222    | 399726 | 58233  | 71263 | 0.00024156971761678047 |
-    +-----------+--------+-------------------+---------------+--------+--------+-------+------------------------+
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | #User  | #Item | #Interactions |  #Train | #Valid | #Test  |        Density         |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | 240464 | 73153 |    2067876    | 1586948 | 240464 | 240464 | 0.00011755531903149089 |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
     """
-    URL = "https://zenodo.org/record/8062815/files/YooChooseClicks164_2501_Chron.zip"
+
+
+class Amazon2018Toys_550_LOU(NextItemRecDataSet):
+    r"""
+    Settings:
+    ---------
+    kcore4user: 5
+    kcore4item: 5
+    star4pos: 0
+    splitting: LOU
+
+    Statistics:
+    -----------
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | #User  | #Item | #Interactions |  #Train | #Valid | #Test  |        Density         |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    | 207725 | 78098 |    1825066    | 1409616 | 207725 | 207725 | 0.00011249931928815434 |
+    +--------+-------+---------------+---------+--------+--------+------------------------+
+    """
```

### Comparing `freerec-0.7.5/freerec/data/preprocessing/base.py` & `freerec-0.8.1/freerec/launcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,849 +1,1000 @@
 
 
-from typing import Tuple, Iterable, Optional, Union, Mapping
+from typing import Any, Literal, Callable, Iterable, List, Dict, Optional, Tuple
 
-import os, random
-import numpy as np
-import pandas as pd
-from math import floor, ceil
-
-from ..tags import USER, SESSION, ITEM, RATING, TIMESTAMP
-
-from ...utils import infoLogger, warnLogger, mkdirs
-
-
-__all__ = ['AtomicConverter']
-
-
-NAME_FORMAT_DICT = {
-    'user_id': USER.name,
-    'session_id': SESSION.name,
-    'item_id': ITEM.name,
-    'venue_id': ITEM.name, # FourSquare
-    'rating': RATING.name,
-    'timestamp': TIMESTAMP.name
+import torch, abc, os, time, sys, signal
+from torch.utils.tensorboard import SummaryWriter
+from functools import partial
+from itertools import product
+from collections import defaultdict
+
+from .data.datasets import RecDataSet
+from .data.postprocessing import PostProcessor
+from .data.fields import Field, FieldTuple
+from .data.tags import USER, ITEM, ID, UNSEEN, SEEN
+from .models import RecSysArch
+from .dict2obj import Config
+from .utils import AverageMeter, Monitor, timemeter, infoLogger, import_pickle, export_pickle
+from .metrics import *
+from .parser import TIME, Parser
+from .ddp import is_main_process, main_process_only, is_distributed, synchronize
+
+
+__all__ = [
+    'ChiefCoach', 'Coach', 'Adapter'
+]
+
+
+DEFAULT_METRICS = {
+    'LOSS': lambda x: x,
+    #############
+    'MSE': mean_squared_error,
+    'MAE': mean_abs_error,
+    'RMSE': root_mse,
+    #############
+    'PRECISION': precision,
+    'RECALL': recall,
+    'F1': f1_score,
+    'AUC': auroc,
+    'HITRATE': hit_rate,
+    #############
+    'NDCG': normalized_dcg,
+    'MRR': mean_reciprocal_rank,
+    'MAP': mean_average_precision
 }
 
+DEFAULT_FMTS = {
+    'LOSS': ".5f",
+    #############
+    'MSE': ".4f",
+    'MAE': ".4f",
+    'RMSE': ".4f",
+    #############
+    'PRECISION': ".4f",
+    'RECALL': ".4f",
+    'F1': ".4f",
+    'AUC': ".4f",
+    'HITRATE': ".4f",
+    #############
+    'NDCG': ".4f",
+    'MRR': ".4f",
+    'MAP': ".4f",
+}
 
-TYPE_FORMAT_DICT = {
-    'token': str,
-    'token_seq': str,
-    'float': float,
-    # 'float_seq': None
+DEFAULT_BEST_CASTER = {
+    'LOSS': min,
+    #############
+    'MSE': min,
+    'MAE': min,
+    'RMSE': min,
+    #############
+    'PRECISION': max,
+    'RECALL': max,
+    'F1': max,
+    'AUC': max,
+    'HITRATE': max,
+    #############
+    'NDCG': max,
+    'MRR': max,
+    'MAP': max,
 }
 
 
-class AtomicConverter:
-    r"""
-    How to convert Atomic files into train|valid|test.txt ?
-
-    Flows:
-    ------
-    1. Download corresponding files from [[RecBole](https://drive.google.com/drive/folders/1so0lckI6N6_niVEYaBu-LIcpOdZf99kj)].
-    2. Import corresponding dataset.
-    3. Call `make_xxx_dataset'.
+class _DummyModule(torch.nn.Module):
+    """This is a dummy module that serves as a placeholder for a real model."""
+    def forward(self, *args, **kwargs):
+        """Dummy forward method that raises a `NotImplementedError`."""
+        raise NotImplementedError("No model available for Coach ...")
+
+    def step(self, *args, **kwargs):
+        """Dummy step method that raises a `NotImplementedError`."""
+        raise NotImplementedError("No optimizer or lr scheduler available for Coach ...")
+
+    def backward(self, *args, **kwargs):
+        """Dummy backward method that raises a `NotImplementedError`."""
+        raise NotImplementedError("No optimizer available for Coach ...")
+
+
+class ChiefCoach(metaclass=abc.ABCMeta):
+    r""" 
+    The `ChiefCoach` class is the top-level class for running the training and evaluation loops.
 
     Parameters:
     -----------
-    root: str
-        The root of data.
-    filename: str
-        The file with Atomic files.
-        - `None': Use cls.filename instead.
-    dataset: str, optional
-        The filename saving dataset.
-        - `None': Use classname instead.
-
-    Notes:
-    ------
-    1. Most of datasets in RecBole have two versions: 
-        merged: remove duplicate interactions.
-        not_merged: not remove duplicate interactions.
+    dataset: RecDataSet,
+        The original dataset.
+    trainpipe : IterDataPipe
+        Iterable data pipeline for training data.
+    validpipe : IterDataPipe, optional
+        Iterable data pipeline for validation data.
+    testpipe : IterDataPipe, optional
+        Iterable data pipeline for testing data.
+        If `None`, use `validpipe` instead.
+    model : RecSysArch
+        Model for training and evaluating. 
+    cfg: Parser
+        Configuration file.
     """
-    filename: str
-
-    _name_format_dict = dict()
-    _type_format_dict = dict()
 
     def __init__(
-        self, root: str, 
-        filename: Optional[str] = None,
-        dataset: Optional[str] = None
-    ) -> None:
-        super().__init__()
+        self, *,
+        dataset: RecDataSet,
+        trainpipe: PostProcessor, validpipe: PostProcessor, testpipe: Optional[PostProcessor], 
+        model: RecSysArch, cfg: Parser
+    ):
+
+        self.cfg = cfg
+        self.__mode = 'train'
+
+        self.set_device(self.cfg.device)
+        self.set_dataset(dataset)
+        self.set_datapipe(
+            trainpipe, validpipe, testpipe
+        )
+        self.set_dataloader()
+
+        self.set_model(model)
+        self.set_optimizer()
+        self.set_lr_scheduler()
+        self.reset_monitors(self.cfg.monitors, self.cfg.which4best)
+
+        # Other setup can be placed here
+        self.set_other()
+
+    def set_device(self, device):
+        self.device = torch.device(device)
+
+    def set_dataset(self, dataset: RecDataSet):
+        self.dataset = dataset
+        self.fields: FieldTuple[Field] = FieldTuple(dataset.fields)
+        self.User = self.fields[USER, ID]
+        self.Item = self.fields[ITEM, ID]
+        self.ISeen = self.Item.fork(SEEN)
+        self.IUnseen = self.Item.fork(UNSEEN)
+
+    def set_datapipe(
+        self,
+        trainpipe,
+        validpipe,
+        testpipe=None,
+    ):
+        self.trainpipe = trainpipe
+        self.validpipe = validpipe
+        self.testpipe = self.validpipe if testpipe is None else testpipe
+
+    def set_model(
+        self, model: RecSysArch
+    ):
+        self.model = model.to(self.device)
+        if is_distributed():
+            self.model = torch.nn.parallel.DistributedDataParallel(model)
+    
+    def set_optimizer(self):
+        if self.cfg.optimizer.lower() == 'sgd':
+            self.optimizer = torch.optim.SGD(
+                self.model.parameters(), lr=self.cfg.lr, 
+                momentum=self.cfg.momentum,
+                nesterov=self.cfg.nesterov,
+                weight_decay=self.cfg.weight_decay
+            )
+        elif self.cfg.optimizer.lower() == 'adam':
+            self.optimizer = torch.optim.Adam(
+                self.model.parameters(), lr=self.cfg.lr,
+                betas=(self.cfg.beta1, self.cfg.beta2),
+                weight_decay=self.cfg.weight_decay
+            )
+        elif self.cfg.optimizer.lower() == 'adamw':
+            self.optimizer = torch.optim.AdamW(
+                self.model.parameters(), lr=self.cfg.lr,
+                betas=(self.cfg.beta1, self.cfg.beta2),
+                weight_decay=self.cfg.weight_decay
+            )
+        else:
+            raise NotImplementedError(
+                f"Unexpected optimizer {self.cfg.optimizer} ..."
+            )
+
+    def set_lr_scheduler(self):
+        self.lr_scheduler = _DummyModule()
+
+    def set_dataloader(self) -> None:
+        from torchdata.dataloader2 import (
+            DataLoader2, 
+            MultiProcessingReadingService, DistributedReadingService, 
+            SequentialReadingService
+        )
 
-        filename = filename if filename else self.filename
-        self.path = os.path.join(root, filename)
-        if not os.path.exists(self.path) or not any(True for _ in os.scandir(self.path)):
-            raise FileNotFoundError(f"No such file of {self.path}, or this dir is empty ...")
-
-        self.root = root
-        self.dataset = dataset if dataset else self.__class__.__name__
-
-        for key, val in NAME_FORMAT_DICT.items():
-            if self._name_format_dict.get(key, None) is None:
-                self._name_format_dict[key] = val
-        for key, val in TYPE_FORMAT_DICT.items():
-            if self._type_format_dict.get(key, None) is None:
-                self._type_format_dict[key] = val
-
-    def convert_by_column(self, df: pd.DataFrame):
-        old_columns = df.columns
-        new_columns = []
-
-        for col in old_columns:
-            col_ = col.lower()
-            name_, type_ = col_.split(":")
-            name_ =  self._name_format_dict.get(name_, name_.capitalize())
-            type_ = self._type_format_dict[type_]
-            try:
-                df[col] = df[col].astype(type_)
-            except ValueError as e:
-                warnLogger(
-                    f"`{type_}' cannot address field `{col}': \n"
-                    f"\t {e} \n"
-                    f"Skip it ..."
+        def get_reading_servie():
+            if is_distributed():
+                rs = SequentialReadingService(
+                    DistributedReadingService(),
+                    MultiProcessingReadingService(self.cfg.num_workers)
                 )
-            new_columns.append(name_)
+            else:
+                rs = MultiProcessingReadingService(self.cfg.num_workers)
+            return rs
+
+        self.trainloader = DataLoader2(
+            datapipe=self.trainpipe, 
+            reading_service=get_reading_servie()
+        )
+        self.validloader = DataLoader2(
+            datapipe=self.validpipe, 
+            reading_service=get_reading_servie()
+        )
+        self.testloader = DataLoader2(
+            datapipe=self.testpipe, 
+            reading_service=get_reading_servie()
+        )
+
+    def set_other(self):
+        ...
+    
+    def get_res_sys_arch(self) -> RecSysArch:
+        model = self.model
+        if isinstance(self.model, torch.nn.parallel.DataParallel):
+            model = self.model.module
+        elif isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
+            model = self.model.module
+        assert isinstance(model, RecSysArch), "No RecSysArch found ..."
+        return model
+
+    @property
+    def fields(self) -> FieldTuple[Field]:
+        return self.__fields
+
+    @fields.setter
+    def fields(self, fields):
+        self.__fields = FieldTuple(fields)
+
+    @property
+    def mode(self):
+        """Get the current mode of the chief coach."""
+        return self.__mode
+
+    @timemeter
+    def train(self, epoch: int):
+        """Start training and return the training loss."""
+        self.__mode = 'train'
+        self.model.train()
+        self.dataloader.seed(epoch)
+        return self.train_per_epoch(epoch)
+
+    @timemeter
+    @torch.no_grad()
+    def valid(self, epoch: int):
+        """Start validation and return the validation metrics."""
+        self.__mode = 'valid'
+        self.model.eval()
+        return self.evaluate(epoch=epoch, mode='valid')
+
+    @timemeter
+    @torch.no_grad()
+    def test(self, epoch: int):
+        """Start testing and return the test metrics."""
+        self.__mode = 'test'
+        self.model.eval()
+        return self.evaluate(epoch=epoch, mode='test')
+
+    @property
+    def dataloader(self):
+        if self.mode == 'train':
+            return self.trainloader
+        elif self.mode == 'valid':
+            return self.validloader
+        else:
+            return self.testloader
+
+    def shutdown(self):
+        self.trainloader.shutdown()
+        self.validloader.shutdown()
+        self.testloader.shutdown()
+
+    @abc.abstractmethod
+    def train_per_epoch(self, epoch: int):
+        raise NotImplementedError(
+            f"{self.__class__.__name__}.train_per_epoch() should be implemented ..."
+        )
+
+    @abc.abstractmethod
+    def evaluate(self, epoch: int, mode: str = 'valid'):
+        raise NotImplementedError(
+            f"{self.__class__.__name__}.evaluate() should be implemented ..."
+        )
+
+    def register_metric(
+        self, name: str, func: Callable, 
+        fmt: str = '.4f', best_caster: Callable = max
+    ) -> None:
+        r"""
+        Register a metric.
+
+        Parameters
+        ----------
+        name : str
+            The complete name of the metric, such as `LOSS2`.
+            The notation `@` should not be included, i.e., 'LOSS@2' is invalid.
+        func : Callable
+            The function to process the data for the metric.
+        fmt : str, optional
+            The format to use when printing the metric, defaults to `'.4f'`.
+        best_caster : Callable, optional
+            A function used to cast the best value of the metric, defaults to `max`.
+            
+        Returns
+        -------
+        None
         
-        df.columns = new_columns
-        return df
+        Raises
+        ------
+        AssertionError
+            When `name` has already been registered or contains the notation `@`.
+        """
 
-    def load_inter_file(self):
-        for file_ in os.scandir(self.path):
-            filename = file_.name
-            if not filename.endswith('.inter'):
-                continue
-            file_ = os.path.join(self.path, filename)
-            df = pd.read_csv(file_, delimiter='\t')
-            infoLogger(f"[Converter] >>> Load `{filename}' ...")
-            return self.convert_by_column(df)
-        infoLogger(f"[Converter] >>> No file ends with `.inter' ...")
-
-    def load_user_file(self):
-        for file_ in os.scandir(self.path):
-            filename = file_.name
-            if not filename.endswith('.user'):
-                continue
-            file_ = os.path.join(self.path, filename)
-            df = pd.read_csv(file_, delimiter='\t')
-            infoLogger(f"[Converter] >>> Load `{filename}' ...")
-            return self.convert_by_column(df)
-        infoLogger(f"[Converter] >>> No file ends with `.user' ...")
-
-    def load_item_file(self):
-        for file_ in os.scandir(self.path):
-            filename = file_.name
-            if not filename.endswith('.item'):
-                continue
-            file_ = os.path.join(self.path, filename)
-            df = pd.read_csv(file_, delimiter='\t')
-            infoLogger(f"[Converter] >>> Load `{filename}' ...")
-            return self.convert_by_column(df)
-        infoLogger(f"[Converter] >>> No file ends with `.item' ...")
-
-    def load_kg_file(self):
-        raise NotImplementedError()
-
-    def load_link_file(self):
-        raise NotImplementedError()
-
-    def load_net_file(self):
-        raise NotImplementedError()
-
-    def load(self):
-        self.interactions = self.load_inter_file()
-        self.userFeats = self.load_user_file()
-        self.itemFeats = self.load_item_file()
-        self.pools = (self.interactions, self.userFeats, self.itemFeats)
-
-    def reserve(self, columns: Iterable[str]):
-        all_columns = self.interactions.columns
-        columns_ = set(columns) & set(all_columns)
-        columns = sorted(columns_, key=columns.index)
-        infoLogger(f"[Converter] >>> Reserve fields: {columns} ...")
-        self.interactions = self.interactions[columns]
-
-    def exclude(self, columns: Iterable[str]):
-        all_columns = self.interactions.columns
-        columns = set(all_columns) - set(columns)
-        columns = sorted(columns, key=all_columns.index)
-        infoLogger(f"[Converter] >>> Exclude fields: {columns} ...")
-        self.interactions = self.interactions[columns]
-
-    def reorder(self, columns: Iterable[str] = (USER.name, ITEM.name)):
-        all_columns = self.interactions.columns
-        columns = columns + all_columns
-        columns_ = set(columns) & set(all_columns)
-        columns = sorted(columns_, key=columns.index)
-        infoLogger(f"[Converter] >>> Reorder fields: {columns} ...")
-        self.interactions = self.interactions[columns]
-
-    def map_col(
-        self, col: str, mapper: Mapping, 
-        pools: Optional[Iterable[pd.DataFrame]] = None
-    ):
-        pools = self.pools if pools is None else pools
-        for df in pools:
-            if df is not None:
-                df[col] = df[col].map(mapper)
-
-    def filter_by_rating(
-        self, 
-        low: Union[None, int, float] = None, 
-        high: Union[None, int, float] = None
+        name = name.upper()
+        assert DEFAULT_METRICS.get(name, None) is None, f"The metric {name} already exists ..."
+        assert '@' not in name, f"The metric name has invalid notation of `@' ..."
+        DEFAULT_METRICS[name] = func
+        DEFAULT_FMTS[name] = fmt
+        DEFAULT_BEST_CASTER[name] = best_caster
+
+        for mode in ('train', 'valid', 'test'):
+            self._set_monitor(
+                name=name,
+                lastname=name,
+                mode=mode
+            )
+
+    def _set_monitor(
+        self, name: str, lastname: str, mode: str = 'train', **kwargs
     ):
+        """Add a monitor for the specified metric."""
         try:
-            df = self.interactions
-            ratings = df[RATING.name]
-            low = low if low is not None else ratings.min()
-            high = high if high is not None else ratings.max()
-            self.interactions = df[(low <= ratings) & (ratings <= high)]
-            infoLogger(f"[Converter] >>> Filter dataframe according to {RATING.name} ...")
+            meter = AverageMeter(
+                    name=name,
+                    metric=partial(DEFAULT_METRICS[lastname], **kwargs),
+                    fmt=DEFAULT_FMTS[lastname],
+                    best_caster=DEFAULT_BEST_CASTER[lastname]
+                )
+            self.__monitors[mode][lastname].append(meter)
         except KeyError:
-            infoLogger(
-                f"[Converter] >>> Skip `filter_by_rating` because of `inter` has no field of `{RATING.name}' ..."
+            raise KeyError(
+                f"The metric of {lastname} is not included. "
+                f"You can register by calling `register_metric(...)' ..."
             )
-    
-    def filter_by_core(
-        self,
-        low4user: Union[None, int, float] = None, 
-        high4user: Union[None, int, float] = None,
-        low4item: Union[None, int, float] = None, 
-        high4item: Union[None, int, float] = None,
-        master: str = USER.name,
-        strict: bool = True
+        return meter
+
+    @property
+    def monitors(self) -> Monitor:
+        """Return the monitor dictionary for the different modes ('train', 'valid', 'test')."""
+        return self.__monitors
+
+    def reset_monitors(
+        self, monitors: List[str], which4best: str = 'LOSS'
     ):
         r"""
-        Filter (user, item) by k-core settings.
+        Set up monitors for training.
+
+        Parameters
+        ----------
+        monitors : List[str]
+            A list of metric names to be monitored during training.
+        which4best : str, defaults `LOSS'
+            The metric used for selecting the best checkpoint.
+
+        Examples
+        --------
+        >>> coach: Coach
+        >>> coach.compile(monitors=['loss', 'recall@10', 'recall@20', 'ndcg@10', 'ndcg@20'])
+        """
+        assert isinstance(monitors, List), f"'monitors' should be a list but {type(monitors)} received ..."
+        assert isinstance(which4best, str), f"'which4best' should be a str but {type(which4best)} received ..."
+
+        # meters for train|valid|test
+        self.__monitors = Monitor()
+        self.__monitors['train'] = defaultdict(list)
+        self.__monitors['valid'] = defaultdict(list)
+        self.__monitors['test'] = defaultdict(list)
+
+        # UPPER
+        which4best = which4best.upper()
+        monitors = ['LOSS'] + [name.upper() for name in monitors] + [which4best]
+        monitors = sorted(set(monitors), key=monitors.index)
+
+        for name in monitors:
+            for mode in ('train', 'valid', 'test'):
+                if '@' in name:
+                    lastname, K = name.split('@')
+                    meter = self._set_monitor(
+                        name=name,
+                        lastname=lastname,
+                        mode=mode,
+                        k=int(K)
+                    )
+                else:
+                    lastname = name
+                    meter = self._set_monitor(
+                        name=name,
+                        lastname=lastname,
+                        mode=mode
+                    )
+                if mode == 'valid' and name == which4best:
+                    self.meter4best = meter
+                    self._best = -float('inf') if meter.caster is max else float('inf')
+                    self._best_epoch = 0
+
+
+class Coach(ChiefCoach):
+
+
+    @property
+    def meter4best(self):
+        return self.__best_meter
+
+    @meter4best.setter
+    def meter4best(self, meter: AverageMeter):
+        self.__best_meter = meter
+        infoLogger(f"[Coach] >>> Set best meter: {meter.name} ")
+
+    @property
+    def remove_seen(self):
+        # remove seen if
+        # 1) retain_seen is not activated and
+        # 2) dataset has no duplicates
+        return not (self.cfg.retain_seen or self.dataset.has_duplicates())
+
+    def save(self, filename: Optional[str] = None) -> None:
+        r"""
+        Save the model to `LOG_PATH` with a given filename.
 
         Parameters:
         -----------
-        low4user: int, float, optional
-            Minimum core for user.
-            - `None`: float('-inf')
-        max4user: int, float, optional
-            Maximum core for user.
-            - `None`: float('inf')
-        low4item: int, float, optional
-            Minimum core for item.
-            - `None`: float('-inf')
-        max4item: int, float, optional
-            Maximum core for item.
-            - `None`: float('inf')
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        """
-        low4user = low4user if low4user else float('-inf')
-        high4user = high4user if high4user else float('inf')
-        low4item = low4item if low4item else float('-inf')
-        high4item = high4item if high4item else float('inf')
-        df = self.interactions
-        dsz = -1
-        infoLogger(
-            f"[Converter] >>> Filter dataframe: "
-            f"{master} in [{low4user}, {high4user}]; "
-            f"Item in [{low4item}, {high4item}] ..."
-        )
-        infoLogger(f"[Converter] >>> Current datasize: {len(df)} ...")
-        while dsz != len(df):
-            dsz = len(df)
-
-            # filter by user
-            users = df[master]
-            counts = users.value_counts()
-            bool_indices = users.isin(
-                counts[(low4user <= counts) & (counts <= high4user)].index
-            )
-            df = df[bool_indices]
+        filename: str, optional
+            `None`: Use `SAVED_FILENAME`
+        """
+        if is_main_process():
+            filename = self.cfg.SAVED_FILENAME if filename is None else filename
+            torch.save(self.model.state_dict(), os.path.join(self.cfg.LOG_PATH, filename))
 
-            # filter by item
-            items = df[ITEM.name]
-            counts = items.value_counts()
-            bool_indices = items.isin(
-                counts[(low4item <= counts) & (counts <= high4item)].index
-            )
-            df = df[bool_indices]
+        synchronize()
+        return 
 
-            infoLogger(f"[Converter] >>> Current datasize: {len(df)}")
+    def load(self, path: str, filename: Optional[str] = None) -> None:
+        filename = self.cfg.SAVED_FILENAME if filename is None else filename
+        self.model.load_state_dict(
+            torch.load(os.path.join(path, filename), map_location=self.device)
+        )
 
-            if not strict:
-                break
+        synchronize()
+        return
 
-        self.interactions = df
+    def save_checkpoint(self, epoch: int) -> None:
+        r"""
+        Save current checkpoint at epoch.
 
-    def user2token(self, master: str = USER.name):
-        infoLogger(f"[Converter] >>> Map user ID to Token ...")
-        user_ids = sorted(self.interactions[master].unique().tolist())
-        self.userCount = len(user_ids)
+        Parameters:
+        -----------
+            epoch :int Current epoch number.
 
-        user_tokens = list(range(len(user_ids)))
-        self.userMaps = dict(
-            zip(user_ids, user_tokens)
-        )
+        Returns:
+        --------
+            None
+        """
+        path = os.path.join(self.cfg.CHECKPOINT_PATH, self.cfg.CHECKPOINT_FILENAME)
+        checkpoint = dict()
+        checkpoint['epoch'] = epoch
+        for module in self.cfg.CHECKPOINT_MODULES:
+            checkpoint[module] = getattr(self, module).state_dict()
+        checkpoint['monitors'] = self.monitors.state_dict()
+        torch.save(checkpoint, path)
 
-        if self.userFeats is not None:
-            self.userFeats = self.userFeats[self.userFeats[master].isin(user_ids)]
-            self.userFeats = self.userFeats.sort_values([master])
-
-        self.map_col(
-            master, self.userMaps, 
-            pools=(self.interactions, self.userFeats)
-        )
+        synchronize()
+        return
 
-    def item2token(self):
-        infoLogger(f"[Converter] >>> Map item ID to Token ...")
-        item_ids = sorted(self.interactions[ITEM.name].unique().tolist())
-        self.itemCount = len(item_ids)
-
-        item_tokens = range(len(item_ids))
-        self.itemMaps = dict(
-            zip(item_ids, item_tokens)
-        )
+    def load_checkpoint(self) -> int:
+        r"""
+        Load last saved checkpoint.
 
-        if self.itemFeats is not None:
-            self.itemFeats = self.itemFeats[self.itemFeats[ITEM.name].isin(item_ids)]
-            self.itemFeats = self.itemFeats.sort_values([ITEM.name])
-
-        self.map_col(
-            ITEM.name, self.itemMaps, 
-            pools=(self.interactions, self.itemFeats)
-        )
+        Returns:
+        --------
+        epoch: int 
+            The epoch number loaded from the checkpoint.
+        """
+        path = os.path.join(self.cfg.CHECKPOINT_PATH, self.cfg.CHECKPOINT_FILENAME)
+        checkpoint = torch.load(path)
+        for module in self.cfg.CHECKPOINT_MODULES:
+            getattr(self, module).load_state_dict(checkpoint[module])
+        self.monitors.load_state_dict(checkpoint['monitors'])
+
+        synchronize()
+        return checkpoint['epoch']
+
+    def save_best(self) -> None:
+        self.save(self.cfg.BEST_FILENAME)
+
+    def load_best(self) -> None:
+        infoLogger(f"[Coach] >>> Load best model @Epoch {self._best_epoch:<4d} ")
+        self.model.load_state_dict(torch.load(os.path.join(self.cfg.LOG_PATH, self.cfg.BEST_FILENAME)))
+
+        synchronize()
+        return
+
+    def check_best(self, epoch: int) -> None:
+        """Update best value."""
+        if self.meter4best.active:
+            best_ = self.meter4best.which_is_better(self._best)
+            if best_ != self._best:
+                self._best = best_
+                self._best_epoch = epoch
+                infoLogger(f"[Coach] >>> Better ***{self.meter4best.name}*** of ***{self._best:.4f}*** ")
+                self.save_best()
 
-    def sort_by_timestamp(self, master: str = USER.name):
-        df = self.interactions
+    def eval_at_best(self):
         try:
-            df = df.sort_values(by=[master, TIMESTAMP.name])
-            infoLogger(f"[Converter] >>> Sort by [{master}] [{TIMESTAMP.name}] ...")
-        except KeyError:
-            df = df.sort_values(by=[master])
-            infoLogger(f"[Converter] >>> Sort by [{master}] ...")
-        finally:
-            self.interactions = df
+            self.load_best()
+            self.valid(self._best_epoch)
+            self.test(self._best_epoch)
+            self.step(self._best_epoch)
+            self.load(self.cfg.LOG_PATH, self.cfg.SAVED_FILENAME)
+        except FileNotFoundError:
+            infoLogger(f"[Coach] >>> No best model was recorded. Skip it ...")
 
-    def gen_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
-        infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
-        traingroups = []
-        validgroups = []
-        testgroups = []
-        markers = np.cumsum(ratios)
-        for _, group in self.interactions.groupby(USER.name):
-            if len(group) == 0:
-                continue
-            l = max(floor(markers[0] * len(group) / markers[-1]), 1)
-            r = floor(markers[1] * len(group) / markers[-1])
-            traingroups.append(group[:l])
-            if l < r:
-                validgroups.append(group[l:r])
-            if r < len(group):
-                testgroups.append(group[r:])
-
-        self.trainiter = pd.concat(traingroups).reset_index(drop=True)
-        self.validiter = pd.concat(validgroups).reset_index(drop=True)
-        self.testiter = pd.concat(testgroups).reset_index(drop=True)
-
-    def seq_split_by_ratio(self, ratios: Iterable = (8, 1, 1), seed: int = 0):
-        infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
-        markers = np.cumsum(ratios)
-        groups = [pair[1] for pair in self.interactions.groupby(USER.name)]
-
-        l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
-        r = floor(markers[1] * len(groups) / markers[-1])
-
-        random.seed(seed)
-        random.shuffle(groups)
-
-        traingroups = groups[:l]
-        validgroups = groups[l:r]
-        testgroups = groups[r:]
-
-        self.trainiter = pd.concat(traingroups).reset_index(drop=True)
-        self.validiter = pd.concat(validgroups).reset_index(drop=True)
-        self.testiter = pd.concat(testgroups).reset_index(drop=True)
-
-    def seq_split_by_last_two(self):
-        infoLogger(f"[Converter] >>> Split by leaving last two ...")
-        traingroups = []
-        validgroups = []
-        testgroups = []
-        for _, group in self.interactions.groupby(USER.name):
-            if len(group) == 0:
-                continue
-            if len(group) <= 3:
-                # Note that sequence with len(group) == 3 cannot be splited into train/valid/test,
-                # because train sequence needs at least length >= 2 for prediction.
-                traingroups.append(group)
-            else:
-                traingroups.append(group[:-2])
-                validgroups.append(group[-2:-1])
-                testgroups.append(group[-1:])
-
-        self.trainiter = pd.concat(traingroups).reset_index(drop=True)
-        self.validiter = pd.concat(validgroups).reset_index(drop=True)
-        self.testiter = pd.concat(testgroups).reset_index(drop=True)
-
-    def sess_split_by_ratio(self, ratios: Iterable = (8, 1, 1)):
-        infoLogger(f"[Converter] >>> Split by ratios: {ratios} ...")
-
-        # max(): choosing the last timestamp as the timestamp for the session
-        groups = list(self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values().index)
-
-        markers = np.cumsum(ratios)
-        l = max(floor(markers[0] * len(groups) / markers[-1]), 1)
-        r = floor(markers[1] * len(groups) / markers[-1])
-
-        traingroups = groups[:l]
-        validgroups = groups[l:r]
-        testgroups = groups[r:]
-
-        self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
-        self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
-        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
-
-    def sess_split_by_day(self, days: int = 1):
-        infoLogger(f"[Converter] >>> Split by days: {days} ...")
-
-        seconds_per_day = 86400
-        seconds = seconds_per_day * days
-        last_date = self.interactions[TIMESTAMP.name].max().item()
-
-        # Group interactions by session and calculate session timestamps
-        session_timestamps = self.interactions.groupby(SESSION.name)[TIMESTAMP.name].max().sort_values()
-
-        # Split interactions into train, validation, and test sets based on session timestamps
-        traingroups = session_timestamps[session_timestamps < (last_date - 2 * seconds)].index
-        validgroups = session_timestamps[(session_timestamps >= (last_date - 2 * seconds)) & (session_timestamps < (last_date - seconds))].index
-        testgroups = session_timestamps[session_timestamps >= (last_date - seconds)].index
-
-        assert len(traingroups) >= 0, f"The given `days` of {days} leads to zero-size trainsets ..."
-        assert len(validgroups) >= 0, f"The given `days` of {days} leads to zero-size validsets ..."
-        assert len(testgroups) >= 0, f"The given `days` of {days} leads to zero-size testsets ..."
-
-        self.trainiter = self.interactions[self.interactions[SESSION.name].isin(traingroups)]
-        self.validiter = self.interactions[self.interactions[SESSION.name].isin(validgroups)]
-        self.testiter = self.interactions[self.interactions[SESSION.name].isin(testgroups)]
-
-    def save(self, path: str):
-        mkdirs(path)
-
-        infoLogger(f"[Converter] >>> Save `train.txt' to {path} ...")
-        df = pd.DataFrame(self.trainiter)
-        df.to_csv(os.path.join(path, 'train.txt'), sep='\t', index=False)
-
-        infoLogger(f"[Converter] >>> Save `valid.txt' to {path} ...")
-        df = pd.DataFrame(self.validiter)
-        df.to_csv(os.path.join(path, 'valid.txt'), sep='\t', index=False)
-
-        infoLogger(f"[Converter] >>> Save `test.txt' to {path} ...")
-        df = pd.DataFrame(self.testiter)
-        df.to_csv(os.path.join(path, 'test.txt'), sep='\t', index=False)
-
-        if self.userFeats is not None:
-            infoLogger(f"[Converter] >>> Save `user.txt' to {path} ...")
-            self.userFeats.to_csv(
-                os.path.join(path, 'user.txt'),
-                sep='\t', index=False
-            )
+    @main_process_only
+    def easy_record_best(self, best: defaultdict):
+        r"""
+        Record the best results on test set.
+        It make easy to watch on tensorboard.
+        """
 
-        if self.itemFeats is not None:
-            infoLogger(f"[Converter] >>> Save `item.txt' to {path} ...")
-            self.itemFeats.to_csv(
-                os.path.join(path, 'item.txt'),
-                sep='\t', index=False
-            )
+        for lastname, meters in self.monitors['test'].items():
+            for meter in meters:
+                # Skip those meters never activated.
+                if len(meter.history) == 0:
+                    continue
+                # Note that meter.history[-1] is the result at the best checkpoint.
+                val = meter.history[-1]
+                best['best'][meter.name] = val
 
-        self.summary()
+        export_pickle(best, os.path.join(self.cfg.LOG_PATH, self.cfg.DATA_DIR, self.cfg.MONITOR_BEST_FILENAME))
 
-    def make_general_dataset(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 10,
-        kcore4item: int = 10,
-        strict: bool = True,
-        ratios: Tuple[int, int, int] = (8, 1, 1),
-        fields: Optional[Iterable[str]] = (USER.name, ITEM.name)
+    def resume(self) -> int:
+        r"""
+        Resume training from the last checkpoint.
+
+        Returns:
+        --------
+        start_epoch: int
+            The epoch number to resume training from.
+        """
+        start_epoch: int = 0
+        if self.cfg.resume:
+            start_epoch = self.load_checkpoint()
+            infoLogger(f"[Coach] >>> Load last checkpoint and train from epoch: {start_epoch}")
+        return start_epoch
+
+    @torch.no_grad()
+    def monitor(
+        self, *values,
+        n: int = 1, reduction: str = 'mean', 
+        mode: Literal['train', 'valid', 'test'] = 'train', 
+        pool: Optional[Iterable] = None
     ):
+
         r"""
-        Make general dataset.
+        Log data values to specific monitors.
 
         Parameters:
         -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        ratios: Tuple[int, int, int], default to (8, 1, 1)
-            The ratios of training|validation|test set.
-        fields: Iterable[str], default to (User, Item)
-            The fields reserved.
-        """
-
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
-        self.user2token()
-        self.item2token()
-        self.sort_by_timestamp()
-        if fields:
-            self.reserve(fields)
-        self.gen_split_by_ratio(ratios)
-
-        code = f"{kcore4user}{kcore4item}{star4pos}{''.join(map(str, ratios))}"
-        path = os.path.join(
-            self.root, 'General', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
+        *values : data
+            The data values to be logged.
+        n : int
+            The batch size in general.
+        reduction : str, optional
+            The reduction to compute the metric. Can be 'sum' or 'mean' (default).
+        mode : str, optional
+            The mode string indicating which mode the values belong to. Can be 'train', 'test' or 'valid'.
+        pool : List[str], optional
+            A list of metric names to log. If None, all metrics in the pool of `mode` will be logged.
+        """
 
-        self.save(path)
+        metrics: Dict[List] = self.monitors[mode]
+        pool = metrics if pool is None else pool
+        for lastname in pool:
+            for meter in metrics.get(lastname.upper(), []):
+                meter(*values, n=n, reduction=reduction)
 
-    def make_sequential_dataset(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 5,
-        kcore4item: int = 5,
-        strict: bool = True,
-        fields: Optional[Iterable[str]] = (USER.name, ITEM.name, TIMESTAMP.name)
-    ):
+    def step(self, epoch: int):
         r"""
-        Make sequential dataset by leaving last two as validation|test samples.
+        Prints training status and evaluation results for each epoch, 
+        and resets the corresponding `AverageMeter` instances.
 
         Parameters:
         -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        fields: Iterable[str], default to (User, Item, TimeStamp)
-            The fields reserved.
-        """
-
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
-        self.user2token()
-        self.item2token()
-        self.sort_by_timestamp()
-        if fields:
-            self.reserve(fields)
-        self.seq_split_by_last_two()
-
-        code = f"{kcore4user}{kcore4item}{star4pos}"
-        path = os.path.join(
-            self.root, 'Sequential', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
+        epoch : int
+            The epoch number.
 
-        self.save(path)
+        Returns:
+        --------
+        None
+        """
+        metrics: Dict[str, List[AverageMeter]]
+        for mode, metrics in self.monitors.items():
+            infos = [f"[Coach] >>> {mode.upper():5} @Epoch: {epoch:<4d} >>> "]
+            for meters in metrics.values():
+                infos += [meter.step() for meter in meters if meter.active]
+            infoLogger(' || '.join(infos))
 
-    def make_sequential_dataset_by_ratio(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 5,
-        kcore4item: int = 5,
-        strict: bool = True,
-        ratios: Tuple[int, int, int] = (8, 1, 1),
-        fields: Optional[Iterable[str]] = (USER.name, ITEM.name, TIMESTAMP.name),
-        seed: int = 0
-    ):
+    @main_process_only
+    @timemeter
+    def summary(self):
         r"""
-        Make sequential dataset by ratios.
+        Summary the whole training process.
 
-        Parameters:
-        -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        ratios: Tuple[int, int, int], default to (8, 1, 1)
-            The ratios of training|validation|test set.
-        fields: Iterable[str], default to (User, Item, Timestamp)
-            The fields reserved.
-        """
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
-        self.user2token()
-        self.item2token()
-        self.sort_by_timestamp()
-        if fields:
-            self.reserve(fields)
-        self.seq_split_by_ratio(ratios, seed=seed)
-
-        code = f"{kcore4user}{kcore4item}{star4pos}{''.join(map(str, ratios))}"
-        path = os.path.join(
-            self.root, 'Sequential', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
+        Generate a summary of the entire training process, including the historical evaluation results, the best
+        historical results, and the curves of historical results. The resulting summary is saved to a Markdown file named
+        "Summary.md" in the `self.cfg.LOG_PATH` directory.
 
-        self.save(path)
+        Additionally, the best historical results are saved to a binary file named `self.cfg.MONITOR_BEST_FILENAME`.
+        """
+        import pandas as pd
 
-    def make_session_dataset_by_day(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 2,
-        kcore4item: int = 5,
-        strict: bool = True,
-        days: int = 7,
-        fields: Optional[Iterable[str]] = (SESSION.name, ITEM.name, TIMESTAMP.name),
-    ):
-        r"""
-        Make session dataset by day.
+        s = "|  {mode}  |   {name}   |   {val}   |   {epoch}   |   {img}   |\n"
+        info = ""
+        info += "|  Mode  |   Metric   |   Best   |   @Epoch   |   Img   |\n"
+        info += "| :-------: | :-------: | :-------: | :-------: | :-------: |\n"
+        data = []
+        best = defaultdict(dict)
+
+        for mode, metrics in self.monitors.items():
+            metrics: defaultdict[str, List[AverageMeter]]
+            freq = 1 if mode == 'train' else self.cfg.eval_freq
+            for lastname, meters in metrics.items():
+                for meter in meters:
+                    # Skip those meters never activated.
+                    if len(meter.history) == 0:
+                        continue
+                    meter.plot(freq=freq)
+                    imgname = meter.save(path=os.path.join(self.cfg.LOG_PATH, self.cfg.SUMMARY_DIR), mode=mode)
+                    epoch, val = meter.argbest(freq)
+                    info += s.format(
+                        mode=mode, name=meter.name,
+                        val=val, epoch=epoch, img=f"![]({imgname})"
+                    )
+                    data.append([mode, meter.name, val, epoch])
+                    if val != -1: # Only save available data.
+                        best[mode][meter.name] = val
+
+        file_ = os.path.join(self.cfg.LOG_PATH, self.cfg.SUMMARY_DIR, self.cfg.SUMMARY_FILENAME)
+        with open(file_, "w", encoding="utf8") as fh:
+            fh.write(info)
+
+        df = pd.DataFrame(data, columns=['Mode', 'Metric', 'Best', '@Epoch'])
+        infoLogger(str(df))
+        infoLogger(f"[LoG_PaTH] >>> {self.cfg.LOG_PATH}")
+
+        self.monitors.write(os.path.join(self.cfg.LOG_PATH, self.cfg.SUMMARY_DIR)) # tensorboard
+        self.monitors.save(os.path.join(self.cfg.LOG_PATH, self.cfg.DATA_DIR), self.cfg.MONITOR_FILENAME)
+
+        return best
+
+    def dict_to_device(self, data: Dict[Field, Any]) -> Dict[Field, Any]:
+        return {field: value.to(self.device) if isinstance(value, torch.Tensor) else value for field, value in data.items()}
+
+    def evaluate(self, epoch: int, mode: str = 'valid'):
+        self.get_res_sys_arch().reset_ranking_buffers()
+        for data in self.dataloader:
+            data = self.dict_to_device(data)
+            users = data[self.User]
+            if self.cfg.ranking == 'full':
+                scores = self.model(data, ranking='full')
+                if self.remove_seen:
+                    seen = self.Item.to_csr(data[self.ISeen]).to(self.device).to_dense().bool()
+                    scores[seen] = -1e23
+                targets = self.Item.to_csr(data[self.IUnseen]).to(self.device).to_dense()
+            elif self.cfg.ranking == 'pool':
+                scores = self.model(data, ranking='pool')
+                targets = torch.zeros_like(scores)
+                targets[:, 0].fill_(1)
+            else:
+                raise NotImplementedError(
+                    f"`ranking` should be 'full' or 'pool' but {self.cfg.ranking} received ..."
+                )
 
-        Flows:
-        ------
-        1. filter out `inactive' items and short sessions;
-        2. training|validation|test set will be splited according to the start time of each session.
+            self.monitor(
+                scores, targets,
+                n=len(users), reduction="mean", mode=mode,
+                pool=['HITRATE', 'PRECISION', 'RECALL', 'NDCG', 'MRR']
+            )
+            
+    @timemeter
+    def fit(self):
 
-        Parameters:
-        -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        days: int, default to 7
-            the number days used for validation and test
-        fields: Iterable[str], default to (User, Item, Timestamp)
-            The fields reserved.
-        """
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, master=SESSION.name, strict=strict)
-        self.user2token(master=SESSION.name)
-        self.item2token()
-        self.sort_by_timestamp(master=SESSION.name)
-        if fields:
-            self.reserve(fields)
-        self.sess_split_by_day(days)
-
-        code = f"{kcore4user}{kcore4item}{star4pos}{days}"
-        path = os.path.join(
-            self.root, 'Session', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
+        start_epoch = self.resume()
+        for epoch in range(start_epoch, self.cfg.epochs):
+            if epoch % self.cfg.CHECKPOINT_FREQ == 0:
+                self.save_checkpoint(epoch)
+            if epoch % self.cfg.eval_freq == 0:
+                if self.cfg.eval_valid:
+                    self.valid(epoch)
+                if self.cfg.eval_test:
+                    self.test(epoch)
+            self.check_best(epoch)
+            self.step(epoch)
+            self.train(epoch)
 
-        self.save(path)
+        self.save()
 
-    def make_session_dataset_by_ratio(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 2,
-        kcore4item: int = 5,
-        strict: bool = True,
-        ratios: Tuple[int, int, int] = (8, 1, 1),
-        fields: Optional[Iterable[str]] = (SESSION.name, ITEM.name, TIMESTAMP.name),
-    ):
-        r"""
-        Make session dataset by ratios.
+        # last epoch
+        self.valid(self.cfg.epochs)
+        self.test(self.cfg.epochs)
 
-        Flows:
-        ------
-        1. filter out `inactive' items and short sessions;
-        2. training|validation|test set will be splited according to the start time of each session.
+        self.check_best(self.cfg.epochs)
+        self.step(self.cfg.epochs)
 
-        Parameters:
-        -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        ratios: Tuple[int, int, int], default to (8, 1, 1)
-            The ratios of training|validation|test set.
-        fields: Iterable[str], default to (User, Item, Timestamp)
-            The fields reserved.
-        """
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, master=SESSION.name, strict=strict)
-        self.user2token(master=SESSION.name)
-        self.item2token()
-        self.sort_by_timestamp(master=SESSION.name)
-        if fields:
-            self.reserve(fields)
-        self.sess_split_by_ratio(ratios)
-
-        code = f"{kcore4user}{kcore4item}{star4pos}{''.join(map(str, ratios))}"
-        path = os.path.join(
-            self.root, 'Session', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
+        best = self.summary()
 
-        self.save(path)
+        self.eval_at_best()
+        self.easy_record_best(best)
 
-    def make_context_dataset_by_last_two(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 5,
-        kcore4item: int = 5,
-        strict: bool = True,
-        fields: Optional[Iterable[str]] = (USER.name, ITEM.name, TIMESTAMP.name)
-    ):
+        self.shutdown()
+
+
+class Adapter:
+    r"""
+    Params tuner.
+
+    Flows:
+    ------
+    1. compile: configure the command, environments, and parameters for training.
+    2. allocate devices for various parameters:
+        - register the ID, log path, and device first
+        - execute the command
+        - collect information from the log path and output to TensorBoard
+        - save the checkpoint
+        - release the corresponding device
+
+    Examples:
+    ---------
+    >>> cfg = {'command': 'python xxx.py', 'params': {'optimizer': ['sgd', 'adam']}}
+    >>> tuner = Adapter()
+    >>> tuner.compile(cfg)
+    >>> tuner.fit()
+    """
+
+    def __init__(self) -> None:
+        self.params = []
+        self.values = []
+        self.devices = tuple()
+
+    @property
+    def COMMAND(self):
+        return self.cfg.COMMAND
+
+    def register(self, device: str) -> Tuple[str, str]:
+        self.cfg.ENVS['id'] = time.strftime(TIME)
+        self.cfg.ENVS['device'] = device
+        command = self.COMMAND + self.get_option('id', self.cfg.ENVS.id)
+        command += self.get_option('device', self.cfg.ENVS.device)
+        return command, self.cfg.ENVS.id, self.cfg.LOG_PATH.format(**self.cfg.ENVS)
+
+    @timemeter
+    def compile(self, cfg: Config) -> None:
         r"""
-        Make context dataset by leaving last two as validation|test samples.
+        Configure the command, environments, and parameters for training.
 
         Parameters:
         -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        fields: Iterable[str], default to (User, Item, TimeStamp)
-            The fields reserved.
-        """
-
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
-        self.user2token()
-        self.item2token()
-        self.sort_by_timestamp()
-        if fields:
-            self.reserve(fields)
-        self.seq_split_by_last_two()
-
-        code = f"{kcore4user}{kcore4item}{star4pos}"
-        path = os.path.join(
-            self.root, 'Context', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
+        cfg : Config
+            An object that contains the command, environments, parameters, and defaults.
 
-        self.save(path)
+        Flows:
+        ------
+        1. Add environmental parameters to the basic `command`.
+        2. Register all available devices.
+        3. Convert all parameters from `cfg.PARAMS`.
+        4. Convert all defaults from `cfg.DEFAULTS`.
+
+        Returns:
+        --------
+        None
+        """
+        self.cfg = cfg
+        piece = "\t{key}: {vals} \n"
+        envs, params, defaults = "", "", ""
+        for key, val in self.cfg.ENVS.items():
+            if key == 'device':
+                self.devices = tuple(val.split(','))
+            else:
+                self.cfg.COMMAND += self.get_option(key, val)
+            envs += piece.format(key=key, vals=val)
+        for key, vals in self.cfg.PARAMS.items():
+            if isinstance(vals, (str, int, float)):
+                vals = [vals]
+            self.deploy_params(key, vals)
+            params += piece.format(key=key, vals=vals)
+        for key, val in self.cfg.DEFAULTS.items():
+            self.cfg.DEFAULTS[key] = val
+            defaults += piece.format(key=key, vals=val)
+
+        cfg_infos = f"command: {self.cfg.COMMAND} \nenvs: \n{envs}params: \n{params}defaults: \n{defaults}"
+        infoLogger(f"\033[0;31;47m{cfg_infos}\033[0m")
+
+    def deploy_params(self, key: str, vals: Iterable):
+        self.params.append(key)
+        self.values.append(vals)
 
-    def make_context_dataset_by_ratio(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 5,
-        kcore4item: int = 5,
-        strict: bool = True,
-        ratios: Tuple[int, int, int] = (8, 1, 1),
-        fields: Optional[Iterable[str]] = (USER.name, ITEM.name, TIMESTAMP.name),
-    ):
+    @staticmethod
+    def get_option(key: str, val: Any):
         r"""
-        Make context dataset by ratios.
+        Convert (key, val) to '--key=val'.
 
         Parameters:
         -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        ratios: Tuple[int, int, int], default to (8, 1, 1)
-            The ratios of training|validation|test set.
-        fields: Iterable[str], default to (User, Item, Timestamp)
-            The fields reserved.
-        """
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, strict=strict)
-        self.user2token()
-        self.item2token()
-        self.sort_by_timestamp()
-        if fields:
-            self.reserve(fields)
-        self.gen_split_by_ratio(ratios)
-
-        code = f"{kcore4user}{kcore4item}{star4pos}{''.join(map(str, ratios))}"
-        path = os.path.join(
-            self.root, 'Context', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
-        self.save(path)
+        key : str
+            The key of the parameter.
+        val : Any
+            The value of the parameter.
 
-    def make_context_dataset_by_day(
-        self,
-        star4pos: int = 0,
-        kcore4user: int = 2,
-        kcore4item: int = 5,
-        strict: bool = True,
-        days: int = 7,
-        fields: Optional[Iterable[str]] = (SESSION.name, ITEM.name, TIMESTAMP.name),
-    ):
+        Notes:
+        ------
+        All '_' in `key` will be replaced by '-'.
+
+        Returns:
+        --------
+        str
+            The parameter with format '--key=val'.
+
+        Examples:
+        ---------
+        >>> Adapter.get_option('lr', '1e-3')
+        '--lr=1e-3'
+        >>> Adapter.get_option('learning_rate', '1e-3')
+        '--learning-rate=1e-3'
+        """
+        return f" --{key.replace('_', '-')}={val}"
+
+    def load_best(self, logPath: str):
+        """Load best.pkl from logPath of corresponding."""
+        file_ = os.path.join(logPath, self.cfg.DATA_DIR, self.cfg.MONITOR_BEST_FILENAME)
+        return import_pickle(file_)
+
+    def write(self, id_: str, logPath: str, params: Dict):
         r"""
-        Make session dataset by day.
+        Write experiment results to tensorboard.
+
+        Parameters:
+        -----------
+        id_: str
+            Experiment ID.
+        logPath: str
+            Path to the experiment logs.
+        params: Dict
+            Configuration parameters of the experiment.
 
         Flows:
         ------
-        1. filter out `inactive' items and short sessions;
-        2. training|validation|test set will be splited according to the start time of each session.
+        1. Load the best data from `logPath`.
+        2. Write the best data to tensorboard with `params`.
 
-        Parameters:
-        -----------
-        star4pos: int, default to 0
-            Select interactions with `Rating >= star4pos'.
-        kcore4user: int, default to 10
-            Select kcore interactions according to User.
-        kcore4item: int, default to 10
-            Select kcore interactions according to Item.
-        strict: bool, default to `True`
-            `True`: strictly filter by core
-            `False`: filter by core only once
-        days: int, default to 7
-            the number days used for validation and test
-        fields: Iterable[str], default to (User, Item, Timestamp)
-            The fields reserved.
-        """
-        self.load()
-        self.filter_by_rating(low=star4pos, high=None)
-        self.filter_by_core(low4user=kcore4user, low4item=kcore4item, master=SESSION.name, strict=strict)
-        self.user2token(master=SESSION.name)
-        self.item2token()
-        self.sort_by_timestamp(master=SESSION.name)
-        if fields:
-            self.reserve(fields)
-        self.sess_split_by_day(days)
-
-        code = f"{kcore4user}{kcore4item}{star4pos}{days}"
-        path = os.path.join(
-            self.root, 'Context', 
-            '_'.join([self.dataset, code, 'Chron'])
-        )
+        Notes:
+        ------
+        If you find `-1` appearing in the tensorboard,
+        it could mean that the data is of `str` type,
+        which will cause an error if it is sent to tensorboard directly!
+        """
+        try:
+            data = self.load_best(logPath)
+            path = os.path.join(self.cfg.CORE_LOG_PATH, id_)
+            with SummaryWriter(log_dir=path) as writer:
+                metrics = dict()
+                for mode, best in data.items():
+                    for metric, val in best.items():
+                        val = val if isinstance(val, (int, float)) else -1
+                        metrics['/'.join([mode, metric])] = val
+                writer.add_hparams(
+                    params, metrics,
+                )
+        except Exception:
+            infoLogger(
+                f"\033[0;31;47m[Adapter] >>> Unknown errors happen. This is mainly due to abnormal exits of child processes.\033[0m"
+            )
 
-        self.save(path)
+    def each_grid(self):
+        """Grid search for each kind of param."""
+        for key, vals in zip(self.params, self.values):
+            for val in vals:
+                yield self.cfg.DEFAULTS | {key: val}
+
+    def product_grid(self):
+        """Grid search across all combination of params"""
+        for vals in product(*self.values):
+            yield self.cfg.DEFAULTS | {option:val for option, val in zip(self.params, vals)}
+
+    def save_checkpoint(self, source: List) -> None:
+        """Save the rest of params."""
+        path = os.path.join(self.cfg.CORE_CHECKPOINT_PATH, self.cfg.CHECKPOINT_FILENAME)
+        checkpoint = dict()
+        checkpoint['source'] = source
+        torch.save(checkpoint, path)
+
+    @timemeter
+    def load_checkpoint(self) -> int:
+        """Load the rest of params."""
+        infoLogger(f"[Coach] >>> Load the recent checkpoint ...")
+        path = os.path.join(self.cfg.CORE_CHECKPOINT_PATH, self.cfg.CHECKPOINT_FILENAME)
+        checkpoint = torch.load(path)
+        return checkpoint['source']
+
+    def resume(self):
+        """Resume from the recent checkpoint."""
+        source = self.each_grid() if self.cfg.EXCLUSIVE else self.product_grid()
+        source = list(source)[::-1]
+        source = self.load_checkpoint() if self.cfg.resume else source
+        return source
+
+    def run(self, command: str, params: Dict):
+        """Start a new subprocess"""
+        import subprocess, shlex
+        for option, val in params.items():
+            command += self.get_option(option, val)
+        infoLogger(f"\033[0;31;47m{command}\033[0m")
+        return subprocess.Popen(shlex.split(command))
+
+    def wait(self, tasks: List):
+        """Wait util all processes terminate."""
+        tasks = [task for task in tasks if task is not None]
+        for process_, id_, logPath, params in tasks:
+            process_.wait()
+            self.write(id_, logPath, params)
+
+    def poll(self, tasks: List):
+        """Wait util any process terminates."""
+        def is_null(task):
+            return task is None
+        buffer_source = [task[-1] for task in tasks if task is not None]
+        time.sleep(1) # for unique id
+        while not any(map(is_null, tasks)):
+            time.sleep(7)
+            buffer_source = []
+            for i, (process_, id_, logPath, params) in enumerate(tasks):
+                if process_.poll() is not None:
+                    self.write(id_, logPath, params)
+                    tasks[i] = None
+                else:
+                    buffer_source.append(params)
+        self.save_checkpoint(self.source + buffer_source)
+        return tasks.index(None)
+
+    def terminate(self, tasks: List):
+        tasks = [task for task in tasks if task is not None]
+        for process_, _, _, _ in tasks:
+            if process_.poll() is None:
+                process_.terminate()
+        time.sleep(3)
+        for process_, _, _, _ in tasks:
+            if process_.poll() is None:
+                process_.kill()
+        sys.exit()
+
+    @timemeter
+    def fit(self):
+        """Grid search."""
+        self.source = self.resume()
+        tasks = [None for _ in range(len(self.devices))]
+
+        def signal_handler(sig, frame):
+            infoLogger(f"\033[0;31;47m===============================TERMINATE ALL SUBPROCESSES===============================\033[0m")
+            self.terminate(tasks)
+        signal.signal(signal.SIGINT, signal_handler)
 
-    def summary(self):
-        from prettytable import PrettyTable
-        table = PrettyTable(['#User', '#Item', '#Interactions', '#Train', '#Valid', '#Test', 'Density'])
-        trainsize = len(self.trainiter)
-        validsize = len(self.validiter)
-        testsize = len(self.testiter)
-        table.add_row([
-            self.userCount, self.itemCount, trainsize + validsize + testsize,
-            trainsize, validsize, testsize,
-            (trainsize + validsize + testsize) / (self.userCount * self.itemCount)
-        ])
-        infoLogger(table)
+        try:
+            while self.source:
+                index = self.poll(tasks)
+                device = self.devices[index]
+                params = self.source.pop()
+                command, id_, logPath = self.register(device)
+                process_ = self.run(command, params)
+                tasks[index] = (process_, id_, logPath, params)
+        finally:
+            self.wait(tasks)
+            self.terminate(tasks)
```

### Comparing `freerec-0.7.5/freerec/data/utils.py` & `freerec-0.8.1/freerec/data/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     str
         The file path of the downloaded file.
     """
     if filename is None:
         filename = url.split('/')[-1]
         # Empty filenames are invalid
         assert filename, 'Can\'t construct file-name from this URL. ' \
-            'Please set the `path` option manually.'
+            'Please set the `filename` option manually.'
     file_ = os.path.join(root, filename)
 
     assert retries >= 0, "Number of retries should be at least 0"
 
     if not verify_ssl:
         warnings.warn(
             'Unverified HTTPS request is being made (verify_ssl=False). '
@@ -112,21 +112,25 @@
         while retries+1 > 0:
             # Disable pyling too broad Exception
             # pylint: disable=W0703
             try:
                 if log:
                     infoLogger('[DataSet] >>> Downloading %s from %s...' % (file_, url))
                 r = requests.get(url, stream=True, verify=verify_ssl)
+                filesize = int(r.headers.get("Content-Length", 0))
                 if r.status_code != 200:
                     raise RuntimeError("Failed downloading url %s" % url)
                 with open(file_, 'wb') as f:
                     if log:
-                        for chunk in tqdm.tqdm(r.iter_content(chunk_size=chunk_size), leave=False, desc="վ'ᴗ' ի-"):
+                        progress_bar = tqdm.tqdm(total=filesize, unit="B", unit_scale=True, desc="վ'ᴗ' ի-")
+                        for chunk in r.iter_content(chunk_size=chunk_size):
                             if chunk:  # filter out keep-alive new chunks
+                                progress_bar.update(len(chunk))
                                 f.write(chunk)
+                        progress_bar.close()
                     else:
                         for chunk in r.iter_content(chunk_size=chunk_size):
                             if chunk:  # filter out keep-alive new chunks
                                 f.write(chunk)
                 if sha1_hash and not check_sha1(file_, sha1_hash):
                     raise DataSetLoadingError(
                         'File {} is downloaded but the content hash does not match.'
@@ -217,42 +221,37 @@
     return sha1.hexdigest() == sha1_hash
 
 
 def negsamp_vectorized_bsearch(
     positives: Union[Tuple, List], n_items: int, 
     size: Union[int, List[int], Tuple[int]] = 1,
     replacement: bool = True
-) -> np.ndarray:
+) -> List:
     r"""
     Uniformly sampling negatives according to a list of ordered positives
     See [here](https://tech.hbc.com/2018-03-23-negative-sampling-in-numpy.html) for more details.
 
     Parameters:
     -----------
     positives: Union[Tuple, List], 1-D
-        The positive indices should be ordered.
+        The positive indices should be in ordered.
     n_items: int
         The number of all items.
     size: int or List[int] or Tuple[int]
         The size of required negatives.
     replacement: bool, default to `True`
         - True: sampling with replacement
         - False: sampling without replacement
     
     Raises:
     -------
     AssertionError:
         Given `positives` is not 1-D.
     ValueError:
         Too much negatives required.
-    
-    Returns:
-    --------
-    neg_inds: np.ndarray
-        A list of negatives in the size of `size`.
     """
     positives = np.array(positives, copy=False)
     assert positives.ndim == 1, f"positives should be 1-D array but {positives.ndim}-D received ..."
     try:
         if replacement:
             raw_samp = np.random.randint(0, n_items - len(positives), size=size)
         else:
@@ -260,8 +259,8 @@
     except ValueError:
         raise ValueError(
             "The number of required negatives is larger than that of candidates, but replacement is False ..."
         )
     pos_inds_adj = positives - np.arange(len(positives))
     ss = np.searchsorted(pos_inds_adj, raw_samp, side='right')
     neg_inds = raw_samp + ss
-    return neg_inds
+    return neg_inds.tolist()
```

### Comparing `freerec-0.7.5/freerec/ddp.py` & `freerec-0.8.1/freerec/ddp.py`

 * *Files identical despite different names*

### Comparing `freerec-0.7.5/freerec/dict2obj.py` & `freerec-0.8.1/freerec/dict2obj.py`

 * *Files identical despite different names*

### Comparing `freerec-0.7.5/freerec/graph.py` & `freerec-0.8.1/freerec/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,20 +134,21 @@
 
     Returns:
     --------
     edge_index: torch.Tensor
     edge_weight: torch.Tensor
     """
     M, N = sim_mat.shape
+    device = sim_mat.device
     if sim_mat.is_sparse:
         sim_mat = sim_mat.to_dense()
     vals, cols = torch.topk(sim_mat, k, dim=1, largest=True)
     del sim_mat
 
-    rows = torch.arange(0, M).unsqueeze(-1).repeat(1, k)
+    rows = torch.arange(0, M, device=device).unsqueeze(-1).repeat(1, k)
     rows, cols = rows.flatten(), cols.flatten()
     edge_index = torch.stack(
         (rows, cols), dim=0
     )
     edge_weight = vals.flatten()
 
     if symmetric:
```

### Comparing `freerec-0.7.5/freerec/metrics.py` & `freerec-0.8.1/freerec/metrics.py`

 * *Files identical despite different names*

### Comparing `freerec-0.7.5/freerec/parser.py` & `freerec-0.8.1/freerec/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os, argparse, time, yaml
 from argparse import ArgumentParser
 
 from .dict2obj import Config
 from .ddp import is_distributed, main_process_only, is_main_process, all_gather
 from .utils import (
     mkdirs, timemeter, set_color, set_seed, activate_benchmark, 
-    set_logger, infoLogger
+    set_logger, infoLogger, warnLogger
 )
 
 
 __all__ = ['Parser', 'CoreParser']
 
 
 r"""
@@ -88,14 +88,18 @@
     BEST_FILENAME = "best.pt",
     CHECKPOINT_FREQ = 1,
     CHECKPOINT_MODULES = ['model', 'optimizer', 'lr_scheduler'],
     CHECKPOINT_FILENAME = "checkpoint.tar",
     SUMMARY_FILENAME = "SUMMARY.md",
     MONITOR_FILENAME = "monitors.pkl",
     MONITOR_BEST_FILENAME = "best.pkl",
+
+    # monitors
+    monitors = [],
+    which4best = "LOSS"
 )
 
 CORE_CONFIG = Config(
     MONITOR_BEST_FILENAME = CONFIG.MONITOR_BEST_FILENAME,
     CHECKPOINT_FILENAME = CONFIG.CHECKPOINT_FILENAME,
     EXCLUSIVE = False,
     COMMAND = None,
@@ -123,14 +127,17 @@
 
     # PATH
     DATA_DIR: str
     SUMMARY_DIR: str
     CHECKPOINT_PATH: str
     LOG_PATH: str
 
+    monitors: list
+    which4best: str
+
     def __init__(self) -> None:
         super().__init__(**CONFIG)
         self.parse()
 
     @main_process_only
     def readme(self, path: str, mode: str = "w") -> None:
         """Add README.md to the path."""
@@ -154,14 +161,15 @@
     def parse(self):
         """Add command-line arguments to the parser."""
 
         self.parser = argparse.ArgumentParser()
 
         self.add_argument("--root", type=str, default=".", help="data path")
         self.add_argument("--dataset", type=str, default="RecDataSet", help="useless if no need to automatically select a dataset")
+        self.add_argument("--tasktag", type=str, choices=('MATCHING', 'NEXTITEM'), default=None, help="to specify a tasktag for dataset")
         self.add_argument("--config", type=str, default=None, help="config.yaml")
         self.add_argument("--ranking", type=str, choices=('full', 'pool'), default='full', help="full: full ranking; pool: sampled-based ranking")
         self.add_argument("--retain-seen", action="store_true", default=False, help="True: retain seen candidates during evaluation")
 
         self.add_argument("--device", default=torch.cuda.current_device() if torch.cuda.is_available() else 'cpu', help="device")
         self.add_argument("--ddp-backend", type=str, default='nccl', help="ddp backend")
 
@@ -182,15 +190,14 @@
 
         # eval
         self.add_argument("--eval-valid", action="store_false", default=True, help="if True, evaluate validset")
         self.add_argument("--eval-test", action="store_true", default=False, help="if True, evaluate testset")
         self.add_argument("--eval-freq", type=int, default=5, help="the evaluation frequency")
 
         self.add_argument("--num-workers", type=int, default=4)
-        self.add_argument("--pin-memory", action="store_true", default=False)
 
         self.add_argument("--seed", type=int, default=1, help="calling --seed=-1 for a random seed")
         self.add_argument("--benchmark", action="store_true", default=False, help="cudnn.benchmark == True ?")
         self.add_argument("--resume", action="store_true", default=False, help="resume the training from the recent checkpoint")
 
         self.add_argument("--id", type=str, default=time.strftime(TIME))
         self.add_argument("-m", "--description", type=str, default="RecSys")
@@ -247,14 +254,19 @@
         import torch.distributed as dist
         if is_distributed():
             dist.init_process_group(backend=self.ddp_backend, init_method="env://")
             self.device = int(os.environ["LOCAL_RANK"])
             # synchronize ids
             self.id = all_gather(self.id)[0]
             infoLogger(f"[DDP] >>> DDP is activated ...")
+
+    def set_tasktag(self):
+        from .data.tags import TaskTags
+        if self.tasktag is not None:
+            self['tasktag'] = TaskTags(self.tasktag.upper())
     
     @timemeter
     def load(self):
         r"""
         Load config.yaml.
 
         Raises:
@@ -272,16 +284,19 @@
         if hasattr(args, 'config') and args.config:
             with open(args.config, encoding="UTF-8", mode='r') as f:
                 for key, val in yaml.full_load(f).items():
                     if key in keys: # overwriting defaults
                         self.set_defaults(**{key: val})
                     elif key.upper() in self:
                         self[key.upper()] = val
+                    elif key in self:
+                        self[key] = val
                     else:
-                        raise KeyError(f"Unexpected parameter of `{key}' in `{args.config}' ...")
+                        self[key] = val
+                        warnLogger(f"Find an undefined parameter `{key}' in `{args.config}' ...")
         return self.parser.parse_args()
 
     @timemeter
     def compile(self):
         r"""
         Generate the configuration file according to the specified settings.
 
@@ -311,14 +326,16 @@
 
         self.set_device(self.device)
         set_logger(path=self.LOG_PATH, log2file=self.log2file, log2console=self.log2console)
 
         activate_benchmark(self.benchmark)
         self.seed = set_seed(self.seed)
 
+        self.set_tasktag()
+
         self.readme(self.CHECKPOINT_PATH) # create README.md
         self.readme(self.LOG_PATH)
 
         if is_main_process():
             infoLogger(str(self))
```

### Comparing `freerec-0.7.5/freerec/utils.py` & `freerec-0.8.1/freerec/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 
-from typing import Callable, Dict, List, Union
+from typing import Callable, Dict, List, Union, Any, NoReturn
 import torch
 import numpy as np
 from torch.utils.tensorboard import SummaryWriter
 
-import logging, time, random, os
+import logging, time, random, os, pickle
 from collections import defaultdict
-from freeplot.base import FreePlot
-from freeplot.utils import export_pickle
+import matplotlib.pyplot as plt
 
 from .dict2obj import Config
 from .ddp import is_main_process, all_gather
 
 
 LOGGER = Config(
     name='RecSys', filename='log.txt', level=logging.DEBUG,
@@ -77,40 +76,40 @@
         """Reset the meter values"""
         self.val = 0.
         self.avg = 0.
         self.sum = 0.
         self.count = 0
         self.active = False
 
-    def gather(self, val: float, n: int, mode: str):
+    def gather(self, val: float, n: int, reduction: str):
         """Gather metrics from other processes (DDP)."""
         vals = all_gather(val)
         ns = all_gather(n)
-        if mode == "mean":
+        if reduction == "mean":
             val = sum([val * n for val, n in zip(vals, ns)])
-        elif mode == "sum":
+        elif reduction == "sum":
             val = sum(vals)
         else:
-            raise ValueError(f"Receive mode {mode} but 'mean' or 'sum' expected ...")
+            raise ValueError(f"Receive reduction {reduction} but 'mean' or 'sum' expected ...")
         return val, int(sum(ns))
 
-    def update(self, val: float, n: int = 1, mode: str = "mean") -> None:
+    def update(self, val: float, n: int = 1, reduction: str = "mean") -> None:
         r"""
         Updates the meter.
 
         Parameters:
         ----------
         val: float
             Value.
         n: int, optional (default: 1)
             Batch size.
-        mode: str, optional (default: "mean")
-            Mode: 'sum'|'mean'.
+        reduction: str, optional (default: "mean")
+            Reduction: 'sum'|'mean'.
         """
-        val, n = self.gather(val, n, mode)
+        val, n = self.gather(val, n, reduction)
         self.val = val
         self.count += n
         self.sum += val
         self.avg = self.sum / self.count
 
     def step(self) -> str:
         r"""
@@ -155,41 +154,41 @@
         Plots the meter values.
         
         Parameters:
         -----------
         freq: int, optional (default: 1)
             Plot frequency.
         """
-        self.fp = FreePlot(
-            shape=(1, 1),
-            titles=(self.name,),
-            dpi=300, latex=False
-        )
         timeline = np.arange(len(self.history)) * freq
-        self.fp.lineplot(timeline, self.history, marker='')
-        self.fp.set_title(y=.98)
+        self.fig = plt.figure(dpi=300)
+        ax = self.fig.gca()
+        ax.plot(
+            timeline, self.history, marker='', figure=self.fig
+        )
+        ax.set_title(self.name)
 
-    def save(self, path: str, prefix: str = '') -> None:
+    def save(self, path: str, mode: str = '') -> None:
         r"""
         Save the curves as a PNG file.
 
         Parameters:
         -----------
         path : str
             The path to save the file to.
-        prefix : str, optional
-            The prefix to add to the filename.
+        mode : str, optional
+            The mode to add to the filename.
 
         Returns:
         --------
         filename : str
             The filename of the saved file.
         """
-        filename = f"{prefix}{self.name}.png"
-        self.fp.savefig(os.path.join(path, filename))
+        filename = f"{mode}{self.name}.png"
+        self.fig.savefig(os.path.join(path, filename))
+        plt.close(self.fig)
         return filename
 
     def which_is_better(self, other: float) -> bool:
         return self.caster(self.avg, other)
 
     def argbest(self, freq: int = 1) -> float:
         r"""
@@ -227,32 +226,31 @@
         --------
         str
             The string representation of this object.
         """
         fmtstr = "{name} Avg: {avg:{fmt}}"
         return fmtstr.format(**self.__dict__)
 
-    def __call__(self, *values, n: int = 1, mode: str = "mean")  -> None:
+    def __call__(self, *values, n: int = 1, reduction: str = "mean")  -> None:
         r"""
         Add a new data point to the history.
 
         Parameters:
         -----------
         values : list or tuple
             The value(s) to add to the history.
         n : int, optional
             The number of times to add each value, defaults to 1.
-        mode : str, optional
-            The mode of adding values: 'mean' or 'sum', defaults to 'mean'.
+        reduction : str, optional
+            The reduction of adding values: 'mean' or 'sum', defaults to 'mean'.
         """
         self.active = True
         self.update(
-            val = self.check(*values),
-            n = n,
-            mode = mode
+            val=self.check(*values),
+            n=n, reduction=reduction
         )
 
 
 class Monitor(Config):
 
     def state_dict(self) -> Dict:
         r"""
@@ -321,14 +319,51 @@
                             writer.add_scalar(
                                 '/'.join([prefix, meter.name]),
                                 val,
                                 t
                             )
 
 
+def export_pickle(data: Any, file: str) -> NoReturn:
+    r"""
+    Export data into pickle format.
+
+    data: Any
+    file: str
+        The file (path/filename) to be saved
+    """
+    fh = None
+    try:
+        fh = open(file, "wb")
+        pickle.dump(data, fh, pickle.HIGHEST_PROTOCOL)
+    except (EnvironmentError, pickle.PicklingError) as err:
+        ExportError_ = type("ExportError", (Exception,), dict())
+        raise ExportError_(f"Export Error: {err}")
+    finally:
+        if fh is not None:
+            fh.close()
+
+def import_pickle(file: str) -> Any:
+    r"""
+    Import data from given file.
+    file: str
+        The file (path/filename).
+    """
+
+    fh = None
+    try:
+        fh = open(file, "rb")
+        return pickle.load(fh)
+    except (EnvironmentError, pickle.UnpicklingError) as err:
+        raise ImportError(f"Import Error: {err}")
+    finally:
+        if fh is not None:
+            fh.close()
+
+
 def set_logger(
     path: str,
     log2file: bool = True, log2console: bool = True
 ) -> None:
     r"""
     Set up a logger instance.
```

### Comparing `freerec-0.7.5/freerec.egg-info/PKG-INFO` & `freerec-0.8.1/freerec.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2066 7265  : 2.1..Name: fre
 00000020: 6572 6563 0d0a 5665 7273 696f 6e3a 2030  erec..Version: 0
-00000030: 2e37 2e35 0d0a 5375 6d6d 6172 793a 2050  .7.5..Summary: P
+00000030: 2e38 2e31 0d0a 5375 6d6d 6172 793a 2050  .8.1..Summary: P
 00000040: 7954 6f72 6368 206c 6962 7261 7279 2066  yTorch library f
 00000050: 6f72 2072 6563 6f6d 6d65 6e64 6572 2073  or recommender s
 00000060: 7973 7465 6d73 0d0a 486f 6d65 2d70 6167  ystems..Home-pag
 00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000080: 622e 636f 6d2f 4d54 616e 6448 4a2f 6672  b.com/MTandHJ/fr
 00000090: 6565 7265 630d 0a41 7574 686f 723a 204d  eerec..Author: M
 000000a0: 5461 6e64 484a 0d0a 4175 7468 6f72 2d65  TandHJ..Author-e
@@ -23,122 +23,125 @@
 00000160: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
 00000170: 6e64 656e 740d 0a52 6571 7569 7265 732d  ndent..Requires-
 00000180: 5079 7468 6f6e 3a20 3e3d 332e 390d 0a44  Python: >=3.9..D
 00000190: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
 000001a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
 000001b0: 726b 646f 776e 0d0a 4c69 6365 6e73 652d  rkdown..License-
 000001c0: 4669 6c65 3a20 4c49 4345 4e53 450d 0a52  File: LICENSE..R
-000001d0: 6571 7569 7265 732d 4469 7374 3a20 6672  equires-Dist: fr
-000001e0: 6565 706c 6f74 3e3d 302e 342e 350d 0a52  eeplot>=0.4.5..R
-000001f0: 6571 7569 7265 732d 4469 7374 3a20 5079  equires-Dist: Py
-00000200: 5941 4d4c 3e3d 362e 300d 0a52 6571 7569  YAML>=6.0..Requi
-00000210: 7265 732d 4469 7374 3a20 7465 6e73 6f72  res-Dist: tensor
-00000220: 626f 6172 643e 3d32 2e31 302e 300d 0a52  board>=2.10.0..R
-00000230: 6571 7569 7265 732d 4469 7374 3a20 7073  equires-Dist: ps
-00000240: 7574 696c 3e3d 352e 392e 300d 0a52 6571  util>=5.9.0..Req
-00000250: 7569 7265 732d 4469 7374 3a20 7072 6574  uires-Dist: pret
-00000260: 7479 7461 626c 653e 3d33 2e34 2e31 0d0a  tytable>=3.4.1..
-00000270: 0d0a 0d0a 0d0a 215b 5d28 646f 6373 2f73  ......![](docs/s
-00000280: 7263 2f6c 6f67 6f2e 706e 6729 0d0a 0d0a  rc/logo.png)....
-00000290: 4672 6565 5265 6320 6973 2061 2072 6570  FreeRec is a rep
-000002a0: 6f73 6974 6f72 7920 6465 7369 676e 6564  ository designed
-000002b0: 2066 6f72 2065 6173 7920 2872 6563 6f6d   for easy (recom
-000002c0: 6d65 6e64 6174 696f 6e29 2064 6174 6120  mendation) data 
-000002d0: 7072 652d 7072 6f63 6573 7369 6e67 2061  pre-processing a
-000002e0: 6e64 206d 6f64 656c 2074 7261 696e 696e  nd model trainin
-000002f0: 672e 0d0a 4920 616d 2061 2062 6567 696e  g...I am a begin
-00000300: 6e65 7220 696e 2074 6865 2066 6965 6c64  ner in the field
-00000310: 206f 6620 7265 636f 6d6d 656e 6465 7220   of recommender 
-00000320: 7379 7374 656d 732c 2073 6f20 6d75 6368  systems, so much
-00000330: 206f 6620 4672 6565 5265 6327 7320 6465   of FreeRec's de
-00000340: 7369 676e 7320 6d61 7920 6e6f 7420 6265  signs may not be
-00000350: 2061 7320 6566 6665 6374 6976 652e 2049   as effective. I
-00000360: 6e20 6164 6469 7469 6f6e 2c20 796f 7520  n addition, you 
-00000370: 6172 6520 6672 6565 2074 6f20 7370 6563  are free to spec
-00000380: 6966 7920 796f 7572 206f 776e 2066 7261  ify your own fra
-00000390: 6d65 776f 726b 2062 6173 6564 206f 6e20  mework based on 
-000003a0: 4672 6565 5265 632e 0d0a 0d0a 0d0a 2323  FreeRec.......##
-000003b0: 2052 6571 7569 7265 6d65 6e74 733a 200d   Requirements: .
-000003c0: 0a0d 0a50 7974 686f 6e20 3e3d 2033 2e39  ...Python >= 3.9
-000003d0: 207c 205b 5079 546f 7263 6820 3e3d 322e   | [PyTorch >=2.
-000003e0: 305d 2868 7474 7073 3a2f 2f70 7974 6f72  0](https://pytor
-000003f0: 6368 2e6f 7267 2f29 207c 205b 546f 7263  ch.org/) | [Torc
-00000400: 6844 6174 6120 3e3d 302e 362e 305d 2868  hData >=0.6.0](h
-00000410: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000420: 6d2f 7079 746f 7263 682f 6461 7461 2920  m/pytorch/data) 
-00000430: 7c20 5b50 7947 203e 3d32 2e33 5d28 6874  | [PyG >=2.3](ht
-00000440: 7470 733a 2f2f 7079 746f 7263 682d 6765  tps://pytorch-ge
-00000450: 6f6d 6574 7269 632e 7265 6164 7468 6564  ometric.readthed
-00000460: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000470: 2f6e 6f74 6573 2f69 6e73 7461 6c6c 6174  /notes/installat
-00000480: 696f 6e2e 6874 6d6c 2329 0d0a 0d0a 0d0a  ion.html#)......
-00000490: 6060 600d 0a63 6f6e 6461 2063 7265 6174  ```..conda creat
-000004a0: 6520 2d2d 6e61 6d65 3d46 7265 6552 6563  e --name=FreeRec
-000004b0: 2070 7974 686f 6e3d 332e 390d 0a63 6f6e   python=3.9..con
-000004c0: 6461 2061 6374 6976 6174 6520 4672 6565  da activate Free
-000004d0: 5265 630d 0a60 6060 0d0a 0d0a 0d0a 2a2a  Rec..```......**
-000004e0: 4e6f 7465 3a2a 2a20 4166 7465 7220 5079  Note:** After Py
-000004f0: 546f 7263 6820 322e 302c 2060 546f 7263  Torch 2.0, `Torc
-00000500: 6844 6174 6160 2073 6565 6d73 2074 6f20  hData` seems to 
-00000510: 6861 7665 2073 746f 7070 6564 2062 6569  have stopped bei
-00000520: 6e67 2075 7064 6174 6564 2c20 616e 6420  ng updated, and 
-00000530: 796f 7520 6361 6e20 696e 7374 616c 6c20  you can install 
-00000540: 6974 2077 6974 6820 602d 2d6e 6f2d 6465  it with `--no-de
-00000550: 7073 6020 746f 2061 766f 6964 2069 6e73  ps` to avoid ins
-00000560: 7461 6c6c 696e 6720 6465 7065 6e64 656e  talling dependen
-00000570: 6369 6573 2e0d 0a0d 0a60 6060 0d0a 7069  cies.....```..pi
-00000580: 7020 696e 7374 616c 6c20 2d2d 6e6f 2d64  p install --no-d
-00000590: 6570 7320 746f 7263 6864 6174 610d 0a60  eps torchdata..`
-000005a0: 6060 0d0a 0d0a 0d0a 2323 2049 6e73 7461  ``......## Insta
-000005b0: 6c6c 6174 696f 6e0d 0a0d 0a20 2020 2070  llation....    p
-000005c0: 6970 2069 6e73 7461 6c6c 2066 7265 6572  ip install freer
-000005d0: 6563 0d0a 0d0a 6f72 2028 666f 7220 6c61  ec....or (for la
-000005e0: 7465 7374 290d 0a0d 0a20 2020 2070 6970  test)....    pip
-000005f0: 2069 6e73 7461 6c6c 2067 6974 2b68 7474   install git+htt
-00000600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000610: 4d54 616e 6448 4a2f 6672 6565 7265 632e  MTandHJ/freerec.
-00000620: 6769 740d 0a0d 0a0d 0a0d 0a23 2320 4461  git........## Da
-00000630: 7461 2050 6970 656c 696e 650d 0a0d 0a21  ta Pipeline....!
-00000640: 5b5d 2864 6f63 732f 7372 632f 7069 7065  [](docs/src/pipe
-00000650: 6c69 6e65 2e70 6e67 290d 0a0d 0a2a 2a4e  line.png)....**N
-00000660: 6f74 653a 2a2a 2054 6f20 6d61 6b65 2064  ote:** To make d
-00000670: 6174 6173 6574 2c20 706c 6561 7365 2064  ataset, please d
-00000680: 6f77 6e6c 6f61 6420 636f 7272 6573 706f  ownload correspo
-00000690: 6e64 696e 6720 4174 6f6d 6963 2066 696c  nding Atomic fil
-000006a0: 6573 2066 726f 6d20 5b5b 5265 6342 6f6c  es from [[RecBol
-000006b0: 655d 2868 7474 7073 3a2f 2f64 7269 7665  e](https://drive
-000006c0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
-000006d0: 652f 666f 6c64 6572 732f 3173 6f30 6c63  e/folders/1so0lc
-000006e0: 6b49 364e 365f 6e69 5645 5961 4275 2d4c  kI6N6_niVEYaBu-L
-000006f0: 4963 704f 645a 6639 396b 6a29 5d2e 200d  IcpOdZf99kj)]. .
-00000700: 0a54 6865 6e2c 2072 756e 2060 6672 6565  .Then, run `free
-00000710: 7265 6320 6d61 6b65 202d 2d68 656c 7060  rec make --help`
-00000720: 2e0d 0a0d 0a23 2320 5472 6169 6e69 6e67  .....## Training
-00000730: 2046 6c6f 770d 0a0d 0a0d 0a21 5b5d 2864   Flow......![](d
-00000740: 6f63 732f 7372 632f 666c 6f77 2e70 6e67  ocs/src/flow.png
-00000750: 290d 0a0d 0a0d 0a23 2320 5265 6665 7265  )......## Refere
-00000760: 6e63 6520 436f 6465 0d0a 0d0a 2d20 546f  nce Code....- To
-00000770: 7263 6852 6563 3a20 6874 7470 733a 2f2f  rchRec: https://
-00000780: 6769 7468 7562 2e63 6f6d 2f70 7974 6f72  github.com/pytor
-00000790: 6368 2f74 6f72 6368 7265 6320 0d0a 2d20  ch/torchrec ..- 
-000007a0: 4465 6570 4354 522d 546f 7263 683a 2068  DeepCTR-Torch: h
-000007b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000007c0: 6d2f 7368 656e 7765 6963 6865 6e2f 4465  m/shenweichen/De
-000007d0: 6570 4354 522d 546f 7263 680d 0a2d 2046  epCTR-Torch..- F
-000007e0: 7578 6943 5452 3a20 6874 7470 733a 2f2f  uxiCTR: https://
-000007f0: 6769 7468 7562 2e63 6f6d 2f78 7565 2d70  github.com/xue-p
-00000800: 6169 2f46 7578 6943 5452 0d0a 2d20 4241  ai/FuxiCTR..- BA
-00000810: 5253 3a20 6874 7470 733a 2f2f 6769 7468  RS: https://gith
-00000820: 7562 2e63 6f6d 2f6f 7065 6e62 656e 6368  ub.com/openbench
-00000830: 6d61 726b 2f42 4152 530d 0a2d 2052 6563  mark/BARS..- Rec
-00000840: 426f 6c65 3a20 6874 7470 733a 2f2f 6769  Bole: https://gi
-00000850: 7468 7562 2e63 6f6d 2f52 5543 4149 426f  thub.com/RUCAIBo
-00000860: 782f 5265 6342 6f6c 650d 0a0d 0a0d 0a0d  x/RecBole.......
-00000870: 0a23 2320 4163 6b6e 6f77 6c65 6467 656d  .## Acknowledgem
-00000880: 656e 7473 0d0a 0d0a 5468 616e 6b73 2074  ents....Thanks t
-00000890: 6f20 4368 6174 4750 5420 666f 7220 7468  o ChatGPT for th
-000008a0: 6520 616e 6e6f 7461 7469 6f6e 206f 6620  e annotation of 
-000008b0: 736f 6d65 2063 6f64 652e 2046 6f72 2074  some code. For t
-000008c0: 6869 7320 7265 6173 6f6e 2c20 736f 6d65  his reason, some
-000008d0: 206f 6620 7468 6520 636f 6d6d 656e 7473   of the comments
-000008e0: 206d 6179 2062 6520 696c 6c6f 6769 6361   may be illogica
-000008f0: 6c2e 0d0a                                l...
+000001d0: 6571 7569 7265 732d 4469 7374 3a20 5079  equires-Dist: Py
+000001e0: 5941 4d4c 3e3d 362e 300d 0a52 6571 7569  YAML>=6.0..Requi
+000001f0: 7265 732d 4469 7374 3a20 7465 6e73 6f72  res-Dist: tensor
+00000200: 626f 6172 643e 3d32 2e31 302e 300d 0a52  board>=2.10.0..R
+00000210: 6571 7569 7265 732d 4469 7374 3a20 7072  equires-Dist: pr
+00000220: 6574 7479 7461 626c 653e 3d33 2e34 2e31  ettytable>=3.4.1
+00000230: 0d0a 0d0a 0d0a 0d0a 215b 5d28 646f 6373  ........![](docs
+00000240: 2f73 7263 2f6c 6f67 6f2e 706e 6729 0d0a  /src/logo.png)..
+00000250: 0d0a 3c68 3420 616c 6967 6e3d 2263 656e  ..<h4 align="cen
+00000260: 7465 7222 3e0d 0a20 2020 203c 703e 0d0a  ter">..    <p>..
+00000270: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
+00000280: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000290: 636f 6d2f 4d54 616e 6448 4a2f 6672 6565  com/MTandHJ/free
+000002a0: 7265 632f 626c 6f62 2f6d 6173 7465 722f  rec/blob/master/
+000002b0: 6461 7461 7365 7425 3230 7072 6f63 6573  dataset%20proces
+000002c0: 7369 6e67 2e6d 6422 3e44 6174 6173 6574  sing.md">Dataset
+000002d0: 2070 726f 6365 7373 696e 673c 2f61 3e20   processing</a> 
+000002e0: 7c0d 0a20 2020 2020 2020 203c 6120 6872  |..        <a hr
+000002f0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000300: 7562 2e63 6f6d 2f4d 5461 6e64 484a 2f66  ub.com/MTandHJ/f
+00000310: 7265 6572 6563 2f62 6c6f 622f 6d61 7374  reerec/blob/mast
+00000320: 6572 2f74 7261 696e 696e 6725 3230 616e  er/training%20an
+00000330: 6425 3230 7475 6e69 6e67 2e6d 6422 3e54  d%20tuning.md">T
+00000340: 7261 696e 696e 6720 616e 6420 5475 6e69  raining and Tuni
+00000350: 6e67 3c2f 613e 207c 0d0a 2020 2020 2020  ng</a> |..      
+00000360: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000370: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d54  ://github.com/MT
+00000380: 616e 6448 4a2f 5265 6342 6f61 7264 223e  andHJ/RecBoard">
+00000390: 5265 6342 6f61 7264 3c2f 613e 0d0a 2020  RecBoard</a>..  
+000003a0: 2020 3c2f 703e 0d0a 3c2f 6834 3e0d 0a0d    </p>..</h4>...
+000003b0: 0a46 7265 6552 6563 2069 7320 6120 7265  .FreeRec is a re
+000003c0: 706f 7369 746f 7279 2064 6573 6967 6e65  pository designe
+000003d0: 6420 666f 7220 6561 7379 2028 7265 636f  d for easy (reco
+000003e0: 6d6d 656e 6461 7469 6f6e 2920 6461 7461  mmendation) data
+000003f0: 2070 7265 2d70 726f 6365 7373 696e 6720   pre-processing 
+00000400: 616e 6420 6d6f 6465 6c20 7472 6169 6e69  and model traini
+00000410: 6e67 2e20 596f 7520 6172 6520 6672 6565  ng. You are free
+00000420: 2074 6f20 7370 6563 6966 7920 796f 7572   to specify your
+00000430: 206f 776e 2066 7261 6d65 776f 726b 2062   own framework b
+00000440: 6173 6564 206f 6e20 4672 6565 5265 632e  ased on FreeRec.
+00000450: 0d0a 0d0a 0d0a 2323 2052 6571 7569 7265  ......## Require
+00000460: 6d65 6e74 733a 200d 0a0d 0a50 7974 686f  ments: ....Pytho
+00000470: 6e20 3e3d 2033 2e39 207c 205b 5079 546f  n >= 3.9 | [PyTo
+00000480: 7263 6820 3e3d 322e 305d 2868 7474 7073  rch >=2.0](https
+00000490: 3a2f 2f70 7974 6f72 6368 2e6f 7267 2f29  ://pytorch.org/)
+000004a0: 207c 205b 546f 7263 6844 6174 6120 3e3d   | [TorchData >=
+000004b0: 302e 362e 305d 2868 7474 7073 3a2f 2f67  0.6.0](https://g
+000004c0: 6974 6875 622e 636f 6d2f 7079 746f 7263  ithub.com/pytorc
+000004d0: 682f 6461 7461 2920 7c20 5b50 7947 203e  h/data) | [PyG >
+000004e0: 3d32 2e33 5d28 6874 7470 733a 2f2f 7079  =2.3](https://py
+000004f0: 746f 7263 682d 6765 6f6d 6574 7269 632e  torch-geometric.
+00000500: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000510: 6e2f 6c61 7465 7374 2f6e 6f74 6573 2f69  n/latest/notes/i
+00000520: 6e73 7461 6c6c 6174 696f 6e2e 6874 6d6c  nstallation.html
+00000530: 2329 0d0a 0d0a 0d0a 6060 600d 0a63 6f6e  #)......```..con
+00000540: 6461 2063 7265 6174 6520 2d2d 6e61 6d65  da create --name
+00000550: 3d46 7265 6552 6563 2070 7974 686f 6e3d  =FreeRec python=
+00000560: 332e 390d 0a63 6f6e 6461 2061 6374 6976  3.9..conda activ
+00000570: 6174 6520 4672 6565 5265 630d 0a60 6060  ate FreeRec..```
+00000580: 0d0a 0d0a 0d0a 2a2a 4e6f 7465 3a2a 2a20  ......**Note:** 
+00000590: 4166 7465 7220 5079 546f 7263 6820 322e  After PyTorch 2.
+000005a0: 302c 2060 546f 7263 6844 6174 6160 2073  0, `TorchData` s
+000005b0: 6565 6d73 2074 6f20 6861 7665 2073 746f  eems to have sto
+000005c0: 7070 6564 2062 6569 6e67 2075 7064 6174  pped being updat
+000005d0: 6564 2c20 616e 6420 796f 7520 6361 6e20  ed, and you can 
+000005e0: 696e 7374 616c 6c20 6974 2077 6974 6820  install it with 
+000005f0: 602d 2d6e 6f2d 6465 7073 6020 746f 2061  `--no-deps` to a
+00000600: 766f 6964 2069 6e73 7461 6c6c 696e 6720  void installing 
+00000610: 6465 7065 6e64 656e 6369 6573 2e0d 0a0d  dependencies....
+00000620: 0a60 6060 0d0a 7069 7020 696e 7374 616c  .```..pip instal
+00000630: 6c20 2d2d 6e6f 2d64 6570 7320 746f 7263  l --no-deps torc
+00000640: 6864 6174 610d 0a60 6060 0d0a 0d0a 0d0a  hdata..```......
+00000650: 2323 2049 6e73 7461 6c6c 6174 696f 6e0d  ## Installation.
+00000660: 0a0d 0a20 2020 2070 6970 2069 6e73 7461  ...    pip insta
+00000670: 6c6c 2066 7265 6572 6563 0d0a 0d0a 6f72  ll freerec....or
+00000680: 2028 666f 7220 6c61 7465 7374 290d 0a0d   (for latest)...
+00000690: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+000006a0: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
+000006b0: 6875 622e 636f 6d2f 4d54 616e 6448 4a2f  hub.com/MTandHJ/
+000006c0: 6672 6565 7265 632e 6769 740d 0a0d 0a0d  freerec.git.....
+000006d0: 0a0d 0a23 2320 4461 7461 2050 6970 656c  ...## Data Pipel
+000006e0: 696e 650d 0a0d 0a3e 2052 6566 6572 2074  ine....> Refer t
+000006f0: 6f20 5b68 6572 655d 282e 2f64 6174 6173  o [here](./datas
+00000700: 6574 2532 3070 726f 6365 7373 696e 672e  et%20processing.
+00000710: 6d64 2920 666f 7220 6461 7461 7365 7420  md) for dataset 
+00000720: 7072 6f63 6573 7369 6e67 2061 6e64 2073  processing and s
+00000730: 706c 6974 7469 6e67 2e0d 0a0d 0a21 5b5d  plitting.....![]
+00000740: 2864 6f63 732f 7372 632f 7069 7065 6c69  (docs/src/pipeli
+00000750: 6e65 2e70 6e67 290d 0a0d 0a0d 0a23 2320  ne.png)......## 
+00000760: 5472 6169 6e69 6e67 2046 6c6f 770d 0a0d  Training Flow...
+00000770: 0a0d 0a21 5b5d 2864 6f63 732f 7372 632f  ...![](docs/src/
+00000780: 666c 6f77 2e70 6e67 290d 0a0d 0a0d 0a23  flow.png)......#
+00000790: 2320 5265 6665 7265 6e63 6520 436f 6465  # Reference Code
+000007a0: 0d0a 0d0a 2d20 546f 7263 6852 6563 3a20  ....- TorchRec: 
+000007b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007c0: 6f6d 2f70 7974 6f72 6368 2f74 6f72 6368  om/pytorch/torch
+000007d0: 7265 6320 0d0a 2d20 4465 6570 4354 522d  rec ..- DeepCTR-
+000007e0: 546f 7263 683a 2068 7474 7073 3a2f 2f67  Torch: https://g
+000007f0: 6974 6875 622e 636f 6d2f 7368 656e 7765  ithub.com/shenwe
+00000800: 6963 6865 6e2f 4465 6570 4354 522d 546f  ichen/DeepCTR-To
+00000810: 7263 680d 0a2d 2046 7578 6943 5452 3a20  rch..- FuxiCTR: 
+00000820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000830: 6f6d 2f78 7565 2d70 6169 2f46 7578 6943  om/xue-pai/FuxiC
+00000840: 5452 0d0a 2d20 4241 5253 3a20 6874 7470  TR..- BARS: http
+00000850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000860: 7065 6e62 656e 6368 6d61 726b 2f42 4152  penbenchmark/BAR
+00000870: 530d 0a2d 2052 6563 426f 6c65 3a20 6874  S..- RecBole: ht
+00000880: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000890: 2f52 5543 4149 426f 782f 5265 6342 6f6c  /RUCAIBox/RecBol
+000008a0: 650d 0a0d 0a0d 0a0d 0a23 2320 4163 6b6e  e........## Ackn
+000008b0: 6f77 6c65 6467 656d 656e 7473 0d0a 0d0a  owledgements....
+000008c0: 5468 616e 6b73 2074 6f20 4368 6174 4750  Thanks to ChatGP
+000008d0: 5420 666f 7220 7468 6520 616e 6e6f 7461  T for the annota
+000008e0: 7469 6f6e 206f 6620 736f 6d65 2063 6f64  tion of some cod
+000008f0: 652e 2046 6f72 2074 6869 7320 7265 6173  e. For this reas
+00000900: 6f6e 2c20 736f 6d65 206f 6620 7468 6520  on, some of the 
+00000910: 636f 6d6d 656e 7473 206d 6179 2062 6520  comments may be 
+00000920: 696c 6c6f 6769 6361 6c2e 0d0a            illogical...
```

### Comparing `freerec-0.7.5/freerec.egg-info/SOURCES.txt` & `freerec-0.8.1/freerec.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,48 +14,30 @@
 freerec.egg-info/PKG-INFO
 freerec.egg-info/SOURCES.txt
 freerec.egg-info/dependency_links.txt
 freerec.egg-info/entry_points.txt
 freerec.egg-info/requires.txt
 freerec.egg-info/top_level.txt
 freerec/data/__init__.py
-freerec/data/dataloader.py
 freerec/data/fields.py
 freerec/data/tags.py
-freerec/data/transformation.py
 freerec/data/utils.py
 freerec/data/datasets/__init__.py
+freerec/data/datasets/allrecipes.py
+freerec/data/datasets/amazon2014.py
+freerec/data/datasets/amazon2018.py
 freerec/data/datasets/base.py
-freerec/data/datasets/context/__init__.py
-freerec/data/datasets/context/amazon.py
-freerec/data/datasets/context/base.py
-freerec/data/datasets/context/mmrec.py
-freerec/data/datasets/context/mmssl.py
-freerec/data/datasets/general/__init__.py
-freerec/data/datasets/general/amazon.py
-freerec/data/datasets/general/base.py
-freerec/data/datasets/general/gowalla.py
-freerec/data/datasets/general/movielens.py
-freerec/data/datasets/general/yelp.py
-freerec/data/datasets/knowledge/__init__.py
-freerec/data/datasets/knowledge/base.py
-freerec/data/datasets/sequential/__init__.py
-freerec/data/datasets/sequential/amazon.py
-freerec/data/datasets/sequential/base.py
-freerec/data/datasets/sequential/movielens.py
-freerec/data/datasets/sequential/steam.py
-freerec/data/datasets/sequential/yelp.py
-freerec/data/datasets/session/__init__.py
-freerec/data/datasets/session/base.py
-freerec/data/datasets/session/diginetica.py
-freerec/data/datasets/session/yoochoose.py
+freerec/data/datasets/gowalla.py
+freerec/data/datasets/movielens.py
+freerec/data/datasets/tiktok.py
+freerec/data/datasets/yelp.py
 freerec/data/postprocessing/__init__.py
 freerec/data/postprocessing/base.py
+freerec/data/postprocessing/base.pyi
 freerec/data/postprocessing/column.py
 freerec/data/postprocessing/row.py
 freerec/data/postprocessing/sampler.py
 freerec/data/postprocessing/source.py
 freerec/data/preprocessing/__init__.py
 freerec/data/preprocessing/base.py
-freerec/data/preprocessing/datasets.py
 freerec/models/__init__.py
 freerec/models/base.py
```

### Comparing `freerec-0.7.5/setup.py` & `freerec-0.8.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import re
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 requires = [
     # "torchdata==0.4.1",
-    "freeplot>=0.4.5",
+    # "freeplot>=0.4.5",
     "PyYAML>=6.0",
     "tensorboard>=2.10.0",
-    "psutil>=5.9.0",
     "prettytable>=3.4.1"
 ]
 
 
 def get_property(prop, project):
     result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
     return result.group(1)
@@ -30,14 +29,19 @@
   author="MTandHJ",
   author_email="congxueric@gmail.com",
   description="PyTorch library for recommender systems",
   long_description=long_description,
   long_description_content_type="text/markdown",
   license='MIT License',
   url="https://github.com/MTandHJ/freerec",
+  package_data={
+      "freerec": [
+          "data/postprocessing/*.pyi",
+      ],
+  },
   packages=setuptools.find_packages(),
   python_requires='>=3.9',
   install_requires=requires,
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

