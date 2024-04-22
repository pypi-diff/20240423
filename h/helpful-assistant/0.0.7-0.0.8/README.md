# Comparing `tmp/helpful_assistant-0.0.7.tar.gz` & `tmp/helpful_assistant-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helpful_assistant-0.0.7.tar", last modified: Mon Apr 22 23:19:42 2024, max compression
+gzip compressed data, was "helpful_assistant-0.0.8.tar", last modified: Mon Apr 22 23:31:19 2024, max compression
```

## Comparing `helpful_assistant-0.0.7.tar` & `helpful_assistant-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.990129 helpful_assistant-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/src/helpful_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:31:19.466785 helpful_assistant-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:31:19.466785 helpful_assistant-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:31:19.466785 helpful_assistant-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:31:19.462785 helpful_assistant-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:31:19.466785 helpful_assistant-0.0.8/src/helpful_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/src/helpful_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/src/helpful_assistant/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/src/helpful_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/src/helpful_assistant/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/src/helpful_assistant/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/src/helpful_assistant/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 23:31:07.000000 helpful_assistant-0.0.8/src/helpful_assistant/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:31:19.466785 helpful_assistant-0.0.8/src/helpful_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:31:19.000000 helpful_assistant-0.0.8/src/helpful_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 23:31:19.000000 helpful_assistant-0.0.8/src/helpful_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:31:19.000000 helpful_assistant-0.0.8/src/helpful_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 23:31:19.000000 helpful_assistant-0.0.8/src/helpful_assistant.egg-info/top_level.txt
```

### Comparing `helpful_assistant-0.0.7/LICENSE` & `helpful_assistant-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.7/PKG-INFO` & `helpful_assistant-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.7
+Version: 0.0.8
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `helpful_assistant-0.0.7/README.md` & `helpful_assistant-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.7/pyproject.toml` & `helpful_assistant-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "helpful-assistant"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Whitelisted" },
 ]
 description = "Allows LLMs to assist you with various tasks, all while being open-source!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `helpful_assistant-0.0.7/src/helpful_assistant/assistant.py` & `helpful_assistant-0.0.8/src/helpful_assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.7/src/helpful_assistant/conversation.py` & `helpful_assistant-0.0.8/src/helpful_assistant/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     def __str__(self) -> str:
         return self.content
 
 
 class Conversation:
     def __init__(self, name: str = "Conversation", history: Optional[List[Message]] = None, assistant: Optional[Assistant] = None) -> None:
         if history is None:
-            history = []
-            if assistant is not None:
-                assistant.event_manager.trigger_event("conversation_create", self)
-                history = [Message("system", assistant.get_system_message())]
+            history = [] if assistant is None else [Message("system", assistant.get_system_message())]
+
+        if assistant is not None:
+            assistant.event_manager.trigger_event("conversation_create", self)
 
         self.name = name
         self.history = history
         self.assistant = assistant
         self.discarded = False
 
     def get_by_role(self, role: str) -> List[Message]:
```

### Comparing `helpful_assistant-0.0.7/src/helpful_assistant/events.py` & `helpful_assistant-0.0.8/src/helpful_assistant/events.py`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.7/src/helpful_assistant/module.py` & `helpful_assistant-0.0.8/src/helpful_assistant/module.py`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.7/src/helpful_assistant.egg-info/PKG-INFO` & `helpful_assistant-0.0.8/src/helpful_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.7
+Version: 0.0.8
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

