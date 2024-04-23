# Comparing `tmp/pydgn-1.5.3.tar.gz` & `tmp/pydgn-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydgn-1.5.3.tar", last modified: Wed Nov 15 17:39:55 2023, max compression
+gzip compressed data, was "pydgn-1.5.4.tar", last modified: Tue Apr 23 16:41:12 2024, max compression
```

## Comparing `pydgn-1.5.3.tar` & `pydgn-1.5.4.tar`

### file list

```diff
@@ -1,73 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.258732 pydgn-1.5.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2023-11-15 17:39:46.000000 pydgn-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2023-11-15 17:39:55.258732 pydgn-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2023-11-15 17:39:46.000000 pydgn-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.250732 pydgn-1.5.3/pydgn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/build_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.254732 pydgn-1.5.3/pydgn/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29660 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    40962 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/data/provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    46462 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/data/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/data/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.254732 pydgn-1.5.3/pydgn/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/evaluation/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    40108 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/evaluation/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/evaluation/random_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    13884 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/evaluation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.254732 pydgn-1.5.3/pydgn/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17117 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/experiment/semi_supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/experiment/supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/experiment/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8269 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/launch_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.254732 pydgn-1.5.3/pydgn/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/log/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.254732 pydgn-1.5.3/pydgn/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.254732 pydgn-1.5.3/pydgn/model/dgn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/dgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/dgn/toy_dgn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/dgn/toy_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.254732 pydgn-1.5.3/pydgn/model/readout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/readout/graph_readout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/readout/link_readout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/model/readout/node_readout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.258732 pydgn-1.5.3/pydgn/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.258732 pydgn-1.5.3/pydgn/training/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/engine_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (127)    47277 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/callback/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    41785 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.258732 pydgn-1.5.3/pydgn/training/event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/event/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/event/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-15 17:39:46.000000 pydgn-1.5.3/pydgn/training/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 17:39:55.250732 pydgn-1.5.3/pydgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2023-11-15 17:39:55.000000 pydgn-1.5.3/pydgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2023-11-15 17:39:55.000000 pydgn-1.5.3/pydgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 17:39:55.000000 pydgn-1.5.3/pydgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-15 17:39:55.000000 pydgn-1.5.3/pydgn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-15 17:39:55.000000 pydgn-1.5.3/pydgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-15 17:39:55.000000 pydgn-1.5.3/pydgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-11-15 17:39:46.000000 pydgn-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 17:39:55.258732 pydgn-1.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-23 16:41:08.000000 pydgn-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-23 16:41:12.833507 pydgn-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-23 16:41:08.000000 pydgn-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.825507 pydgn-1.5.4/pydgn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.825507 pydgn-1.5.4/pydgn/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29660 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40962 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46462 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.825507 pydgn-1.5.4/pydgn/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40108 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/semi_supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/log/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/model/dgn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/dgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/dgn/toy_dgn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/dgn/toy_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/model/readout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/graph_readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/link_readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/node_readout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/pydgn/pydgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/pydgn/training/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/engine_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41785 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/pydgn/training/event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-23 16:41:08.000000 pydgn-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:41:12.833507 pydgn-1.5.4/setup.cfg
```

### Comparing `pydgn-1.5.3/LICENSE` & `pydgn-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/PKG-INFO` & `pydgn-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydgn
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python Package for Deep Graph Networks
 Author-email: Federico Errica <f.errica@protonmail.com>
 Project-URL: Homepage, https://pydgn.readthedocs.io/en/latest/
 Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydgn-1.5.3/README.md` & `pydgn-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/data/dataset.py` & `pydgn-1.5.4/pydgn/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/data/provider.py` & `pydgn-1.5.4/pydgn/data/provider.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/data/sampler.py` & `pydgn-1.5.4/pydgn/data/sampler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/data/splitter.py` & `pydgn-1.5.4/pydgn/data/splitter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/data/transform.py` & `pydgn-1.5.4/pydgn/data/transform.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/data/util.py` & `pydgn-1.5.4/pydgn/data/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/evaluation/config.py` & `pydgn-1.5.4/pydgn/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/evaluation/evaluator.py` & `pydgn-1.5.4/pydgn/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/evaluation/grid.py` & `pydgn-1.5.4/pydgn/evaluation/grid.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/evaluation/random_search.py` & `pydgn-1.5.4/pydgn/evaluation/random_search.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/evaluation/util.py` & `pydgn-1.5.4/pydgn/evaluation/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import datetime
 import json
 import math
 import os
 import random
 from typing import Tuple, Callable, List
 
