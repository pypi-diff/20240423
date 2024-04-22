# Comparing `tmp/helpful_assistant-0.0.6.tar.gz` & `tmp/helpful_assistant-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helpful_assistant-0.0.6.tar", last modified: Mon Apr 22 22:32:26 2024, max compression
+gzip compressed data, was "helpful_assistant-0.0.7.tar", last modified: Mon Apr 22 23:19:42 2024, max compression
```

## Comparing `helpful_assistant-0.0.6.tar` & `helpful_assistant-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.450614 helpful_assistant-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:32:26.450614 helpful_assistant-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/src/helpful_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 22:32:22.000000 helpful_assistant-0.0.6/src/helpful_assistant/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:32:26.446614 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 22:32:26.000000 helpful_assistant-0.0.6/src/helpful_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.990129 helpful_assistant-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/src/helpful_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 23:19:33.000000 helpful_assistant-0.0.7/src/helpful_assistant/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:42.994129 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 23:19:42.000000 helpful_assistant-0.0.7/src/helpful_assistant.egg-info/top_level.txt
```

### Comparing `helpful_assistant-0.0.6/LICENSE` & `helpful_assistant-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.6/PKG-INFO` & `helpful_assistant-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.6
+Version: 0.0.7
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `helpful_assistant-0.0.6/README.md` & `helpful_assistant-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.6/pyproject.toml` & `helpful_assistant-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "helpful-assistant"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Whitelisted" },
 ]
 description = "Allows LLMs to assist you with various tasks, all while being open-source!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `helpful_assistant-0.0.6/src/helpful_assistant/assistant.py` & `helpful_assistant-0.0.7/src/helpful_assistant/assistant.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,26 @@
         Returns:
         Conversation: A new conversation instance.
         """
         c = Conversation(name=name, history=history, assistant=self)
         self.conversation_list.append(c)
         return c
 
+    def remove_conversation(self, conversation: Conversation) -> None:
+        """
+        Removes a conversation from the conversation list. Calls the conversation's `discard` function.
+
+        Parameters:
+        conversation (Conversation): The conversation to remove and discard.
+        """
+
+        self.event_manager.trigger_event("conversation_discard", conversation)
+        self.conversation_list.remove(conversation)
+
+
     def add_module(self, module: Module) -> None:
         """
         Appends a module to the Assistant object.
 
         Parameters:
         module (Module): A Module object to append to the assistant's module list.
         """
@@ -61,30 +73,30 @@
         stream (bool, optional, defaults to False): Should the output be returned as a generator.
         allow_action_execution (bool, defaults to True): Allow for actions to be executed by the LLM.
 
         Returns:
         Union[Stream, str]: A Stream object or a string depending on the stream parameter. The output from the LLM.
         """
 
-        generation_conversation = Conversation(history=copy.deepcopy(conversation.history), assistant=self)
+        generation_conversation = self.new_conversation(history=copy.deepcopy(conversation.history))
 
         if allow_action_execution:
             # execute a task, if needed, and add that information to the covnersation
             task_output, used_module, used_action = self._app_action_cycle(conversation)
 
             # if the task actually ran append it to user input
             if task_output is not None:
                 generation_conversation.history[-1].content += f"\n\n(An action was run. Action Output: ```{task_output}```. Use this output in your response, if applicable.)"
 
         def conversation_callback(x):
             conversation._add_to_history(Message("assistant", "".join(x)))
             generation_conversation.discard()
 
         # Make a Stream object that adds the generation result to history once it has completed
-        output = Stream(self.llm.generate(generation_conversation.history, stream=stream), conversation_callback)
+        output = Stream(self.llm.generate(generation_conversation, stream=stream), conversation_callback)
 
         # return the Stream object
         return output
 
     def _app_action_cycle(self, conversation: Conversation) -> List[Union[str, None], Union[Module, None], Union[Action, None]]:
         """
         Internal function which allows for the model to choose from the Modules and Actions.
@@ -93,35 +105,27 @@
         conversation (Conversation): The Conversation object in which to get data from
 
         Returns:
         List[Union[str, None], Union[Module, None], Union[Action, None]]: The output from the action run, the module used, and the action run.
         """
 
         # create a new conversation
