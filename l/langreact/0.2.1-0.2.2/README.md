# Comparing `tmp/langreact-0.2.1.tar.gz` & `tmp/langreact-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langreact-0.2.1.tar", max compression
+gzip compressed data, was "langreact-0.2.2.tar", max compression
```

## Comparing `langreact-0.2.1.tar` & `langreact-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1074 2024-04-22 13:18:00.035637 langreact-0.2.1/LICENSE
--rw-r--r--   0        0        0      721 2024-04-22 08:07:05.274786 langreact-0.2.1/README.md
--rw-r--r--   0        0        0       85 2024-04-18 13:49:04.824380 langreact-0.2.1/core/__init__.py
--rw-r--r--   0        0        0     4165 2024-04-22 14:10:08.540602 langreact-0.2.1/core/application.py
--rw-r--r--   0        0        0        0 2024-03-27 09:42:55.763066 langreact-0.2.1/core/builder/__init__.py
--rw-r--r--   0        0        0      954 2024-04-22 09:16:40.251004 langreact-0.2.1/core/builder/output_builder.py
--rw-r--r--   0        0        0        0 2024-04-12 12:05:21.553794 langreact-0.2.1/core/common/__init__.py
--rw-r--r--   0        0        0     1551 2024-04-22 09:50:10.247516 langreact-0.2.1/core/common/agent.py
--rw-r--r--   0        0        0      967 2024-04-15 17:34:22.427697 langreact-0.2.1/core/common/chunk.py
--rw-r--r--   0        0        0      939 2024-04-18 12:45:12.483205 langreact-0.2.1/core/common/event.py
--rw-r--r--   0        0        0     1763 2024-04-22 08:48:43.075596 langreact-0.2.1/core/common/event_manager.py
--rw-r--r--   0        0        0      687 2024-04-12 12:05:24.755315 langreact-0.2.1/core/common/feedback_chunk.py
--rw-r--r--   0        0        0      629 2024-04-22 13:16:53.116706 langreact-0.2.1/core/configure/configure.py
--rw-r--r--   0        0        0     6866 2024-04-22 10:30:57.473255 langreact-0.2.1/core/configure/default.py
--rw-r--r--   0        0        0      215 2024-04-15 16:43:49.865253 langreact-0.2.1/core/constants.py
--rw-r--r--   0        0        0     2266 2024-04-22 13:16:56.101916 langreact-0.2.1/core/context.py
--rw-r--r--   0        0        0    13690 2024-04-22 13:20:11.768152 langreact-0.2.1/core/flow.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:31.478339 langreact-0.2.1/core/memory/__init__.py
--rw-r--r--   0        0        0     3099 2024-04-22 09:24:01.442856 langreact-0.2.1/core/memory/memory.py
--rw-r--r--   0        0        0     4506 2024-04-22 13:18:35.717870 langreact-0.2.1/core/memory/memory_chunk.py
--rw-r--r--   0        0        0     5774 2024-04-22 09:23:35.369623 langreact-0.2.1/core/memory/memory_index.py
--rw-r--r--   0        0        0        0 2024-03-27 09:43:28.725120 langreact-0.2.1/core/modifier/__init__.py
--rw-r--r--   0        0        0     1536 2024-04-12 12:42:11.472771 langreact-0.2.1/core/modifier/chunk_modifier.py
--rw-r--r--   0        0        0     1717 2024-04-15 17:23:17.172743 langreact-0.2.1/core/modifier/context_modifier.py
--rw-r--r--   0        0        0        0 2024-03-27 09:43:25.687711 langreact-0.2.1/core/observer/__init__.py
--rw-r--r--   0        0        0     1601 2024-04-12 09:50:30.838214 langreact-0.2.1/core/observer/feedback.py
--rw-r--r--   0        0        0      977 2024-04-12 09:47:17.439471 langreact-0.2.1/core/observer/observer.py
--rw-r--r--   0        0        0      282 2024-04-15 16:43:48.968972 langreact-0.2.1/core/observer/observer_manager.py
--rw-r--r--   0        0        0     1645 2024-04-22 14:46:30.359935 langreact-0.2.1/core/params.py
--rw-r--r--   0        0        0        0 2024-03-27 09:42:59.759214 langreact-0.2.1/core/planning/__init__.py
--rw-r--r--   0        0        0     1457 2024-04-15 07:19:05.473968 langreact-0.2.1/core/planning/agent.py
--rw-r--r--   0        0        0        0 2024-03-27 09:43:23.054223 langreact-0.2.1/core/plugin/__init__.py
--rw-r--r--   0        0        0      335 2024-04-18 12:47:46.269881 langreact-0.2.1/core/plugin/base.py
--rw-r--r--   0        0        0     2135 2024-04-22 13:17:08.626086 langreact-0.2.1/core/plugin/plugins.py
--rw-r--r--   0        0        0      594 2024-04-22 09:05:03.399671 langreact-0.2.1/core/plugin/qwen_plugin.py
--rw-r--r--   0        0        0     8630 2024-04-22 13:57:46.616634 langreact-0.2.1/core/steps.py
--rw-r--r--   0        0        0     1909 2024-04-12 12:11:03.816597 langreact-0.2.1/core/tools.py
--rw-r--r--   0        0        0      458 2024-04-22 15:00:48.938089 langreact-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 langreact-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-22 13:18:00.035637 langreact-0.2.2/LICENSE
+-rw-r--r--   0        0        0      721 2024-04-22 08:07:05.274786 langreact-0.2.2/README.md
+-rw-r--r--   0        0        0       85 2024-04-18 13:49:04.824380 langreact-0.2.2/core/__init__.py
+-rw-r--r--   0        0        0     4165 2024-04-22 14:10:08.540602 langreact-0.2.2/core/application.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:42:55.763066 langreact-0.2.2/core/builder/__init__.py
+-rw-r--r--   0        0        0      954 2024-04-22 09:16:40.251004 langreact-0.2.2/core/builder/output_builder.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:05:21.553794 langreact-0.2.2/core/common/__init__.py
+-rw-r--r--   0        0        0     1551 2024-04-22 09:50:10.247516 langreact-0.2.2/core/common/agent.py
+-rw-r--r--   0        0        0      967 2024-04-15 17:34:22.427697 langreact-0.2.2/core/common/chunk.py
+-rw-r--r--   0        0        0      939 2024-04-18 12:45:12.483205 langreact-0.2.2/core/common/event.py
+-rw-r--r--   0        0        0     1763 2024-04-22 08:48:43.075596 langreact-0.2.2/core/common/event_manager.py
+-rw-r--r--   0        0        0      687 2024-04-12 12:05:24.755315 langreact-0.2.2/core/common/feedback_chunk.py
+-rw-r--r--   0        0        0      629 2024-04-22 13:16:53.116706 langreact-0.2.2/core/configure/configure.py
+-rw-r--r--   0        0        0     6866 2024-04-22 10:30:57.473255 langreact-0.2.2/core/configure/default.py
+-rw-r--r--   0        0        0      215 2024-04-15 16:43:49.865253 langreact-0.2.2/core/constants.py
+-rw-r--r--   0        0        0     2266 2024-04-22 13:16:56.101916 langreact-0.2.2/core/context.py
+-rw-r--r--   0        0        0    13690 2024-04-22 13:20:11.768152 langreact-0.2.2/core/flow.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:31.478339 langreact-0.2.2/core/memory/__init__.py
+-rw-r--r--   0        0        0     3099 2024-04-22 09:24:01.442856 langreact-0.2.2/core/memory/memory.py
+-rw-r--r--   0        0        0     4506 2024-04-22 13:18:35.717870 langreact-0.2.2/core/memory/memory_chunk.py
+-rw-r--r--   0        0        0     5774 2024-04-22 09:23:35.369623 langreact-0.2.2/core/memory/memory_index.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:43:28.725120 langreact-0.2.2/core/modifier/__init__.py
+-rw-r--r--   0        0        0     1536 2024-04-12 12:42:11.472771 langreact-0.2.2/core/modifier/chunk_modifier.py
+-rw-r--r--   0        0        0     1717 2024-04-15 17:23:17.172743 langreact-0.2.2/core/modifier/context_modifier.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:43:25.687711 langreact-0.2.2/core/observer/__init__.py
+-rw-r--r--   0        0        0     1601 2024-04-12 09:50:30.838214 langreact-0.2.2/core/observer/feedback.py
+-rw-r--r--   0        0        0      977 2024-04-12 09:47:17.439471 langreact-0.2.2/core/observer/observer.py
+-rw-r--r--   0        0        0      282 2024-04-15 16:43:48.968972 langreact-0.2.2/core/observer/observer_manager.py
+-rw-r--r--   0        0        0     1645 2024-04-22 14:46:30.359935 langreact-0.2.2/core/params.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:42:59.759214 langreact-0.2.2/core/planning/__init__.py
+-rw-r--r--   0        0        0     1457 2024-04-15 07:19:05.473968 langreact-0.2.2/core/planning/agent.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:43:23.054223 langreact-0.2.2/core/plugin/__init__.py
+-rw-r--r--   0        0        0      335 2024-04-18 12:47:46.269881 langreact-0.2.2/core/plugin/base.py
+-rw-r--r--   0        0        0     2135 2024-04-22 13:17:08.626086 langreact-0.2.2/core/plugin/plugins.py
+-rw-r--r--   0        0        0      594 2024-04-22 09:05:03.399671 langreact-0.2.2/core/plugin/qwen_plugin.py
+-rw-r--r--   0        0        0     8630 2024-04-22 13:57:46.616634 langreact-0.2.2/core/steps.py
+-rw-r--r--   0        0        0     1909 2024-04-12 12:11:03.816597 langreact-0.2.2/core/tools.py
+-rw-r--r--   0        0        0      458 2024-04-22 15:01:37.702842 langreact-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 langreact-0.2.2/PKG-INFO
```

### Comparing `langreact-0.2.1/LICENSE` & `langreact-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/README.md` & `langreact-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/application.py` & `langreact-0.2.2/core/application.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/builder/output_builder.py` & `langreact-0.2.2/core/builder/output_builder.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/common/agent.py` & `langreact-0.2.2/core/common/agent.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/common/chunk.py` & `langreact-0.2.2/core/common/chunk.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/common/event.py` & `langreact-0.2.2/core/common/event.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/common/event_manager.py` & `langreact-0.2.2/core/common/event_manager.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/common/feedback_chunk.py` & `langreact-0.2.2/core/common/feedback_chunk.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/configure/configure.py` & `langreact-0.2.2/core/configure/configure.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/configure/default.py` & `langreact-0.2.2/core/configure/default.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/context.py` & `langreact-0.2.2/core/context.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/flow.py` & `langreact-0.2.2/core/flow.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/memory/memory.py` & `langreact-0.2.2/core/memory/memory.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/memory/memory_chunk.py` & `langreact-0.2.2/core/memory/memory_chunk.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/memory/memory_index.py` & `langreact-0.2.2/core/memory/memory_index.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/modifier/chunk_modifier.py` & `langreact-0.2.2/core/modifier/chunk_modifier.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/modifier/context_modifier.py` & `langreact-0.2.2/core/modifier/context_modifier.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/observer/feedback.py` & `langreact-0.2.2/core/observer/feedback.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/observer/observer.py` & `langreact-0.2.2/core/observer/observer.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/params.py` & `langreact-0.2.2/core/params.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/planning/agent.py` & `langreact-0.2.2/core/planning/agent.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/plugin/plugins.py` & `langreact-0.2.2/core/plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/plugin/qwen_plugin.py` & `langreact-0.2.2/core/plugin/qwen_plugin.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/steps.py` & `langreact-0.2.2/core/steps.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/core/tools.py` & `langreact-0.2.2/core/tools.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.1/PKG-INFO` & `langreact-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langreact
-Version: 0.2.1
+Version: 0.2.2
 Summary: LangReact Project
 License: MIT
 Author: zhangli
 Author-email: max_and_min@163.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain (>=0.1.16,<0.2.0)
-Requires-Dist: milvus (==2.3.7)
+Requires-Dist: milvus (==2.3.5)
 Requires-Dist: openai (>=1.23.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # 🦜️🔗 LangReact
 
 ⚡ 用 Planning Agent 来优化的大模型应用 ⚡
 ⚡ Build your LLM Application based on planning agent ⚡
```