+import torch
 import tqdm
 
+from pydgn.data.dataset import DatasetInterface
 from pydgn.experiment.util import s2c
+from pydgn.model.interface import ModelInterface
 from pydgn.static import *
 
 
 def return_class_and_args(
     config: dict, key: str, return_class_name: bool = False
 ) -> Tuple[Callable[..., object], dict]:
     r"""
@@ -345,14 +348,17 @@
     :param model_selection_folder: path to the folder of a model selection,
         that is, your_results_path/..../MODEL_SELECTION/
     :return: a list of dictionaries, one per configuration, each with an extra
         key "exp_folder" which identifies the config folder.
     """
     config_directory = os.path.join(model_selection_folder)
 
+    if not os.path.exists(config_directory):
+        raise FileNotFoundError(f"Directory not found: {config_directory}")
+
     folder_names = []
     for _, dirs, _ in os.walk(config_directory):
         for d in dirs:
             if "config" in d:
                 folder_names.append(os.path.join(config_directory, d))
         break  # do not recursively explore subfolders
 
@@ -444,7 +450,85 @@
                     keep = False
                     break
 
         if keep:
             filtered_config_list.append(config)
 
     return filtered_config_list
+
+
+def retrieve_best_configuration(model_selection_folder) -> dict:
+    """
+    Once the experiments are done, retrieves the winning configuration from
+     a specific model selection folder, and returns it as a dictionaries
+
+    :param model_selection_folder: path to the folder of a model selection,
+        that is, your_results_path/..../MODEL_SELECTION/
+    :return: a dictionary with info about the best configuration
+    """
+    config_directory = os.path.join(model_selection_folder)
+
+    if not os.path.exists(config_directory):
+        raise FileNotFoundError(f"Directory not found: {config_directory}")
+
+    best_config = json.load(
+        open(os.path.join(config_directory, "winner_config.json"), "rb")
+    )
+    return best_config
+
+
+def instantiate_dataset_from_config(config: dict) -> DatasetInterface:
+    """
+    Instantiate a dataset from a configuration file.
+    :param config (dict): the configuration file
+    :return: an instance of DatasetInterface, i.e., the dataset
+    """
+    data_root = config[CONFIG][DATA_ROOT]
+    dataset_name = config[CONFIG][DATASET]
+    dataset_class = s2c(config[CONFIG][DATASET_CLASS])
+
+    return dataset_class(data_root, dataset_name)
+
+
+def instantiate_model_from_config(config: dict,
+                                  dataset: DatasetInterface,
+                                  config_type: str = "supervised_config") -> ModelInterface:
+    """
+    Instantiate a model from a configuration file.
+    :param config (dict): the configuration file
+    :param dataset (DatasetInterface): the dataset used in the experiment
+    :param config_type (str): the type of model in ["supervised_config", "unsupervised_config"],
+        as written on the YAML experiment configuration file. Defaults to "supervised_config"
+    :return: an instance of ModelInterface, i.e., the model
+    """
+    config_ = config[CONFIG][config_type]
+    readout_class = s2c(config_["readout"])
+
+    model_class = s2c(config_[MODEL])
+    model = model_class(dataset.dim_node_features,
+                        dataset.dim_edge_features,
+                        dataset.dim_target,
+                        readout_class,
+                        config=config_)
+
+    return model
+
+
+def load_checkpoint(checkpoint_path: str, model: ModelInterface,
+                    device: torch.device):
+    """
+    Load a checkpoint from a checkpoint file into a model.
+    :param checkpoint_path: the checkpoint file path
+    :param model (ModelInterface): the model
+    :param device (torch.device): the device, e.g, "cpu" or "cuda"
+    """
+    ckpt_dict = torch.load(
+        checkpoint_path, map_location="cpu" if device == "cpu" else None
+    )
+    model_state = ckpt_dict[MODEL_STATE]
+
+    # Needed only when moving from cpu to cuda (due to changes in config
+    # file). Move all parameters to cuda.
+    for param in model_state.keys():
+        model_state[param] = model_state[param].to(device)
+
+    model.load_state_dict(model_state)
```

### Comparing `pydgn-1.5.3/pydgn/experiment/experiment.py` & `pydgn-1.5.4/pydgn/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/experiment/semi_supervised_task.py` & `pydgn-1.5.4/pydgn/experiment/semi_supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/experiment/supervised_task.py` & `pydgn-1.5.4/pydgn/experiment/supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/log/logger.py` & `pydgn-1.5.4/pydgn/log/logger.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/model/dgn/toy_dgn.py` & `pydgn-1.5.4/pydgn/model/dgn/toy_dgn.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/model/dgn/toy_mlp.py` & `pydgn-1.5.4/pydgn/model/dgn/toy_mlp.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/model/interface.py` & `pydgn-1.5.4/pydgn/model/interface.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/model/readout/graph_readout.py` & `pydgn-1.5.4/pydgn/model/readout/graph_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/model/readout/link_readout.py` & `pydgn-1.5.4/pydgn/model/readout/link_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/model/readout/node_readout.py` & `pydgn-1.5.4/pydgn/model/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/callback/early_stopping.py` & `pydgn-1.5.4/pydgn/training/callback/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/callback/engine_callback.py` & `pydgn-1.5.4/pydgn/training/callback/engine_callback.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/callback/gradient_clipping.py` & `pydgn-1.5.4/pydgn/training/callback/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/callback/metric.py` & `pydgn-1.5.4/pydgn/training/callback/metric.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/callback/optimizer.py` & `pydgn-1.5.4/pydgn/training/callback/optimizer.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/callback/plotter.py` & `pydgn-1.5.4/pydgn/training/callback/plotter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/callback/scheduler.py` & `pydgn-1.5.4/pydgn/training/callback/scheduler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/engine.py` & `pydgn-1.5.4/pydgn/training/engine.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/event/dispatcher.py` & `pydgn-1.5.4/pydgn/training/event/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/event/handler.py` & `pydgn-1.5.4/pydgn/training/event/handler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/event/state.py` & `pydgn-1.5.4/pydgn/training/event/state.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/profiler.py` & `pydgn-1.5.4/pydgn/training/profiler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn/training/util.py` & `pydgn-1.5.4/pydgn/training/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.3/pydgn.egg-info/PKG-INFO` & `pydgn-1.5.4/pydgn/pydgn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydgn
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python Package for Deep Graph Networks
 Author-email: Federico Errica <f.errica@protonmail.com>
 Project-URL: Homepage, https://pydgn.readthedocs.io/en/latest/
 Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydgn-1.5.3/pydgn.egg-info/SOURCES.txt` & `pydgn-1.5.4/pydgn/pydgn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-pydgn/__init__.py
