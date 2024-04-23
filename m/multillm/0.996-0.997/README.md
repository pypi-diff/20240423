# Comparing `tmp/multillm-0.996.tar.gz` & `tmp/multillm-0.997.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multillm-0.996.tar", last modified: Sun Apr 21 22:05:35 2024, max compression
+gzip compressed data, was "multillm-0.997.tar", last modified: Tue Apr 23 00:50:30 2024, max compression
```

## Comparing `multillm-0.996.tar` & `multillm-0.997.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 22:05:35.464631 multillm-0.996/
--rw-r--r--   0 sandeep    (502) staff       (20)     1090 2024-04-19 07:14:31.000000 multillm-0.996/LICENSE
--rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 22:05:35.463838 multillm-0.996/PKG-INFO
--rw-r--r--   0 sandeep    (502) staff       (20)    23438 2024-04-19 07:14:31.000000 multillm-0.996/README.md
--rw-r--r--   0 sandeep    (502) staff       (20)      154 2024-04-19 07:14:31.000000 multillm-0.996/README.txt
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 22:05:35.447613 multillm-0.996/multillm/
--rw-r--r--   0 sandeep    (502) staff       (20)     2646 2024-04-19 07:14:31.000000 multillm-0.996/multillm/Action.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3335 2024-04-19 07:14:31.000000 multillm-0.996/multillm/BaseLLM.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3459 2024-04-19 07:14:31.000000 multillm-0.996/multillm/DynamicClass.py
--rw-r--r--   0 sandeep    (502) staff       (20)     9433 2024-04-19 07:14:31.000000 multillm-0.996/multillm/MultiLLM.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3105 2024-04-19 07:14:31.000000 multillm-0.996/multillm/Prompt.py
--rw-r--r--   0 sandeep    (502) staff       (20)     2167 2024-04-19 07:14:31.000000 multillm-0.996/multillm/Rank.py
--rw-r--r--   0 sandeep    (502) staff       (20)     1209 2024-04-19 07:14:31.000000 multillm-0.996/multillm/Redis.py
--rw-r--r--   0 sandeep    (502) staff       (20)       26 2024-04-19 07:14:31.000000 multillm-0.996/multillm/__init__.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5551 2024-04-19 07:14:31.000000 multillm-0.996/multillm/example.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3491 2024-04-19 07:14:31.000000 multillm-0.996/multillm/example_rank_callback.py
--rw-r--r--   0 sandeep    (502) staff       (20)    12433 2024-04-19 07:14:31.000000 multillm-0.996/multillm/example_rank_callback3_scaled.py
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 22:05:35.462734 multillm-0.996/multillm/models/
--rw-r--r--   0 sandeep    (502) staff       (20)     4022 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/Codegen.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3780 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/Dolly.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4065 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/GPT.py
--rw-r--r--   0 sandeep    (502) staff       (20)     2519 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/GPTJ.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5326 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/LLAMA2.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5348 2024-04-21 22:04:37.000000 multillm-0.996/multillm/models/LLAMA3.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4298 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/Mistral.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4474 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/Zephyr.py
--rw-r--r--   0 sandeep    (502) staff       (20)     6399 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/bard.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5513 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/claude.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4026 2024-04-19 07:14:31.000000 multillm-0.996/multillm/models/gemini.py
--rw-r--r--   0 sandeep    (502) staff       (20)    12554 2024-04-19 07:14:31.000000 multillm-0.996/multillm/rank_callback.py
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 22:05:35.463297 multillm-0.996/multillm.egg-info/
--rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 22:05:35.000000 multillm-0.996/multillm.egg-info/PKG-INFO
--rw-r--r--   0 sandeep    (502) staff       (20)      768 2024-04-21 22:05:35.000000 multillm-0.996/multillm.egg-info/SOURCES.txt
--rw-r--r--   0 sandeep    (502) staff       (20)        1 2024-04-21 22:05:35.000000 multillm-0.996/multillm.egg-info/dependency_links.txt
--rw-r--r--   0 sandeep    (502) staff       (20)       51 2024-04-21 22:05:35.000000 multillm-0.996/multillm.egg-info/entry_points.txt
--rw-r--r--   0 sandeep    (502) staff       (20)        9 2024-04-21 22:05:35.000000 multillm-0.996/multillm.egg-info/top_level.txt
--rw-r--r--   0 sandeep    (502) staff       (20)      946 2024-04-21 22:04:49.000000 multillm-0.996/pyproject.toml
--rw-r--r--   0 sandeep    (502) staff       (20)       38 2024-04-21 22:05:35.464765 multillm-0.996/setup.cfg
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-23 00:50:30.137636 multillm-0.997/
+-rw-r--r--   0 sandeep    (502) staff       (20)     1090 2024-04-19 07:14:31.000000 multillm-0.997/LICENSE
+-rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-23 00:50:30.136742 multillm-0.997/PKG-INFO
+-rw-r--r--   0 sandeep    (502) staff       (20)    23438 2024-04-19 07:14:31.000000 multillm-0.997/README.md
+-rw-r--r--   0 sandeep    (502) staff       (20)      154 2024-04-19 07:14:31.000000 multillm-0.997/README.txt
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-23 00:50:30.120764 multillm-0.997/multillm/
+-rw-r--r--   0 sandeep    (502) staff       (20)     2646 2024-04-19 07:14:31.000000 multillm-0.997/multillm/Action.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3335 2024-04-19 07:14:31.000000 multillm-0.997/multillm/BaseLLM.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3459 2024-04-19 07:14:31.000000 multillm-0.997/multillm/DynamicClass.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     9433 2024-04-19 07:14:31.000000 multillm-0.997/multillm/MultiLLM.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3105 2024-04-19 07:14:31.000000 multillm-0.997/multillm/Prompt.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     2167 2024-04-19 07:14:31.000000 multillm-0.997/multillm/Rank.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     1209 2024-04-19 07:14:31.000000 multillm-0.997/multillm/Redis.py
+-rw-r--r--   0 sandeep    (502) staff       (20)       26 2024-04-19 07:14:31.000000 multillm-0.997/multillm/__init__.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5551 2024-04-19 07:14:31.000000 multillm-0.997/multillm/example.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3491 2024-04-19 07:14:31.000000 multillm-0.997/multillm/example_rank_callback.py
+-rw-r--r--   0 sandeep    (502) staff       (20)    12433 2024-04-19 07:14:31.000000 multillm-0.997/multillm/example_rank_callback3_scaled.py
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-23 00:50:30.134592 multillm-0.997/multillm/models/
+-rw-r--r--   0 sandeep    (502) staff       (20)     4022 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/Codegen.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3780 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/Dolly.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4065 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/GPT.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     2519 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/GPTJ.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4005 2024-04-23 00:48:56.000000 multillm-0.997/multillm/models/Gemma.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5326 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/LLAMA2.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5348 2024-04-21 22:04:37.000000 multillm-0.997/multillm/models/LLAMA3.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4298 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/Mistral.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4474 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/Zephyr.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     6399 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/bard.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5513 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/claude.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4026 2024-04-19 07:14:31.000000 multillm-0.997/multillm/models/gemini.py
+-rw-r--r--   0 sandeep    (502) staff       (20)    12554 2024-04-19 07:14:31.000000 multillm-0.997/multillm/rank_callback.py
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-23 00:50:30.135833 multillm-0.997/multillm.egg-info/
+-rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-23 00:50:30.000000 multillm-0.997/multillm.egg-info/PKG-INFO
+-rw-r--r--   0 sandeep    (502) staff       (20)      793 2024-04-23 00:50:30.000000 multillm-0.997/multillm.egg-info/SOURCES.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)        1 2024-04-23 00:50:30.000000 multillm-0.997/multillm.egg-info/dependency_links.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)       51 2024-04-23 00:50:30.000000 multillm-0.997/multillm.egg-info/entry_points.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)        9 2024-04-23 00:50:30.000000 multillm-0.997/multillm.egg-info/top_level.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)      946 2024-04-23 00:49:38.000000 multillm-0.997/pyproject.toml
+-rw-r--r--   0 sandeep    (502) staff       (20)       38 2024-04-23 00:50:30.137785 multillm-0.997/setup.cfg
```

### Comparing `multillm-0.996/LICENSE` & `multillm-0.997/LICENSE`

 * *Files identical despite different names*

### Comparing `multillm-0.996/PKG-INFO` & `multillm-0.997/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multillm
-Version: 0.996
+Version: 0.997
 Summary: VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results
 Author-email: VerifAI Inc <hello@verifai.ai>
 Project-URL: Homepage, https://github.com/verifai/multiLLM
 Project-URL: Bug Tracker, https://github.com/verifai/multiLLM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multillm-0.996/README.md` & `multillm-0.997/README.md`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/Action.py` & `multillm-0.997/multillm/Action.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/BaseLLM.py` & `multillm-0.997/multillm/BaseLLM.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/DynamicClass.py` & `multillm-0.997/multillm/DynamicClass.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/MultiLLM.py` & `multillm-0.997/multillm/MultiLLM.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/Prompt.py` & `multillm-0.997/multillm/Prompt.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/Rank.py` & `multillm-0.997/multillm/Rank.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/Redis.py` & `multillm-0.997/multillm/Redis.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/example.py` & `multillm-0.997/multillm/example.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/example_rank_callback.py` & `multillm-0.997/multillm/example_rank_callback.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/example_rank_callback3_scaled.py` & `multillm-0.997/multillm/example_rank_callback3_scaled.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/Codegen.py` & `multillm-0.997/multillm/models/Codegen.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/Dolly.py` & `multillm-0.997/multillm/models/Dolly.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/GPT.py` & `multillm-0.997/multillm/models/GPT.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/GPTJ.py` & `multillm-0.997/multillm/models/GPTJ.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/LLAMA2.py` & `multillm-0.997/multillm/models/LLAMA2.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/LLAMA3.py` & `multillm-0.997/multillm/models/LLAMA3.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/Mistral.py` & `multillm-0.997/multillm/models/Mistral.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/Zephyr.py` & `multillm-0.997/multillm/models/Zephyr.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/bard.py` & `multillm-0.997/multillm/models/bard.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/claude.py` & `multillm-0.997/multillm/models/claude.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/models/gemini.py` & `multillm-0.997/multillm/models/gemini.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm/rank_callback.py` & `multillm-0.997/multillm/rank_callback.py`

 * *Files identical despite different names*

