# Comparing `tmp/explainitall-1.0.0.tar.gz` & `tmp/explainitall-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainitall-1.0.0.tar", last modified: Sun Apr 21 06:10:54 2024, max compression
+gzip compressed data, was "explainitall-1.0.1.tar", last modified: Tue Apr 23 19:54:14 2024, max compression
```

## Comparing `explainitall-1.0.0.tar` & `explainitall-1.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)    11357 2024-04-21 05:36:03.000000 explainitall-1.0.0/LICENSE
--rw-r--r--   0 laptop    (1000) laptop    (1000)     6072 2024-04-21 06:10:54.076128 explainitall-1.0.0/PKG-INFO
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     5378 2024-04-21 05:36:03.000000 explainitall-1.0.0/README.md
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.072128 explainitall-1.0.0/explainitall/
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.072128 explainitall-1.0.0/explainitall/QA/
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.072128 explainitall-1.0.0/explainitall/QA/extractive_qa_sbert/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     6777 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/QA/extractive_qa_sbert/QABotsBase.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1912 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/QA/extractive_qa_sbert/SVDBert.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.072128 explainitall-1.0.0/explainitall/QA/interp_qa/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     3629 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/QA/interp_qa/KNNWithGenerative.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        0 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/__init__.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     7261 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/clusters.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.072128 explainitall-1.0.0/explainitall/embedder_interp/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2329 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/embedder_interp/embd_interpret.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.072128 explainitall-1.0.0/explainitall/fast_tuning/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     4722 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/Embedder.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      185 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/ExpertBase.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2490 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/SimpleModelCreator.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/explainitall/fast_tuning/generators/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     5632 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/generators/GeneratorWithExpert.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      294 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/generators/MCExpert.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2325 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/generators/MCModel.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1187 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/generators/SimpleGenerator.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/explainitall/fast_tuning/trainers/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2593 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/trainers/DenceKerasTrainer.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2971 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/trainers/HMMTrainer.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2550 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/fast_tuning/trainers/ProjectionTrainer.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/explainitall/gpt_like_interp/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        0 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/gpt_like_interp/__init__.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     3460 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/gpt_like_interp/downloader.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     8521 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/gpt_like_interp/inseq_helpers.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     4483 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/gpt_like_interp/interp.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1912 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/gpt_like_interp/viz.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/explainitall/gui/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      666 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/gui/df_to_heatmap_plot.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)    20087 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/gui/interface.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/explainitall/metrics/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2172 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/CheckingForHallucinations.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     4002 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/Metrics.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1621 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/Metrics_calculator.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      690 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/create_database.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     4097 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/helpers.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     9815 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/metric_calculation_interface.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1233 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_L.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      888 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_N.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1517 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_l_helpers.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1125 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_n_helpers.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2024 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/nlp.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     3283 2024-04-21 05:36:03.000000 explainitall-1.0.0/explainitall/stat_helpers.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/explainitall.egg-info/
--rw-r--r--   0 laptop    (1000) laptop    (1000)     6072 2024-04-21 06:10:54.000000 explainitall-1.0.0/explainitall.egg-info/PKG-INFO
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     1816 2024-04-21 06:10:54.000000 explainitall-1.0.0/explainitall.egg-info/SOURCES.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)        1 2024-04-21 06:10:54.000000 explainitall-1.0.0/explainitall.egg-info/dependency_links.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      305 2024-04-21 06:10:54.000000 explainitall-1.0.0/explainitall.egg-info/requires.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       13 2024-04-21 06:10:54.000000 explainitall-1.0.0/explainitall.egg-info/top_level.txt
--rw-rw-r--   0 laptop    (1000) laptop    (1000)       38 2024-04-21 06:10:54.076128 explainitall-1.0.0/setup.cfg
--rw-rw-r--   0 laptop    (1000) laptop    (1000)      524 2024-04-21 05:36:03.000000 explainitall-1.0.0/setup.py
-drwxrwxr-x   0 laptop    (1000) laptop    (1000)        0 2024-04-21 06:10:54.076128 explainitall-1.0.0/tests/
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     2419 2024-04-21 05:36:03.000000 explainitall-1.0.0/tests/test_inseq_helpers.py
--rw-rw-r--   0 laptop    (1000) laptop    (1000)     4140 2024-04-21 05:36:03.000000 explainitall-1.0.0/tests/test_stat_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.181783 explainitall-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-23 19:53:25.000000 explainitall-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5497 2024-04-23 19:54:14.181783 explainitall-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5378 2024-04-23 19:53:25.000000 explainitall-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.174782 explainitall-1.0.1/explainitall/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.172782 explainitall-1.0.1/explainitall/QA/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.175782 explainitall-1.0.1/explainitall/QA/extractive_qa_sbert/
+-rw-r--r--   0 root         (0) root         (0)     6777 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/QA/extractive_qa_sbert/QABotsBase.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/QA/extractive_qa_sbert/SVDBert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.176782 explainitall-1.0.1/explainitall/QA/interp_qa/
+-rw-r--r--   0 root         (0) root         (0)     3628 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/QA/interp_qa/KNNWithGenerative.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/clusters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.176782 explainitall-1.0.1/explainitall/embedder_interp/
+-rw-r--r--   0 root         (0) root         (0)     2329 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/embedder_interp/embd_interpret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.176782 explainitall-1.0.1/explainitall/fast_tuning/
+-rw-r--r--   0 root         (0) root         (0)     4722 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/Embedder.py
+-rw-r--r--   0 root         (0) root         (0)      185 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/ExpertBase.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/SimpleModelCreator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.177782 explainitall-1.0.1/explainitall/fast_tuning/generators/
+-rw-r--r--   0 root         (0) root         (0)     5632 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/generators/GeneratorWithExpert.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/generators/MCExpert.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/generators/MCModel.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/generators/SimpleGenerator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.177782 explainitall-1.0.1/explainitall/fast_tuning/trainers/
+-rw-r--r--   0 root         (0) root         (0)     2593 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/trainers/DenceKerasTrainer.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/trainers/HMMTrainer.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/fast_tuning/trainers/ProjectionTrainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.178782 explainitall-1.0.1/explainitall/gpt_like_interp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/gpt_like_interp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/gpt_like_interp/downloader.py
+-rw-r--r--   0 root         (0) root         (0)     8521 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/gpt_like_interp/inseq_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/gpt_like_interp/interp.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/gpt_like_interp/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.179782 explainitall-1.0.1/explainitall/gui/
+-rw-r--r--   0 root         (0) root         (0)      888 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/gui/df_to_heatmap_plot.py
+-rw-r--r--   0 root         (0) root         (0)    20238 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/gui/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.179782 explainitall-1.0.1/explainitall/metrics/
+-rw-r--r--   0 root         (0) root         (0)     2172 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/CheckingForHallucinations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.180782 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/
+-rw-r--r--   0 root         (0) root         (0)     3849 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/Metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/Metrics_calculator.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/create_database.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     9489 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/metric_calculation_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_L.py
+-rw-r--r--   0 root         (0) root         (0)      888 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_N.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_l_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_n_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2024-04-23 19:53:25.000000 explainitall-1.0.1/explainitall/stat_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.175782 explainitall-1.0.1/explainitall.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5497 2024-04-23 19:54:13.000000 explainitall-1.0.1/explainitall.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-23 19:54:14.000000 explainitall-1.0.1/explainitall.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 19:54:13.000000 explainitall-1.0.1/explainitall.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-23 19:54:13.000000 explainitall-1.0.1/explainitall.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-23 19:54:13.000000 explainitall-1.0.1/explainitall.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 19:54:14.181783 explainitall-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      524 2024-04-23 19:53:25.000000 explainitall-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:54:14.181783 explainitall-1.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-23 19:53:25.000000 explainitall-1.0.1/tests/test_inseq_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4140 2024-04-23 19:53:25.000000 explainitall-1.0.1/tests/test_stat_helpers.py
```

### Comparing `explainitall-1.0.0/LICENSE` & `explainitall-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/PKG-INFO` & `explainitall-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,12 @@
 Metadata-Version: 2.1
 Name: explainitall
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gensim==4.3.2
-Requires-Dist: gradio==4.4.1
-Requires-Dist: gradio_client==0.7.0
-Requires-Dist: inseq==0.5.0
-Requires-Dist: matplotlib==3.8.4
-Requires-Dist: nltk==3.8.1
-Requires-Dist: pandas==2.2.1
-Requires-Dist: pymorphy2==0.9.1
-Requires-Dist: scikit-learn==1.4.1.post1
-Requires-Dist: seaborn==0.13.2
-Requires-Dist: sentence_transformers==2.6.1
-Requires-Dist: SQLAlchemy==2.0.29
-Requires-Dist: statsmodels==0.14.1
-Requires-Dist: torch>=2.0
-Requires-Dist: transformers>=4.39
-Requires-Dist: uvicorn==0.29
-Requires-Dist: scipy==1.12.0
-Requires-Dist: numpy==1.26.4
 
 # **ExplainitAll**
 
 **ExplainitAll** — это библиотека для интерпретируемого ИИ, предназначенная для интерпретации генеративных моделей (
 GPT-like), и векторизаторов, например, Sbert. Библиотека предоставляет пользователям инструменты для анализа и понимания
 работы этих сложных моделей. Кроме того, содержит модули RAG QA, fast_tuning и пользовательский интерфейс.
