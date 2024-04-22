# Comparing `tmp/databonsai-0.5.0.tar.gz` & `tmp/databonsai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databonsai-0.5.0.tar", last modified: Thu Apr 18 23:33:01 2024, max compression
+gzip compressed data, was "databonsai-0.6.0.tar", last modified: Mon Apr 22 23:22:00 2024, max compression
```

## Comparing `databonsai-0.5.0.tar` & `databonsai-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.726221 databonsai-0.5.0/
--rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     8368 2024-04-18 23:33:01.724211 databonsai-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     7489 2024-04-18 21:28:28.000000 databonsai-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.632252 databonsai-0.5.0/databonsai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.5.0/databonsai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.681449 databonsai-0.5.0/databonsai/categorize/
--rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.5.0/databonsai/categorize/__init__.py
--rw-rw-rw-   0        0        0     7771 2024-04-18 21:45:39.000000 databonsai-0.5.0/databonsai/categorize/base_categorizer.py
--rw-rw-rw-   0        0        0     5634 2024-04-17 06:22:44.000000 databonsai-0.5.0/databonsai/categorize/multi_categorizer.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.700304 databonsai-0.5.0/databonsai/llm_providers/
--rw-rw-rw-   0        0        0      209 2024-04-18 20:42:59.000000 databonsai-0.5.0/databonsai/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     6003 2024-04-18 21:09:15.000000 databonsai-0.5.0/databonsai/llm_providers/anthropic_provider.py
--rw-rw-rw-   0        0        0     1246 2024-04-18 21:04:49.000000 databonsai-0.5.0/databonsai/llm_providers/llm_provider.py
--rw-rw-rw-   0        0        0     3950 2024-04-18 21:09:34.000000 databonsai-0.5.0/databonsai/llm_providers/ollama_provider.py
--rw-rw-rw-   0        0        0     6266 2024-04-18 21:09:07.000000 databonsai-0.5.0/databonsai/llm_providers/openai_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.714712 databonsai-0.5.0/databonsai/transform/
--rw-rw-rw-   0        0        0      104 2024-04-07 00:17:44.000000 databonsai-0.5.0/databonsai/transform/__init__.py
--rw-rw-rw-   0        0        0     5564 2024-04-17 05:51:57.000000 databonsai-0.5.0/databonsai/transform/base_transformer.py
--rw-rw-rw-   0        0        0     9886 2024-04-17 06:08:58.000000 databonsai-0.5.0/databonsai/transform/decompose_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.717805 databonsai-0.5.0/databonsai/utils/
--rw-rw-rw-   0        0        0       59 2024-04-13 21:14:08.000000 databonsai-0.5.0/databonsai/utils/__init__.py
--rw-rw-rw-   0        0        0     5583 2024-04-14 20:38:55.000000 databonsai-0.5.0/databonsai/utils/apply.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.717805 databonsai-0.5.0/databonsai.egg-info/
--rw-rw-rw-   0        0        0     8368 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 23:33:01.000000 databonsai-0.5.0/databonsai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      580 2024-04-18 23:32:31.000000 databonsai-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 23:33:01.726221 databonsai-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1054 2024-04-18 23:32:21.000000 databonsai-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 23:33:01.717805 databonsai-0.5.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.5.0/tests/test_categorization.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.690665 databonsai-0.6.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     8579 2024-04-22 23:22:00.690665 databonsai-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7700 2024-04-22 23:08:59.000000 databonsai-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.633943 databonsai-0.6.0/databonsai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.6.0/databonsai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.671694 databonsai-0.6.0/databonsai/categorize/
+-rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.6.0/databonsai/categorize/__init__.py
+-rw-rw-rw-   0        0        0     8044 2024-04-22 23:04:15.000000 databonsai-0.6.0/databonsai/categorize/base_categorizer.py
+-rw-rw-rw-   0        0        0     5830 2024-04-22 23:04:26.000000 databonsai-0.6.0/databonsai/categorize/multi_categorizer.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.677925 databonsai-0.6.0/databonsai/llm_providers/
+-rw-rw-rw-   0        0        0      209 2024-04-18 20:42:59.000000 databonsai-0.6.0/databonsai/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     6003 2024-04-18 21:09:15.000000 databonsai-0.6.0/databonsai/llm_providers/anthropic_provider.py
+-rw-rw-rw-   0        0        0     1246 2024-04-18 21:04:49.000000 databonsai-0.6.0/databonsai/llm_providers/llm_provider.py
+-rw-rw-rw-   0        0        0     3950 2024-04-18 21:09:34.000000 databonsai-0.6.0/databonsai/llm_providers/ollama_provider.py
+-rw-rw-rw-   0        0        0     6266 2024-04-22 23:05:34.000000 databonsai-0.6.0/databonsai/llm_providers/openai_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.681842 databonsai-0.6.0/databonsai/transform/
+-rw-rw-rw-   0        0        0      100 2024-04-22 22:21:51.000000 databonsai-0.6.0/databonsai/transform/__init__.py
+-rw-rw-rw-   0        0        0     5650 2024-04-22 20:55:37.000000 databonsai-0.6.0/databonsai/transform/base_transformer.py
+-rw-rw-rw-   0        0        0     9868 2024-04-22 22:12:09.000000 databonsai-0.6.0/databonsai/transform/extract_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.684594 databonsai-0.6.0/databonsai/utils/
+-rw-rw-rw-   0        0        0       86 2024-04-22 21:08:24.000000 databonsai-0.6.0/databonsai/utils/__init__.py
+-rw-rw-rw-   0        0        0    10520 2024-04-22 23:06:15.000000 databonsai-0.6.0/databonsai/utils/apply.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.688984 databonsai-0.6.0/databonsai.egg-info/
+-rw-rw-rw-   0        0        0     8579 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      580 2024-04-22 23:21:13.000000 databonsai-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 23:22:00.690665 databonsai-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2024-04-22 23:21:19.000000 databonsai-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.686090 databonsai-0.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.6.0/tests/test_categorization.py
```

### Comparing `databonsai-0.5.0/LICENSE` & `databonsai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databonsai-0.5.0/PKG-INFO` & `databonsai-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 ## Clean &amp; curate your data with LLMs
 
 databonsai is a Python library that uses LLMs to perform data cleaning tasks.
 
 ## Features
 
 -   Suite of tools for data processing using LLMs including categorization,
