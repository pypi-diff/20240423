# Comparing `tmp/emm-2.1.0.tar.gz` & `tmp/emm-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emm-2.1.0.tar", last modified: Mon Apr 22 07:53:12 2024, max compression
+gzip compressed data, was "emm-2.1.1.tar", last modified: Tue Apr 23 11:27:46 2024, max compression
```

## Comparing `emm-2.1.0.tar` & `emm-2.1.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.351721 emm-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.323721 emm-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.327721 emm-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-22 07:53:05.000000 emm-2.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-22 07:53:05.000000 emm-2.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 07:53:05.000000 emm-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 07:53:05.000000 emm-2.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 07:53:05.000000 emm-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-22 07:53:05.000000 emm-2.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-22 07:53:12.351721 emm-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-22 07:53:05.000000 emm-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.323721 emm-2.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.327721 emm-2.1.0/docs/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      289 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/autogenerate.sh
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.331721 emm-2.1.0/docs/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/api_index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.aggregation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.helper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.indexing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.loggers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.rst
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.supervised_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.threshold.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/fitting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/persistence.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/spark.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.331721 emm-2.1.0/emm/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-22 07:53:05.000000 emm-2.1.0/emm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/base_entity_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/pandas_entity_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/spark_entity_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 07:53:06.000000 emm-2.1.0/emm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 07:53:06.000000 emm-2.1.0/emm/base/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-22 07:53:06.000000 emm-2.1.0/emm/base/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/data/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/create_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/negative_data_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/noiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/prepare_name_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/unittest_sample_namepairs.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/base_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_lef.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/pandas_feature_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/helper/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/blocking_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/custom_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/sklearn_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/spark_custom_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/spark_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/base_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_candidate_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_cos_sim_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_naive_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_normalized_tfidf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_sni.py
--rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_candidate_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_character_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_cos_sim_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_indexing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_normalized_tfidf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_sni.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_word_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-22 07:53:06.000000 emm-2.1.0/emm/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-22 07:53:06.000000 emm-2.1.0/emm/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-22 07:53:06.000000 emm-2.1.0/emm/loggers/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-22 07:53:06.000000 emm-2.1.0/emm/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14514 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/base_entity_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    38661 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/pandas_entity_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    39097 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/spark_entity_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/emm/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/abbreviation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/base_name_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/pandas_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/pandas_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/spark_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-22 07:53:06.000000 emm-2.1.0/emm/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/emm/supervised_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/base_supervised_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/pandas_supervised_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/spark_supervised_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/emm/threshold/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 07:53:06.000000 emm-2.1.0/emm/threshold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-22 07:53:06.000000 emm-2.1.0/emm/threshold/threshold_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-22 07:53:06.000000 emm-2.1.0/emm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/emm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-22 07:53:06.000000 emm-2.1.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/01-entity-matching-pandas-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/02-entity-matching-spark-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/03-entity-matching-training-pandas-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/04-entity-matching-aggregation-pandas-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-22 07:53:06.000000 emm-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:53:12.351721 emm-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 07:53:06.000000 emm-2.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/tests/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-22 07:53:06.000000 emm-2.1.0/tests/benchmark/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-22 07:53:06.000000 emm-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_artificial_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_em_add_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26454 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_entity_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_indexers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_normalized_tfidf.py
--rw-r--r--   0 runner    (1001) docker     (127)    36602 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_pandas_em.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_readme_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_spark_vs_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_training_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/tests/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-22 07:53:06.000000 emm-2.1.0/tests/notebooks/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_abbreviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_carry_on_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_commonshorthands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_cos_sim_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_custom_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_entity_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_features_abbreviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_features_lef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_features_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_name_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_negative_sample_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_threshold_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-22 07:53:06.000000 emm-2.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.689861 emm-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.657861 emm-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.661861 emm-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-23 11:27:40.000000 emm-2.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 11:27:40.000000 emm-2.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 11:27:40.000000 emm-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-23 11:27:40.000000 emm-2.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 11:27:40.000000 emm-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-23 11:27:40.000000 emm-2.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-23 11:27:46.689861 emm-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-23 11:27:40.000000 emm-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.657861 emm-2.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.661861 emm-2.1.1/docs/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      289 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/autogenerate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.665861 emm-2.1.1/docs/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/api_index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.aggregation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.helper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.loggers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.supervised_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/emm.threshold.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/fitting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/persistence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-23 11:27:40.000000 emm-2.1.1/docs/sphinx/source/spark.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.665861 emm-2.1.1/emm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-23 11:27:40.000000 emm-2.1.1/emm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.669861 emm-2.1.1/emm/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-23 11:27:40.000000 emm-2.1.1/emm/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-23 11:27:40.000000 emm-2.1.1/emm/aggregation/base_entity_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-23 11:27:40.000000 emm-2.1.1/emm/aggregation/pandas_entity_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-04-23 11:27:40.000000 emm-2.1.1/emm/aggregation/spark_entity_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.669861 emm-2.1.1/emm/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 11:27:40.000000 emm-2.1.1/emm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-23 11:27:40.000000 emm-2.1.1/emm/base/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-23 11:27:40.000000 emm-2.1.1/emm/base/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.669861 emm-2.1.1/emm/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 11:27:40.000000 emm-2.1.1/emm/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 11:27:40.000000 emm-2.1.1/emm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-23 11:27:40.000000 emm-2.1.1/emm/data/create_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-04-23 11:27:40.000000 emm-2.1.1/emm/data/negative_data_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-23 11:27:40.000000 emm-2.1.1/emm/data/noiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-23 11:27:40.000000 emm-2.1.1/emm/data/prepare_name_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-23 11:27:40.000000 emm-2.1.1/emm/data/unittest_sample_namepairs.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.673861 emm-2.1.1/emm/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/base_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/features_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/features_lef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/features_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/features_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/features_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-23 11:27:40.000000 emm-2.1.1/emm/features/pandas_feature_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.673861 emm-2.1.1/emm/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/blocking_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/custom_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/sklearn_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/spark_custom_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/spark_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-23 11:27:40.000000 emm-2.1.1/emm/helper/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.677861 emm-2.1.1/emm/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/base_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/pandas_candidate_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/pandas_cos_sim_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/pandas_naive_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/pandas_normalized_tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/pandas_sni.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/spark_candidate_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/spark_character_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31867 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/spark_cos_sim_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/spark_indexing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/spark_normalized_tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/spark_sni.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-23 11:27:40.000000 emm-2.1.1/emm/indexing/spark_word_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.677861 emm-2.1.1/emm/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-23 11:27:40.000000 emm-2.1.1/emm/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-23 11:27:40.000000 emm-2.1.1/emm/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-23 11:27:40.000000 emm-2.1.1/emm/loggers/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-23 11:27:40.000000 emm-2.1.1/emm/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.677861 emm-2.1.1/emm/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-23 11:27:40.000000 emm-2.1.1/emm/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14514 2024-04-23 11:27:40.000000 emm-2.1.1/emm/pipeline/base_entity_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38661 2024-04-23 11:27:40.000000 emm-2.1.1/emm/pipeline/pandas_entity_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39097 2024-04-23 11:27:40.000000 emm-2.1.1/emm/pipeline/spark_entity_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.677861 emm-2.1.1/emm/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/abbreviation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/base_name_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/pandas_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/pandas_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-23 11:27:40.000000 emm-2.1.1/emm/preprocessing/spark_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-23 11:27:40.000000 emm-2.1.1/emm/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.681861 emm-2.1.1/emm/supervised_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-23 11:27:40.000000 emm-2.1.1/emm/supervised_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-23 11:27:40.000000 emm-2.1.1/emm/supervised_model/base_supervised_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-23 11:27:40.000000 emm-2.1.1/emm/supervised_model/pandas_supervised_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-23 11:27:40.000000 emm-2.1.1/emm/supervised_model/spark_supervised_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.681861 emm-2.1.1/emm/threshold/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 11:27:40.000000 emm-2.1.1/emm/threshold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-23 11:27:40.000000 emm-2.1.1/emm/threshold/threshold_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-23 11:27:40.000000 emm-2.1.1/emm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.685861 emm-2.1.1/emm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-23 11:27:46.000000 emm-2.1.1/emm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-23 11:27:46.000000 emm-2.1.1/emm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:27:46.000000 emm-2.1.1/emm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-23 11:27:46.000000 emm-2.1.1/emm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 11:27:46.000000 emm-2.1.1/emm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-23 11:27:40.000000 emm-2.1.1/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.681861 emm-2.1.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-23 11:27:40.000000 emm-2.1.1/notebooks/01-entity-matching-pandas-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-04-23 11:27:40.000000 emm-2.1.1/notebooks/02-entity-matching-spark-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-04-23 11:27:40.000000 emm-2.1.1/notebooks/03-entity-matching-training-pandas-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-23 11:27:40.000000 emm-2.1.1/notebooks/04-entity-matching-aggregation-pandas-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-23 11:27:40.000000 emm-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:27:46.689861 emm-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.681861 emm-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 11:27:40.000000 emm-2.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.681861 emm-2.1.1/tests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:40.000000 emm-2.1.1/tests/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-23 11:27:40.000000 emm-2.1.1/tests/benchmark/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-23 11:27:40.000000 emm-2.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.685861 emm-2.1.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_artificial_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_em_add_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26454 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_entity_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_indexers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_normalized_tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36602 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_pandas_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_readme_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_spark_vs_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-23 11:27:40.000000 emm-2.1.1/tests/integration/test_training_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.685861 emm-2.1.1/tests/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:40.000000 emm-2.1.1/tests/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-23 11:27:40.000000 emm-2.1.1/tests/notebooks/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:46.685861 emm-2.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_abbreviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_carry_on_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_commonshorthands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_cos_sim_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_custom_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_entity_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_features_abbreviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_features_lef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_features_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_name_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_negative_sample_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_threshold_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-23 11:27:40.000000 emm-2.1.1/tests/unit/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-23 11:27:40.000000 emm-2.1.1/tests/utils.py
```

### Comparing `emm-2.1.0/.github/workflows/test.yml` & `emm-2.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/LICENSE` & `emm-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/NOTICE` & `emm-2.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/PKG-INFO` & `emm-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emm
-Version: 2.1.0
+Version: 2.1.1
 Summary: Entity Matching Model package
 Author-email: Max Baak <max.baak@ing.com>, Stephane Collot <stephane.collot@gmail.com>, Apoorva Mahajan <apoorva.mahajan@ing.com>, Tomasz Waleń <tomasz.walen@ing.com>, Simon Brugman <simon.brugman@ing.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.20.1
