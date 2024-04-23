# Comparing `tmp/getai-0.0.1.tar.gz` & `tmp/getai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getai-0.0.1.tar", max compression
+gzip compressed data, was "getai-0.0.2.tar", max compression
```

## Comparing `getai-0.0.1.tar` & `getai-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.1/LICENSE
--rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.1/getai/__init__.py
--rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.1/getai/__main__.py
--rw-r--r--   0        0        0    13484 2024-04-23 11:37:33.678508 getai-0.0.1/getai/dataset_downloader.py
--rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.1/getai/getai_config.yaml
--rw-r--r--   0        0        0     7327 2024-04-23 11:39:31.809895 getai-0.0.1/getai/main.py
--rw-r--r--   0        0        0    27321 2024-04-23 11:38:50.364408 getai-0.0.1/getai/model_downloader.py
--rw-r--r--   0        0        0     3088 2024-04-23 11:52:12.548596 getai-0.0.1/getai/utils.py
--rw-r--r--   0        0        0      687 2024-04-23 11:56:07.243281 getai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.2/LICENSE
+-rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.2/getai/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.2/getai/__main__.py
+-rw-r--r--   0        0        0    13484 2024-04-23 11:37:33.678508 getai-0.0.2/getai/dataset_downloader.py
+-rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.2/getai/getai_config.yaml
+-rw-r--r--   0        0        0     7327 2024-04-23 11:39:31.809895 getai-0.0.2/getai/main.py
+-rw-r--r--   0        0        0    27321 2024-04-23 11:38:50.364408 getai-0.0.2/getai/model_downloader.py
+-rw-r--r--   0        0        0     3088 2024-04-23 11:52:12.548596 getai-0.0.2/getai/utils.py
+-rw-r--r--   0        0        0      736 2024-04-23 12:08:28.720863 getai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.2/PKG-INFO
```

### Comparing `getai-0.0.1/LICENSE` & `getai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `getai-0.0.1/README.md` & `getai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `getai-0.0.1/getai/dataset_downloader.py` & `getai-0.0.2/getai/dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.1/getai/main.py` & `getai-0.0.2/getai/main.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.1/getai/model_downloader.py` & `getai-0.0.2/getai/model_downloader.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.1/getai/utils.py` & `getai-0.0.2/getai/utils.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.1/pyproject.toml` & `getai-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getai"
-version = "0.0.1"
+version = "0.0.2"
 description = "GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more."
 authors = ["Ben Gorlick <ben@unifiedlearning.ai>"]
 license = "MIT - with attribution"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -18,7 +18,10 @@
 pytest = "^8.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 include = ["getai/getai_config.yaml"]
+
+[tool.poetry.scripts]
+getai = "getai.main:main"
```

### Comparing `getai-0.0.1/PKG-INFO` & `getai-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getai
-Version: 0.0.1
+Version: 0.0.2
 Summary: GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more.
 License: MIT - with attribution
 Author: Ben Gorlick
 Author-email: ben@unifiedlearning.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