```

### Comparing `explainitall-1.0.0/README.md` & `explainitall-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/QA/extractive_qa_sbert/QABotsBase.py` & `explainitall-1.0.1/explainitall/QA/extractive_qa_sbert/QABotsBase.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/QA/extractive_qa_sbert/SVDBert.py` & `explainitall-1.0.1/explainitall/QA/extractive_qa_sbert/SVDBert.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/QA/interp_qa/KNNWithGenerative.py` & `explainitall-1.0.1/explainitall/QA/interp_qa/KNNWithGenerative.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from explainitall.QA.extractive_qa_sbert.QABotsBase import SimpleTransformer
 
 nltk.download('punkt')
 
 
 class FredStruct:
 
-    def __init__(self, path='FractalGPT/FRED-T5-Interp', device='cpu'):
+    def __init__(self, path='Ponimash/FredInterpreter', device='cpu'):
         self.tokenizer = AutoTokenizer.from_pretrained(path)
         self.fred_model = AutoModelForSeq2SeqLM.from_pretrained(path)
         self.fred_model = self.fred_model.to(device)
         self.fred_model.eval()
 
     def get_model(self):
         return self.fred_model
```

### Comparing `explainitall-1.0.0/explainitall/clusters.py` & `explainitall-1.0.1/explainitall/clusters.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/embedder_interp/embd_interpret.py` & `explainitall-1.0.1/explainitall/embedder_interp/embd_interpret.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/Embedder.py` & `explainitall-1.0.1/explainitall/fast_tuning/Embedder.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/SimpleModelCreator.py` & `explainitall-1.0.1/explainitall/fast_tuning/SimpleModelCreator.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/generators/GeneratorWithExpert.py` & `explainitall-1.0.1/explainitall/fast_tuning/generators/GeneratorWithExpert.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/generators/MCModel.py` & `explainitall-1.0.1/explainitall/fast_tuning/generators/MCModel.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/generators/SimpleGenerator.py` & `explainitall-1.0.1/explainitall/fast_tuning/generators/SimpleGenerator.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/trainers/DenceKerasTrainer.py` & `explainitall-1.0.1/explainitall/fast_tuning/trainers/DenceKerasTrainer.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/trainers/HMMTrainer.py` & `explainitall-1.0.1/explainitall/fast_tuning/trainers/HMMTrainer.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/fast_tuning/trainers/ProjectionTrainer.py` & `explainitall-1.0.1/explainitall/fast_tuning/trainers/ProjectionTrainer.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/gpt_like_interp/downloader.py` & `explainitall-1.0.1/explainitall/gpt_like_interp/downloader.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/gpt_like_interp/inseq_helpers.py` & `explainitall-1.0.1/explainitall/gpt_like_interp/inseq_helpers.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/gpt_like_interp/interp.py` & `explainitall-1.0.1/explainitall/gpt_like_interp/interp.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,13 +93,17 @@
         word_imp_df = inseq_helpers.attr_to_df(group_attr)
         word_imp_norm_df = inseq_helpers.attr_to_df(norm_attr)
 
         cluster_interpreter = clusters.ClusterInterpreter(clusters_discr=cluster_desc,
                                                           cluster_manager=self._cluster_manager)
 
         cluster_imp_df = cluster_interpreter.get_cluster_importance_df(self.attributions)