```

### Comparing `emm-2.1.0/README.md` & `emm-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/Makefile` & `emm-2.1.1/docs/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/README.rst` & `emm-2.1.1/docs/sphinx/README.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/make.bat` & `emm-2.1.1/docs/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/conf.py` & `emm-2.1.1/docs/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.aggregation.rst` & `emm-2.1.1/docs/sphinx/source/emm.aggregation.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.data.rst` & `emm-2.1.1/docs/sphinx/source/emm.data.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.features.rst` & `emm-2.1.1/docs/sphinx/source/emm.features.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.helper.rst` & `emm-2.1.1/docs/sphinx/source/emm.helper.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.indexing.rst` & `emm-2.1.1/docs/sphinx/source/emm.indexing.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.pipeline.rst` & `emm-2.1.1/docs/sphinx/source/emm.pipeline.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.preprocessing.rst` & `emm-2.1.1/docs/sphinx/source/emm.preprocessing.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.rst` & `emm-2.1.1/docs/sphinx/source/emm.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/emm.supervised_model.rst` & `emm-2.1.1/docs/sphinx/source/emm.supervised_model.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/fitting.rst` & `emm-2.1.1/docs/sphinx/source/fitting.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/overview.rst` & `emm-2.1.1/docs/sphinx/source/overview.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/parameters.rst` & `emm-2.1.1/docs/sphinx/source/parameters.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/persistence.rst` & `emm-2.1.1/docs/sphinx/source/persistence.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/pipeline.rst` & `emm-2.1.1/docs/sphinx/source/pipeline.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/docs/sphinx/source/spark.rst` & `emm-2.1.1/docs/sphinx/source/spark.rst`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/__init__.py` & `emm-2.1.1/emm/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/aggregation/__init__.py` & `emm-2.1.1/emm/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/aggregation/base_entity_aggregation.py` & `emm-2.1.1/emm/aggregation/base_entity_aggregation.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/aggregation/pandas_entity_aggregation.py` & `emm-2.1.1/emm/aggregation/pandas_entity_aggregation.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/aggregation/spark_entity_aggregation.py` & `emm-2.1.1/emm/aggregation/spark_entity_aggregation.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/base/__init__.py` & `emm-2.1.1/emm/base/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/base/module.py` & `emm-2.1.1/emm/base/module.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/base/pipeline.py` & `emm-2.1.1/emm/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/data/__init__.py` & `emm-2.1.1/emm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/data/create_data.py` & `emm-2.1.1/emm/data/create_data.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/data/negative_data_creation.py` & `emm-2.1.1/emm/data/negative_data_creation.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/data/noiser.py` & `emm-2.1.1/emm/data/noiser.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/data/prepare_name_pairs.py` & `emm-2.1.1/emm/data/prepare_name_pairs.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/data/unittest_sample_namepairs.csv.gz` & `emm-2.1.1/emm/data/unittest_sample_namepairs.csv.gz`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/__init__.py` & `emm-2.1.1/emm/features/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/base_feature_extractor.py` & `emm-2.1.1/emm/features/base_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/features_extra.py` & `emm-2.1.1/emm/features/features_extra.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/features_lef.py` & `emm-2.1.1/emm/features/features_lef.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/features_name.py` & `emm-2.1.1/emm/features/features_name.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/features_rank.py` & `emm-2.1.1/emm/features/features_rank.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/features_vocabulary.py` & `emm-2.1.1/emm/features/features_vocabulary.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/features/pandas_feature_extractor.py` & `emm-2.1.1/emm/features/pandas_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/__init__.py` & `emm-2.1.1/emm/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/blocking_functions.py` & `emm-2.1.1/emm/helper/blocking_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,21 +19,49 @@
 
 """List of blocking functions.
 
 Their names are used to name indexers.
 Please don't modify the function names.
 """
 
