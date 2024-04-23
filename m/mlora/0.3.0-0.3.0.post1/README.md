# Comparing `tmp/mlora-0.3.0.tar.gz` & `tmp/mlora-0.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlora-0.3.0.tar", last modified: Tue Apr 16 13:15:56 2024, max compression
+gzip compressed data, was "mlora-0.3.0.post1.tar", last modified: Tue Apr 23 06:58:50 2024, max compression
```

## Comparing `mlora-0.3.0.tar` & `mlora-0.3.0.post1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.567340 mlora-0.3.0/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2024-01-06 04:20:01.000000 mlora-0.3.0/LICENSE
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11715 2024-04-16 13:15:56.567151 mlora-0.3.0/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)    10954 2024-04-10 06:30:53.000000 mlora-0.3.0/README.md
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.560441 mlora-0.3.0/mlora/
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1195 2024-04-09 15:43:19.000000 mlora-0.3.0/mlora/__init__.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.562734 mlora-0.3.0/mlora/backends/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      987 2024-04-09 13:04:56.000000 mlora-0.3.0/mlora/backends/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1324 2024-04-09 13:09:12.000000 mlora-0.3.0/mlora/backends/common.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1571 2024-04-09 13:03:52.000000 mlora-0.3.0/mlora/backends/cpu.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1343 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/backends/cuda.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2044 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/backends/mps.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.564374 mlora-0.3.0/mlora/common/
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2171 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5197 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/attention.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5040 2024-04-09 12:44:14.000000 mlora-0.3.0/mlora/common/checkpoint.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2859 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/common/feed_forward.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    14330 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/lora_linear.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11145 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/common/mix_lora.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2266 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/model.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     9628 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/common/modelargs.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    13118 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/dispatcher.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     9770 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/evaluator.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     7872 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/generator.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    18206 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/model.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.565658 mlora-0.3.0/mlora/models/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      872 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/models/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     6308 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_gemma.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    20566 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_llama.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    12070 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_mistral.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    22465 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_phi.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1764 2024-04-03 07:55:06.000000 mlora-0.3.0/mlora/prompter.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.566451 mlora-0.3.0/mlora/tasks/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      528 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/tasks/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     6439 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tasks/common.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     3182 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tasks/glue_tasks.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5850 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tasks/qa_tasks.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1370 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tokenizer.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     7862 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/trainer.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2125 2024-04-09 15:43:44.000000 mlora-0.3.0/mlora/utils.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.566873 mlora-0.3.0/mlora.egg-info/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11715 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)      927 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/SOURCES.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/dependency_links.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      106 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/requires.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/top_level.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      817 2024-04-16 13:15:44.000000 mlora-0.3.0/pyproject.toml
--rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2024-04-16 13:15:56.567373 mlora-0.3.0/setup.cfg
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.566621 mlora-0.3.0/tests/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      166 2024-04-03 07:54:48.000000 mlora-0.3.0/tests/test_demo.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.768962 mlora-0.3.0.post1/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2024-01-06 04:20:01.000000 mlora-0.3.0.post1/LICENSE
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11721 2024-04-23 06:58:50.768699 mlora-0.3.0.post1/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    10954 2024-04-10 06:30:53.000000 mlora-0.3.0.post1/README.md
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.759861 mlora-0.3.0.post1/mlora/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1195 2024-04-23 06:58:34.000000 mlora-0.3.0.post1/mlora/__init__.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.762415 mlora-0.3.0.post1/mlora/backends/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      987 2024-04-09 13:04:56.000000 mlora-0.3.0.post1/mlora/backends/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1324 2024-04-09 13:09:12.000000 mlora-0.3.0.post1/mlora/backends/common.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1571 2024-04-09 13:03:52.000000 mlora-0.3.0.post1/mlora/backends/cpu.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1343 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/backends/cuda.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2044 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/backends/mps.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.764952 mlora-0.3.0.post1/mlora/common/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2171 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5197 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/attention.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5040 2024-04-09 12:44:14.000000 mlora-0.3.0.post1/mlora/common/checkpoint.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2859 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/common/feed_forward.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    14330 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/lora_linear.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11145 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/common/mix_lora.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2266 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/model.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9628 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/common/modelargs.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    13118 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/dispatcher.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9770 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/evaluator.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7872 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/generator.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    18206 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/model.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.766665 mlora-0.3.0.post1/mlora/models/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      872 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/models/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     6308 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_gemma.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    20566 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_llama.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    12070 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_mistral.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    22465 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_phi.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1764 2024-04-03 07:55:06.000000 mlora-0.3.0.post1/mlora/prompter.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.767847 mlora-0.3.0.post1/mlora/tasks/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      528 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/tasks/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     6439 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/tasks/common.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     3182 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/tasks/glue_tasks.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5850 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/tasks/qa_tasks.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1679 2024-04-23 06:58:34.000000 mlora-0.3.0.post1/mlora/tokenizer.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7862 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/trainer.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2125 2024-04-09 15:43:44.000000 mlora-0.3.0.post1/mlora/utils.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.768414 mlora-0.3.0.post1/mlora.egg-info/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11721 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      927 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/SOURCES.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/dependency_links.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      106 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/requires.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/top_level.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      823 2024-04-23 06:58:34.000000 mlora-0.3.0.post1/pyproject.toml
+-rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2024-04-23 06:58:50.769047 mlora-0.3.0.post1/setup.cfg
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.768069 mlora-0.3.0.post1/tests/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      166 2024-04-03 07:54:48.000000 mlora-0.3.0.post1/tests/test_demo.py
```

### Comparing `mlora-0.3.0/LICENSE` & `mlora-0.3.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/PKG-INFO` & `mlora-0.3.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mlora
-Version: 0.3.0
+Version: 0.3.0.post1
 Summary: A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently.
 Project-URL: Homepage, https://github.com/scukdde-llm/mlora
 Project-URL: Bug Tracker, https://github.com/scukdde-llm/mlora/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.1.2
 Requires-Dist: datasets
 Requires-Dist: evaluate
 Requires-Dist: accelerate
