# Comparing `tmp/notdiamond-0.1.5b0.tar.gz` & `tmp/notdiamond-0.1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.5b0.tar", max compression
+gzip compressed data, was "notdiamond-0.1.6b0.tar", max compression
```

## Comparing `notdiamond-0.1.5b0.tar` & `notdiamond-0.1.6b0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     4667 2024-04-09 10:12:26.438700 notdiamond-0.1.5b0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.5b0/notdiamond/__init__.py
--rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.5b0/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.5b0/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0    32135 2024-04-16 19:48:35.309547 notdiamond-0.1.5b0/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.5b0/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.5b0/notdiamond/llms/providers.py
--rw-r--r--   0        0        0    10752 2024-04-17 11:29:51.041486 notdiamond-0.1.5b0/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.5b0/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.5b0/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.5b0/notdiamond/metrics/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.5b0/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.5b0/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     7782 2024-04-06 09:04:10.351913 notdiamond-0.1.5b0/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.5b0/notdiamond/settings.py
--rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.5b0/notdiamond/types.py
--rw-r--r--   0        0        0     1458 2024-04-17 11:29:23.215804 notdiamond-0.1.5b0/pyproject.toml
--rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 notdiamond-0.1.5b0/PKG-INFO
+-rw-r--r--   0        0        0     5862 2024-04-22 18:39:28.549020 notdiamond-0.1.6b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.6b0/notdiamond/__init__.py
+-rw-r--r--   0        0        0      831 2024-04-22 18:35:58.307978 notdiamond-0.1.6b0/notdiamond/callbacks.py
+-rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.6b0/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.6b0/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0    35174 2024-04-22 18:35:58.308337 notdiamond-0.1.6b0/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.6b0/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.6b0/notdiamond/llms/providers.py
+-rw-r--r--   0        0        0    10648 2024-04-19 07:58:41.324295 notdiamond-0.1.6b0/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.6b0/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.6b0/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.6b0/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.6b0/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.6b0/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     5007 2024-04-19 07:58:41.324616 notdiamond-0.1.6b0/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.6b0/notdiamond/settings.py
+-rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.6b0/notdiamond/types.py
+-rw-r--r--   0        0        0     1458 2024-04-22 18:40:11.952162 notdiamond-0.1.6b0/pyproject.toml
+-rw-r--r--   0        0        0     6974 1970-01-01 00:00:00.000000 notdiamond-0.1.6b0/PKG-INFO
```

### Comparing `notdiamond-0.1.5b0/README.md` & `notdiamond-0.1.6b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 # Getting started with Not Diamond
 
