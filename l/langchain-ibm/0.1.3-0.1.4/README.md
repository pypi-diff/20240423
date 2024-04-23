# Comparing `tmp/langchain_ibm-0.1.3.tar.gz` & `tmp/langchain_ibm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ibm-0.1.3.tar", max compression
+gzip compressed data, was "langchain_ibm-0.1.4.tar", max compression
```

## Comparing `langchain_ibm-0.1.3.tar` & `langchain_ibm-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-03-14 23:00:11.639670 langchain_ibm-0.1.3/LICENSE
--rw-r--r--   0        0        0     4395 2024-03-14 23:00:11.639670 langchain_ibm-0.1.3/README.md
--rw-r--r--   0        0        0       68 2024-03-14 23:00:11.639670 langchain_ibm-0.1.3/langchain_ibm/__init__.py
--rw-r--r--   0        0        0    16309 2024-03-14 23:00:11.639670 langchain_ibm-0.1.3/langchain_ibm/llms.py
--rw-r--r--   0        0        0        0 2024-03-14 23:00:11.639670 langchain_ibm-0.1.3/langchain_ibm/py.typed
--rw-r--r--   0        0        0     2559 2024-03-14 23:00:11.639670 langchain_ibm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 langchain_ibm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4395 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/README.md
+-rw-r--r--   0        0        0      144 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/__init__.py
+-rw-r--r--   0        0        0     6888 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/embeddings.py
+-rw-r--r--   0        0        0    16309 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/llms.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/py.typed
+-rw-r--r--   0        0        0     2559 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 langchain_ibm-0.1.4/PKG-INFO
```

### Comparing `langchain_ibm-0.1.3/LICENSE` & `langchain_ibm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.3/README.md` & `langchain_ibm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.3/langchain_ibm/llms.py` & `langchain_ibm-0.1.4/langchain_ibm/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.3/pyproject.toml` & `langchain_ibm-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-ibm"
-version = "0.1.3"
+version = "0.1.4"
 description = "An integration package connecting IBM watsonx.ai and LangChain"
 authors = ["IBM"]
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/ibm"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-langchain-core = "^0.1.29"
-ibm-watsonx-ai = "^0.2.0"
+langchain-core = "^0.1.42"
+ibm-watsonx-ai = "^0.2.6"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
```

### Comparing `langchain_ibm-0.1.3/PKG-INFO` & `langchain_ibm-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-ibm
-Version: 0.1.3
+Version: 0.1.4
 Summary: An integration package connecting IBM watsonx.ai and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Author: IBM
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ibm-watsonx-ai (>=0.2.0,<0.3.0)
-Requires-Dist: langchain-core (>=0.1.29,<0.2.0)
+Requires-Dist: ibm-watsonx-ai (>=0.2.6,<0.3.0)
+Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/ibm
 Description-Content-Type: text/markdown
 
 # langchain-ibm
 
 This package provides the integration between LangChain and IBM watsonx.ai through the `ibm-watsonx-ai` SDK.
```

