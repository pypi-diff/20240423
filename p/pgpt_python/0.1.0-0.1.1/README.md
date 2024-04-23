# Comparing `tmp/pgpt_python-0.1.0.tar.gz` & `tmp/pgpt_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpt_python-0.1.0.tar", max compression
+gzip compressed data, was "pgpt_python-0.1.1.tar", max compression
```

## Comparing `pgpt_python-0.1.0.tar` & `pgpt_python-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-01-22 21:05:51.078122 pgpt_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     6414 2024-01-22 22:18:41.310243 pgpt_python-0.1.0/README.md
--rw-r--r--   0        0        0     1228 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/__init__.py
--rw-r--r--   0        0        0     2202 2024-01-22 21:00:36.973904 pgpt_python-0.1.0/pgpt_python/client.py
--rw-r--r--   0        0        0      519 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/core/__init__.py
--rw-r--r--   0        0        0      426 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/core/api_error.py
--rw-r--r--   0        0        0      817 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      170 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      242 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/context_chunks/__init__.py
--rw-r--r--   0        0        0     6562 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/context_chunks/client.py
--rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/contextual_completions/__init__.py
--rw-r--r--   0        0        0    28568 2024-01-22 20:23:41.783297 pgpt_python-0.1.0/pgpt_python/resources/contextual_completions/client.py
--rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/embeddings/__init__.py
--rw-r--r--   0        0        0     3501 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/embeddings/client.py
--rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/health/__init__.py
--rw-r--r--   0        0        0     2598 2024-01-22 21:00:36.975470 pgpt_python-0.1.0/pgpt_python/resources/health/client.py
--rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/ingestion/__init__.py
--rw-r--r--   0        0        0    14332 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/resources/ingestion/client.py
--rw-r--r--   0        0        0     1431 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/__init__.py
--rw-r--r--   0        0        0     1144 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/chat_body.py
--rw-r--r--   0        0        0     1070 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/chunk.py
--rw-r--r--   0        0        0      956 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/chunks_response.py
--rw-r--r--   0        0        0     1123 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/completions_body.py
--rw-r--r--   0        0        0      904 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/context_filter.py
--rw-r--r--   0        0        0      924 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/embedding.py
--rw-r--r--   0        0        0      138 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/embeddings_body_input.py
--rw-r--r--   0        0        0      972 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/embeddings_response.py
--rw-r--r--   0        0        0      897 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/health_response.py
--rw-r--r--   0        0        0      966 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/http_validation_error.py
--rw-r--r--   0        0        0      975 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/ingest_response.py
--rw-r--r--   0        0        0      957 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/ingested_doc.py
--rw-r--r--   0        0        0     1349 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/open_ai_choice.py
--rw-r--r--   0        0        0     1249 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/open_ai_completion.py
--rw-r--r--   0        0        0      574 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/open_ai_completion_object.py
--rw-r--r--   0        0        0      986 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/open_ai_delta.py
--rw-r--r--   0        0        0     1155 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/open_ai_message.py
--rw-r--r--   0        0        0      653 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/open_ai_message_role.py
--rw-r--r--   0        0        0      992 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-01-22 12:45:52.000000 pgpt_python-0.1.0/pgpt_python/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      328 2024-01-22 21:38:42.275686 pgpt_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 pgpt_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-22 21:05:51.078122 pgpt_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6401 2024-01-22 22:31:37.496466 pgpt_python-0.1.1/README.md
+-rw-r--r--   0        0        0     1228 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/__init__.py
+-rw-r--r--   0        0        0     2202 2024-01-22 21:00:36.973904 pgpt_python-0.1.1/pgpt_python/client.py
+-rw-r--r--   0        0        0      519 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/core/api_error.py
+-rw-r--r--   0        0        0      817 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      170 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      242 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/context_chunks/__init__.py
+-rw-r--r--   0        0        0     6562 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/context_chunks/client.py
+-rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/contextual_completions/__init__.py
+-rw-r--r--   0        0        0    28568 2024-01-22 20:23:41.783297 pgpt_python-0.1.1/pgpt_python/resources/contextual_completions/client.py
+-rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/embeddings/__init__.py
+-rw-r--r--   0        0        0     3501 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/embeddings/client.py
+-rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/health/__init__.py
+-rw-r--r--   0        0        0     2598 2024-01-22 21:00:36.975470 pgpt_python-0.1.1/pgpt_python/resources/health/client.py
+-rw-r--r--   0        0        0       65 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/ingestion/__init__.py
+-rw-r--r--   0        0        0    14332 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/resources/ingestion/client.py
+-rw-r--r--   0        0        0     1431 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/__init__.py
+-rw-r--r--   0        0        0     1144 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/chat_body.py
+-rw-r--r--   0        0        0     1070 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/chunk.py
+-rw-r--r--   0        0        0      956 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/chunks_response.py
+-rw-r--r--   0        0        0     1123 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/completions_body.py
+-rw-r--r--   0        0        0      904 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/context_filter.py
+-rw-r--r--   0        0        0      924 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/embedding.py
+-rw-r--r--   0        0        0      138 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/embeddings_body_input.py
+-rw-r--r--   0        0        0      972 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/embeddings_response.py
+-rw-r--r--   0        0        0      897 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/health_response.py
+-rw-r--r--   0        0        0      966 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/http_validation_error.py
+-rw-r--r--   0        0        0      975 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/ingest_response.py
+-rw-r--r--   0        0        0      957 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/ingested_doc.py
+-rw-r--r--   0        0        0     1349 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/open_ai_choice.py
+-rw-r--r--   0        0        0     1249 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/open_ai_completion.py
+-rw-r--r--   0        0        0      574 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/open_ai_completion_object.py
+-rw-r--r--   0        0        0      986 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/open_ai_delta.py
+-rw-r--r--   0        0        0     1155 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/open_ai_message.py
+-rw-r--r--   0        0        0      653 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/open_ai_message_role.py
+-rw-r--r--   0        0        0      992 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-01-22 12:45:52.000000 pgpt_python-0.1.1/pgpt_python/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      328 2024-04-23 07:55:51.695491 pgpt_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6842 1970-01-01 00:00:00.000000 pgpt_python-0.1.1/PKG-INFO
```

### Comparing `pgpt_python-0.1.0/LICENSE` & `pgpt_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/README.md` & `pgpt_python-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# pgpt-python: Python SDK for PrivateGPT API
+# Python SDK for PrivateGPT API
 
