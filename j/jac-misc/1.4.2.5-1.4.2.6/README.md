# Comparing `tmp/jac_misc-1.4.2.5.tar.gz` & `tmp/jac_misc-1.4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_misc-1.4.2.5.tar", last modified: Tue Jan  9 16:44:27 2024, max compression
+gzip compressed data, was "jac_misc-1.4.2.6.tar", last modified: Tue Apr 23 19:42:46 2024, max compression
```

## Comparing `jac_misc-1.4.2.5.tar` & `jac_misc-1.4.2.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.586887 jac_misc-1.4.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-01-09 16:44:27.586887 jac_misc-1.4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.570887 jac_misc-1.4.2.5/jac_misc/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.570887 jac_misc-1.4.2.5/jac_misc/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/cluster/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/cluster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/cluster/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/cluster/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/cluster/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/cluster/tests/fixtures/cluster.jac
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/cluster/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/elastic_retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/elastic_retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/elastic_retrieval/elastic_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/elastic_retrieval/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/elastic_retrieval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/example_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/example_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/example_module/example_module.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/example_module/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/forecast/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/forecast/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/forecast/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/forecast/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/forecast/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/forecast/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/forecast/tests/test_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/huggingface/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/huggingface/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/huggingface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.574887 jac_misc-1.4.2.5/jac_misc/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/langchain/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/langchain/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.578887 jac_misc-1.4.2.5/jac_misc/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17341 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/openai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/openai/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.578887 jac_misc-1.4.2.5/jac_misc/pdf_ext/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/pdf_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/pdf_ext/pdf_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/pdf_ext/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.578887 jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.578887 jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/test_pdf_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.578887 jac_misc-1.4.2.5/jac_misc/ph/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/ph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/ph_train_data.json
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/run_ph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.582887 jac_misc-1.4.2.5/jac_misc/ph/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/ph/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.582887 jac_misc-1.4.2.5/jac_misc/translator/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/translator/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/jac_misc/translator/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:27.582887 jac_misc-1.4.2.5/jac_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-01-09 16:44:27.000000 jac_misc-1.4.2.5/jac_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-01-09 16:44:27.000000 jac_misc-1.4.2.5/jac_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 16:44:27.000000 jac_misc-1.4.2.5/jac_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-09 16:44:27.000000 jac_misc-1.4.2.5/jac_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-09 16:44:27.000000 jac_misc-1.4.2.5/jac_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 16:44:27.586887 jac_misc-1.4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-01-09 16:44:13.000000 jac_misc-1.4.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.957794 jac_misc-1.4.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-23 19:42:46.957794 jac_misc-1.4.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.941794 jac_misc-1.4.2.6/jac_misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/cluster/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/cluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/cluster/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/cluster/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/cluster/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/cluster/tests/fixtures/cluster.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/cluster/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/elastic_retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/elastic_retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/elastic_retrieval/elastic_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/elastic_retrieval/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/elastic_retrieval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/example_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/example_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/example_module/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/example_module/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/forecast/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/forecast/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/forecast/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/forecast/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/forecast/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/forecast/tests/test_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.945794 jac_misc-1.4.2.6/jac_misc/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/huggingface/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/huggingface/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/huggingface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.949794 jac_misc-1.4.2.6/jac_misc/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/langchain/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/langchain/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.949794 jac_misc-1.4.2.6/jac_misc/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/openai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/openai/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.949794 jac_misc-1.4.2.6/jac_misc/pdf_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/pdf_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/pdf_ext/pdf_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/pdf_ext/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.949794 jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.949794 jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/test_pdf_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.949794 jac_misc-1.4.2.6/jac_misc/ph/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/ph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/ph_train_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-23 19:42:32.000000 jac_misc-1.4.2.6/jac_misc/ph/run_ph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.953794 jac_misc-1.4.2.6/jac_misc/ph/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/ph/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.953794 jac_misc-1.4.2.6/jac_misc/translator/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/translator/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/jac_misc/translator/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:46.953794 jac_misc-1.4.2.6/jac_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-23 19:42:46.000000 jac_misc-1.4.2.6/jac_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-23 19:42:46.000000 jac_misc-1.4.2.6/jac_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:42:46.000000 jac_misc-1.4.2.6/jac_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-23 19:42:46.000000 jac_misc-1.4.2.6/jac_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 19:42:46.000000 jac_misc-1.4.2.6/jac_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:42:46.957794 jac_misc-1.4.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-23 19:42:33.000000 jac_misc-1.4.2.6/setup.py
```

### Comparing `jac_misc-1.4.2.5/PKG-INFO` & `jac_misc-1.4.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jac_misc
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci/jaseci_ai_kit/jac_misc
 Author: Jason Mars
 Author-email: jason@jaseci.org
