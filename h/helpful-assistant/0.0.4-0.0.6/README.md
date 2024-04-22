# Comparing `tmp/helpful-assistant-0.0.4.tar.gz` & `tmp/helpful_assistant-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helpful-assistant-0.0.4.tar", last modified: Thu Apr 11 23:21:54 2024, max compression
+gzip compressed data, was "helpful_assistant-0.0.6.tar", last modified: Mon Apr 22 22:32:26 2024, max compression
```

## Comparing `helpful-assistant-0.0.4.tar` & `helpful_assistant-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:21:54.960754 helpful-assistant-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-11 23:21:54.960754 helpful-assistant-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:21:54.960754 helpful-assistant-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:21:54.960754 helpful-assistant-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:21:54.960754 helpful-assistant-0.0.4/src/helpful-assistant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/src/helpful-assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:21:54.960754 helpful-assistant-0.0.4/src/helpful_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/src/helpful_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/src/helpful_assistant/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/src/helpful_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/src/helpful_assistant/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/src/helpful_assistant/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-11 23:21:50.000000 helpful-assistant-0.0.4/src/helpful_assistant/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:21:54.960754 helpful-assistant-0.0.4/src/helpful_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-11 23:21:54.000000 helpful-assistant-0.0.4/src/helpful_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-11 23:21:54.000000 helpful-assistant-0.0.4/src/helpful_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:21:54.000000 helpful-assistant-0.0.4/src/helpful_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 23:21:54.000000 helpful-assistant-0.0.4/src/helpful_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.450614 helpful_assistant-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:32:26.450614 helpful_assistant-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/src/helpful_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/top_level.txt
```

### Comparing `helpful-assistant-0.0.4/LICENSE` & `helpful_assistant-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helpful-assistant-0.0.4/PKG-INFO` & `helpful_assistant-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.4
+Version: 0.0.6
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `helpful-assistant-0.0.4/README.md` & `helpful_assistant-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `helpful-assistant-0.0.4/pyproject.toml` & `helpful_assistant-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "helpful-assistant"
-version = "0.0.4"
+version = "0.0.6"
 authors = [
   { name="Whitelisted" },
 ]
 description = "Allows LLMs to assist you with various tasks, all while being open-source!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `helpful-assistant-0.0.4/src/helpful_assistant/conversation.py` & `helpful_assistant-0.0.6/src/helpful_assistant/conversation.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,23 +16,74 @@
 
 
 class Conversation:
     def __init__(self, name: str = "Conversation", history: Optional[List[Message]] = None, assistant: Optional[Assistant] = None) -> None:
         if history is None:
             history = []
             if assistant is not None:
+                assistant.event_manager.trigger_event("conversation_create", self)
                 history = [Message("system", assistant.get_system_message())]
 
         self.name = name
         self.history = history
         self.assistant = assistant
+        self.discarded = False
 
-    def _add_to_history(self, message: Message) -> None:
-        self.history.append(message)
+    def get_by_role(self, role: str) -> List[Message]:
+        """
+        Fetches all messages by a specific role in the Conversation history.
+
+        Parameters:
+        role (str): the role to search for.
+
+        Returns:
+        List[Message]: A list of the messages by the specified role.
+        """
+
+        out = []
+        for message in self.history:
+            if message.role == role:
+                out.append(message)
+        return out
 
     def generate(self, prompt: str = None, *args, **kwargs) -> Union[Stream, str]:
+        """
+        Generates text from the Large Language Model.
+
+        Parameters:
+        prompt (str): The prompt for the model. Appends to conversation history.
+        args (*args): Arguments to pass to the generate function.
+        kwargs (**kwargs) Keyword arguments to pass to the generate function.
+
+        Returns:
+        Union[Stream, str]: Generated text or text Stream.
+        """
+
         if self.assistant is None:
             raise RuntimeError("No assistant object specified in this conversation.")
 
         self._add_to_history(Message("user", prompt))
 
         return self.assistant.generate(conversation=self, *args, **kwargs)
+
+    def discard(self) -> None:
+        """
+        Discards the conversation object. Main purpose is to trigger the "conversation_discarded" event.
+        """
+
+        if self.assistant is not None:
+            self.assistant.event_manager.trigger_event("conversation_discard", self)
+
+        self.history.clear()
+        self.assistant = None
+        self.name = None
+        self.discarded = True
+
+    def _add_to_history(self, message: Message) -> None:
+        """
+        Adds a message to Conversation history.
+
+        Parameters:
+        message (Message): The Message object to add to conversation history.
+        """
+
+        self.history.append(message)
```

### Comparing `helpful-assistant-0.0.4/src/helpful_assistant/module.py` & `helpful_assistant-0.0.6/src/helpful_assistant/module.py`

 * *Files identical despite different names*

### Comparing `helpful-assistant-0.0.4/src/helpful_assistant.egg-info/PKG-INFO` & `helpful_assistant-0.0.6/src/helpful_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.4
+Version: 0.0.6
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

