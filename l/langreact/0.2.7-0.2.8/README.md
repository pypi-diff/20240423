# Comparing `tmp/langreact-0.2.7.tar.gz` & `tmp/langreact-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langreact-0.2.7.tar", max compression
+gzip compressed data, was "langreact-0.2.8.tar", max compression
```

## Comparing `langreact-0.2.7.tar` & `langreact-0.2.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1074 2024-04-23 02:59:22.421581 langreact-0.2.7/LICENSE
--rw-r--r--   0        0        0     1191 2024-04-23 03:11:02.970011 langreact-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-04-23 14:59:32.019852 langreact-0.2.7/langreact/core/__init__.py
--rw-r--r--   0        0        0     4263 2024-04-23 14:52:03.115645 langreact-0.2.7/langreact/core/application.py
--rw-r--r--   0        0        0        0 2024-03-27 09:42:55.763066 langreact-0.2.7/langreact/core/builder/__init__.py
--rw-r--r--   0        0        0      964 2024-04-23 14:30:12.339998 langreact-0.2.7/langreact/core/builder/output_builder.py
--rw-r--r--   0        0        0        0 2024-04-12 12:05:21.553794 langreact-0.2.7/langreact/core/common/__init__.py
--rw-r--r--   0        0        0     1581 2024-04-23 14:30:12.299870 langreact-0.2.7/langreact/core/common/agent.py
--rw-r--r--   0        0        0      967 2024-04-15 17:34:22.427697 langreact-0.2.7/langreact/core/common/chunk.py
--rw-r--r--   0        0        0      949 2024-04-23 14:30:12.339979 langreact-0.2.7/langreact/core/common/event.py
--rw-r--r--   0        0        0     1803 2024-04-23 14:30:12.339956 langreact-0.2.7/langreact/core/common/event_manager.py
--rw-r--r--   0        0        0      707 2024-04-23 14:30:12.339894 langreact-0.2.7/langreact/core/common/feedback_chunk.py
--rw-r--r--   0        0        0        0 2024-04-23 14:18:29.223389 langreact-0.2.7/langreact/core/configure/__init__.py
--rw-r--r--   0        0        0      662 2024-04-23 15:02:31.190056 langreact-0.2.7/langreact/core/configure/configure.py
--rw-r--r--   0        0        0     6866 2024-04-22 10:30:57.473255 langreact-0.2.7/langreact/core/configure/default.py
--rw-r--r--   0        0        0      513 2024-04-18 13:43:00.127030 langreact-0.2.7/langreact/core/configure/logging.conf
--rw-r--r--   0        0        0      235 2024-04-23 14:30:17.251953 langreact-0.2.7/langreact/core/constants.py
--rw-r--r--   0        0        0     2346 2024-04-23 14:30:12.257861 langreact-0.2.7/langreact/core/context.py
--rw-r--r--   0        0        0    13835 2024-04-23 14:44:40.928868 langreact-0.2.7/langreact/core/flow.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:31.478339 langreact-0.2.7/langreact/core/memory/__init__.py
--rw-r--r--   0        0        0     3159 2024-04-23 14:30:12.299816 langreact-0.2.7/langreact/core/memory/memory.py
--rw-r--r--   0        0        0     4586 2024-04-23 14:30:12.299837 langreact-0.2.7/langreact/core/memory/memory_chunk.py
--rw-r--r--   0        0        0     5784 2024-04-23 14:30:12.299851 langreact-0.2.7/langreact/core/memory/memory_index.py
--rw-r--r--   0        0        0        0 2024-03-27 09:43:28.725120 langreact-0.2.7/langreact/core/modifier/__init__.py
--rw-r--r--   0        0        0     1546 2024-04-23 14:30:12.299802 langreact-0.2.7/langreact/core/modifier/chunk_modifier.py
--rw-r--r--   0        0        0     1717 2024-04-15 17:23:17.172743 langreact-0.2.7/langreact/core/modifier/context_modifier.py
--rw-r--r--   0        0        0        0 2024-03-27 09:43:25.687711 langreact-0.2.7/langreact/core/observer/__init__.py
--rw-r--r--   0        0        0     1641 2024-04-23 14:30:12.299782 langreact-0.2.7/langreact/core/observer/feedback.py
--rw-r--r--   0        0        0     1017 2024-04-23 14:30:12.299770 langreact-0.2.7/langreact/core/observer/observer.py
--rw-r--r--   0        0        0      292 2024-04-23 14:30:12.299793 langreact-0.2.7/langreact/core/observer/observer_manager.py
--rw-r--r--   0        0        0     1645 2024-04-22 14:46:30.359935 langreact-0.2.7/langreact/core/params.py
--rw-r--r--   0        0        0        0 2024-03-27 09:42:59.759214 langreact-0.2.7/langreact/core/planning/__init__.py
--rw-r--r--   0        0        0     1487 2024-04-23 14:30:12.340034 langreact-0.2.7/langreact/core/planning/agent.py
--rw-r--r--   0        0        0        0 2024-03-27 09:43:23.054223 langreact-0.2.7/langreact/core/plugin/__init__.py
--rw-r--r--   0        0        0      335 2024-04-18 12:47:46.269881 langreact-0.2.7/langreact/core/plugin/base.py
--rw-r--r--   0        0        0     2235 2024-04-23 14:30:12.299758 langreact-0.2.7/langreact/core/plugin/plugins.py
--rw-r--r--   0        0        0      404 2024-04-23 14:30:12.282116 langreact-0.2.7/langreact/core/plugin/qwen_plugin.py
--rw-r--r--   0        0        0     8700 2024-04-23 14:30:12.276758 langreact-0.2.7/langreact/core/steps.py
--rw-r--r--   0        0        0     1909 2024-04-12 12:11:03.816597 langreact-0.2.7/langreact/core/tools.py
--rw-r--r--   0        0        0      564 2024-04-23 15:02:55.237278 langreact-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 langreact-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-23 02:59:22.421581 langreact-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1191 2024-04-23 03:11:02.970011 langreact-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 14:59:32.019852 langreact-0.2.8/langreact/core/__init__.py
+-rw-r--r--   0        0        0     4263 2024-04-23 14:52:03.115645 langreact-0.2.8/langreact/core/application.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:42:55.763066 langreact-0.2.8/langreact/core/builder/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-23 14:30:12.339998 langreact-0.2.8/langreact/core/builder/output_builder.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:05:21.553794 langreact-0.2.8/langreact/core/common/__init__.py
+-rw-r--r--   0        0        0     1581 2024-04-23 14:30:12.299870 langreact-0.2.8/langreact/core/common/agent.py
+-rw-r--r--   0        0        0      967 2024-04-15 17:34:22.427697 langreact-0.2.8/langreact/core/common/chunk.py
+-rw-r--r--   0        0        0      949 2024-04-23 14:30:12.339979 langreact-0.2.8/langreact/core/common/event.py
+-rw-r--r--   0        0        0     1803 2024-04-23 14:30:12.339956 langreact-0.2.8/langreact/core/common/event_manager.py
+-rw-r--r--   0        0        0      707 2024-04-23 14:30:12.339894 langreact-0.2.8/langreact/core/common/feedback_chunk.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:18:29.223389 langreact-0.2.8/langreact/core/configure/__init__.py
+-rw-r--r--   0        0        0      741 2024-04-23 15:07:38.027990 langreact-0.2.8/langreact/core/configure/configure.py
+-rw-r--r--   0        0        0     6866 2024-04-22 10:30:57.473255 langreact-0.2.8/langreact/core/configure/default.py
+-rw-r--r--   0        0        0      513 2024-04-18 13:43:00.127030 langreact-0.2.8/langreact/core/configure/logging.conf
+-rw-r--r--   0        0        0      235 2024-04-23 14:30:17.251953 langreact-0.2.8/langreact/core/constants.py
+-rw-r--r--   0        0        0     2346 2024-04-23 14:30:12.257861 langreact-0.2.8/langreact/core/context.py
+-rw-r--r--   0        0        0    13835 2024-04-23 14:44:40.928868 langreact-0.2.8/langreact/core/flow.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:31.478339 langreact-0.2.8/langreact/core/memory/__init__.py
+-rw-r--r--   0        0        0     3159 2024-04-23 14:30:12.299816 langreact-0.2.8/langreact/core/memory/memory.py
+-rw-r--r--   0        0        0     4586 2024-04-23 14:30:12.299837 langreact-0.2.8/langreact/core/memory/memory_chunk.py
+-rw-r--r--   0        0        0     5784 2024-04-23 14:30:12.299851 langreact-0.2.8/langreact/core/memory/memory_index.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:43:28.725120 langreact-0.2.8/langreact/core/modifier/__init__.py
+-rw-r--r--   0        0        0     1546 2024-04-23 14:30:12.299802 langreact-0.2.8/langreact/core/modifier/chunk_modifier.py
+-rw-r--r--   0        0        0     1717 2024-04-15 17:23:17.172743 langreact-0.2.8/langreact/core/modifier/context_modifier.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:43:25.687711 langreact-0.2.8/langreact/core/observer/__init__.py
+-rw-r--r--   0        0        0     1641 2024-04-23 14:30:12.299782 langreact-0.2.8/langreact/core/observer/feedback.py
+-rw-r--r--   0        0        0     1017 2024-04-23 14:30:12.299770 langreact-0.2.8/langreact/core/observer/observer.py
+-rw-r--r--   0        0        0      292 2024-04-23 14:30:12.299793 langreact-0.2.8/langreact/core/observer/observer_manager.py
+-rw-r--r--   0        0        0     1645 2024-04-22 14:46:30.359935 langreact-0.2.8/langreact/core/params.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:42:59.759214 langreact-0.2.8/langreact/core/planning/__init__.py
+-rw-r--r--   0        0        0     1487 2024-04-23 14:30:12.340034 langreact-0.2.8/langreact/core/planning/agent.py
+-rw-r--r--   0        0        0        0 2024-03-27 09:43:23.054223 langreact-0.2.8/langreact/core/plugin/__init__.py
+-rw-r--r--   0        0        0      335 2024-04-18 12:47:46.269881 langreact-0.2.8/langreact/core/plugin/base.py
+-rw-r--r--   0        0        0     2235 2024-04-23 14:30:12.299758 langreact-0.2.8/langreact/core/plugin/plugins.py
+-rw-r--r--   0        0        0      404 2024-04-23 14:30:12.282116 langreact-0.2.8/langreact/core/plugin/qwen_plugin.py
+-rw-r--r--   0        0        0     8700 2024-04-23 14:30:12.276758 langreact-0.2.8/langreact/core/steps.py
+-rw-r--r--   0        0        0     1909 2024-04-12 12:11:03.816597 langreact-0.2.8/langreact/core/tools.py
+-rw-r--r--   0        0        0      564 2024-04-23 15:08:27.841645 langreact-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 langreact-0.2.8/PKG-INFO
```

### Comparing `langreact-0.2.7/LICENSE` & `langreact-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/README.md` & `langreact-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/application.py` & `langreact-0.2.8/langreact/core/application.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/builder/output_builder.py` & `langreact-0.2.8/langreact/core/builder/output_builder.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/common/agent.py` & `langreact-0.2.8/langreact/core/common/agent.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/common/chunk.py` & `langreact-0.2.8/langreact/core/common/chunk.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/common/event.py` & `langreact-0.2.8/langreact/core/common/event.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/common/event_manager.py` & `langreact-0.2.8/langreact/core/common/event_manager.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/common/feedback_chunk.py` & `langreact-0.2.8/langreact/core/common/feedback_chunk.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/configure/configure.py` & `langreact-0.2.8/langreact/core/configure/configure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import asdict, replace
 import importlib
 import importlib.util
 from langreact.core.configure.default import Configure
 
 configure_cache = {}
 
 