-        cluster_imp_aggr_df = aggregate_cluster_df(cluster_imp_df, aggr_f=aggr_f)
+        try:
+            cluster_imp_aggr_df = aggregate_cluster_df(cluster_imp_df, aggr_f=aggr_f)
+        except Exception as e:
+            print(f"Неверно заданы выходные кластеры: {e}")
+            cluster_imp_aggr_df = pd.DataFrame()
 
         return ExplainerGPT2Output(
             attributions=self.attributions, attributions_grouped=group_attr, attributions_grouped_norm=norm_attr,
             cluster_imp_df=cluster_imp_df, cluster_imp_aggr_df=cluster_imp_aggr_df,
             word_imp_df=word_imp_df, word_imp_norm_df=word_imp_norm_df)
```

### Comparing `explainitall-1.0.0/explainitall/gpt_like_interp/viz.py` & `explainitall-1.0.1/explainitall/gpt_like_interp/viz.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,18 +41,23 @@
     arr.sort()
     qqplot((arr - dic_stat["mean"]) / dic_stat["std"], line='45')
     plt.grid()
     plt.show()
 
 
 def df_to_heatmap(df, title=None, annot=True):
-    df_temp = copy.deepcopy(df)
-    df_temp.set_index('Tokens', inplace=True)
+    try:
+        df_temp = copy.deepcopy(df)
+        df_temp.set_index('Tokens', inplace=True)
 