-    transformation, and decomposition
+    transformation, and extraction
 -   Validation of LLM outputs
 -   Batch processing for token savings
 -   Retry logic with exponential backoff for handling rate limits and transient
     errors
 
 ## Installation
 
@@ -117,48 +117,42 @@
 
 Output:
 
 ```python
 ['Weather', 'Sports', 'Celebrities']
 ```
 
-### Dataframes & Lists
+### AutoBatch for Larger datasets
 
-If you have a pandas dataframe or list, use `apply_to_column_batch` for some
-handy features:
+If you have a pandas dataframe or list, use `apply_to_column_autobatch`
 
--   batching saves tokens by not resending the schema each time.
--   progress bar
--   returns the last successful index so you can resume from there, in case of
-    any error (llm_provider already implements exponential backoff, but just in
-    case)
--   modifies your output list in place, so you don't lose any progress
+-   Batching data for LLM api calls saves tokens by not sending the prompt for
+    every row. However, too large a batch size / complex tasks can lead to
+    errors. Naturally, the better the LLM model, the larger the batch size you
+    can use.
 
-Use the method as such:
+-   This batching is handled adaptively (i.e., it will increase the batch size
+    if the response is valid and reduce it if it's not, with a decay factor)
 
-```python
-success_idx = apply_to_column_batch(input_column, output_column, function, batch_size, start_idx)
-```
-
-Parameters:
+Other features:
 
--   `input_column`: The name of the column from which data will be read.
--   `output_column`: The name of the column to which data will be written.
--   `function`: The function to apply to each batch of data.
--   `batch_size`: The number of rows in each batch.
--   `start_idx`: The starting index from which to begin processing.
+-   Progress bar
+-   Returns the last successful index so you can resume from there, in case it
+    exceeds max_retries
+-   Modifies your output list in place, so you don't lose any progress
 
-Returns:
+Retry Logic:
 
--   `success_idx`: The index of the last successful row processed.
-
-(Continued from the previous code example)
+-   LLM providers have retry logic built in for API related errors. This can be
+    configured in the provider.
+-   The retry logic in the apply_to_column_autobatch is for handling invalid
+    responses (e.g. unexpected category, different number of outputs, etc.)
 
 ```python
-from databonsai.utils import apply_to_column_batch, apply_to_column
+from databonsai.utils import apply_to_column_batch, apply_to_column, apply_to_column_autobatch
 import pandas as pd
 
 headlines = [
     "Massive Blizzard Hits the Northeast, Thousands Without Power",
     "Local High School Basketball Team Wins State Championship After Dramatic Final",
     "Celebrated Actor Launches New Environmental Awareness Campaign",
     "President Announces Comprehensive Plan to Combat Cybersecurity Threats",
@@ -167,33 +161,40 @@
     "Olympic Gold Medalist Announces Retirement, Plans Coaching Career",
     "Film Industry Legends Team Up for Blockbuster Biopic",
     "Government Proposes Sweeping Reforms in Public Health Sector",
     "Startup Develops App That Predicts Traffic Patterns Using AI",
 ]
 df = pd.DataFrame(headlines, columns=["Headline"])
 df["Category"] = None # Initialize it if it doesn't exist, as we modify it in place
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
+success_idx = apply_to_column_autobatch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
 ```
 
-By default, exponential backoff is used to handle rate limiting. This is handled
-in the LLM providers and can be configured.
+There are many more options available for autobatch, such as setting a
+max_retries, decay factor, and more. Check [Utils](./docs/Utils.md) for more
+details
 
 If it fails midway (even after exponential backoff), you can resume from the
 last successful index + 1.
 
 ```python
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10, start_idx=success_idx+1)
+success_idx = apply_to_column_autobatch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10, start_idx=success_idx+1)
 ```
 
 This also works for regular python lists.
 
 Note that the better the LLM model, the greater the batch_size you can use
 (depending on the length of your inputs). If you're getting errors, reduce the
 batch_size, or use a better LLM model.
 
+To use it with batching, but with a fixed batch size:
+
+```python
+success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
+```
+
 To use it without batching:
 
 ```python
 success_idx = apply_to_column( df["Headline"], df["Category"], categorizer.categorize)
 ```
 
 ### View System Prompt
@@ -218,16 +219,16 @@
 ### Tools (Check out the docs for usage examples and details)
 
 -   [BaseCategorizer](./docs/BaseCategorizer.md) - categorize data into a
     category
 -   [MultiCategorizer](./docs/MultiCategorizer.md) - categorize data into
     multiple categories
 -   [BaseTransformer](./docs/BaseTransformer.md) - transform data with a prompt
--   [DecomposeTransformer](./docs/DecomposeTransformer.md) - decompose data into
-    a structured format based on a schema
+-   [ExtractTransformer](./docs/ExtractTransformer.md) - Extract data into a
+    structured format based on a schema
 -   .. more coming soon!
 
 ### LLM Providers
 
 -   [OpenAIProvider](./docs/OpenAIProvider.md) - OpenAI
 -   [AnthropicProvider](./docs/AnthropicProvider.md) - Anthropic
 -   [OllamaProvider](./docs/OllamaProvider.md) - Ollama
```

### Comparing `databonsai-0.5.0/README.md` & `databonsai-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## Clean &amp; curate your data with LLMs
 
 databonsai is a Python library that uses LLMs to perform data cleaning tasks.
 
 ## Features
 
 -   Suite of tools for data processing using LLMs including categorization,
-    transformation, and decomposition
+    transformation, and extraction
 -   Validation of LLM outputs
 -   Batch processing for token savings
 -   Retry logic with exponential backoff for handling rate limits and transient
     errors
 
 ## Installation
 
@@ -92,48 +92,42 @@
 
 Output:
 
 ```python
 ['Weather', 'Sports', 'Celebrities']
 ```
 
-### Dataframes & Lists
+### AutoBatch for Larger datasets
 
-If you have a pandas dataframe or list, use `apply_to_column_batch` for some
-handy features:
+If you have a pandas dataframe or list, use `apply_to_column_autobatch`
 
--   batching saves tokens by not resending the schema each time.
--   progress bar
--   returns the last successful index so you can resume from there, in case of
-    any error (llm_provider already implements exponential backoff, but just in
-    case)
--   modifies your output list in place, so you don't lose any progress
+-   Batching data for LLM api calls saves tokens by not sending the prompt for
+    every row. However, too large a batch size / complex tasks can lead to
+    errors. Naturally, the better the LLM model, the larger the batch size you
+    can use.
 
-Use the method as such:
+-   This batching is handled adaptively (i.e., it will increase the batch size
+    if the response is valid and reduce it if it's not, with a decay factor)
 
-```python
-success_idx = apply_to_column_batch(input_column, output_column, function, batch_size, start_idx)
-```
-
-Parameters:
+Other features:
 
--   `input_column`: The name of the column from which data will be read.
--   `output_column`: The name of the column to which data will be written.
--   `function`: The function to apply to each batch of data.
--   `batch_size`: The number of rows in each batch.
--   `start_idx`: The starting index from which to begin processing.
+-   Progress bar
+-   Returns the last successful index so you can resume from there, in case it
+    exceeds max_retries
+-   Modifies your output list in place, so you don't lose any progress
 
-Returns:
+Retry Logic:
 
--   `success_idx`: The index of the last successful row processed.
-
-(Continued from the previous code example)
+-   LLM providers have retry logic built in for API related errors. This can be
+    configured in the provider.
+-   The retry logic in the apply_to_column_autobatch is for handling invalid
+    responses (e.g. unexpected category, different number of outputs, etc.)
 
 ```python
-from databonsai.utils import apply_to_column_batch, apply_to_column
+from databonsai.utils import apply_to_column_batch, apply_to_column, apply_to_column_autobatch
 import pandas as pd
 
 headlines = [
     "Massive Blizzard Hits the Northeast, Thousands Without Power",
     "Local High School Basketball Team Wins State Championship After Dramatic Final",
     "Celebrated Actor Launches New Environmental Awareness Campaign",
     "President Announces Comprehensive Plan to Combat Cybersecurity Threats",
@@ -142,33 +136,40 @@
     "Olympic Gold Medalist Announces Retirement, Plans Coaching Career",
     "Film Industry Legends Team Up for Blockbuster Biopic",
     "Government Proposes Sweeping Reforms in Public Health Sector",
     "Startup Develops App That Predicts Traffic Patterns Using AI",
 ]
 df = pd.DataFrame(headlines, columns=["Headline"])
 df["Category"] = None # Initialize it if it doesn't exist, as we modify it in place
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
+success_idx = apply_to_column_autobatch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
 ```
 
-By default, exponential backoff is used to handle rate limiting. This is handled
-in the LLM providers and can be configured.
+There are many more options available for autobatch, such as setting a
+max_retries, decay factor, and more. Check [Utils](./docs/Utils.md) for more
+details
 
 If it fails midway (even after exponential backoff), you can resume from the
 last successful index + 1.
 
 ```python
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10, start_idx=success_idx+1)
+success_idx = apply_to_column_autobatch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10, start_idx=success_idx+1)
 ```
 
 This also works for regular python lists.
 
 Note that the better the LLM model, the greater the batch_size you can use
 (depending on the length of your inputs). If you're getting errors, reduce the
 batch_size, or use a better LLM model.
 
+To use it with batching, but with a fixed batch size:
+
+```python
+success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
+```
+
 To use it without batching:
 
 ```python
 success_idx = apply_to_column( df["Headline"], df["Category"], categorizer.categorize)
 ```
 
 ### View System Prompt
@@ -193,16 +194,16 @@
 ### Tools (Check out the docs for usage examples and details)
 
 -   [BaseCategorizer](./docs/BaseCategorizer.md) - categorize data into a
     category
 -   [MultiCategorizer](./docs/MultiCategorizer.md) - categorize data into
     multiple categories
 -   [BaseTransformer](./docs/BaseTransformer.md) - transform data with a prompt
--   [DecomposeTransformer](./docs/DecomposeTransformer.md) - decompose data into
-    a structured format based on a schema
+-   [ExtractTransformer](./docs/ExtractTransformer.md) - Extract data into a
+    structured format based on a schema
 -   .. more coming soon!
 
 ### LLM Providers
 
 -   [OpenAIProvider](./docs/OpenAIProvider.md) - OpenAI
 -   [AnthropicProvider](./docs/AnthropicProvider.md) - Anthropic
 -   [OllamaProvider](./docs/OllamaProvider.md) - Ollama
```

### Comparing `databonsai-0.5.0/databonsai/categorize/base_categorizer.py` & `databonsai-0.6.0/databonsai/categorize/base_categorizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     @property
     def system_message(self) -> str:
         system_message = f"""
         Each category is formatted as <category>: <description of data that fits the category>
         {str(self.categories)}
         Classify the given text snippet into one of the following categories:
         {str(list(self.categories.keys()))}
+        Do not use any other categories.
         Only reply with the category. Do not make any other conversation.
         """
 
         # Add in fewshot examples
         if self.examples:
             for example in self.examples:
                 system_message += (
@@ -108,27 +109,28 @@
     @computed_field
     @property
     def system_message_batch(self) -> str:
         system_message = f"""
         Each category is formatted as <category>: <description of data that fits the category>
         {str(self.categories)}
         Classify each given text snippet into one of the following categories:
-        {str(list(self.categories.keys()))}. If there are multiple snippets, separate each category with ||. 
+        {str(list(self.categories.keys()))}.
+         Do not use any other categories. If there are multiple snippets, separate each category with ||. 
         EXAMPLE: <Text about category 1>  RESPONSE: <Category 1> 
         EXAMPLE: Content 1: <Text about category 1>, Content 2: <Text about category 2> RESPONSE: <Category 1> || <Category 2>
         Choose one category for each text snippet.
         Only reply with the categories. Do not make any other conversation.
         """
 
         # Add in fewshot examples
         if self.examples:
             system_message += "\n EXAMPLE:"
             for idx, example in enumerate(self.examples):
                 system_message += f"Content {idx+1}: {example['example']}, "
-            system_message += f"\n RESPONSE: {','.join([example['response'] for example in self.examples])}"
+            system_message += f"\n RESPONSE: {'||'.join([example['response'] for example in self.examples])}"
 
         return system_message
 
     def categorize(self, input_data: str) -> str:
         """
         Categorizes the input data using the specified LLM provider.
 
@@ -162,15 +164,17 @@
 
         Returns:
             List[str]: A list of predicted categories for the input data.
 
         Raises:
             ValueError: If the predicted categories are not a subset of the provided categories.
         """
-
+        # If there is only one input, call the categorize method
+        if len(input_data) == 1:
+            return self.validate_predicted_categories([self.categorize(input_data[0])])
         # Call the LLM provider to get the predicted category
         response = self.llm_provider.generate_batch(
             self.system_message_batch, input_data
         )
         predicted_categories = [category.strip() for category in response.split("||")]
         if len(predicted_categories) != len(input_data):
             raise ValueError(
```

### Comparing `databonsai-0.5.0/databonsai/categorize/multi_categorizer.py` & `databonsai-0.6.0/databonsai/categorize/multi_categorizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     @property
     def system_message(self) -> str:
         system_message = f"""
         Each category is formatted as <category>: <description of data that fits the category>
         {str(self.categories)}
         Classify the given text snippet into one or more of the following categories:
         {str(list(self.categories.keys()))}
+        Do not use any other categories.
         Reply with a list of categories separated by || for each text snippet. Do not make any other conversation.
         """
 
         # Add in fewshot examples
         if self.examples:
             for example in self.examples:
                 system_message += f"\nEXAMPLE: {example['example']}  RESPONSE: {example['response'].replace(',', '||')}"
@@ -55,25 +56,24 @@
     def system_message_batch(self) -> str:
         categories = self.categories
         system_message = f"""
         Each category is formatted as <category>: <description of data that fits the category>
         {str(categories)}
         Classify the given text snippet into one or more of the following categories:
         {str(list(categories.keys()))}
-        Reply with a list of || separated categories for each content snippet. Separate them with ##. Example: Content 1: <content>, Content 2: <content> \n Response: <category>||<category>##<category>. Do not make any other conversation. Do not mention Content in your response.
+        Do not use any other categories.
+        Reply with a list of || separated categories for each content snippet. Separate them with ##. EXAMPLE: Content 1: <content>, Content 2: <content> \n RESPONSE: <category of content1>||<category of content1>##<category of content2> Do not make any other conversation. Do not mention Content in your response.
         """
 
         # Add in fewshot examples
         if self.examples:
-            system_message += "\nExample: "
+            system_message += "\nEXAMPLE: "
             for idx, example in enumerate(self.examples):
                 system_message += f"Content {str(idx+1)}: {example['example']}, "
-            system_message += f"\nResponse: "
-            for example in self.examples:
-                system_message += f"{example['response'].replace(',', '||')}##"
+            system_message += f"\nRESPONSE: {'##'.join([example['response'].replace(',', '||') for example in self.examples])}"
         return system_message
 
     def categorize(self, input_data: str) -> str:
         """
         Categorizes the input data into multiple categories using the specified LLM provider.
 
         Args:
@@ -101,20 +101,20 @@
 
         Returns:
             List[str]: A list of predicted categories for the input data. If there are multiple categories, they will be separated by commas.
 
         Raises:
             ValueError: If the predicted categories are not a subset of the provided categories.
         """
-
+        if len(input_data) == 1:
+            return self.validate_predicted_categories([self.categorize(input_data[0])])
         # Call the LLM provider to get the predicted categories
         response = self.llm_provider.generate_batch(
             self.system_message_batch, input_data
         )
-
         # Split the response into category sets for each input data
         category_sets = response.split("##")
 
         if len(category_sets) != len(input_data):
             raise ValueError(
                 f"Number of predicted category sets ({len(category_sets)}) does not match the number of input data ({len(input_data)})."
             )
```

### Comparing `databonsai-0.5.0/databonsai/llm_providers/anthropic_provider.py` & `databonsai-0.6.0/databonsai/llm_providers/anthropic_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.5.0/databonsai/llm_providers/llm_provider.py` & `databonsai-0.6.0/databonsai/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.5.0/databonsai/llm_providers/ollama_provider.py` & `databonsai-0.6.0/databonsai/llm_providers/ollama_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.5.0/databonsai/llm_providers/openai_provider.py` & `databonsai-0.6.0/databonsai/llm_providers/openai_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.5.0/databonsai/transform/base_transformer.py` & `databonsai-0.6.0/databonsai/transform/base_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,16 @@
         Args:
             input_data (List[str]): A list of text data to be transformed.
             max_tokens (int, optional): The maximum number of tokens to generate in each response. Defaults to 1000.
 
         Returns:
             List[str]: A list of transformed data, where each element corresponds to the transformed version of the respective input data.
         """
+        if len(input_data) == 1:
+            return [self.transform(input_data[0])]
         # Call the LLM provider to perform the batch transformation
         response = self.llm_provider.generate_batch(
             self.system_message_batch, input_data, max_tokens=max_tokens
         )
 
         # Split the response into individual transformed data
         transformed_data_list = response.split("||")
```

### Comparing `databonsai-0.5.0/databonsai/transform/decompose_transformer.py` & `databonsai-0.6.0/databonsai/transform/extract_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Dict, List, Optional
 from pydantic import field_validator, model_validator, computed_field
 from databonsai.transform.base_transformer import BaseTransformer
 
 
-class DecomposeTransformer(BaseTransformer):
+class ExtractTransformer(BaseTransformer):
     """
-    This class extends the BaseTransformer class and overrides the transform method to decompose the input data into a list of dictionaries based on a provided output schema.
+    This class extends the BaseTransformer class and overrides the transform method to extract  a given schema from the input data into a list of dictionaries.
 
     Attributes:
         output_schema (Dict[str, str]): A dictionary representing the schema of the output dictionaries.
-        examples (Optional[List[Dict[str, str]]]): A list of example inputs and their corresponding decomposed outputs.
+        examples (Optional[List[Dict[str, str]]]): A list of example inputs and their corresponding extracted outputs.
 
     Raises:
         ValueError: If the output schema dictionary is empty, or if the transformed data does not match the expected format or schema.
     """
 
     output_schema: Dict[str, str]
     examples: Optional[List[Dict[str, str]]] = []
```

### Comparing `databonsai-0.5.0/databonsai.egg-info/PKG-INFO` & `databonsai-0.6.0/databonsai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 ## Clean &amp; curate your data with LLMs
 
 databonsai is a Python library that uses LLMs to perform data cleaning tasks.
 
 ## Features
 
 -   Suite of tools for data processing using LLMs including categorization,
-    transformation, and decomposition
+    transformation, and extraction
 -   Validation of LLM outputs
 -   Batch processing for token savings
 -   Retry logic with exponential backoff for handling rate limits and transient
     errors
 
 ## Installation
 
@@ -117,48 +117,42 @@
 
 Output:
 
 ```python
 ['Weather', 'Sports', 'Celebrities']
 ```
 
-### Dataframes & Lists
+### AutoBatch for Larger datasets
 
-If you have a pandas dataframe or list, use `apply_to_column_batch` for some
-handy features:
+If you have a pandas dataframe or list, use `apply_to_column_autobatch`
 
--   batching saves tokens by not resending the schema each time.
--   progress bar
--   returns the last successful index so you can resume from there, in case of
-    any error (llm_provider already implements exponential backoff, but just in
-    case)
--   modifies your output list in place, so you don't lose any progress
+-   Batching data for LLM api calls saves tokens by not sending the prompt for
+    every row. However, too large a batch size / complex tasks can lead to
+    errors. Naturally, the better the LLM model, the larger the batch size you
+    can use.
 
-Use the method as such:
+-   This batching is handled adaptively (i.e., it will increase the batch size
+    if the response is valid and reduce it if it's not, with a decay factor)
 
-```python
-success_idx = apply_to_column_batch(input_column, output_column, function, batch_size, start_idx)
-```
-
-Parameters:
+Other features:
 
--   `input_column`: The name of the column from which data will be read.
--   `output_column`: The name of the column to which data will be written.
--   `function`: The function to apply to each batch of data.
--   `batch_size`: The number of rows in each batch.
--   `start_idx`: The starting index from which to begin processing.
+-   Progress bar
+-   Returns the last successful index so you can resume from there, in case it
+    exceeds max_retries
+-   Modifies your output list in place, so you don't lose any progress
 
-Returns:
+Retry Logic:
 
--   `success_idx`: The index of the last successful row processed.
-
-(Continued from the previous code example)
+-   LLM providers have retry logic built in for API related errors. This can be
+    configured in the provider.
+-   The retry logic in the apply_to_column_autobatch is for handling invalid
+    responses (e.g. unexpected category, different number of outputs, etc.)
 
 ```python
-from databonsai.utils import apply_to_column_batch, apply_to_column
+from databonsai.utils import apply_to_column_batch, apply_to_column, apply_to_column_autobatch
 import pandas as pd
 
 headlines = [
     "Massive Blizzard Hits the Northeast, Thousands Without Power",
     "Local High School Basketball Team Wins State Championship After Dramatic Final",
     "Celebrated Actor Launches New Environmental Awareness Campaign",
     "President Announces Comprehensive Plan to Combat Cybersecurity Threats",
@@ -167,33 +161,40 @@
     "Olympic Gold Medalist Announces Retirement, Plans Coaching Career",
     "Film Industry Legends Team Up for Blockbuster Biopic",
     "Government Proposes Sweeping Reforms in Public Health Sector",
     "Startup Develops App That Predicts Traffic Patterns Using AI",
 ]
 df = pd.DataFrame(headlines, columns=["Headline"])
 df["Category"] = None # Initialize it if it doesn't exist, as we modify it in place
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
+success_idx = apply_to_column_autobatch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
 ```
 
-By default, exponential backoff is used to handle rate limiting. This is handled
-in the LLM providers and can be configured.
+There are many more options available for autobatch, such as setting a
+max_retries, decay factor, and more. Check [Utils](./docs/Utils.md) for more
+details
 
 If it fails midway (even after exponential backoff), you can resume from the
 last successful index + 1.
 
 ```python
-success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10, start_idx=success_idx+1)
+success_idx = apply_to_column_autobatch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=10, start_idx=success_idx+1)
 ```
 
 This also works for regular python lists.
 
 Note that the better the LLM model, the greater the batch_size you can use
 (depending on the length of your inputs). If you're getting errors, reduce the
 batch_size, or use a better LLM model.
 
+To use it with batching, but with a fixed batch size:
+
+```python
+success_idx = apply_to_column_batch( df["Headline"], df["Category"], categorizer.categorize_batch, batch_size=3, start_idx=0)
+```
+
 To use it without batching:
 
 ```python
 success_idx = apply_to_column( df["Headline"], df["Category"], categorizer.categorize)
 ```
 
 ### View System Prompt
@@ -218,16 +219,16 @@
 ### Tools (Check out the docs for usage examples and details)
 
 -   [BaseCategorizer](./docs/BaseCategorizer.md) - categorize data into a
     category
 -   [MultiCategorizer](./docs/MultiCategorizer.md) - categorize data into
     multiple categories
 -   [BaseTransformer](./docs/BaseTransformer.md) - transform data with a prompt
--   [DecomposeTransformer](./docs/DecomposeTransformer.md) - decompose data into
-    a structured format based on a schema
+-   [ExtractTransformer](./docs/ExtractTransformer.md) - Extract data into a
+    structured format based on a schema
 -   .. more coming soon!
 
 ### LLM Providers
 
 -   [OpenAIProvider](./docs/OpenAIProvider.md) - OpenAI
 -   [AnthropicProvider](./docs/AnthropicProvider.md) - Anthropic
 -   [OllamaProvider](./docs/OllamaProvider.md) - Ollama
```

### Comparing `databonsai-0.5.0/databonsai.egg-info/SOURCES.txt` & `databonsai-0.6.0/databonsai.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 databonsai/llm_providers/__init__.py
 databonsai/llm_providers/anthropic_provider.py
 databonsai/llm_providers/llm_provider.py
 databonsai/llm_providers/ollama_provider.py
 databonsai/llm_providers/openai_provider.py
 databonsai/transform/__init__.py
 databonsai/transform/base_transformer.py
-databonsai/transform/decompose_transformer.py
+databonsai/transform/extract_transformer.py
 databonsai/utils/__init__.py
 databonsai/utils/apply.py
 tests/__init__.py
 tests/test_categorization.py
```

### Comparing `databonsai-0.5.0/pyproject.toml` & `databonsai-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databonsai"
-version = "0.5.0"
+version = "0.6.0"
 description = "A Python package to clean and curate your data with LLMs"
 authors = ["Alvin Ryanputra <databonsai.ai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"  
 
 openai = "^1.16.2"
```

### Comparing `databonsai-0.5.0/setup.py` & `databonsai-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="databonsai",
-    version="0.5.0",
+    version="0.6.0",
     description="A package for cleaning and curating data with LLMs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Alvin Ryanputra",
     author_email="databonsai.ai@gmail.com",
     url="https://github.com/databonsai/databonsai",
     packages=find_packages(),
```

### Comparing `databonsai-0.5.0/tests/test_categorization.py` & `databonsai-0.6.0/tests/test_categorization.py`

 * *Files identical despite different names*