+from __future__ import annotations
+
+from typing import Callable
+
 
 def first(x: str) -> str:
     """First character blocking function."""
     return x.strip().lower()[:1]
 
 
 def first2(x: str) -> str:
     """First two characters blocking function."""
     return x.strip().lower()[:2]
 
 
 def first3(x: str) -> str:
     """First two characters blocking function."""
     return x.strip().lower()[:3]
+
+
+BLOCKING_MAP = {"first": first, "first2": first2, "first3": first3}
+
+
+def _parse_blocking_func(input: Callable[[str], str] | str | None = None) -> Callable[[str], str] | None:
+    """Helper function to get blocking function
+
+    Args:
+        input: blocking function or name of existing blocking function
+
+    Returns:
+        blocking function or None
+    """
+    if input is None or callable(input):
+        return input
+    if isinstance(input, str):
+        if input not in BLOCKING_MAP:
+            msg = f"Input {input} is not a recognized blocking function."
+            raise ValueError(msg)
+        return BLOCKING_MAP[input]
+
+    msg = "Input is not None, no string and not callable."
+    raise TypeError(msg)
```

### Comparing `emm-2.1.0/emm/helper/custom_path.py` & `emm-2.1.1/emm/helper/custom_path.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/io.py` & `emm-2.1.1/emm/helper/io.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/sklearn_pipeline.py` & `emm-2.1.1/emm/helper/sklearn_pipeline.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/spark_custom_reader_writer.py` & `emm-2.1.1/emm/helper/spark_custom_reader_writer.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/spark_ml_pipeline.py` & `emm-2.1.1/emm/helper/spark_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/spark_utils.py` & `emm-2.1.1/emm/helper/spark_utils.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/helper/util.py` & `emm-2.1.1/emm/helper/util.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/__init__.py` & `emm-2.1.1/emm/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/base_indexer.py` & `emm-2.1.1/emm/indexing/base_indexer.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/pandas_candidate_selection.py` & `emm-2.1.1/emm/indexing/pandas_candidate_selection.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/pandas_cos_sim_matcher.py` & `emm-2.1.1/emm/indexing/pandas_cos_sim_matcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import numpy as np
 import pandas as pd
 import scipy
 import scipy.sparse
 from sklearn.base import TransformerMixin
 from sparse_dot_topn import sp_matmul_topn
 
