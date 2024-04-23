# Comparing `tmp/opentelemetry_semantic_conventions_ai-0.1.1.tar.gz` & `tmp/opentelemetry_semantic_conventions_ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_semantic_conventions_ai-0.1.1.tar", max compression
+gzip compressed data, was "opentelemetry_semantic_conventions_ai-0.2.0.tar", max compression
```

## Comparing `opentelemetry_semantic_conventions_ai-0.1.1.tar` & `opentelemetry_semantic_conventions_ai-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      520 2024-01-25 18:03:35.113475 opentelemetry_semantic_conventions_ai-0.1.1/README.md
--rw-r--r--   0        0        0     2657 2024-03-25 22:35:09.568410 opentelemetry_semantic_conventions_ai-0.1.1/opentelemetry/semconv/ai/__init__.py
--rw-r--r--   0        0        0       23 2024-02-13 16:40:50.733559 opentelemetry_semantic_conventions_ai-0.1.1/opentelemetry/semconv/ai/version.py
--rw-r--r--   0        0        0      805 2024-03-25 22:35:24.312265 opentelemetry_semantic_conventions_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 opentelemetry_semantic_conventions_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      520 2024-04-19 07:47:16.767711 opentelemetry_semantic_conventions_ai-0.2.0/README.md
+-rw-r--r--   0        0        0     3235 2024-04-23 17:20:06.458280 opentelemetry_semantic_conventions_ai-0.2.0/opentelemetry/semconv/ai/__init__.py
+-rw-r--r--   0        0        0      728 2024-04-19 08:25:54.050324 opentelemetry_semantic_conventions_ai-0.2.0/opentelemetry/semconv/ai/utils.py
+-rw-r--r--   0        0        0       22 2024-04-23 17:20:54.469079 opentelemetry_semantic_conventions_ai-0.2.0/opentelemetry/semconv/ai/version.py
+-rw-r--r--   0        0        0      805 2024-04-23 17:20:25.475854 opentelemetry_semantic_conventions_ai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 opentelemetry_semantic_conventions_ai-0.2.0/PKG-INFO
```

### Comparing `opentelemetry_semantic_conventions_ai-0.1.1/README.md` & `opentelemetry_semantic_conventions_ai-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_semantic_conventions_ai-0.1.1/pyproject.toml` & `opentelemetry_semantic_conventions_ai-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING:']
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-semantic-conventions-ai"
-version = "0.1.1"
+version = "0.2.0"
 description = "OpenTelemetry Semantic Conventions Extension for Large Language Models"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 license = "Apache-2.0"
```

### Comparing `opentelemetry_semantic_conventions_ai-0.1.1/PKG-INFO` & `opentelemetry_semantic_conventions_ai-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-semantic-conventions-ai
-Version: 0.1.1
+Version: 0.2.0
 Summary: OpenTelemetry Semantic Conventions Extension for Large Language Models
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-semantic-conventions-ai Version:
-0.1.1 Summary: OpenTelemetry Semantic Conventions Extension for Large Language
+0.2.0 Summary: OpenTelemetry Semantic Conventions Extension for Large Language
 Models License: Apache-2.0 Author: Gal Kleinman Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Description-Content-Type: text/markdown
 # OpenTelemetry Semantic Conventions extensions for gen-AI applications _[_h_t_t_p_s_:
```

