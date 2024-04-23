# Comparing `tmp/notdiamond-0.1.6b0.tar.gz` & `tmp/notdiamond-0.1.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.6b0.tar", max compression
+gzip compressed data, was "notdiamond-0.1.7b0.tar", max compression
```

## Comparing `notdiamond-0.1.6b0.tar` & `notdiamond-0.1.7b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     5862 2024-04-22 18:39:28.549020 notdiamond-0.1.6b0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.6b0/notdiamond/__init__.py
--rw-r--r--   0        0        0      831 2024-04-22 18:35:58.307978 notdiamond-0.1.6b0/notdiamond/callbacks.py
--rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.6b0/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.6b0/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0    35174 2024-04-22 18:35:58.308337 notdiamond-0.1.6b0/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.6b0/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.6b0/notdiamond/llms/providers.py
--rw-r--r--   0        0        0    10648 2024-04-19 07:58:41.324295 notdiamond-0.1.6b0/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.6b0/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.6b0/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.6b0/notdiamond/metrics/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.6b0/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.6b0/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     5007 2024-04-19 07:58:41.324616 notdiamond-0.1.6b0/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.6b0/notdiamond/settings.py
--rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.6b0/notdiamond/types.py
--rw-r--r--   0        0        0     1458 2024-04-22 18:40:11.952162 notdiamond-0.1.6b0/pyproject.toml
--rw-r--r--   0        0        0     6974 1970-01-01 00:00:00.000000 notdiamond-0.1.6b0/PKG-INFO
+-rw-r--r--   0        0        0     5862 2024-04-22 18:39:28.549020 notdiamond-0.1.7b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.7b0/notdiamond/__init__.py
+-rw-r--r--   0        0        0      831 2024-04-22 18:35:58.307978 notdiamond-0.1.7b0/notdiamond/callbacks.py
+-rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.7b0/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.7b0/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0    38807 2024-04-23 15:21:39.834488 notdiamond-0.1.7b0/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.7b0/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.7b0/notdiamond/llms/providers.py
+-rw-r--r--   0        0        0    10648 2024-04-19 07:58:41.324295 notdiamond-0.1.7b0/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.7b0/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.7b0/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.7b0/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.7b0/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.7b0/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     5760 2024-04-23 15:21:39.834968 notdiamond-0.1.7b0/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.7b0/notdiamond/settings.py
+-rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.7b0/notdiamond/types.py
+-rw-r--r--   0        0        0     1458 2024-04-23 15:21:55.729790 notdiamond-0.1.7b0/pyproject.toml
+-rw-r--r--   0        0        0     6974 1970-01-01 00:00:00.000000 notdiamond-0.1.7b0/PKG-INFO
```

### Comparing `notdiamond-0.1.6b0/README.md` & `notdiamond-0.1.7b0/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/callbacks.py` & `notdiamond-0.1.7b0/notdiamond/callbacks.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/llms/llm.py` & `notdiamond-0.1.7b0/notdiamond/llms/llm.py`

 * *Files 16% similar despite different names*

```diff
@@ -220,47 +220,54 @@
     ) -> str:
         if stop is not None:
             raise ValueError("stop kwargs are not permitted.")
         return "This function is deprecated for the latest LangChain version, use invoke instead"
 
     def invoke(
         self,
-        prompt_template: Union[
-            NDPromptTemplate,
-            PromptTemplate,
-            NDChatPromptTemplate,
-            ChatPromptTemplate,
-            str,
-        ],
+        prompt_template: Optional[
+            Union[
+                NDPromptTemplate,
+                PromptTemplate,
+                NDChatPromptTemplate,
+                ChatPromptTemplate,
+                str,
+            ]
+        ] = None,
+        messages: Optional[List[Dict[str, str]]] = None,
         input: Optional[Dict[str, Any]] = None,
         metric: NDMetric = NDMetric("accuracy"),
         **kwargs,
     ) -> AIMessage:
         """
         Function to invoke the LLM. Behind the scenes what happens:
         1. API call to NotDiamond backend to get the most suitable LLM for the given prompt
         2. Invoke the returned LLM client side
         3. Return the response
 
         Parameters:
-            prompt_template (Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ]):
+            prompt_template (Optional(Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ])):
                 the prompt template defined by the user. It also supports Langchain prompt template types.
+            messages (Optional[List[Dict[str, str]], optional): Can be used instead of prompt_template to pass
+                the messages OpenAI style.
             input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
                                                         the values for those variables. Defaults to None, assuming no variables.
             metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
                                             Defaults to NDMetric("accuracy").
             **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
 
         Raises:
             ApiError: when the NotDiamond API fails
 
         Returns:
             AIMessage: type defined by Langchain, contains the response from the LLM.
         """