@@ -10,10 +11,10 @@
         return Configure()
     cache_key = path + ":" + name
     if cache_key in configure_cache:
         return configure_cache[cache_key]
     configure_spec = importlib.util.spec_from_file_location("conf", path)
     configure_module = importlib.util.module_from_spec(configure_spec)
     configure_spec.loader.exec_module(configure_module)
-    configure = getattr(configure_module, name)()
-    configure_cache[cache_key] = configure
-    return configure
+    conf = getattr(configure_module, name)()
+    configure_cache[cache_key] = replace(Configure(), **asdict(conf))
+    return configure_cache[cache_key]
```

### Comparing `langreact-0.2.7/langreact/core/configure/default.py` & `langreact-0.2.8/langreact/core/configure/default.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/configure/logging.conf` & `langreact-0.2.8/langreact/core/configure/logging.conf`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/context.py` & `langreact-0.2.8/langreact/core/context.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/flow.py` & `langreact-0.2.8/langreact/core/flow.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/memory/memory.py` & `langreact-0.2.8/langreact/core/memory/memory.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/memory/memory_chunk.py` & `langreact-0.2.8/langreact/core/memory/memory_chunk.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/memory/memory_index.py` & `langreact-0.2.8/langreact/core/memory/memory_index.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/modifier/chunk_modifier.py` & `langreact-0.2.8/langreact/core/modifier/chunk_modifier.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/modifier/context_modifier.py` & `langreact-0.2.8/langreact/core/modifier/context_modifier.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/observer/feedback.py` & `langreact-0.2.8/langreact/core/observer/feedback.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/observer/observer.py` & `langreact-0.2.8/langreact/core/observer/observer.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/params.py` & `langreact-0.2.8/langreact/core/params.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/planning/agent.py` & `langreact-0.2.8/langreact/core/planning/agent.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/plugin/plugins.py` & `langreact-0.2.8/langreact/core/plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/steps.py` & `langreact-0.2.8/langreact/core/steps.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/langreact/core/tools.py` & `langreact-0.2.8/langreact/core/tools.py`

 * *Files identical despite different names*

### Comparing `langreact-0.2.7/pyproject.toml` & `langreact-0.2.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langreact"
-version = "0.2.7"
+version = "0.2.8"
 description = "LangReact Project"
 authors = ["zhangli <max_and_min@163.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "langreact", format = "wheel" },
     { include = "langreact", format = "sdist" },
```

### Comparing `langreact-0.2.7/PKG-INFO` & `langreact-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langreact
-Version: 0.2.7
+Version: 0.2.8
 Summary: LangReact Project
 License: MIT
 Author: zhangli
 Author-email: max_and_min@163.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