-    plt.figure(figsize=(15, 10))
-    sns.heatmap(df_temp, annot=annot, cmap='coolwarm', linewidths=0.5, linecolor='lightgrey')
-    if title:
-        plt.title(title, fontsize=14)
-    plt.yticks(rotation=45, va='top', fontsize=10)
-    plt.xticks(rotation=45, fontsize=10)
-    plt.tight_layout()
-    plt.show()
+        plt.figure(figsize=(15, 10))
+        sns.heatmap(df_temp, annot=annot, cmap='coolwarm', linewidths=0.5, linecolor='lightgrey')
+        if title:
+            plt.title(title, fontsize=14)
+        plt.yticks(rotation=45, va='top', fontsize=10)
+        plt.xticks(rotation=45, fontsize=10)
+        plt.tight_layout()
+        plt.show()
+    except:
+        print("Данные отсутствуют или неполны.")
+        plt.figure(figsize=(15, 10))
+        plt.text(0.5, 0.5, 'Данные отсутствуют или неполны, Нет данных для отображения', fontsize=14, ha='center')
```

### Comparing `explainitall-1.0.0/explainitall/gui/interface.py` & `explainitall-1.0.1/explainitall/gui/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,35 +303,38 @@
         imp_df_cl = expl_data.cluster_imp_aggr_df
         cl_desc = interp_cl(imp_df_cl)
 
         clean = [clean_string(cl_data) for cl_data in cl_desc]
         vects_x = self.sbert_.encode(clean)
         m = vects_x.mean(axis=0)
         s = vects_x.std(axis=0)
-        knn_vects_x = (vects_x - m) / s
-        knn = KNeighborsClassifier(metric=cos_dist)
-        knn.fit(knn_vects_x, cl_desc)
-
-        self.interp_bot_ = PromptBot(knn, self.sbert_, self.fred_, cl_desc, device='cpu')
-
+        try:
+            knn_vects_x = (vects_x - m) / s
+            knn = KNeighborsClassifier(metric=cos_dist)
+            knn.fit(knn_vects_x, cl_desc)
+
+            self.interp_bot_ = PromptBot(knn, self.sbert_, self.fred_, cl_desc, device='cpu')
+        except:
+            print("Err")
+            self.interp_bot_ = None
         word_importance_plt = df_to_heatmap_plot(expl_data.word_imp_df, title="Карта важности слов")
         word_importance_norm_plt = df_to_heatmap_plot(expl_data.word_imp_norm_df,
                                                       title="Карта важности слов, нормированная")
 
         cluster_importance_plt = df_to_heatmap_plot(expl_data.cluster_imp_df, title="Карта важности кластеров")
         cluster_importance_norm_plt = df_to_heatmap_plot(expl_data.cluster_imp_aggr_df,
                                                          title="Карта важности кластеров, группированная")
 
         return word_importance_plt, word_importance_norm_plt, cluster_importance_plt, cluster_importance_norm_plt
 
     # PRIVATE FUNCTIONS:
 
     def respond_(self, message, chat_history):
         ans = self.interp_bot_.get_answers(message, top_k=3)