-        prompt_template = self._prepare_prompt_template(prompt_template)
+        prompt_template = self._prepare_prompt_template(
+            prompt_template, messages
+        )
 
         if input is None:
             input = {}
 
         prompt_template.partial_variables = {
             **prompt_template.partial_variables,
             **input,
@@ -357,47 +364,54 @@
         if isinstance(result, str):
             result = AIMessage(content=result)
 
         return result, session_id, best_llm
 
     async def ainvoke(
         self,
-        prompt_template: Union[
-            NDPromptTemplate,
-            PromptTemplate,
-            NDChatPromptTemplate,
-            ChatPromptTemplate,
-            str,
-        ],
+        prompt_template: Optional[
+            Union[
+                NDPromptTemplate,
+                PromptTemplate,
+                NDChatPromptTemplate,
+                ChatPromptTemplate,
+                str,
+            ]
+        ] = None,
+        messages: Optional[List[Dict[str, str]]] = None,
         input: Optional[Dict[str, Any]] = None,
         metric: NDMetric = NDMetric("accuracy"),
         **kwargs,
     ) -> AIMessage:
         """
         Function to invoke the LLM. Behind the scenes what happens:
         1. API call to NotDiamond backend to get the most suitable LLM for the given prompt
         2. Invoke the returned LLM client side
         3. Return the response
 
         Parameters:
-            prompt_template (Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ]):
+            prompt_template (Optional(Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ])):
                 the prompt template defined by the user. It also supports Langchain prompt template types.
+            messages (Optional[List[Dict[str, str]], optional): Can be used instead of prompt_template to pass
+                the messages OpenAI style.
             input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
                                                         the values for those variables. Defaults to None, assuming no variables.
             metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
                                             Defaults to NDMetric("accuracy").
             **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
 
         Raises:
             ApiError: when the NotDiamond API fails
 
         Returns:
             AIMessage: type defined by Langchain, contains the response from the LLM.
         """
-        prompt_template = self._prepare_prompt_template(prompt_template)
+        prompt_template = self._prepare_prompt_template(
+            prompt_template, messages
+        )
 
         if input is None:
             input = {}
 
         prompt_template.partial_variables = {
             **prompt_template.partial_variables,
             **input,
@@ -494,36 +508,68 @@
                 raise e
 
         if isinstance(result, str):
             result = AIMessage(content=result)
 
         return result, session_id, best_llm
 
-    def stream(self, input=None, **kwargs) -> Iterator[BaseMessageChunk]:
+    def stream(
+        self,
+        prompt_template: Optional[
+            Union[
+                NDPromptTemplate,
+                PromptTemplate,
+                NDChatPromptTemplate,
+                ChatPromptTemplate,
+                str,
+            ]
+        ] = None,
+        messages: Optional[List[Dict[str, str]]] = None,
+        input: Optional[Dict[str, Any]] = None,
+        metric: NDMetric = NDMetric("accuracy"),
+        **kwargs,
+    ) -> Iterator[BaseMessageChunk]:
         """
         This function calls the NotDiamond backend to fetch the most suitable model for the given prompt,
         and calls the LLM client side to stream the response.
 
         Parameters:
+            prompt_template (Optional(Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ])):
+                the prompt template defined by the user. It also supports Langchain prompt template types.
+            messages (Optional[List[Dict[str, str]], optional): Can be used instead of prompt_template to pass
+                the messages OpenAI style.
             input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
                                                         the values for those variables. Defaults to None, assuming no variables.
+            metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
+                                            Defaults to NDMetric("accuracy").
             **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
 
         Raises:
             ApiError: when the NotDiamond API fails
 
         Yields:
             Iterator[BaseMessageChunk]: returns the response in chunks
         """
 
-        prompt_template = self._prepare_prompt_template(prompt_template=input)
+        prompt_template = self._prepare_prompt_template(
+            prompt_template=prompt_template, messages=messages
+        )
+
+        if input is None:
+            input = {}
+
+        prompt_template.partial_variables = {
+            **prompt_template.partial_variables,
+            **input,
+        }
+
         best_llm, session_id = model_select(
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
-            metric=NDMetric("accuracy"),
+            metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
         )
 
         if not best_llm:
@@ -538,47 +584,76 @@
                 raise ApiError(error_message)
         self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
         llm = self._llm_from_provider(best_llm, callbacks=self.callbacks)
         if self.tools:
             llm = llm.bind_tools(self.tools)
 
-        for chunk in llm.stream(input, **kwargs):
+        for chunk in llm.stream(prompt_template.format(), **kwargs):
             yield chunk
 
     async def astream(
-        self, input=None, **kwargs
+        self,
+        prompt_template: Optional[
+            Union[
+                NDPromptTemplate,
+                PromptTemplate,
+                NDChatPromptTemplate,
+                ChatPromptTemplate,
+                str,
+            ]
+        ] = None,
+        messages: Optional[List[Dict[str, str]]] = None,
+        input: Optional[Dict[str, Any]] = None,
+        metric: NDMetric = NDMetric("accuracy"),
+        **kwargs,
     ) -> AsyncIterator[BaseMessageChunk]:
         """
         This function calls the NotDiamond backend to fetch the most suitable model for the given prompt,
         and calls the LLM client side to stream the response. The function is async, so it's suitable for async codebases.
 
         Parameters:
+            prompt_template (Optional(Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ])):
+                the prompt template defined by the user. It also supports Langchain prompt template types.
+            messages (Optional[List[Dict[str, str]], optional): Can be used instead of prompt_template to pass
+                the messages OpenAI style.
             input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
                                                         the values for those variables. Defaults to None, assuming no variables.
+            metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
+                                            Defaults to NDMetric("accuracy").
             **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
 
         Raises:
             ApiError: when the NotDiamond API fails
 
         Yields:
             AsyncIterator[BaseMessageChunk]: returns the response in chunks
         """
 
-        prompt_template = self._prepare_prompt_template(prompt_template=input)
+        prompt_template = self._prepare_prompt_template(
+            prompt_template=prompt_template, messages=messages
+        )
         best_llm, session_id = await amodel_select(
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
-            metric=NDMetric("accuracy"),
+            metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
         )
 
+        if input is None:
+            input = {}
+
+        prompt_template.partial_variables = {
+            **prompt_template.partial_variables,
+            **input,
+        }
+
         if not best_llm:
             best_llm = self.default_llm_provider
 
             if best_llm is None:
                 error_message = (
                     "ND couldn't find a suitable model to call."
                     + "To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
@@ -587,15 +662,15 @@
                 raise ApiError(error_message)
         self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
         llm = self._llm_from_provider(best_llm, callbacks=self.callbacks)
         if self.tools:
             llm = llm.bind_tools(self.tools)
 
-        async for chunk in llm.astream(input, **kwargs):
+        async for chunk in llm.astream(prompt_template.format(), **kwargs):
             yield chunk
 
     async def amodel_select(
         self,
         prompt_template: Optional[
             Union[
                 NDPromptTemplate,
@@ -855,36 +930,47 @@
                 callbacks=callbacks,
                 **provider.kwargs,
             )
         raise ValueError(f"Unsupported provider: {provider.provider}")
 
     @staticmethod
     def _prepare_prompt_template(
-        prompt_template,
+        prompt_template, messages=None
     ) -> Union[NDPromptTemplate, NDChatPromptTemplate]:
-        if isinstance(prompt_template, NDPromptTemplate) or isinstance(
-            prompt_template, NDChatPromptTemplate
-        ):
-            return prompt_template
-        if isinstance(prompt_template, str):
-            return NDPromptTemplate(template=prompt_template)
-        if isinstance(prompt_template, PromptTemplate):
-            return NDPromptTemplate.from_langchain_prompt_template(
-                prompt_template
+        if prompt_template is not None and messages is not None:
+            print(
+                "Warning: prompt_template value is overriding messages value. Set one of those values for optimal performance."
             )
-        if isinstance(prompt_template, ChatPromptTemplate):
-            return NDChatPromptTemplate.from_langchain_chat_prompt_template(
-                prompt_template
+        if prompt_template is not None:
+            if isinstance(prompt_template, NDPromptTemplate) or isinstance(
+                prompt_template, NDChatPromptTemplate
+            ):
+                return prompt_template
+            if isinstance(prompt_template, str):
+                return NDPromptTemplate(template=prompt_template)
+            if isinstance(prompt_template, PromptTemplate):
+                return NDPromptTemplate.from_langchain_prompt_template(
+                    prompt_template
+                )
+            if isinstance(prompt_template, ChatPromptTemplate):
+                return (
+                    NDChatPromptTemplate.from_langchain_chat_prompt_template(
+                        prompt_template
+                    )
+                )
+            if isinstance(prompt_template, list):
+                if all(isinstance(pt, BaseMessage) for pt in prompt_template):
+                    return NDChatPromptTemplate.from_messages(prompt_template)
+            raise ValueError(
+                f"Unsupported prompt_template type {type(prompt_template)}"
             )
-        if isinstance(prompt_template, list):
-            if all(isinstance(pt, BaseMessage) for pt in prompt_template):
-                return NDChatPromptTemplate.from_messages(prompt_template)
-        raise ValueError(
-            f"Unsupported prompt_template type {type(prompt_template)}"
-        )
+        if messages is not None:
+            return NDChatPromptTemplate.from_openai_messages(messages)
+
+        raise ValueError("prompt_template or messages must be specified.")
 
     def bind_tools(
         self,
         tools: Sequence[Union[Dict[str, Any], Callable]],
     ) -> "NDLLM":
         """
         Bind tools to the LLM object. The tools will be passed to the LLM object when invoking it.
```

### Comparing `notdiamond-0.1.6b0/notdiamond/llms/provider.py` & `notdiamond-0.1.7b0/notdiamond/llms/provider.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/llms/providers.py` & `notdiamond-0.1.7b0/notdiamond/llms/providers.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/llms/request.py` & `notdiamond-0.1.7b0/notdiamond/llms/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/metrics/metric.py` & `notdiamond-0.1.7b0/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/metrics/request.py` & `notdiamond-0.1.7b0/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/prompts/prompt.py` & `notdiamond-0.1.7b0/notdiamond/prompts/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,14 +94,32 @@
     ):
         return cls(
             messages=chat_prompt_template.messages,
             input_variables=chat_prompt_template.input_variables,
             partial_variables=chat_prompt_template.partial_variables,
         )
 
+    @classmethod
+    def from_openai_messages(cls, messages: List[Dict[str, str]]):
+        transformed_messages = []
+        for message in messages:
+            if message["role"] == "system":
+                transformed_messages.append(SystemMessage(message["content"]))
+            elif message["role"] == "assistant":
+                transformed_messages.append(AIMessage(message["content"]))
+            elif message["role"] == "user":
+                transformed_messages.append(HumanMessage(message["content"]))
+            else:
+                raise ValueError(f"Unsupported role: {message['role']}")
+        return cls(
+            messages=transformed_messages,
+            input_variables=None,
+            partial_variables={},
+        )
+
     def format(self, **kwargs: Any) -> str:
         """Format the prompt template with the given variables. and converts it to NDChatPromptTemplate."""
         return super(NDChatPromptTemplate, self).format(**kwargs)
 
     def get_last_human_message(self, formated_messages: List) -> str:
         for message in reversed(formated_messages):
             if isinstance(message, HumanMessage):
```

### Comparing `notdiamond-0.1.6b0/notdiamond/settings.py` & `notdiamond-0.1.7b0/notdiamond/settings.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/notdiamond/types.py` & `notdiamond-0.1.7b0/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.6b0/pyproject.toml` & `notdiamond-0.1.7b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.6-beta"
+version = "0.1.7-beta"
 description = "Not Diamond Python Library"
 authors = ["Not Diamond <t5@notdiamond.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 langchain = ">=0.1.16"
```

### Comparing `notdiamond-0.1.6b0/PKG-INFO` & `notdiamond-0.1.7b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.6b0
+Version: 0.1.7b0
 Summary: Not Diamond Python Library
 Author: Not Diamond
 Author-email: t5@notdiamond.ai
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