-Not Diamond automatically determines which model is best-suited to respond to any query. Unlike any other model router, Not Diamond is **fully privacy-preserving** and **continuously adapts to your preferences**.
+Not Diamond automatically determines which model is best-suited to respond to any query, **drastically improving LLM output quality** while reducing costs and latency and avoiding vendor lock-in. Unlike any other model router, Not Diamond is **100% privacy-preserving** and **continuously adapts to your preferences** ([demo video](https://www.loom.com/share/6e5dee9d99434de6bafbcd96ff5d663c?sid=d771348d-e9e5-49f9-9f21-6310d12541ec)).
+
+# Installation
+
+Requires **Python 3.9+**
+
+```bash
+pip install notdiamond
+```
+
+If your application isn't in Python, you can directly call our [REST API endpoint](https://notdiamond.readme.io/v0.1.0-beta/reference).
 
 # Key features
 
-- **Maintain privacy**: All inputs are [fuzzy hashed](https://en.wikipedia.org/wiki/Fuzzy_hashing) before being sent to the Not Diamond API. We return a label for the recommended model and LLM calls go out client-side. _This means we never see your raw query strings or response outputs._
-- **Maximize performance**: Not Diamond [outperforms foundation models](https://notdiamond.readme.io/v0.1.0-beta/docs/how-not-diamond-works#not-diamond-vs-claude-3-opus) out of the box. Our cold-start recommendations are based on hundreds of thousands of data points from rigorous evaluation benchmarks and real-world data.
+- **Maintain privacy**: All inputs are [fuzzy hashed](https://en.wikipedia.org/wiki/Fuzzy_hashing) before being sent to the Not Diamond API. We return a label for the recommended model and LLM calls go out client-side. _This means we never see your raw query strings or your response outputs._
+- **Maximize performance**: Not Diamond [outperforms Claude 3 Opus](https://notdiamond.readme.io/v0.1.0-beta/docs/how-not-diamond-works#not-diamond-vs-claude-3-opus) on major evaluation benchmarks. Our cold-start recommendations are based on hundreds of thousands of data points from rigorous evaluation benchmarks and real-world data.
 - **Continuously improve**: By [providing feedback on routing decisions](https://notdiamond.readme.io/v0.1.0-beta/docs/personalization), Not Diamond _continuously learns_ a hyper-personalized routing algorithm optimized to your preferences and your application's requirements.
-- **Reduce cost and latency**: Define explicit quality, cost, and latency tradeoffs to cut down your inference costs and achieve blazing fast speeds. Not Diamond determines which model to call in under 40ms—less than the time it takes an LLM to stream a single token.
+- **Reduce cost and latency**: Define explicit [quality, cost, and latency tradeoffs](https://notdiamond.readme.io/v0.1.0-beta/docs/personalization#quality-cost-and-latency-tradeoffs) to cut down your inference costs and achieve blazing fast speeds. Not Diamond determines which model to call in under 40ms—less than the time it takes an LLM to stream a single token.
+
+# Not Diamond vs. Claude 3 Opus
+
+These are preliminary results and require further validation, but initial evaluations show that Not Diamond outperforms Claude 3 Opus on major benchmarks:
+
+| Dataset        | Claude 3 Opus | Not Diamond |
+| :------------- | :------------ | :---------- |
+| MMLU           | 85.21         | **88.25**   |
+| BIG-Bench-Hard | 81.06         | **81.24**   |
+| ARC-Challenge  | 93.56         | **95.59**   |
+| WinoGrande     | 76.80         | **79.60**   |
+| MBPP           | 47.40         | **69.05**   |
+
+As can be seen with the MBPP benchmark, the biggest gains emerge when Claude 3 Opus scores particularly low on a benchmark. More testing is required however and we will be releasing a full technical report soon.
 
 > 🚧 Beta testing ahead
 >
 > Not Diamond is still in beta! Please let us know if you have any feedback or ideas on how we can improve. Tomás is at [t5@notdiamond.ai](mailto:t5@notdiamond.ai) or 917 725 2192.
 
 > 👍 Free to use!
 >
 > Not Diamond is 100% free to use during beta ♡
 
-# Installation
-
-Requires **Python 3.9+**
-
-```shell
-pip install notdiamond
-```
-
 # API keys
 
 > 👍 [Sign up](https://app.notdiamond.ai/) and get a Not Diamond API key.
 
 Create a `.env` file with your Not Diamond API key, and the API keys of the models you want to route between.
 
 ```shell
@@ -54,30 +70,27 @@
 
 Create a `main.py` file in the same folder as the [`.env`](#api-keys) file you created earlier, or **[try it in Colab](https://colab.research.google.com/drive/1Ao-YhYF_S6QP5UGp_kYhgKps_Sw3a2RO?usp=sharing).**
 
 ```python
 from notdiamond.llms.llm import NDLLM
 from notdiamond.prompts.prompt import NDPromptTemplate
 
-
-# Define the prompt template -> the string that will be routed to the best LLM
+# Define the template object -> the string that will be routed to the best LLM
 prompt_template = NDPromptTemplate("Write a merge sort in Python.")
 
 # Define the available LLMs you'd like to route between
 llm_providers = ['openai/gpt-3.5-turbo', 'openai/gpt-4','openai/gpt-4-1106-preview', 'openai/gpt-4-turbo-preview',
-                 'anthropic/claude-2.1', 'anthropic/claude-3-sonnet-20240229', 'anthropic/claude-3-opus-20240229',
-                 'google/gemini-pro']
+                 'anthropic/claude-3-haiku-20240307', 'anthropic/claude-3-sonnet-20240229', 'anthropic/claude-3-opus-20240229']
 
 # Create the NDLLM object -> like a 'meta-LLM' combining all of the specified models
 nd_llm = NDLLM(llm_providers=llm_providers)
 
 # After fuzzy hashing the inputs, the best LLM is determined by the ND API and the LLM is called client-side
 result, session_id, provider = nd_llm.invoke(prompt_template=prompt_template)
 
-
 print("ND session ID: ", session_id)  # A unique ID of the invoke. Important for personalizing ND to your use-case
 print("LLM called: ", provider.model)  # The LLM routed to
 print("LLM output: ", result.content)  # The LLM response
 ```
 
 > 👍 **Run it!**
 >
```

### Comparing `notdiamond-0.1.5b0/notdiamond/llms/llm.py` & `notdiamond-0.1.6b0/notdiamond/llms/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,28 @@
     Sequence,
     Union,
 )
 
 from langchain.prompts import PromptTemplate
 from langchain_anthropic import ChatAnthropic
 from langchain_cohere.chat_models import ChatCohere
+from langchain_core.callbacks.base import BaseCallbackHandler
 from langchain_core.callbacks.manager import CallbackManagerForLLMRun
 from langchain_core.language_models.llms import LLM
 from langchain_core.messages import AIMessage, BaseMessage, BaseMessageChunk
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_google_genai import ChatGoogleGenerativeAI
 from langchain_google_genai.chat_models import ChatGoogleGenerativeAIError
 from langchain_mistralai.chat_models import ChatMistralAI
 from langchain_openai import ChatOpenAI
 from langchain_together import Together
 from litellm import token_counter
 
 from notdiamond import settings
+from notdiamond.callbacks import NDLLMBaseCallbackHandler
 from notdiamond.exceptions import ApiError, MissingLLMProviders
 from notdiamond.llms.provider import NDLLMProvider
 from notdiamond.llms.request import amodel_select, model_select, report_latency
 from notdiamond.metrics.metric import NDMetric
 from notdiamond.prompts.prompt import NDChatPromptTemplate, NDPromptTemplate
 from notdiamond.types import NDApiKeyValidator
 
@@ -97,24 +99,39 @@
 
     Defaults to None.
     """
     preference_id: Optional[str]
     """The ID of the router preference that was configured via the Dashboard. Defaults to None."""
 
     tools: Optional[Sequence[Union[Dict[str, Any], Callable]]]
+    """Bind tools to the LLM object. The tools will be passed to the LLM object when invoking it."""
+
+    callbacks: Optional[
+        List[Union[BaseCallbackHandler, NDLLMBaseCallbackHandler]]
+    ]
+    """
+    Callback handler for the LLM object. It will be passed to the LLM object when invoking it.
+    Also has custom NDLLM callbacks:
+    - on_model_select
+    - on_latency_tracking
+    - on_api_error
+    """
 
     def __init__(
         self,
         llm_providers: List[NDLLMProvider],
         api_key: Optional[str] = None,
         default: Optional[Union[NDLLMProvider, int, str]] = None,
         max_model_depth: Optional[int] = None,
         latency_tracking: bool = True,
         preference_weights: Optional[Dict[str, float]] = None,
         preference_id: Optional[str] = None,
+        callbacks: Optional[
+            List[Union[BaseCallbackHandler, NDLLMBaseCallbackHandler]]
+        ] = None,
         **kwargs,
     ) -> None:
         if api_key is None:
             api_key = settings.NOTDIAMOND_API_KEY
         NDApiKeyValidator(api_key=api_key)
 
         if llm_providers is None or len(llm_providers) == 0:
@@ -149,14 +166,15 @@
             api_key=api_key,
             llm_providers=llm_providers,
             default=default,
             max_model_depth=max_model_depth,
             latency_tracking=latency_tracking,
             preference_weights=preference_weights,
             preference_id=preference_id,
+            callbacks=callbacks,
             **kwargs,
         )
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
         address = hex(id(self))  # Gets the memory address of the object
         return f"<{class_name} object at {address}>"
@@ -260,20 +278,23 @@
 
         is_default = False
         if not best_llm:
             best_llm = self.default_llm_provider
             is_default = True
 
             if best_llm is None:
-                raise ApiError(
+                error_message = (
                     "ND couldn't find a suitable model to call."
                     + "To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
                 )
+                self.call_callbacks("on_api_error", error_message)
+                raise ApiError(error_message)
+        self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
-        llm = self._llm_from_provider(best_llm)
+        llm = self._llm_from_provider(best_llm, callbacks=self.callbacks)
 
         if self.tools:
             llm = llm.bind_tools(self.tools)
 
         chain = prompt_template | llm
 
         try:
@@ -308,15 +329,17 @@
                         if llm_provider.provider != "google"
                     ),
                     None,
                 )
 
                 if non_google_llm is not None:
                     best_llm = non_google_llm
-                    llm = self._llm_from_provider(best_llm)
+                    llm = self._llm_from_provider(
+                        best_llm, callbacks=self.callbacks
+                    )
                     chain = prompt_template | llm
 
                     if self.latency_tracking:
                         result = self._invoke_with_latency_tracking(
                             session_id=session_id,
                             chain=chain,
                             llm_provider=best_llm,
@@ -392,20 +415,23 @@
 
         is_default = False
         if not best_llm:
             best_llm = self.default_llm_provider
             is_default = True
 
             if best_llm is None:
-                raise ApiError(
+                error_message = (
                     "ND couldn't find a suitable model to call."
                     + "To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
                 )
+                self.call_callbacks("on_api_error", error_message)
+                raise ApiError(error_message)
+        self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
-        llm = self._llm_from_provider(best_llm)
+        llm = self._llm_from_provider(best_llm, callbacks=self.callbacks)
 
         if self.tools:
             llm = llm.bind_tools(self.tools)
 
         chain = prompt_template | llm
 
         try:
@@ -440,15 +466,17 @@
                         if llm_provider.provider != "google"
                     ),
                     None,
                 )
 
                 if non_google_llm is not None:
                     best_llm = non_google_llm
-                    llm = self._llm_from_provider(best_llm)
+                    llm = self._llm_from_provider(
+                        best_llm, callbacks=self.callbacks
+                    )
                     chain = prompt_template | llm
 
                     if self.latency_tracking:
                         result = (
                             await self._async_invoke_with_latency_tracking(
                                 session_id=session_id,
                                 chain=chain,
@@ -493,24 +521,28 @@
             llm_providers=self.llm_providers,
             metric=NDMetric("accuracy"),
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
         )
+
         if not best_llm:
             best_llm = self.default_llm_provider
 
             if best_llm is None:
-                raise ApiError(
+                error_message = (
                     "ND couldn't find a suitable model to call."
-                    + " To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
+                    + "To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
                 )
+                self.call_callbacks("on_api_error", error_message)
+                raise ApiError(error_message)
+        self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
-        llm = self._llm_from_provider(best_llm)
+        llm = self._llm_from_provider(best_llm, callbacks=self.callbacks)
         if self.tools:
             llm = llm.bind_tools(self.tools)
 
         for chunk in llm.stream(input, **kwargs):
             yield chunk
 
     async def astream(
@@ -538,24 +570,28 @@
             llm_providers=self.llm_providers,
             metric=NDMetric("accuracy"),
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
         )
+
         if not best_llm:
             best_llm = self.default_llm_provider
 
             if best_llm is None:
-                raise ApiError(
+                error_message = (
                     "ND couldn't find a suitable model to call."
-                    + " To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
+                    + "To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
                 )
+                self.call_callbacks("on_api_error", error_message)
+                raise ApiError(error_message)
+        self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
-        llm = self._llm_from_provider(best_llm)
+        llm = self._llm_from_provider(best_llm, callbacks=self.callbacks)
         if self.tools:
             llm = llm.bind_tools(self.tools)
 
         async for chunk in llm.astream(input, **kwargs):
             yield chunk
 
     async def amodel_select(
@@ -609,14 +645,15 @@
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
         )
 
         if not best_llm and self.default is not None:
             print("ND API error. Falling back to default provider.")
             best_llm = self.default_llm_provider
+        self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
         return session_id, best_llm
 
     def model_select(
         self,
         prompt_template: Optional[
             Union[
@@ -666,30 +703,34 @@
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
         )
 
         if not best_llm and self.default is not None:
             print("ND API error. Falling back to default provider.")
             best_llm = self.default_llm_provider
+        self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
         return session_id, best_llm
 
     async def _async_invoke_with_latency_tracking(
         self,
         session_id: str,
         chain: Any,
         llm_provider: NDLLMProvider,
         input: Optional[Dict[str, Any]] = {},
         is_default: bool = True,
         **kwargs,
     ):
         if session_id in ("NO-SESSION-ID", "") and not is_default:
-            raise ApiError(
-                "ND session_id is not valid for latency tracking. Please check the API response."
+            error_message = (
+                "ND session_id is not valid for latency tracking."
+                + "Please check the API response."
             )
+            self.call_callbacks("on_api_error", error_message)
+            raise ApiError(error_message)
 
         start_time = time.time()
 
         result = await chain.ainvoke(input, **kwargs)
 
         end_time = time.time()
 
@@ -704,30 +745,36 @@
 
         report_latency(
             session_id=session_id,
             llm_provider=llm_provider,
             tokens_per_second=tokens_per_second,
             notdiamond_api_key=self.api_key,
         )
+        self.call_callbacks(
+            "on_latency_tracking", session_id, llm_provider, tokens_per_second
+        )
 
         return result
 
     def _invoke_with_latency_tracking(
         self,
         session_id: str,
         chain: Any,
         llm_provider: NDLLMProvider,
         input: Optional[Dict[str, Any]] = {},
         is_default: bool = True,
         **kwargs,
     ):
         if session_id in ("NO-SESSION-ID", "") and not is_default:
-            raise ApiError(
-                "ND session_id is not valid for latency tracking. Please check the API response."
+            error_message = (
+                "ND session_id is not valid for latency tracking."
+                + "Please check the API response."
             )
+            self.call_callbacks("on_api_error", error_message)
+            raise ApiError(error_message)
 
         start_time = time.time()
         result = chain.invoke(input, **kwargs)
         end_time = time.time()
 
         if isinstance(result, str):
             result = AIMessage(content=result)
@@ -740,62 +787,76 @@
 
         report_latency(
             session_id=session_id,
             llm_provider=llm_provider,
             tokens_per_second=tokens_per_second,
             notdiamond_api_key=self.api_key,
         )
+        self.call_callbacks(
+            "on_latency_tracking", session_id, llm_provider, tokens_per_second
+        )
 
         return result
 
     @staticmethod
-    def _llm_from_provider(provider: NDLLMProvider) -> Any:
+    def _llm_from_provider(
+        provider: NDLLMProvider,
+        callbacks: Optional[
+            List[Union[BaseCallbackHandler, NDLLMBaseCallbackHandler]]
+        ],
+    ) -> Any:
         if provider.provider == "openai":
             return ChatOpenAI(
                 openai_api_key=provider.api_key,
                 model_name=provider.model,
+                callbacks=callbacks,
                 **provider.kwargs,
             )
         if provider.provider == "anthropic":
             return ChatAnthropic(
                 anthropic_api_key=provider.api_key,
                 model=provider.model,
+                callbacks=callbacks,
                 **provider.kwargs,
             )
         if provider.provider == "google":
             return ChatGoogleGenerativeAI(
                 google_api_key=provider.api_key,
                 model=provider.model,
                 convert_system_message_to_human=True,
+                callbacks=callbacks,
                 **provider.kwargs,
             )
         if provider.provider == "cohere":
             return ChatCohere(
                 cohere_api_key=provider.api_key,
                 model=provider.model,
+                callbacks=callbacks,
                 **provider.kwargs,
             )
         if provider.provider == "mistral":
             return ChatMistralAI(
                 mistral_api_key=provider.api_key,
                 model=provider.model,
+                callbacks=callbacks,
                 **provider.kwargs,
             )
         if provider.provider == "togetherai":
             provider_settings = settings.PROVIDERS.get(provider.provider, None)
             model_prefixes = provider_settings.get("model_prefix", None)
             model_prefix = model_prefixes.get(provider.model, None)
 
             model = provider.model
             if model_prefix is not None:
                 model = f"{model_prefix}/{provider.model}"
             print(f"MODEL: {model}")
             return Together(
                 together_api_key=provider.api_key,
                 model=model,
+                callbacks=callbacks,
                 **provider.kwargs,
             )
         raise ValueError(f"Unsupported provider: {provider.provider}")
 
     @staticmethod
     def _prepare_prompt_template(
         prompt_template,
@@ -829,7 +890,19 @@
         Bind tools to the LLM object. The tools will be passed to the LLM object when invoking it.
         Results in the tools being available in the LLM object.
         You can access the tool_calls in the result via `result.tool_calls`.
         """
         self.tools = tools
 
         return self
+
+    def call_callbacks(self, function_name: str, *args, **kwargs) -> None:
+        """
+        Call all callbacks with a specific function name.
+        """
+
+        if self.callbacks is None:
+            return
+
+        for callback in self.callbacks:
+            if hasattr(callback, function_name):
+                getattr(callback, function_name)(*args, **kwargs)
```

### Comparing `notdiamond-0.1.5b0/notdiamond/llms/provider.py` & `notdiamond-0.1.6b0/notdiamond/llms/provider.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.5b0/notdiamond/llms/providers.py` & `notdiamond-0.1.6b0/notdiamond/llms/providers.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.5b0/notdiamond/llms/request.py` & `notdiamond-0.1.6b0/notdiamond/llms/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import aiohttp
 import requests
 
 from notdiamond import settings
 from notdiamond.llms.provider import NDLLMProvider
 from notdiamond.metrics.metric import NDMetric
-from notdiamond.prompts.hash import nd_hash
 from notdiamond.prompts.prompt import NDChatPromptTemplate, NDPromptTemplate
 from notdiamond.types import ModelSelectRequestPayload
 
 
 def model_select_prepare(
     prompt_template: Optional[Union[NDPromptTemplate, NDChatPromptTemplate]],
     llm_providers: List[NDLLMProvider],
@@ -37,20 +36,19 @@
                                                     Defaults to None.
         async_mode (bool, optional): whether to run the request in async mode. Defaults to False.
 
     Returns:
         tuple(url, payload, headers): returns data to be used for the API call of modelSelect
     """
 
-    url = f"{settings.ND_BASE_URL}/v1/optimizer/modelSelect"
+    url = f"{settings.ND_BASE_URL}/v2/optimizer/modelSelect"
 
     payload: ModelSelectRequestPayload = {
-        "prompt_template": prompt_template.template,
-        "formatted_prompt": nd_hash(prompt_template.format()),
-        "components": prompt_template.prepare_for_request(),
+        "messages": prompt_template.prepare_for_request(),
+        "hash_digest": prompt_template.get_hash_digest(),
         "llm_providers": [
             llm_provider.prepare_for_request()
             for llm_provider in llm_providers
         ],
         "metric": metric.metric,
         "max_model_depth": max_model_depth,
     }
```

### Comparing `notdiamond-0.1.5b0/notdiamond/metrics/metric.py` & `notdiamond-0.1.6b0/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.5b0/notdiamond/metrics/request.py` & `notdiamond-0.1.6b0/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.5b0/notdiamond/settings.py` & `notdiamond-0.1.6b0/notdiamond/settings.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.5b0/notdiamond/types.py` & `notdiamond-0.1.6b0/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.5b0/pyproject.toml` & `notdiamond-0.1.6b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.5-beta"
+version = "0.1.6-beta"
 description = "Not Diamond Python Library"
 authors = ["Not Diamond <t5@notdiamond.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 langchain = ">=0.1.16"
```

### Comparing `notdiamond-0.1.5b0/PKG-INFO` & `notdiamond-0.1.6b0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.5b0
+Version: 0.1.6b0
 Summary: Not Diamond Python Library
 Author: Not Diamond
 Author-email: t5@notdiamond.ai
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,39 +24,55 @@
 Requires-Dist: ppdeep (>=20200505,<20200506)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: together (>=0.2.11,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Getting started with Not Diamond
 
-Not Diamond automatically determines which model is best-suited to respond to any query. Unlike any other model router, Not Diamond is **fully privacy-preserving** and **continuously adapts to your preferences**.
+Not Diamond automatically determines which model is best-suited to respond to any query, **drastically improving LLM output quality** while reducing costs and latency and avoiding vendor lock-in. Unlike any other model router, Not Diamond is **100% privacy-preserving** and **continuously adapts to your preferences** ([demo video](https://www.loom.com/share/6e5dee9d99434de6bafbcd96ff5d663c?sid=d771348d-e9e5-49f9-9f21-6310d12541ec)).
+
+# Installation
+
+Requires **Python 3.9+**
+
+```bash
+pip install notdiamond
+```
+
+If your application isn't in Python, you can directly call our [REST API endpoint](https://notdiamond.readme.io/v0.1.0-beta/reference).
 
 # Key features
 
-- **Maintain privacy**: All inputs are [fuzzy hashed](https://en.wikipedia.org/wiki/Fuzzy_hashing) before being sent to the Not Diamond API. We return a label for the recommended model and LLM calls go out client-side. _This means we never see your raw query strings or response outputs._
-- **Maximize performance**: Not Diamond [outperforms foundation models](https://notdiamond.readme.io/v0.1.0-beta/docs/how-not-diamond-works#not-diamond-vs-claude-3-opus) out of the box. Our cold-start recommendations are based on hundreds of thousands of data points from rigorous evaluation benchmarks and real-world data.
+- **Maintain privacy**: All inputs are [fuzzy hashed](https://en.wikipedia.org/wiki/Fuzzy_hashing) before being sent to the Not Diamond API. We return a label for the recommended model and LLM calls go out client-side. _This means we never see your raw query strings or your response outputs._
+- **Maximize performance**: Not Diamond [outperforms Claude 3 Opus](https://notdiamond.readme.io/v0.1.0-beta/docs/how-not-diamond-works#not-diamond-vs-claude-3-opus) on major evaluation benchmarks. Our cold-start recommendations are based on hundreds of thousands of data points from rigorous evaluation benchmarks and real-world data.
 - **Continuously improve**: By [providing feedback on routing decisions](https://notdiamond.readme.io/v0.1.0-beta/docs/personalization), Not Diamond _continuously learns_ a hyper-personalized routing algorithm optimized to your preferences and your application's requirements.
-- **Reduce cost and latency**: Define explicit quality, cost, and latency tradeoffs to cut down your inference costs and achieve blazing fast speeds. Not Diamond determines which model to call in under 40ms—less than the time it takes an LLM to stream a single token.
+- **Reduce cost and latency**: Define explicit [quality, cost, and latency tradeoffs](https://notdiamond.readme.io/v0.1.0-beta/docs/personalization#quality-cost-and-latency-tradeoffs) to cut down your inference costs and achieve blazing fast speeds. Not Diamond determines which model to call in under 40ms—less than the time it takes an LLM to stream a single token.
+
+# Not Diamond vs. Claude 3 Opus
+
+These are preliminary results and require further validation, but initial evaluations show that Not Diamond outperforms Claude 3 Opus on major benchmarks:
+
+| Dataset        | Claude 3 Opus | Not Diamond |
+| :------------- | :------------ | :---------- |
+| MMLU           | 85.21         | **88.25**   |
+| BIG-Bench-Hard | 81.06         | **81.24**   |
+| ARC-Challenge  | 93.56         | **95.59**   |
+| WinoGrande     | 76.80         | **79.60**   |
+| MBPP           | 47.40         | **69.05**   |
+
+As can be seen with the MBPP benchmark, the biggest gains emerge when Claude 3 Opus scores particularly low on a benchmark. More testing is required however and we will be releasing a full technical report soon.
 
 > 🚧 Beta testing ahead
 >
 > Not Diamond is still in beta! Please let us know if you have any feedback or ideas on how we can improve. Tomás is at [t5@notdiamond.ai](mailto:t5@notdiamond.ai) or 917 725 2192.
 
 > 👍 Free to use!
 >
 > Not Diamond is 100% free to use during beta ♡
 
-# Installation
-
-Requires **Python 3.9+**
-
-```shell
-pip install notdiamond
-```
-
 # API keys
 
 > 👍 [Sign up](https://app.notdiamond.ai/) and get a Not Diamond API key.
 
 Create a `.env` file with your Not Diamond API key, and the API keys of the models you want to route between.
 
 ```shell
@@ -82,30 +98,27 @@
 
 Create a `main.py` file in the same folder as the [`.env`](#api-keys) file you created earlier, or **[try it in Colab](https://colab.research.google.com/drive/1Ao-YhYF_S6QP5UGp_kYhgKps_Sw3a2RO?usp=sharing).**
 
 ```python
 from notdiamond.llms.llm import NDLLM
 from notdiamond.prompts.prompt import NDPromptTemplate
 
-
-# Define the prompt template -> the string that will be routed to the best LLM
+# Define the template object -> the string that will be routed to the best LLM
 prompt_template = NDPromptTemplate("Write a merge sort in Python.")
 
 # Define the available LLMs you'd like to route between
 llm_providers = ['openai/gpt-3.5-turbo', 'openai/gpt-4','openai/gpt-4-1106-preview', 'openai/gpt-4-turbo-preview',
-                 'anthropic/claude-2.1', 'anthropic/claude-3-sonnet-20240229', 'anthropic/claude-3-opus-20240229',
-                 'google/gemini-pro']
+                 'anthropic/claude-3-haiku-20240307', 'anthropic/claude-3-sonnet-20240229', 'anthropic/claude-3-opus-20240229']
 
 # Create the NDLLM object -> like a 'meta-LLM' combining all of the specified models
 nd_llm = NDLLM(llm_providers=llm_providers)
 
 # After fuzzy hashing the inputs, the best LLM is determined by the ND API and the LLM is called client-side
 result, session_id, provider = nd_llm.invoke(prompt_template=prompt_template)
 
-
 print("ND session ID: ", session_id)  # A unique ID of the invoke. Important for personalizing ND to your use-case
 print("LLM called: ", provider.model)  # The LLM routed to
 print("LLM output: ", result.content)  # The LLM response
 ```
 
 > 👍 **Run it!**
 >
```