-Requires-Dist: jaseci==1.4.2.5
+Requires-Dist: jaseci==1.4.2.6
 Requires-Dist: pytest<7.1,>=7.0.1
 Requires-Dist: pytest-order<1.1,>=1.0.1
 Provides-Extra: all
 Requires-Dist: pypdf==3.15.4; extra == "all"
 Requires-Dist: transformers>=4.0.0; extra == "all"
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
```

### Comparing `jac_misc-1.4.2.5/README.md` & `jac_misc-1.4.2.6/README.md`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/cluster/cluster.py` & `jac_misc-1.4.2.6/jac_misc/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/cluster/tests/fixtures/cluster.jac` & `jac_misc-1.4.2.6/jac_misc/cluster/tests/fixtures/cluster.jac`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/cluster/tests/test_cluster.py` & `jac_misc-1.4.2.6/jac_misc/cluster/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/elastic_retrieval/elastic_retrieval.py` & `jac_misc-1.4.2.6/jac_misc/elastic_retrieval/elastic_retrieval.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/elastic_retrieval/utils.py` & `jac_misc-1.4.2.6/jac_misc/elastic_retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/forecast/action_utils.py` & `jac_misc-1.4.2.6/jac_misc/forecast/action_utils.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/forecast/forecast.py` & `jac_misc-1.4.2.6/jac_misc/forecast/forecast.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/forecast/tests/test_forecast.py` & `jac_misc-1.4.2.6/jac_misc/forecast/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/huggingface/huggingface.py` & `jac_misc-1.4.2.6/jac_misc/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/huggingface/utils.py` & `jac_misc-1.4.2.6/jac_misc/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/langchain/main.py` & `jac_misc-1.4.2.6/jac_misc/langchain/main.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/openai/main.py` & `jac_misc-1.4.2.6/jac_misc/openai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     - GPT-3 (Completion and Chat)
     - Codex (Code Completion)
     - DALL-E (Image Generation)
     - Whispers (Audio Transcription)
 
 Requires OpenAI API Key
 """
+
 from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import logger
 from openai import OpenAI
 from openai._base_client import DEFAULT_MAX_RETRIES
 from typing import Union, Mapping
 
 openai_client = None
```

### Comparing `jac_misc-1.4.2.5/jac_misc/pdf_ext/pdf_ext.py` & `jac_misc-1.4.2.6/jac_misc/pdf_ext/pdf_ext.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac` & `jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/pdf_ext/tests/test_pdf_ext.py` & `jac_misc-1.4.2.6/jac_misc/pdf_ext/tests/test_pdf_ext.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/config.yaml` & `jac_misc-1.4.2.6/jac_misc/ph/config.yaml`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/custom.py` & `jac_misc-1.4.2.6/jac_misc/ph/custom.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/inference.py` & `jac_misc-1.4.2.6/jac_misc/ph/inference.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/ph.py` & `jac_misc-1.4.2.6/jac_misc/ph/ph.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/ph_train_data.json` & `jac_misc-1.4.2.6/jac_misc/ph/ph_train_data.json`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/run_ph.py` & `jac_misc-1.4.2.6/jac_misc/ph/run_ph.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/train.py` & `jac_misc-1.4.2.6/jac_misc/ph/train.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/base.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/base.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/dataloader.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/logger.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/logger.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/loss.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/loss.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/metric.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/metric.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/model.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/model.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/process.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/process.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/trainer.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/ph/utils/util.py` & `jac_misc-1.4.2.6/jac_misc/ph/utils/util.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc/translator/translator.py` & `jac_misc-1.4.2.6/jac_misc/translator/translator.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc.egg-info/PKG-INFO` & `jac_misc-1.4.2.6/jac_misc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jac_misc
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci/jaseci_ai_kit/jac_misc
 Author: Jason Mars
 Author-email: jason@jaseci.org
-Requires-Dist: jaseci==1.4.2.5
+Requires-Dist: jaseci==1.4.2.6
 Requires-Dist: pytest<7.1,>=7.0.1
 Requires-Dist: pytest-order<1.1,>=1.0.1
 Provides-Extra: all
 Requires-Dist: pypdf==3.15.4; extra == "all"
 Requires-Dist: transformers>=4.0.0; extra == "all"
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
```

### Comparing `jac_misc-1.4.2.5/jac_misc.egg-info/SOURCES.txt` & `jac_misc-1.4.2.6/jac_misc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.2.5/jac_misc.egg-info/requires.txt` & `jac_misc-1.4.2.6/jac_misc.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jaseci==1.4.2.5
+jaseci==1.4.2.6
 pytest<7.1,>=7.0.1
 pytest-order<1.1,>=1.0.1
 
 [all]
 pypdf==3.15.4
 transformers>=4.0.0
 torch<2.0.0,>=1.10.2
@@ -13,15 +13,14 @@
 scikit-learn<1.3.0
 uuid<2.0.0,>=1.30
 transformers>=4.25.1
 openai==1.3.0
 soundfile<0.13,>=0.12.1
 elasticsearch==8.9.0
 tenacity>=8.2.1
-PyPDF==3.15.4
 docx2txt>=0.8
 python-pptx>=0.6.21
 tiktoken>=0.2.0
 langchain
 openai
 chromadb
 tiktoken
```

### Comparing `jac_misc-1.4.2.5/setup.py` & `jac_misc-1.4.2.6/setup.py`

 * *Files identical despite different names*