+from emm.helper.blocking_functions import _parse_blocking_func
 from emm.helper.util import groupby
 from emm.indexing.base_indexer import CosSimBaseIndexer
 from emm.indexing.pandas_normalized_tfidf import PandasNormalizedTfidfVectorizer
 from emm.loggers import Timer
 from emm.loggers.logger import logger
 
 
@@ -48,15 +49,15 @@
         binary_countvectorizer: bool = False,
         num_candidates: int = 5,
         cos_sim_lower_bound: float = 0.5,
         partition_size: int = 5000,
         max_features: int | None = None,
         n_jobs: int = 1,
         spark_session: Any | None = None,
-        blocking_func: Callable[[str], str] | None = None,
+        blocking_func: Callable[[str], str] | str | None = None,
         dtype: type[float] = np.float32,
         indexer_id: int | None = None,
     ) -> None:
         """Cosine similarity indexer to generate candidate name-pairs of possible matches
 
         Pipeline of tokenization, ngram creation, vectorization, tfidf, cosine similarity.
         The vectorizer used is a customized version of sklearn's TfidfVectorizer.
@@ -95,15 +96,15 @@
         CosSimBaseIndexer.__init__(self, num_candidates=num_candidates)
         self.input_col = input_col
         self.ngram = ngram
         self.tokenizer = tokenizer
         self.dtype = dtype
         self.cos_sim_lower_bound = cos_sim_lower_bound
         self.partition_size = partition_size
-        self.blocking_func = blocking_func
+        self.blocking_func = _parse_blocking_func(blocking_func)
         self.n_jobs = n_jobs if n_jobs != -1 else multiprocessing.cpu_count()
         self.spark_session = spark_session
         # attributes below are set during fit
         self.tfidf = PandasNormalizedTfidfVectorizer(
             analyzer={"words": "word", "characters": "char"}[tokenizer],
             binary=binary_countvectorizer,
             ngram_range=(ngram, ngram),
```

### Comparing `emm-2.1.0/emm/indexing/pandas_naive_indexer.py` & `emm-2.1.1/emm/indexing/pandas_naive_indexer.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/pandas_normalized_tfidf.py` & `emm-2.1.1/emm/indexing/pandas_normalized_tfidf.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/pandas_sni.py` & `emm-2.1.1/emm/indexing/pandas_sni.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/spark_candidate_selection.py` & `emm-2.1.1/emm/indexing/spark_candidate_selection.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/spark_character_tokenizer.py` & `emm-2.1.1/emm/indexing/spark_character_tokenizer.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/spark_cos_sim_matcher.py` & `emm-2.1.1/emm/indexing/spark_cos_sim_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from pyspark.ml.util import DefaultParamsReadable, DefaultParamsWritable
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql import functions as F
 from pyspark.sql import types as T
 from pyspark.sql.types import ArrayType, FloatType, LongType, StringType, StructField, StructType
 from sparse_dot_topn import awesome_cossim_topn
 
+from emm.helper.blocking_functions import _parse_blocking_func
 from emm.helper.spark_custom_reader_writer import SparkReadable, SparkWriteable
 from emm.helper.spark_utils import set_spark_job_group
 from emm.indexing.base_indexer import BaseIndexer, CosSimBaseIndexer
 from emm.indexing.spark_character_tokenizer import SparkCharacterTokenizer
 from emm.indexing.spark_indexing_utils import (
     as_matrix,
     collect_matrix,
@@ -70,15 +71,15 @@
         parameters: dict | None = None,
         tokenizer: Literal["words", "characters"] = "words",
         ngram: int = 1,
         binary_countvectorizer: bool = False,
         num_candidates: int = 2,
         cos_sim_lower_bound: float = 0.5,
         max_features: int = 2**25,
-        blocking_func: Callable[[str], str] | None = None,
+        blocking_func: Callable[[str], str] | str | None = None,
         streaming: bool = False,
         indexer_id: int | None = None,
         keep_all_cols: bool = False,
         n_threads: int = 1,
     ) -> None:
         """Unfitted Cosine similarity indexer to generate candidate name-pairs of possible matches
 
