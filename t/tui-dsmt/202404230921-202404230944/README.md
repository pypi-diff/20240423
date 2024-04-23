# Comparing `tmp/tui_dsmt-202404230921.tar.gz` & `tmp/tui_dsmt-202404230944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404230921.tar", last modified: Tue Apr 23 09:21:51 2024, max compression
+gzip compressed data, was "tui_dsmt-202404230944.tar", last modified: Tue Apr 23 09:44:24 2024, max compression
```

## Comparing `tui_dsmt-202404230921.tar` & `tui_dsmt-202404230944.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1167 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.160547 tui_dsmt-202404230921/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.160547 tui_dsmt-202404230921/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.164547 tui_dsmt-202404230921/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/PAM.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19467 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.168547 tui_dsmt-202404230921/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-18 13:39:20.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-18 13:39:20.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)   112423 2024-04-18 13:39:20.000000 tui_dsmt-202404230921/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.172547 tui_dsmt-202404230921/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-16 12:44:34.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5766 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.172547 tui_dsmt-202404230921/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-23 09:21:43.000000 tui_dsmt-202404230921/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404230921/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.172547 tui_dsmt-202404230921/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404230921/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:21:51.176548 tui_dsmt-202404230921/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1613 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-23 09:21:51.000000 tui_dsmt-202404230921/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.428511 tui_dsmt-202404230944/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 09:44:24.428511 tui_dsmt-202404230944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 09:44:24.428511 tui_dsmt-202404230944/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1167 2024-04-23 09:22:23.000000 tui_dsmt-202404230944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.408511 tui_dsmt-202404230944/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.412511 tui_dsmt-202404230944/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-16 12:44:18.000000 tui_dsmt-202404230944/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.416511 tui_dsmt-202404230944/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2024-04-23 09:22:23.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/PAM.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-23 09:22:23.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19467 2024-04-23 09:22:23.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.420511 tui_dsmt-202404230944/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-18 13:39:20.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-18 13:39:20.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-16 12:44:18.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)   112423 2024-04-18 13:39:20.000000 tui_dsmt-202404230944/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.428511 tui_dsmt-202404230944/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-16 12:44:18.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-16 12:44:18.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-16 12:44:18.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-16 12:44:18.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     5766 2024-04-23 09:22:23.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.428511 tui_dsmt-202404230944/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2024-04-23 09:44:16.000000 tui_dsmt-202404230944/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404230944/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.428511 tui_dsmt-202404230944/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404230944/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:44:24.428511 tui_dsmt-202404230944/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 09:44:24.000000 tui_dsmt-202404230944/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1613 2024-04-23 09:44:24.000000 tui_dsmt-202404230944/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 09:44:24.000000 tui_dsmt-202404230944/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-23 09:44:24.000000 tui_dsmt-202404230944/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-23 09:44:24.000000 tui_dsmt-202404230944/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202404230921/PKG-INFO` & `tui_dsmt-202404230944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404230921
+Version: 202404230944
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404230921/setup.py` & `tui_dsmt-202404230944/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/__init__.py` & `tui_dsmt-202404230944/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/clustering/PAM.py` & `tui_dsmt-202404230944/src/tui_dsmt/clustering/PAM.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202404230944/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202404230944/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202404230944/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202404230944/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202404230944/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/HashTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202404230944/src/tui_dsmt/fpm/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/game.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/html.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/html.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202404230944/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404230921/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202404230944/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,43 @@
 import json
 import os
 from typing import Dict, Optional, List
 from uuid import uuid4
 
-from IPython.core.display import HTML
+from IPython.core.display import HTML, display_html
 
+# location of this file is required to load resource urls
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 
 
+# read and inject required files as soon as this class is loaded
+def __init():
+    with open(os.path.join(__location__, 'resources', 'vue-3.4.24.js')) as vue_file:
+        vue = vue_file.read()
+
+    display_html(HTML(f'''
+        <script type="text/javascript">
+            {vue}
+        </script>
+    '''))
+
+    with open(os.path.join(__location__, 'resources', 'style.css')) as css_file:
+        css = css_file.read()
+
+    display_html(HTML(f'''
+        <style type="text/css">
+            {css}
+        </style>
+    '''))
+
+
+__init()
+
+
+# main class
 class JupyterAnimation(HTML):
     def __init__(self,
                  html: str, frames: Dict[str, Dict],
                  style: Optional[List[str] | str] = None, js: List[str] | str = None,
                  fast_forward: bool = False):
         self._html: str = html
         self._frames: Dict[str, Dict] = frames
@@ -29,17 +55,14 @@
 
         self._id: str = str(uuid4()).replace('-', '')
 
         super().__init__(self._construct())
 
     def _construct(self) -> str:
         # read templates from file
-        with open(os.path.join(__location__, 'resources', 'style.css')) as css_file:
-            css = css_file.read()
-
         if len(self._frames) > 1:
             if self._fast_forward:
                 filename = 'controls-ff.html'
             else:
                 filename = 'controls.html'
 
             with open(os.path.join(__location__, 'resources', filename)) as html_file:
@@ -58,24 +81,22 @@
             '__key': key,
             **frame
         } for key, frame in self._frames.items()], indent=4)
 
         # return string containing the content
         return f'''
             <style type="text/css">
-                {css}
                 {self._style}
             </style>
             
             <div id="container_{self._id}">
                 {self._html}
                 {html}
             </div>
             
-            <script type="text/javascript" async="false" src="https://unpkg.com/vue@3/dist/vue.global.prod.js"></script>
             <script type="text/javascript">
                 (function() {{
                     {js}
                     
                     app.frames = {frames}
                     app.mount('#container_{self._id}')
                 }})()
```

### Comparing `tui_dsmt-202404230921/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202404230944/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404230921
+Version: 202404230944
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404230921/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202404230944/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

