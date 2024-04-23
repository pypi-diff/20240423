# Comparing `tmp/tui_dsmt-202404181339.tar.gz` & `tmp/tui_dsmt-202404230921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404181339.tar", last modified: Thu Apr 18 13:39:27 2024, max compression
+gzip compressed data, was "tui_dsmt-202404230921.tar", last modified: Tue Apr 23 09:21:51 2024, max compression
```

## Comparing `tui_dsmt-202404181339.tar` & `tui_dsmt-202404230921.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.302510 tui_dsmt-202404181339/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-18 13:39:27.298510 tui_dsmt-202404181339/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 13:39:27.302510 tui_dsmt-202404181339/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.290510 tui_dsmt-202404181339/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.290510 tui_dsmt-202404181339/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-16 12:44:18.000000 tui_dsmt-202404181339/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.294510 tui_dsmt-202404181339/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19108 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.294510 tui_dsmt-202404181339/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-18 13:39:20.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-18 13:39:20.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-16 12:44:18.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)   112423 2024-04-18 13:39:20.000000 tui_dsmt-202404181339/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.298510 tui_dsmt-202404181339/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-16 12:44:18.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-16 12:44:18.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-16 12:44:18.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-16 12:44:18.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5734 2024-04-18 13:39:20.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.298510 tui_dsmt-202404181339/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-18 13:39:20.000000 tui_dsmt-202404181339/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404181339/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.298510 tui_dsmt-202404181339/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404181339/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:39:27.298510 tui_dsmt-202404181339/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-18 13:39:27.000000 tui_dsmt-202404181339/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1582 2024-04-18 13:39:27.000000 tui_dsmt-202404181339/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 13:39:27.000000 tui_dsmt-202404181339/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-18 13:39:27.000000 tui_dsmt-202404181339/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-18 13:39:27.000000 tui_dsmt-202404181339/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1167 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.160547 tui_dsmt-202404230921/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.160547 tui_dsmt-202404230921/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.164547 tui_dsmt-202404230921/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/PAM.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19467 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.168547 tui_dsmt-202404230921/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-18 13:39:20.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-18 13:39:20.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)   112423 2024-04-18 13:39:20.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.172547 tui_dsmt-202404230921/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     5766 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.172547 tui_dsmt-202404230921/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.172547 tui_dsmt-202404230921/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1613 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202404181339/PKG-INFO` & `tui_dsmt-202404230921/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404181339
+Version: 202404230921
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jupyter
 Requires-Dist: ipywidgets
 Requires-Dist: checkmarkandcross
+Requires-Dist: matplotlib~=3.8.4
 Requires-Dist: networkx~=3.2.1
 Requires-Dist: plotly~=5.20.0
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: pyarrow~=15.0.2
-Requires-Dist: scikit-learn~=1.4.0
+Requires-Dist: scikit-learn~=1.4.2
+Requires-Dist: scikit-learn-extra~=0.3.0
 
 everything you need for our jupyter notebooks
```

### Comparing `tui_dsmt-202404181339/setup.py` & `tui_dsmt-202404230921/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,18 @@
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     python_requires='>=3.10',
     install_requires=[
         'jupyter',
         'ipywidgets',
         'checkmarkandcross',
+        'matplotlib~=3.8.4',
         'networkx~=3.2.1',
         'plotly~=5.20.0',
         'pandas~=2.2.1',
         'pyarrow~=15.0.2',
-        'scikit-learn~=1.4.0'
+        'scikit-learn~=1.4.2',
+        'scikit-learn-extra~=0.3.0'
     ],
     package_data={},
     include_package_data=True
 )
```

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/__init__.py` & `tui_dsmt-202404230921/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202404230921/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202404230921/src/tui_dsmt/clustering/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,7 +180,15 @@
 })
 
 # 4-132
 clustering_example3 = pd.DataFrame({
     'x': [1., 2., 2., 3., 4., 4., 4., 5., 6.],
     'y': [1.5, 4., 3., 4., 2., 3., 6., 7., 7.],
 })
+
+# 2-27
+clustering_example4 = pd.DataFrame({
+    'x': [1.0, 2.5, 0.5, 2.0, 1.0, 1.0, 1.5, 2.5, 2.0, 1.5, 3.0, 4.0, 1.0, 2.0, 3.0, 3.5, 1.5, 3.0, 5.5, 5.5, 6.0, 6.0,
+          6.5, 6.5, 6.5, 7.5, 7.5],
+    'y': [1.0, 0.5, 1.5, 1.5, 2.0, 2.5, 2.5, 2.0, 3.0, 6.5, 6.5, 6.5, 5.5, 5.5, 6.0, 5.5, 5.0, 4.5, 3.0, 4.0, 3.0, 4.5,
+          2.5, 3.5, 5.0, 4.0, 5.0]
+})
```

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202404230921/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202404230921/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202404230921/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/HashTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202404230921/src/tui_dsmt/fpm/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/game.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/html.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
                 {nodes_html_str}
             </div>
         </div>
     ''', f'''
         #{wrapper_id} {{
             padding: calc({node_height} / 2) calc({node_width} / 2);
             box-sizing: border-box;
+            overflow-y: hidden;
         }}
     
         #{wrapper_id} .node-container {{
             width: 100%;
             max-width: {max_width};
             height: {display_height};
             position: relative;
```

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202404230921/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202404230921/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404181339/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202404230921/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404181339
+Version: 202404230921
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jupyter
 Requires-Dist: ipywidgets
 Requires-Dist: checkmarkandcross
+Requires-Dist: matplotlib~=3.8.4
 Requires-Dist: networkx~=3.2.1
 Requires-Dist: plotly~=5.20.0
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: pyarrow~=15.0.2
-Requires-Dist: scikit-learn~=1.4.0
+Requires-Dist: scikit-learn~=1.4.2
+Requires-Dist: scikit-learn-extra~=0.3.0
 
 everything you need for our jupyter notebooks
```

### Comparing `tui_dsmt-202404181339/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202404230921/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 setup.py
 src/tui_dsmt/__init__.py
 src/tui_dsmt.egg-info/PKG-INFO
 src/tui_dsmt.egg-info/SOURCES.txt
 src/tui_dsmt.egg-info/dependency_links.txt
 src/tui_dsmt.egg-info/requires.txt
 src/tui_dsmt.egg-info/top_level.txt
+src/tui_dsmt/clustering/PAM.py
 src/tui_dsmt/clustering/__init__.py
 src/tui_dsmt/clustering/animation.py
 src/tui_dsmt/clustering/datasets.py
 src/tui_dsmt/clustering/draw.py
 src/tui_dsmt/clustering/evaluation.py
 src/tui_dsmt/clustering/hierarchical.py
 src/tui_dsmt/clustering/interactive.py
```

