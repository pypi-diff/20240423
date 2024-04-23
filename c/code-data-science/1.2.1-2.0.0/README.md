# Comparing `tmp/code_data_science-1.2.1.tar.gz` & `tmp/code_data_science-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_data_science-1.2.1.tar", last modified: Thu Nov 30 06:09:47 2023, max compression
+gzip compressed data, was "code_data_science-2.0.0.tar", last modified: Mon Apr 22 21:08:36 2024, max compression
```

## Comparing `code_data_science-1.2.1.tar` & `code_data_science-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 06:09:47.429098 code_data_science-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-30 06:09:47.429098 code_data_science-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-30 06:09:33.000000 code_data_science-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 06:09:47.425098 code_data_science-1.2.1/code_data_science/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 06:09:47.429098 code_data_science-1.2.1/code_data_science/clustering_src/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/datasets_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/hf_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/logging_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/training_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/clustering_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/data_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/data_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/palette.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/scm_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/tree_data_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 06:09:47.429098 code_data_science-1.2.1/code_data_science/types/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/types/notebook_parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/types/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/unique_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2023-11-30 06:09:33.000000 code_data_science-1.2.1/code_data_science/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 06:09:47.429098 code_data_science-1.2.1/code_data_science.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-30 06:09:47.000000 code_data_science-1.2.1/code_data_science.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-11-30 06:09:47.000000 code_data_science-1.2.1/code_data_science.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 06:09:47.000000 code_data_science-1.2.1/code_data_science.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-30 06:09:47.000000 code_data_science-1.2.1/code_data_science.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-30 06:09:47.000000 code_data_science-1.2.1/code_data_science.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-11-30 06:09:33.000000 code_data_science-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 06:09:47.429098 code_data_science-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:08:36.945964 code_data_science-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-22 21:08:36.945964 code_data_science-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-22 21:08:26.000000 code_data_science-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:08:36.941964 code_data_science-2.0.0/code_data_science/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:08:36.945964 code_data_science-2.0.0/code_data_science/clustering_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/datasets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/hf_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/clustering_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/data_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/data_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/palette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-22 21:08:26.000000 code_data_science-2.0.0/code_data_science/scm_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-22 21:08:27.000000 code_data_science-2.0.0/code_data_science/tree_data_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:08:36.945964 code_data_science-2.0.0/code_data_science/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-22 21:08:27.000000 code_data_science-2.0.0/code_data_science/types/notebook_parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 21:08:27.000000 code_data_science-2.0.0/code_data_science/types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-22 21:08:27.000000 code_data_science-2.0.0/code_data_science/unique_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-22 21:08:27.000000 code_data_science-2.0.0/code_data_science/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:08:36.945964 code_data_science-2.0.0/code_data_science.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-22 21:08:36.000000 code_data_science-2.0.0/code_data_science.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-22 21:08:36.000000 code_data_science-2.0.0/code_data_science.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:08:36.000000 code_data_science-2.0.0/code_data_science.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 21:08:36.000000 code_data_science-2.0.0/code_data_science.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 21:08:36.000000 code_data_science-2.0.0/code_data_science.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-22 21:08:27.000000 code_data_science-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 21:08:36.945964 code_data_science-2.0.0/setup.cfg
```

### Comparing `code_data_science-1.2.1/code_data_science/clustering_src/datasets_loader.py` & `code_data_science-2.0.0/code_data_science/clustering_src/datasets_loader.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/clustering_src/distributed_utils.py` & `code_data_science-2.0.0/code_data_science/clustering_src/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/clustering_src/hf_trainer.py` & `code_data_science-2.0.0/code_data_science/clustering_src/hf_trainer.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/clustering_src/logging_callback.py` & `code_data_science-2.0.0/code_data_science/clustering_src/logging_callback.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/clustering_src/preprocessing_utils.py` & `code_data_science-2.0.0/code_data_science/clustering_src/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/clustering_src/training_args.py` & `code_data_science-2.0.0/code_data_science/clustering_src/training_args.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/clustering_src/utils.py` & `code_data_science-2.0.0/code_data_science/clustering_src/utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/data_grid.py` & `code_data_science-2.0.0/code_data_science/data_grid.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/scm_link.py` & `code_data_science-2.0.0/code_data_science/scm_link.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/tree_data_grid.py` & `code_data_science-2.0.0/code_data_science/tree_data_grid.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/unique_dictionaries.py` & `code_data_science-2.0.0/code_data_science/unique_dictionaries.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science/versions.py` & `code_data_science-2.0.0/code_data_science/versions.py`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/code_data_science.egg-info/SOURCES.txt` & `code_data_science-2.0.0/code_data_science.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `code_data_science-1.2.1/pyproject.toml` & `code_data_science-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "code_data_science"
-version = "1.2.1"
+version = "2.0.0"
 description = "A python implementation of various tools used in code data science."
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io" },
     { name = "Kyle Scully", email = "kyle@moderne.io" }
 ]
 license = { text = "Apache-2.0" }
 dependencies = ["pandas==2.0.3", "ipython==8.13.0"]
```