-pydgn/build_dataset.py
-pydgn/launch_experiment.py
-pydgn/static.py
-pydgn.egg-info/PKG-INFO
-pydgn.egg-info/SOURCES.txt
-pydgn.egg-info/dependency_links.txt
-pydgn.egg-info/entry_points.txt
-pydgn.egg-info/requires.txt
-pydgn.egg-info/top_level.txt
 pydgn/data/__init__.py
 pydgn/data/dataset.py
 pydgn/data/provider.py
 pydgn/data/sampler.py
 pydgn/data/splitter.py
 pydgn/data/transform.py
 pydgn/data/util.py
@@ -36,14 +26,20 @@
 pydgn/model/dgn/__init__.py
 pydgn/model/dgn/toy_dgn.py
 pydgn/model/dgn/toy_mlp.py
 pydgn/model/readout/__init__.py
 pydgn/model/readout/graph_readout.py
 pydgn/model/readout/link_readout.py
 pydgn/model/readout/node_readout.py
+pydgn/pydgn.egg-info/PKG-INFO
+pydgn/pydgn.egg-info/SOURCES.txt
+pydgn/pydgn.egg-info/dependency_links.txt
+pydgn/pydgn.egg-info/entry_points.txt
+pydgn/pydgn.egg-info/requires.txt
+pydgn/pydgn.egg-info/top_level.txt
 pydgn/training/__init__.py
 pydgn/training/engine.py
 pydgn/training/profiler.py
 pydgn/training/util.py
 pydgn/training/callback/__init__.py
 pydgn/training/callback/early_stopping.py
 pydgn/training/callback/engine_callback.py
```

### Comparing `pydgn-1.5.3/pyproject.toml` & `pydgn-1.5.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.packages.find]
+where = ["pydgn"]
+
 [project]
 name = "pydgn"
-version = "1.5.3"
+version = "1.5.4"
 description = "A Python Package for Deep Graph Networks"
 authors = [ { name="Federico Errica", email="f.errica@protonmail.com" } ]
 readme = "README.md"
 keywords = ["deep-graph-networks", "evaluation-framework", "deep-learning-for-graphs"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
```

