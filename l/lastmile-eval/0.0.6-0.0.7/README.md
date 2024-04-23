# Comparing `tmp/lastmile-eval-0.0.6.tar.gz` & `tmp/lastmile_eval-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastmile-eval-0.0.6.tar", last modified: Tue Apr  2 00:42:07 2024, max compression
+gzip compressed data, was "lastmile_eval-0.0.7.tar", last modified: Tue Apr 23 14:14:03 2024, max compression
```

## Comparing `lastmile-eval-0.0.6.tar` & `lastmile_eval-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.889550 lastmile-eval-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:42:07.889550 lastmile-eval-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.881550 lastmile-eval-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.881550 lastmile-eval-0.0.6/src/lastmile_eval/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/examples/rag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/examples/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/rag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval/text/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/metrics_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/openai_batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/tests/test_custom_llm_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/tests/test_default_text_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/tests/test_rag_scores_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.263065 lastmile_eval-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-23 14:14:03.263065 lastmile_eval-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:14:03.263065 lastmile_eval-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.251066 lastmile_eval-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      951 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/run_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/rag_debugger/tracing/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/examples/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.255066 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/api/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/query_trace_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/evaluation_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/prompt_iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/prompt_iteration/run_user_llm_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/scripts/test_run_eval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/trace_extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/rag/debugger/tracing/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/metrics_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/openai_batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/src/lastmile_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 14:14:03.000000 lastmile_eval-0.0.7/src/lastmile_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:14:03.259065 lastmile_eval-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/tests/test_custom_llm_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/tests/test_default_text_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 14:13:58.000000 lastmile_eval-0.0.7/tests/test_rag_scores_e2e.py
```

### Comparing `lastmile-eval-0.0.6/LICENSE` & `lastmile_eval-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/PKG-INFO` & `lastmile_eval-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile-eval
-Version: 0.0.6
+Version: 0.0.7
 Summary: An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/eval
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/eval/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -17,14 +17,24 @@
 Requires-Dist: nltk
 Requires-Dist: openai>=1.0.0
 Requires-Dist: anthropic
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: arize-phoenix-evals==0.5.0
 Requires-Dist: pandas==2.1.2
 Requires-Dist: instructor
+Requires-Dist: opentelemetry-api
+Requires-Dist: opentelemetry-sdk
+Requires-Dist: opentelemetry-exporter-otlp
+Requires-Dist: opentelemetry-semantic-conventions
+Requires-Dist: openinference-semantic-conventions
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn
+Requires-Dist: result
+Requires-Dist: lastmile_utils
+Requires-Dist: email_validator==2.1.1
 
 # LastMile AI Eval
 
 Library of tools to evaluate your RAG system.
 
 ## Setup
```

### Comparing `lastmile-eval-0.0.6/README.md` & `lastmile_eval-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/pyproject.toml` & `lastmile_eval-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lastmile-eval"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="LastMile AI" },
 ]
 description = "An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/examples/rag.py` & `lastmile_eval-0.0.7/src/lastmile_eval/examples/rag.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/examples/text.py` & `lastmile_eval-0.0.7/src/lastmile_eval/examples/text.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/text/__init__.py` & `lastmile_eval-0.0.7/src/lastmile_eval/text/__init__.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/text/batch_lib.py` & `lastmile_eval-0.0.7/src/lastmile_eval/text/batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/text/metrics.py` & `lastmile_eval-0.0.7/src/lastmile_eval/text/metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/text/metrics_lib.py` & `lastmile_eval-0.0.7/src/lastmile_eval/text/metrics_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/text/openai_batch_lib.py` & `lastmile_eval-0.0.7/src/lastmile_eval/text/openai_batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval/utils.py` & `lastmile_eval-0.0.7/src/lastmile_eval/utils.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/src/lastmile_eval.egg-info/PKG-INFO` & `lastmile_eval-0.0.7/src/lastmile_eval.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile-eval
-Version: 0.0.6
+Version: 0.0.7
 Summary: An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/eval
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/eval/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -17,14 +17,24 @@
 Requires-Dist: nltk
 Requires-Dist: openai>=1.0.0
 Requires-Dist: anthropic
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: arize-phoenix-evals==0.5.0
 Requires-Dist: pandas==2.1.2
 Requires-Dist: instructor
+Requires-Dist: opentelemetry-api
+Requires-Dist: opentelemetry-sdk
+Requires-Dist: opentelemetry-exporter-otlp
+Requires-Dist: opentelemetry-semantic-conventions
+Requires-Dist: openinference-semantic-conventions
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn
+Requires-Dist: result
+Requires-Dist: lastmile_utils
+Requires-Dist: email_validator==2.1.1
 
 # LastMile AI Eval
 
 Library of tools to evaluate your RAG system.
 
 ## Setup
```

### Comparing `lastmile-eval-0.0.6/tests/test_custom_llm_metrics.py` & `lastmile_eval-0.0.7/tests/test_custom_llm_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/tests/test_default_text_metrics.py` & `lastmile_eval-0.0.7/tests/test_default_text_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.6/tests/test_rag_scores_e2e.py` & `lastmile_eval-0.0.7/tests/test_rag_scores_e2e.py`

 * *Files identical despite different names*