-**pgpt-python** is an open-source Python SDK designed to interact with the PrivateGPT API. PrivateGPT is a popular AI Open Source project that provides secure and private access to advanced natural language processing capabilities. This SDK simplifies the integration of PrivateGPT into Python applications, allowing developers to harness the power of PrivateGPT for various language-related tasks.
+**pgpt_python** is an open-source Python SDK designed to interact with the PrivateGPT API. PrivateGPT is a popular AI Open Source project that provides secure and private access to advanced natural language processing capabilities. This SDK simplifies the integration of PrivateGPT into Python applications, allowing developers to harness the power of PrivateGPT for various language-related tasks.
 
 This SDK has been created using [Fern](https://buildwithfern.com/).
 
 ## Installation
 
-To install the pgpt-python SDK, use the following pip command:
+To install the pgpt_python SDK, use the following pip command:
 
 ```bash
-pip install pgpt-python
+pip install pgpt_python
 ```
 
 ## Getting Started
 
-To begin using pgpt-python with the PrivateGPT API, follow these steps:
+To begin using pgpt_python with the PrivateGPT API, follow these steps:
 
 1. **Import the PrivateGPTApi class:**
 
     ```python
     from pgpt_python.client import PrivateGPTApi
     ```
 
@@ -28,15 +28,15 @@
     client = PrivateGPTApi(base_url="http://localhost:8001")
     ```
 
 3. Certainly! Here's the completed "Perform API calls" section:
 
 ## Perform API Calls
 
-Once you have set up the PrivateGPTApi instance, you can perform various API calls using the pgpt-python SDK. Below are examples of common API calls:
+Once you have set up the PrivateGPTApi instance, you can perform various API calls using the pgpt_python SDK. Below are examples of common API calls:
 
 ### 1. **Health Check:**
 
 ```python
 print(client.health.health())
 
 > status='ok'
@@ -186,15 +186,15 @@
 client.ingestion.delete_ingested("e2989f56-1729-4557-b30a-e4b023628629")
 ```
 
 Delete previously ingested documents using their document IDs.
 
 ## Examples
 
-The provided `examples_script.py` showcases various features of the pgpt-python SDK. Feel free to explore and modify this script to suit your specific use cases.
+The provided `examples_script.py` showcases various features of the pgpt_python SDK. Feel free to explore and modify this script to suit your specific use cases.
 
 ## Documentation
 
 For detailed information on available methods and their parameters, refer to the [official documentation](https://docs.privategpt.dev/api-reference/overview/sd-ks).
 
 ## Contributing
```

### Comparing `pgpt_python-0.1.0/pgpt_python/__init__.py` & `pgpt_python-0.1.1/pgpt_python/__init__.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/client.py` & `pgpt_python-0.1.1/pgpt_python/client.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/core/__init__.py` & `pgpt_python-0.1.1/pgpt_python/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/core/client_wrapper.py` & `pgpt_python-0.1.1/pgpt_python/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/core/datetime_utils.py` & `pgpt_python-0.1.1/pgpt_python/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/core/jsonable_encoder.py` & `pgpt_python-0.1.1/pgpt_python/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/resources/context_chunks/client.py` & `pgpt_python-0.1.1/pgpt_python/resources/context_chunks/client.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/resources/contextual_completions/client.py` & `pgpt_python-0.1.1/pgpt_python/resources/contextual_completions/client.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/resources/embeddings/client.py` & `pgpt_python-0.1.1/pgpt_python/resources/embeddings/client.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/resources/health/client.py` & `pgpt_python-0.1.1/pgpt_python/resources/health/client.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/resources/ingestion/client.py` & `pgpt_python-0.1.1/pgpt_python/resources/ingestion/client.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/__init__.py` & `pgpt_python-0.1.1/pgpt_python/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/chat_body.py` & `pgpt_python-0.1.1/pgpt_python/types/chat_body.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/chunk.py` & `pgpt_python-0.1.1/pgpt_python/types/chunk.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/chunks_response.py` & `pgpt_python-0.1.1/pgpt_python/types/chunks_response.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/completions_body.py` & `pgpt_python-0.1.1/pgpt_python/types/completions_body.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/context_filter.py` & `pgpt_python-0.1.1/pgpt_python/types/context_filter.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/embedding.py` & `pgpt_python-0.1.1/pgpt_python/types/embedding.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/embeddings_response.py` & `pgpt_python-0.1.1/pgpt_python/types/embeddings_response.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/health_response.py` & `pgpt_python-0.1.1/pgpt_python/types/health_response.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/http_validation_error.py` & `pgpt_python-0.1.1/pgpt_python/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/ingest_response.py` & `pgpt_python-0.1.1/pgpt_python/types/ingest_response.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/ingested_doc.py` & `pgpt_python-0.1.1/pgpt_python/types/ingested_doc.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/open_ai_choice.py` & `pgpt_python-0.1.1/pgpt_python/types/open_ai_choice.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/open_ai_completion.py` & `pgpt_python-0.1.1/pgpt_python/types/open_ai_completion.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/open_ai_completion_object.py` & `pgpt_python-0.1.1/pgpt_python/types/open_ai_completion_object.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/open_ai_delta.py` & `pgpt_python-0.1.1/pgpt_python/types/open_ai_delta.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/open_ai_message.py` & `pgpt_python-0.1.1/pgpt_python/types/open_ai_message.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/open_ai_message_role.py` & `pgpt_python-0.1.1/pgpt_python/types/open_ai_message_role.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/pgpt_python/types/validation_error.py` & `pgpt_python-0.1.1/pgpt_python/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `pgpt_python-0.1.0/PKG-INFO` & `pgpt_python-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: pgpt_python
-Version: 0.1.0
+Version: 0.1.1
 Summary: PrivateGPT Python SDK
 Author: imartinez
 Author-email: ivanmartit@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Description-Content-Type: text/markdown
 
-# pgpt-python: Python SDK for PrivateGPT API
+# Python SDK for PrivateGPT API
 
-**pgpt-python** is an open-source Python SDK designed to interact with the PrivateGPT API. PrivateGPT is a popular AI Open Source project that provides secure and private access to advanced natural language processing capabilities. This SDK simplifies the integration of PrivateGPT into Python applications, allowing developers to harness the power of PrivateGPT for various language-related tasks.
+**pgpt_python** is an open-source Python SDK designed to interact with the PrivateGPT API. PrivateGPT is a popular AI Open Source project that provides secure and private access to advanced natural language processing capabilities. This SDK simplifies the integration of PrivateGPT into Python applications, allowing developers to harness the power of PrivateGPT for various language-related tasks.
 
 This SDK has been created using [Fern](https://buildwithfern.com/).
 
 ## Installation
 
-To install the pgpt-python SDK, use the following pip command:
+To install the pgpt_python SDK, use the following pip command:
 
 ```bash
-pip install pgpt-python
+pip install pgpt_python
 ```
 
 ## Getting Started
 
-To begin using pgpt-python with the PrivateGPT API, follow these steps:
+To begin using pgpt_python with the PrivateGPT API, follow these steps:
 
 1. **Import the PrivateGPTApi class:**
 
     ```python
     from pgpt_python.client import PrivateGPTApi
     ```
 
@@ -41,15 +42,15 @@
     client = PrivateGPTApi(base_url="http://localhost:8001")
     ```
 
 3. Certainly! Here's the completed "Perform API calls" section:
 
 ## Perform API Calls
 
-Once you have set up the PrivateGPTApi instance, you can perform various API calls using the pgpt-python SDK. Below are examples of common API calls:
+Once you have set up the PrivateGPTApi instance, you can perform various API calls using the pgpt_python SDK. Below are examples of common API calls:
 
 ### 1. **Health Check:**
 
 ```python
 print(client.health.health())
 
 > status='ok'
@@ -199,15 +200,15 @@
 client.ingestion.delete_ingested("e2989f56-1729-4557-b30a-e4b023628629")
 ```
 
 Delete previously ingested documents using their document IDs.
 
 ## Examples
 
-The provided `examples_script.py` showcases various features of the pgpt-python SDK. Feel free to explore and modify this script to suit your specific use cases.
+The provided `examples_script.py` showcases various features of the pgpt_python SDK. Feel free to explore and modify this script to suit your specific use cases.
 
 ## Documentation
 
 For detailed information on available methods and their parameters, refer to the [official documentation](https://docs.privategpt.dev/api-reference/overview/sd-ks).
 
 ## Contributing
```