-Requires-Dist: transformers==4.38.2
+Requires-Dist: transformers>=4.40.0
 Requires-Dist: sentencepiece
 Requires-Dist: huggingface_hub
 Requires-Dist: scikit-learn
 
 # m-LoRA: Efficient LLM Model Fine-Tune via Multi-LoRA Optimization
 [![](https://github.com/scukdde-llm/mlora/actions/workflows/python-test.yml/badge.svg)](https://github.com/scukdde-llm/mlora/actions/workflows/python-test.yml)
 [![](https://github.com/scukdde-llm/mlora/actions/workflows/mlora-test.yml/badge.svg)](https://github.com/scukdde-llm/mlora/actions/workflows/mlora-test.yml)
```

### Comparing `mlora-0.3.0/README.md` & `mlora-0.3.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/__init__.py` & `mlora-0.3.0.post1/mlora/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     lora_config_factory,
 )
 from .utils import is_package_available
 
 assert is_package_available(
     "torch", "2.1.2"), "m-LoRA requires torch>=2.1.2"
 assert is_package_available(
-    "transformers", "4.38.2"), "m-LoRA requires transformers>=4.38.2"
+    "transformers", "4.40.0"), "m-LoRA requires transformers>=4.40.0"
 
 
 setup_logging()
 
 __all__ = [
     "LLMModelArgs",
     "LLMModelOutput",
```

### Comparing `mlora-0.3.0/mlora/backends/__init__.py` & `mlora-0.3.0.post1/mlora/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/backends/common.py` & `mlora-0.3.0.post1/mlora/backends/common.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/backends/cpu.py` & `mlora-0.3.0.post1/mlora/backends/cpu.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/backends/cuda.py` & `mlora-0.3.0.post1/mlora/backends/cuda.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/backends/mps.py` & `mlora-0.3.0.post1/mlora/backends/mps.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/__init__.py` & `mlora-0.3.0.post1/mlora/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/attention.py` & `mlora-0.3.0.post1/mlora/common/attention.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/checkpoint.py` & `mlora-0.3.0.post1/mlora/common/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/feed_forward.py` & `mlora-0.3.0.post1/mlora/common/feed_forward.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/lora_linear.py` & `mlora-0.3.0.post1/mlora/common/lora_linear.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/mix_lora.py` & `mlora-0.3.0.post1/mlora/common/mix_lora.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/model.py` & `mlora-0.3.0.post1/mlora/common/model.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/common/modelargs.py` & `mlora-0.3.0.post1/mlora/common/modelargs.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/dispatcher.py` & `mlora-0.3.0.post1/mlora/dispatcher.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/evaluator.py` & `mlora-0.3.0.post1/mlora/evaluator.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/generator.py` & `mlora-0.3.0.post1/mlora/generator.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/model.py` & `mlora-0.3.0.post1/mlora/model.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/models/__init__.py` & `mlora-0.3.0.post1/mlora/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/models/modeling_gemma.py` & `mlora-0.3.0.post1/mlora/models/modeling_gemma.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/models/modeling_llama.py` & `mlora-0.3.0.post1/mlora/models/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/models/modeling_mistral.py` & `mlora-0.3.0.post1/mlora/models/modeling_mistral.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/models/modeling_phi.py` & `mlora-0.3.0.post1/mlora/models/modeling_phi.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/prompter.py` & `mlora-0.3.0.post1/mlora/prompter.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/tasks/__init__.py` & `mlora-0.3.0.post1/mlora/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/tasks/common.py` & `mlora-0.3.0.post1/mlora/tasks/common.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/tasks/glue_tasks.py` & `mlora-0.3.0.post1/mlora/tasks/glue_tasks.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/tasks/qa_tasks.py` & `mlora-0.3.0.post1/mlora/tasks/qa_tasks.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/tokenizer.py` & `mlora-0.3.0.post1/mlora/tokenizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from .common import Tokens, Masks
 
 from transformers import AutoTokenizer
 from typing import List, Union
 
+import logging
+
 
 class Tokenizer:
     def __init__(self, model_path: str):
         self.tokenizer = AutoTokenizer.from_pretrained(model_path)
         self.vocab_size_ = self.tokenizer.vocab_size
         self.bos_id_ = self.tokenizer.bos_token_id
         self.eos_id_ = self.tokenizer.eos_token_id
         self.pad_id_ = self.tokenizer.pad_token_id
         self.unk_id_ = self.tokenizer.unk_token_id
         # maybe pad id is unk
         if self.pad_id_ is None and self.unk_id_ is not None:
             self.pad_id_ = self.unk_id_
+        if self.pad_id_ is None and self.eos_id_ is not None:
+            self.pad_id_ = self.eos_id_
+            logging.warn("Padding token ID is None, setting to <eos>.")
+        else:
+            raise ValueError(
+                "Can not set padding token id. <eos> and <unk> are None.")
 
     def encode(self, data: Union[str, List[str]], add_special_tokens: bool = True) -> Tokens:
         if isinstance(data, str):
             data = [data]
         tokens = []
         ret = self.tokenizer(
             data, add_special_tokens=add_special_tokens, return_attention_mask=False).input_ids
```

### Comparing `mlora-0.3.0/mlora/trainer.py` & `mlora-0.3.0.post1/mlora/trainer.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora/utils.py` & `mlora-0.3.0.post1/mlora/utils.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/mlora.egg-info/PKG-INFO` & `mlora-0.3.0.post1/mlora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mlora
-Version: 0.3.0
+Version: 0.3.0.post1
 Summary: A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently.
 Project-URL: Homepage, https://github.com/scukdde-llm/mlora
 Project-URL: Bug Tracker, https://github.com/scukdde-llm/mlora/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.1.2
 Requires-Dist: datasets
 Requires-Dist: evaluate
 Requires-Dist: accelerate
-Requires-Dist: transformers==4.38.2
+Requires-Dist: transformers>=4.40.0
 Requires-Dist: sentencepiece
 Requires-Dist: huggingface_hub
 Requires-Dist: scikit-learn
 
 # m-LoRA: Efficient LLM Model Fine-Tune via Multi-LoRA Optimization
 [![](https://github.com/scukdde-llm/mlora/actions/workflows/python-test.yml/badge.svg)](https://github.com/scukdde-llm/mlora/actions/workflows/python-test.yml)
 [![](https://github.com/scukdde-llm/mlora/actions/workflows/mlora-test.yml/badge.svg)](https://github.com/scukdde-llm/mlora/actions/workflows/mlora-test.yml)
```

### Comparing `mlora-0.3.0/mlora.egg-info/SOURCES.txt` & `mlora-0.3.0.post1/mlora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0/pyproject.toml` & `mlora-0.3.0.post1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlora"
-version = "0.3.0"
+version = "0.3.0.post1"
 description = "A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "torch>=2.1.2",
     "datasets",
     "evaluate",
     "accelerate",
-    "transformers==4.38.2",
+    "transformers>=4.40.0",
     "sentencepiece",
     "huggingface_hub",
     "scikit-learn",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/scukdde-llm/mlora"
```

