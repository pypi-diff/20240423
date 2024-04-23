# Comparing `tmp/simple_chatbot_lib-0.1.0.tar.gz` & `tmp/simple_chatbot_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_chatbot_lib-0.1.0.tar", last modified: Mon Apr 22 15:04:21 2024, max compression
+gzip compressed data, was "simple_chatbot_lib-0.1.1.tar", last modified: Tue Apr 23 17:13:18 2024, max compression
```

## Comparing `simple_chatbot_lib-0.1.0.tar` & `simple_chatbot_lib-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 15:04:21.948270 simple_chatbot_lib-0.1.0/
--rw-rw-rw-   0        0        0    35821 2024-02-07 17:53:23.000000 simple_chatbot_lib-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    46315 2024-04-22 15:04:21.946269 simple_chatbot_lib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4255 2024-04-22 15:02:31.000000 simple_chatbot_lib-0.1.0/README.md
--rw-rw-rw-   0        0        0      893 2024-04-19 13:54:04.000000 simple_chatbot_lib-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 15:04:21.949268 simple_chatbot_lib-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 15:04:21.881268 simple_chatbot_lib-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 15:04:21.907269 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/
--rw-rw-rw-   0        0        0    21094 2024-04-22 14:24:15.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/chatbots.py
--rw-rw-rw-   0        0        0     3857 2024-04-22 14:30:38.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/context_services.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:04:21.932269 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/core/
--rw-rw-rw-   0        0        0     1738 2024-04-22 14:25:00.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/core/models.py
--rw-rw-rw-   0        0        0     2741 2024-04-22 14:32:45.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/mappers.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:04:21.936270 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/third_parties/
--rw-rw-rw-   0        0        0     2553 2024-04-22 14:34:45.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/third_parties/context_services.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:04:21.940270 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib.egg-info/
--rw-rw-rw-   0        0        0    46315 2024-04-22 15:04:21.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-22 15:04:21.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 15:04:21.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-04-22 15:04:21.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-22 15:04:21.000000 simple_chatbot_lib-0.1.0/src/simple_chatbot_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 17:13:18.022751 simple_chatbot_lib-0.1.1/
+-rw-rw-rw-   0        0        0    35821 2024-02-07 17:53:23.000000 simple_chatbot_lib-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    46315 2024-04-23 17:13:18.020749 simple_chatbot_lib-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4255 2024-04-22 15:02:31.000000 simple_chatbot_lib-0.1.1/README.md
+-rw-rw-rw-   0        0        0      893 2024-04-23 16:50:44.000000 simple_chatbot_lib-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 17:13:18.023752 simple_chatbot_lib-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 17:13:17.978543 simple_chatbot_lib-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:13:17.994745 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/
+-rw-rw-rw-   0        0        0    21615 2024-04-23 16:49:42.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/chatbots.py
+-rw-rw-rw-   0        0        0     3902 2024-04-23 16:50:11.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/context_services.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:13:18.011746 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/core/
+-rw-rw-rw-   0        0        0     1751 2024-04-23 16:50:28.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/core/models.py
+-rw-rw-rw-   0        0        0     2741 2024-04-22 14:32:45.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/mappers.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:13:18.014747 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/third_parties/
+-rw-rw-rw-   0        0        0     2553 2024-04-22 14:34:45.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/third_parties/context_services.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:13:18.016748 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib.egg-info/
+-rw-rw-rw-   0        0        0    46315 2024-04-23 17:13:17.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-23 17:13:17.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 17:13:17.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2024-04-23 17:13:17.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-23 17:13:17.000000 simple_chatbot_lib-0.1.1/src/simple_chatbot_lib.egg-info/top_level.txt
```

### Comparing `simple_chatbot_lib-0.1.0/LICENSE` & `simple_chatbot_lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_chatbot_lib-0.1.0/PKG-INFO` & `simple_chatbot_lib-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_chatbot_lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple package for create chatbots using LangChain
 Author-email: Gabriel Pinto Sasaki <gabrielpintosasaki@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `simple_chatbot_lib-0.1.0/README.md` & `simple_chatbot_lib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `simple_chatbot_lib-0.1.0/pyproject.toml` & `simple_chatbot_lib-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_chatbot_lib"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Gabriel Pinto Sasaki", email="gabrielpintosasaki@outlook.com" },
 ]
 description = "A simple package for create chatbots using LangChain"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
```

### Comparing `simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/chatbots.py` & `simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/chatbots.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 from langchain_core.messages import BaseMessage
 from langchain_core.language_models import BaseChatModel
 from langchain_core.tools import StructuredTool
 from langchain_core.messages import HumanMessage
 
 # Langchain
 from langchain.prompts import SystemMessagePromptTemplate, HumanMessagePromptTemplate
-from langchain.output_parsers import PydanticOutputParser
+from langchain.output_parsers import PydanticOutputParser, OutputFixingParser
 