-        bot_reply = ans.split('.')[0]
+        bot_reply = 'Кластер' + ans.split('.')[0].split('Кластер')[1]
         chat_history.append((message, bot_reply))
 
         return "", chat_history
 
     def load_context_and_generated_text_(self, context, generated_text):
         self.context_ = context
         self.generated_text_ = generated_text
```

### Comparing `explainitall-1.0.0/explainitall/metrics/CheckingForHallucinations.py` & `explainitall-1.0.1/explainitall/metrics/CheckingForHallucinations.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/Metrics.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/Metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,32 +89,30 @@
         max_length = self.model_.config.n_positions
         seq_len = len(reference_encodings)
 
         nlls = []
         prev_end_loc = 0
         for begin_loc in range(0, seq_len, self.stride_):
             end_loc = min(begin_loc + max_length, seq_len)
-            trg_len = end_loc - prev_end_loc  # may be different from stride on last loop
+            trg_len = end_loc - prev_end_loc
             input_ids = torch.tensor(reference_encodings[begin_loc:end_loc])
             input_ids = input_ids.to(self.model_.device)
             target_ids = input_ids.clone()
             target_ids[:-trg_len] = -100
-            # target_ids = [-100] * (len(input_ids) - trg_len) + input_ids[trg_len:]
+            input_ids = input_ids.unsqueeze(0)
+            # with open(f'output_file{begin_loc}.txt', 'w') as file:
+            #     output_info = f"input_ids: {str(input_ids)}, type: {(input_ids.dtype)}"
+            #     print(output_info)
+            #     file.write(output_info + "\n")
 
             with torch.no_grad():
                 outputs = self.model_(input_ids, labels=target_ids)
-
-                # loss is calculated using CrossEntropyLoss which averages over input tokens.
-                # Multiply it with trg_len to get the summation instead of average.
-                # We will take average over all the tokens to get the true average
-                # in the last step of this example.
                 neg_log_likelihood = outputs.loss * trg_len
 
             nlls.append(neg_log_likelihood)
 
             prev_end_loc = end_loc
             if end_loc == seq_len:
                 break
 
         ppl = torch.exp(torch.stack(nlls).sum() / end_loc)
         return {'value': ppl.item()}