-        action_conversation = Conversation(assistant=self)
-        action_conversation_history = action_conversation.history
-
-        action_conversation_history.append(Message("system", f'''This application has different modules and actions. Here are your available modules:
-
-{self.convert_modules_to_llm_readable()}
-
-You must only use the provided modules and actions in this conversation.'''))
-
+        action_conversation = self.new_conversation(history=[Message("system", f'This application has different modules and actions. Here are your available modules:\n\n{self.convert_modules_to_llm_readable()}\n\nYou must only use the provided modules and actions in this conversation.')])
 
         # split conversation history into newlines, excluding the system prompt
         user_message_history = "\n".join(f"{m.role}: {m.content}" for m in conversation.get_by_role("user"))
 
         # Make a prompt for the model to choose a module
         modules_prompt = f'''Given the user prompts, respond with the name of the module you want to learn more about. Only use modules relevant to the latest user message. Respond with "null" if none apply.\n\n{user_message_history}'''
-        action_conversation_history.append(Message("user", modules_prompt))
+        action_conversation.history.append(Message("user", modules_prompt))
 
 
         # Get the model output and append it to conversation_history
-        output: str = self.llm.generate(action_conversation_history, stream=False)
-        action_conversation_history.append(Message("assistant", output))
+        output: str = self.llm.generate(action_conversation, stream=False)
+        action_conversation.history.append(Message("assistant", output))
         output = output.strip().lower()
 
         logging.debug(f"Model chose Module: {output}")
 
         # if the model did not select a module, then stop
         if output == "null":
             action_conversation.discard()
@@ -136,19 +140,19 @@
 
         # if the model chose an invalid module, then stop
         if active_module is None:
             action_conversation.discard()
             return None, None, None
 
         # Make the model choose an action
-        action_conversation_history.append(Message("user", f'''The "{active_module.name}" module has the following actions:\n```\n{active_module.convert_actions_to_llm_readable()}\n```\n\nRespond with ONLY the name of the action that you would like to execute. Any other text or tokens will break the application. If you do not wish to execute any of the given actions, respond with EXACTLY "null".'''))
+        action_conversation.history.append(Message("user", f'''The "{active_module.name}" module has the following actions:\n```\n{active_module.convert_actions_to_llm_readable()}\n```\n\nRespond with ONLY the name of the action that you would like to execute. Any other text or tokens will break the application. If you do not wish to execute any of the given actions, respond with EXACTLY "null".'''))
 
         # get model output and append it to conversation_history
-        output: str = self.llm.generate(action_conversation_history, stream=False)
-        action_conversation_history.append(Message("assistant", output))
+        output: str = self.llm.generate(action_conversation, stream=False)
+        action_conversation.history.append(Message("assistant", output))
         output = output.strip().lower()
 
         logging.debug(f"Model chose Action: {output}")
 
         # if the model did not select an action, then stop
         if output == "null":
             action_conversation.discard()
```

### Comparing `helpful_assistant-0.0.6/src/helpful_assistant/conversation.py` & `helpful_assistant-0.0.7/src/helpful_assistant/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,23 +67,23 @@
 
     def discard(self) -> None:
         """
         Discards the conversation object. Main purpose is to trigger the "conversation_discarded" event.
         """
 
         if self.assistant is not None:
-            self.assistant.event_manager.trigger_event("conversation_discard", self)
+            self.assistant.remove_conversation(self)
 
         self.history.clear()
         self.assistant = None
         self.name = None
         self.discarded = True
 
     def _add_to_history(self, message: Message) -> None:
         """
         Adds a message to Conversation history.
 
         Parameters:
         message (Message): The Message object to add to conversation history.
         """
 
-        self.history.append(message)
+        self.history.append(message)
```

### Comparing `helpful_assistant-0.0.6/src/helpful_assistant/events.py` & `helpful_assistant-0.0.7/src/helpful_assistant/events.py`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.6/src/helpful_assistant/module.py` & `helpful_assistant-0.0.7/src/helpful_assistant/module.py`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.6/src/helpful_assistant.egg-info/PKG-INFO` & `helpful_assistant-0.0.7/src/helpful_assistant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.6
+Version: 0.0.7
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