@@ -142,15 +143,15 @@
         # would be another Estimator later in the pipeline. We don't want this.
         # https://spark.apache.org/docs/latest/ml-pipeline.html#pipeline-components
         self.cossim = (
             SparkCosSimMatcher(
                 num_candidates=parameters.get("num_candidates", 10),
                 cos_sim_lower_bound=parameters["cos_sim_lower_bound"],
                 streaming=parameters["streaming"],
-                blocking_func=parameters["blocking_func"],
+                blocking_func=_parse_blocking_func(parameters["blocking_func"]),
                 indexer_id=parameters["indexer_id"],
                 n_threads=parameters.get("n_threads", 1),
             )
             ._set(outputCol="candidates")
             ._set(inputCol="features")
         )
```

### Comparing `emm-2.1.0/emm/indexing/spark_indexing_utils.py` & `emm-2.1.1/emm/indexing/spark_indexing_utils.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/spark_normalized_tfidf.py` & `emm-2.1.1/emm/indexing/spark_normalized_tfidf.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/spark_sni.py` & `emm-2.1.1/emm/indexing/spark_sni.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/indexing/spark_word_tokenizer.py` & `emm-2.1.1/emm/indexing/spark_word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/loggers/__init__.py` & `emm-2.1.1/emm/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/loggers/logger.py` & `emm-2.1.1/emm/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/loggers/timer.py` & `emm-2.1.1/emm/loggers/timer.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/parameters.py` & `emm-2.1.1/emm/parameters.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/pipeline/__init__.py` & `emm-2.1.1/emm/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/pipeline/base_entity_matching.py` & `emm-2.1.1/emm/pipeline/base_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/pipeline/pandas_entity_matching.py` & `emm-2.1.1/emm/pipeline/pandas_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/pipeline/spark_entity_matching.py` & `emm-2.1.1/emm/pipeline/spark_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/__init__.py` & `emm-2.1.1/emm/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/abbreviation_util.py` & `emm-2.1.1/emm/preprocessing/abbreviation_util.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/base_name_preprocessor.py` & `emm-2.1.1/emm/preprocessing/base_name_preprocessor.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/functions.py` & `emm-2.1.1/emm/preprocessing/functions.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/pandas_functions.py` & `emm-2.1.1/emm/preprocessing/pandas_functions.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/pandas_preprocessor.py` & `emm-2.1.1/emm/preprocessing/pandas_preprocessor.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/spark_functions.py` & `emm-2.1.1/emm/preprocessing/spark_functions.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/preprocessing/spark_preprocessor.py` & `emm-2.1.1/emm/preprocessing/spark_preprocessor.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/resources.py` & `emm-2.1.1/emm/resources.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/supervised_model/__init__.py` & `emm-2.1.1/emm/supervised_model/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/supervised_model/base_supervised_model.py` & `emm-2.1.1/emm/supervised_model/base_supervised_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/supervised_model/pandas_supervised_model.py` & `emm-2.1.1/emm/supervised_model/pandas_supervised_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/supervised_model/spark_supervised_model.py` & `emm-2.1.1/emm/supervised_model/spark_supervised_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/threshold/__init__.py` & `emm-2.1.1/emm/threshold/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/threshold/threshold_decision.py` & `emm-2.1.1/emm/threshold/threshold_decision.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm/version.py` & `emm-2.1.1/emm/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-VERSION = "2.1.0"
+VERSION = "2.1.1"
 
 __version__ = VERSION
