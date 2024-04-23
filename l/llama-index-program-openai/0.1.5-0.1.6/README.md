# Comparing `tmp/llama_index_program_openai-0.1.5.tar.gz` & `tmp/llama_index_program_openai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_program_openai-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_program_openai-0.1.6.tar", max compression
```

## Comparing `llama_index_program_openai-0.1.5.tar` & `llama_index_program_openai-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       49 2024-03-27 16:58:05.610424 llama_index_program_openai-0.1.5/README.md
--rw-r--r--   0        0        0      103 2024-03-27 16:58:05.610424 llama_index_program_openai-0.1.5/llama_index/program/openai/__init__.py
--rw-r--r--   0        0        0    10140 2024-03-27 16:58:05.610424 llama_index_program_openai-0.1.5/llama_index/program/openai/base.py
--rw-r--r--   0        0        0     1524 2024-03-27 16:58:05.610424 llama_index_program_openai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 llama_index_program_openai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-04-23 15:16:35.244405 llama_index_program_openai-0.1.6/README.md
+-rw-r--r--   0        0        0      103 2024-04-23 15:16:35.244405 llama_index_program_openai-0.1.6/llama_index/program/openai/__init__.py
+-rw-r--r--   0        0        0    11448 2024-04-23 15:16:35.244405 llama_index_program_openai-0.1.6/llama_index/program/openai/base.py
+-rw-r--r--   0        0        0     2173 2024-04-23 15:16:35.244405 llama_index_program_openai-0.1.6/llama_index/program/openai/utils.py
+-rw-r--r--   0        0        0     1524 2024-04-23 15:16:35.244405 llama_index_program_openai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 llama_index_program_openai-0.1.6/PKG-INFO
```

### Comparing `llama_index_program_openai-0.1.5/llama_index/program/openai/base.py` & `llama_index_program_openai-0.1.6/llama_index/program/openai/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import logging
 from typing import Any, Dict, Generator, List, Optional, Tuple, Type, Union, cast
 
+from llama_index.core.bridge.pydantic import ValidationError
 from llama_index.agent.openai.utils import resolve_tool_choice
 from llama_index.core.llms.llm import LLM
 from llama_index.core.program.llm_prompt_program import BaseLLMFunctionProgram
 from llama_index.core.program.utils import create_list_model
 from llama_index.core.prompts.base import BasePromptTemplate, PromptTemplate
 from llama_index.core.settings import Settings
 from llama_index.core.types import Model
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.openai.utils import OpenAIToolCall, to_openai_tool
 
+from llama_index.program.openai.utils import parse_partial_json
+
 _logger = logging.getLogger(__name__)
 
 
 def _default_tool_choice(
     output_cls: Type[Model], allow_multiple: bool = False
 ) -> Union[str, Dict[str, Any]]:
     """Default OpenAI tool to choose."""
@@ -272,14 +275,44 @@
             if new_obj_json_str is not None:
                 obj_json_str = new_obj_json_str
                 obj = self._output_cls.parse_raw(obj_json_str)
                 if self._verbose:
                     print(f"Extracted object: {obj.json()}")
                 yield obj
 
+    def stream_partial_objects(
+        self,
+        llm_kwargs: Optional[Dict[str, Any]] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Generator[Model, None, None]:
+        """Streams the intermediate partial object."""
+        llm_kwargs = llm_kwargs or {}
+        messages = self._prompt.format_messages(llm=self._llm, **kwargs)
+
+        description = self._description_eval(**kwargs)
+        openai_fn_spec = to_openai_tool(self._output_cls, description=description)
+        chat_response_gen = self._llm.stream_chat(
+            messages=messages,
+            tools=[openai_fn_spec],
+            tool_choice=self._tool_choice,
+            **llm_kwargs,
+        )
+        for partial_resp in chat_response_gen:
+            kwargs = partial_resp.message.additional_kwargs
+            tool_calls = kwargs["tool_calls"]
+            if len(tool_calls) == 0:
+                continue
+            fn_args = kwargs["tool_calls"][0].function.arguments
+            try:
+                partial_object = parse_partial_json(fn_args)
+                yield self._output_cls.parse_obj(partial_object)
+            except (ValidationError, ValueError):
+                continue
+
     def _description_eval(self, **kwargs: Any) -> Optional[str]:
         description = kwargs.get("description", None)
 
         ## __doc__ checks if docstring is provided in the Pydantic Model
         if not (self._output_cls.__doc__ or description):
             raise ValueError(
                 "Must provide description for your Pydantic Model. Either provide a docstring or add `description=<your_description>` to the method. Required to convert Pydantic Model to OpenAI Function."
```

### Comparing `llama_index_program_openai-0.1.5/pyproject.toml` & `llama_index_program_openai-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index program openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-program-openai"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-llms-openai = "^0.1.1"
 llama-index-core = "^0.10.1"
 llama-index-agent-openai = ">=0.1.1,<0.3.0"
```

### Comparing `llama_index_program_openai-0.1.5/PKG-INFO` & `llama_index_program_openai-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-program-openai
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index program openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