### Comparing `multillm-0.996/multillm.egg-info/PKG-INFO` & `multillm-0.997/multillm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multillm
-Version: 0.996
+Version: 0.997
 Summary: VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results
 Author-email: VerifAI Inc <hello@verifai.ai>
 Project-URL: Homepage, https://github.com/verifai/multiLLM
 Project-URL: Bug Tracker, https://github.com/verifai/multiLLM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multillm-0.996/multillm.egg-info/SOURCES.txt` & `multillm-0.997/multillm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 multillm.egg-info/dependency_links.txt
 multillm.egg-info/entry_points.txt
 multillm.egg-info/top_level.txt
 multillm/models/Codegen.py
 multillm/models/Dolly.py
 multillm/models/GPT.py
 multillm/models/GPTJ.py
+multillm/models/Gemma.py
 multillm/models/LLAMA2.py
 multillm/models/LLAMA3.py
 multillm/models/Mistral.py
 multillm/models/Zephyr.py
 multillm/models/bard.py
 multillm/models/claude.py
 multillm/models/gemini.py
```

### Comparing `multillm-0.996/pyproject.toml` & `multillm-0.997/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multillm"
-version = "0.996"
+version = "0.997"
 authors = [
   { name="VerifAI Inc", email="hello@verifai.ai" },
 ]
 
 description = "VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results"
 readme = "README.md"
 requires-python = ">=3.8"
```