-
```

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/Metrics_calculator.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/Metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/create_database.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/create_database.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/helpers.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/helpers.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/metric_calculation_interface.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/metric_calculation_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import os
-
 import gradio as gr
 import pandas as pd
-import sqlalchemy as db
-from transformers import GPT2LMHeadModel, GPT2TokenizerFast
+from transformers import GPT2LMHeadModel, GPT2TokenizerFast, AutoTokenizer, AutoModel, AutoModelForCausalLM
 
 from explainitall.metrics.RougeAndPPL.Metrics import Metric_ppl, MetricRougeL, MetricRougeN
 from explainitall.metrics.RougeAndPPL.Metrics_calculator import Metrics_calculator
 from explainitall.metrics.RougeAndPPL.create_database import data_table, ENGINE
 from explainitall.metrics.RougeAndPPL.helpers import (
     get_max_dataset_version, generate_candidates, calculate_average_metric_values,
     insert_new_record, get_records_from_database, make_dataframe_from_history_records)
@@ -58,15 +55,14 @@
                                         dataset_file = gr.File(label='Dataset (CSV)')
                                         dataset_title = gr.Text(label='Dataset title',
                                                                 info="Это поле обязательно к заполнению. Без указания названия датасета процесс не будет запущен.",
                                                                 placeholder="Введите название датасета")
 
                                     dataset_visualization = gr.Dataframe(label='Dataset',
                                                                          headers=['context', 'reference'],
-                                                                         # overflow_row_behaviour='paginate',
                                                                          wrap=False,
                                                                          height=500)
                                 with gr.Row():
                                     dataset_load_button = gr.Button("Load dataset")
                                     dataset_checkbox = gr.Checkbox(label='dataset loaded', interactive=False)
 
                         with gr.Row():
@@ -113,24 +109,20 @@
         self.demo_.launch(share=True, debug=False, server_name="127.0.0.1", inbrowser=True)
 
     def load_model_(self, model_name_or_path):
         if not model_name_or_path:
             print("Model name or path is required.", model_name_or_path)
 
         self.model_successfully_loaded_ = False
-        # self.model_checkbox_.value = False
 
-        self.tokenizer_ = GPT2TokenizerFast.from_pretrained(model_name_or_path)
+        self.tokenizer_ = AutoTokenizer.from_pretrained(model_name_or_path)
         if self.tokenizer_.pad_token is None:
             self.tokenizer_.pad_token = self.tokenizer_.eos_token
-        self.model_ = GPT2LMHeadModel.from_pretrained(model_name_or_path)
+        self.model_ = AutoModelForCausalLM.from_pretrained(model_name_or_path)
 
-        # path = os.path.normpath(model_name_or_path)
-        # path_list = path.split(os.sep)
-        # self.model_name_ = path_list[-1]
         self.model_name_ = str(model_name_or_path)
 
         self.calculator_ = Metrics_calculator(self.tokenizer_)
 
         self.calculator_.add_metric('PPL', Metric_ppl(self.model_, stride=512))
 
         self.calculator_.add_metric('R3', MetricRougeN(3))
@@ -139,15 +131,14 @@
         self.calculator_.add_metric('R-L', MetricRougeL(3))
 
         self.model_successfully_loaded_ = True
         return True
 
     def load_dataset_(self, csvfile, title):
         self.dataset_successfully_loaded_ = False
-        # self.dataset_checkbox_.value = False
 
         print("csvfile", csvfile)
         print("title", title)
 
         if csvfile is None or title == '':
             return pd.DataFrame(), False
         dataframe = pd.read_csv(csvfile.name, delimiter=',', encoding='utf-8')
```

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_L.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_L.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_N.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_N.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_l_helpers.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_l_helpers.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/metrics/RougeAndPPL/rouge_n_helpers.py` & `explainitall-1.0.1/explainitall/metrics/RougeAndPPL/rouge_n_helpers.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/nlp.py` & `explainitall-1.0.1/explainitall/nlp.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall/stat_helpers.py` & `explainitall-1.0.1/explainitall/stat_helpers.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/explainitall.egg-info/PKG-INFO` & `explainitall-1.0.1/explainitall.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,12 @@
 Metadata-Version: 2.1
 Name: explainitall
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gensim==4.3.2
-Requires-Dist: gradio==4.4.1
-Requires-Dist: gradio_client==0.7.0
-Requires-Dist: inseq==0.5.0
-Requires-Dist: matplotlib==3.8.4
-Requires-Dist: nltk==3.8.1
-Requires-Dist: pandas==2.2.1
-Requires-Dist: pymorphy2==0.9.1
-Requires-Dist: scikit-learn==1.4.1.post1
-Requires-Dist: seaborn==0.13.2
-Requires-Dist: sentence_transformers==2.6.1
-Requires-Dist: SQLAlchemy==2.0.29
-Requires-Dist: statsmodels==0.14.1
-Requires-Dist: torch>=2.0
-Requires-Dist: transformers>=4.39
-Requires-Dist: uvicorn==0.29
-Requires-Dist: scipy==1.12.0
-Requires-Dist: numpy==1.26.4
 
 # **ExplainitAll**
 
 **ExplainitAll** — это библиотека для интерпретируемого ИИ, предназначенная для интерпретации генеративных моделей (
 GPT-like), и векторизаторов, например, Sbert. Библиотека предоставляет пользователям инструменты для анализа и понимания
 работы этих сложных моделей. Кроме того, содержит модули RAG QA, fast_tuning и пользовательский интерфейс.
```

### Comparing `explainitall-1.0.0/explainitall.egg-info/SOURCES.txt` & `explainitall-1.0.1/explainitall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/setup.py` & `explainitall-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 except ImportError:
     from distutils.core import setup, find_namespace_packages
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(
     name='explainitall',
-    version='1.0.0',
+    version='1.0.1',
     long_description=open('README.md', encoding='utf-8', errors='ignore').read(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['explainitall', 'explainitall.*']),
     install_requires=REQUIREMENTS
 )
```

### Comparing `explainitall-1.0.0/tests/test_inseq_helpers.py` & `explainitall-1.0.1/tests/test_inseq_helpers.py`

 * *Files identical despite different names*

### Comparing `explainitall-1.0.0/tests/test_stat_helpers.py` & `explainitall-1.0.1/tests/test_stat_helpers.py`

 * *Files identical despite different names*