-# Chatbot Lib
+# Simple Chatbot Lib
 from simple_chatbot_lib.context_services import ContextService
 from simple_chatbot_lib.mappers import MessageMapper
 from simple_chatbot_lib.core.models import ToolSet
 
 class BaseChatbot(metaclass=abc.ABCMeta):
     """A BaseChatbot class that uses the abc.ABCMeta metaclass. This class
     represents a base chatbot that can chat with users, 
@@ -355,36 +355,40 @@
                  llm: BaseChatModel,
                  restrictions: list[str],
                  personality: str,
                  language: str,
                  message_mapper: MessageMapper,
                  tools: list[StructuredTool],
                  keep_messages: bool = True,
-                 base_messages: Optional[list[BaseMessage]] = None) -> None:
+                 base_messages: Optional[list[BaseMessage]] = None,
+                 max_retries_parser: int = 1) -> None:
         """Initializes an AgentChatbot object.
 
         Args:
             llm (BaseChatModel): The language model used by the chatbot.
             restrictions (list[str]): The list of restrictions for the chatbot.
             personality (str): The personality of the chatbot.
             language (str): The language used by the chatbot.
             message_mapper (MessageMapper): The message mapper used by the chatbot.
             tools (list[StructuredTool]): The list of tools available to the chatbot.
             keep_messages (bool, optional): Whether to keep the chatbot's messages.
             Defaults to True.
             base_messages (Optional[list[BaseMessage]], optional): The base messages
             for the chatbot. Defaults to None.
+            max_retries_parser (int, optional): The maximum number of retries for the parser.
+            Defaults to 1.
         """
         super(AgentChatbot, self).__init__(llm, restrictions, personality, language,
                                            message_mapper, keep_messages, base_messages)
         self.tools = {}
         for tool in tools:
             if not tool.__doc__:
                 raise ValueError(f'Tool {tool.name} must have a docstring')
             self.tools[tool.name] = tool
+        self._max_retries_parser = max_retries_parser
 
     def chat(self, question: str) -> str:
         """Chat with the chatbot by asking a question.
 
         Args:
             question (str): The question to ask the chatbot.
 
@@ -446,21 +450,24 @@
             function_schema = {
                 'name': tool.name,
                 'description': tool.description,
                 'arguments': tool.args
             }
             str_tools += json.dumps(function_schema) + '\n\n'
         output_parser = PydanticOutputParser(pydantic_object=ToolSet)
+        output_fixing_parser = OutputFixingParser.from_llm(llm=self._llm,
+                                                           output_parser=output_parser,
+                                                           max_retries=self._max_retries_parser)
         format_instructions = output_parser.get_format_instructions()
         messages = system_prompt.format_messages(tools=str_tools,
                                                  question=question,
                                                  format_instructions=format_instructions)
         human_message = HumanMessage(content=question)
         messages.append(human_message)
-        chain = self._llm | output_parser
+        chain = self._llm | output_fixing_parser
         return chain.invoke(messages)
 
     def _execute_tools(self, toolset: ToolSet):
         """Executes a set of tools and returns the results.
 
         Args:
             toolset (ToolSet): The set of tools to execute.
```

### Comparing `simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/context_services.py` & `simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/context_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 a constructor and an abstract method retrieve_context for retrieving context.
 
 The APIContextService class is a class for API context services. It extends the ContextService
 class and provides a constructor and a method retrieve_context for retrieving context from an API.
 It has attributes llm, documentation, credentials, headers, and domains for configuring the API
 context service.
 """
+# Python
 import abc
 from typing import Any
+
+# Langchain Core
 from langchain_core.language_models import BaseChatModel
+
+# Langchain
 from langchain.chains.api.base import APIChain
 
 class ContextService(metaclass=abc.ABCMeta):
     """An abstract base class for context services.
 
     This class provides a constructor and an abstract method for retrieving context.
```

### Comparing `simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/core/models.py` & `simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/core/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 has attributes tool_name and tool_arguments, which store the name
 of the tool and a dictionary containing the tool arguments, respectively.
 
 The ToolSet class represents a set of tools. It has an attribute
 tool_results, which is a list of ToolResult objects containing
 the tool name and tool arguments.
 """
+# Langchain
 from langchain.pydantic_v1 import BaseModel, Field
 
 class ToolResult(BaseModel):
     """Represents the result of a tool execution.
 
     Attributes:
         tool_name (str): The name of the tool.
```

### Comparing `simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/mappers.py` & `simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/mappers.py`

 * *Files identical despite different names*

### Comparing `simple_chatbot_lib-0.1.0/src/simple_chatbot_lib/third_parties/context_services.py` & `simple_chatbot_lib-0.1.1/src/simple_chatbot_lib/third_parties/context_services.py`

 * *Files identical despite different names*

### Comparing `simple_chatbot_lib-0.1.0/src/simple_chatbot_lib.egg-info/PKG-INFO` & `simple_chatbot_lib-0.1.1/src/simple_chatbot_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_chatbot_lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple package for create chatbots using LangChain
 Author-email: Gabriel Pinto Sasaki <gabrielpintosasaki@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