```

### Comparing `emm-2.1.0/emm.egg-info/PKG-INFO` & `emm-2.1.1/emm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emm
-Version: 2.1.0
+Version: 2.1.1
 Summary: Entity Matching Model package
 Author-email: Max Baak <max.baak@ing.com>, Stephane Collot <stephane.collot@gmail.com>, Apoorva Mahajan <apoorva.mahajan@ing.com>, Tomasz Waleń <tomasz.walen@ing.com>, Simon Brugman <simon.brugman@ing.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.20.1
```

### Comparing `emm-2.1.0/emm.egg-info/SOURCES.txt` & `emm-2.1.1/emm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/emm.egg-info/requires.txt` & `emm-2.1.1/emm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/example.py` & `emm-2.1.1/example.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/notebooks/01-entity-matching-pandas-version.ipynb` & `emm-2.1.1/notebooks/01-entity-matching-pandas-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/notebooks/02-entity-matching-spark-version.ipynb` & `emm-2.1.1/notebooks/02-entity-matching-spark-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/notebooks/03-entity-matching-training-pandas-version.ipynb` & `emm-2.1.1/notebooks/03-entity-matching-training-pandas-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/notebooks/04-entity-matching-aggregation-pandas-version.ipynb` & `emm-2.1.1/notebooks/04-entity-matching-aggregation-pandas-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/pyproject.toml` & `emm-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/__init__.py` & `emm-2.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/benchmark/test_bench.py` & `emm-2.1.1/tests/benchmark/test_bench.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/conftest.py` & `emm-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_artificial_integration.py` & `emm-2.1.1/tests/integration/test_artificial_integration.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_em_add_model.py` & `emm-2.1.1/tests/integration/test_em_add_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_entity_matching.py` & `emm-2.1.1/tests/integration/test_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_indexers.py` & `emm-2.1.1/tests/integration/test_indexers.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_normalized_tfidf.py` & `emm-2.1.1/tests/integration/test_normalized_tfidf.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_pandas_em.py` & `emm-2.1.1/tests/integration/test_pandas_em.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_readme_example.py` & `emm-2.1.1/tests/integration/test_readme_example.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_spark_vs_pandas.py` & `emm-2.1.1/tests/integration/test_spark_vs_pandas.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_supervised.py` & `emm-2.1.1/tests/integration/test_supervised.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/integration/test_training_classifier.py` & `emm-2.1.1/tests/integration/test_training_classifier.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/notebooks/test_notebooks.py` & `emm-2.1.1/tests/notebooks/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_abbreviations.py` & `emm-2.1.1/tests/unit/test_abbreviations.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_carry_on_cols.py` & `emm-2.1.1/tests/unit/test_carry_on_cols.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_commonshorthands.py` & `emm-2.1.1/tests/unit/test_commonshorthands.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_cos_sim_matcher.py` & `emm-2.1.1/tests/unit/test_cos_sim_matcher.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_custom_path.py` & `emm-2.1.1/tests/unit/test_custom_path.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_data.py` & `emm-2.1.1/tests/unit/test_data.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_entity_aggregation.py` & `emm-2.1.1/tests/unit/test_entity_aggregation.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_feature_extractor.py` & `emm-2.1.1/tests/unit/test_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_features_abbreviations.py` & `emm-2.1.1/tests/unit/test_features_abbreviations.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_features_lef.py` & `emm-2.1.1/tests/unit/test_features_lef.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_features_vocabulary.py` & `emm-2.1.1/tests/unit/test_features_vocabulary.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_name_preprocessing.py` & `emm-2.1.1/tests/unit/test_name_preprocessing.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_negative_sample_creation.py` & `emm-2.1.1/tests/unit/test_negative_sample_creation.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_serialization.py` & `emm-2.1.1/tests/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_threshold_decision.py` & `emm-2.1.1/tests/unit/test_threshold_decision.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_timer.py` & `emm-2.1.1/tests/unit/test_timer.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/unit/test_util.py` & `emm-2.1.1/tests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `emm-2.1.0/tests/utils.py` & `emm-2.1.1/tests/utils.py`

 * *Files identical despite different names*

