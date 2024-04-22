# Comparing `tmp/basicbedrock-0.1.3.tar.gz` & `tmp/basicbedrock-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.1.3.tar", last modified: Thu Apr 11 01:10:19 2024, max compression
+gzip compressed data, was "basicbedrock-0.1.4.tar", last modified: Mon Apr 22 22:01:59 2024, max compression
```

## Comparing `basicbedrock-0.1.3.tar` & `basicbedrock-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:10:19.260425 basicbedrock-0.1.3/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.3/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 01:10:19.260190 basicbedrock-0.1.3/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-11 01:09:42.000000 basicbedrock-0.1.3/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-11 01:10:19.260476 basicbedrock-0.1.3/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:10:19.254930 basicbedrock-0.1.3/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:10:19.256042 basicbedrock-0.1.3/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-11 01:09:42.000000 basicbedrock-0.1.3/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    16041 2024-04-11 01:08:56.000000 basicbedrock-0.1.3/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:10:19.258963 basicbedrock-0.1.3/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3008 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3659 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/ai21.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     6036 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     7095 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4710 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3221 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2864 2024-04-11 00:27:04.000000 basicbedrock-0.1.3/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:10:19.259921 basicbedrock-0.1.3/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 01:10:19.000000 basicbedrock-0.1.3/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-11 01:10:19.000000 basicbedrock-0.1.3/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-11 01:10:19.000000 basicbedrock-0.1.3/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-11 01:10:19.000000 basicbedrock-0.1.3/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-11 01:10:19.000000 basicbedrock-0.1.3/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:10:19.259213 basicbedrock-0.1.3/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.3/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.015299 basicbedrock-0.1.4/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.4/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-22 22:01:59.015028 basicbedrock-0.1.4/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.4/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-22 22:01:13.000000 basicbedrock-0.1.4/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-22 22:01:59.015427 basicbedrock-0.1.4/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.010460 basicbedrock-0.1.4/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.011499 basicbedrock-0.1.4/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-22 22:01:13.000000 basicbedrock-0.1.4/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    16155 2024-04-11 01:17:00.000000 basicbedrock-0.1.4/src/basicbedrock/basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.013926 basicbedrock-0.1.4/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2984 2024-04-22 22:00:00.000000 basicbedrock-0.1.4/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.4/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.4/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.4/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.4/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.4/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2315 2024-04-22 21:52:22.000000 basicbedrock-0.1.4/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.4/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.014725 basicbedrock-0.1.4/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-22 22:01:59.000000 basicbedrock-0.1.4/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-22 22:01:59.014086 basicbedrock-0.1.4/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.4/test/tests.py
```

### Comparing `basicbedrock-0.1.3/LICENSE` & `basicbedrock-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.3/PKG-INFO` & `basicbedrock-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.3
+Version: 0.1.4
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.3/README.md` & `basicbedrock-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.3/pyproject.toml` & `basicbedrock-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
```

### Comparing `basicbedrock-0.1.3/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.1.4/src/basicbedrock/basicbedrock.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,16 +295,18 @@
     @top_p.setter
     def top_p(self, top_p: float):
         """
         sets the top_p parameter
         :param top_p:
         :return:
         """
-        if not (0 < top_p <= 1) or not isinstance(top_p, float):
-            raise ValueError(f"top_p value must be between 0 and 1, but got {top_p}")
+        if not isinstance(top_p, float) or isinstance(top_p, int):
+            raise ValueError(f"top_p value must be a float, but got {type(top_p)}")
+        if not (0 <= top_p <= 1):
+            raise ValueError(f"top_p value must be between 0 and 1 inclusive, but got {top_p}")
         self._p = top_p
 
     @top_p.deleter
     def top_p(self):
         """
         resets the top_p parameter
         :return:
@@ -324,16 +326,16 @@
         """
         sets the top_k parameter
         :param k:
         :return:
         """
         if not isinstance(k, int):
             raise ValueError(f"top_k value must be an int, but got {type(k)}")
-        if k < 1 or not isinstance(k, int):
-            raise ValueError(f"top_k value must be positive and an integer, but got {top_k}")
+        if k < 1:
+            raise ValueError(f"top_k value must be positive, but got {top_k}")
         self._k = k
 
     @top_k.deleter
     def top_k(self):
         """
         resets the top_k parameter
         :return:
@@ -351,15 +353,15 @@
     @temp.setter
     def temp(self, temp: float):
         """
         sets the temp parameter
         :param temp:
         :return:
         """
-        if not isinstance(temp, float):
+        if not isinstance(temp, float) or isinstance(temp, int):
             raise ValueError(f"temp value must be float but got {type(temp)}")
         if not (0 <= temp <= 1) or not isinstance(temp, float):
             raise ValueError(f"temp value must be between 0 and 1, but got {temp}")
         self._t = temp
 
     @temp.deleter
     def temp(self):
```

### Comparing `basicbedrock-0.1.3/src/basicbedrock/models/__init__.py` & `basicbedrock-0.1.4/src/basicbedrock/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,49 +10,51 @@
 from .anthropic import *
 from .baseclasses import BaseAbstractRequest
 from .cohere import *
 from .meta import *
 from .mistral import *
 
 model_request_mapping = {
-    "ai21.j2-ultra-v1": AI21Jurassic2UltraV1Request,
-    "ai21.j2-mid-v1": AI21Jurassic2MidV1Request,
+    "ai21.j2-ultra-v1": AI21Jurassic2BaseRequest,
+    "ai21.j2-mid-v1": AI21Jurassic2BaseRequest,
     "amazon.titan-embed-text-v1": AmazonTitanEmbedTextV1Request,
-    "amazon.titan-text-lite-v1": AmazonTitanTextLiteV1Request,
-    "amazon.titan-text-express-v1": AmazonTitanTextExpressV1Request,
-    "anthropic.claude-instant-v1": AnthropicClaudeInstantV1Request,
-    "anthropic.claude-v2": AnthropicClaudeV2Request,
-    "anthropic.claude-v2:1": AnthropicClaudeV2_1Request,
-    "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3Sonnet20240229V1_0Request,
-    "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3Haiku20240307V1_0Request,
-    "cohere.command-text-v14": CohereCommandTextV14Request,
-    "cohere.command-light-text-v14": CohereCommandLightTextV14Request,
-    "cohere.embed-english-v3": CohereEmbedEnglishV3Request,
-    "cohere.embed-multilingual-v3": CohereEmbedMultilingualV3Request,
-    "meta.llama2-13b-chat-v1": MetaLlama213bChatV1Request,
-    "meta.llama2-70b-chat-v1": MetaLlama270bChatV1Request,
-    "mistral.mistral-7b-instruct-v0:2": MistralMistral7bInstructV0_2Request,
-    "mistral.mixtral-8x7b-instruct-v0:1": MistralMistral8x7bInstructV0_1Request,
-    "mistral.mistral-large-2402-v1:0": MistralMistralLarge2402V1_0Request
+    "amazon.titan-text-lite-v1": AmazonTitanTextV1Request,
+    "amazon.titan-text-express-v1": AmazonTitanTextV1Request,
+    "anthropic.claude-instant-v1": AnthropicClaudeV1V2BaseRequest,
+    "anthropic.claude-v2": AnthropicClaudeV1V2BaseRequest,
+    "anthropic.claude-v2:1": AnthropicClaudeV1V2BaseRequest,
+    "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3BaseRequest,
+    "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3BaseRequest,
+    #  unavailable "anthropic.claude-3-opus-20240229-v1:0":AnthropicClaude3BaseRequest,
+    "cohere.command-text-v14": CohereCommandTextBaseRequest,
+    "cohere.command-light-text-v14": CohereCommandTextBaseRequest,
+    "cohere.embed-english-v3": CohereEmbedBaseRequest,
+    "cohere.embed-multilingual-v3": CohereEmbedBaseRequest,
+    "meta.llama2-13b-chat-v1": MetaLlama2ChatV1BaseRequest,
+    "meta.llama2-70b-chat-v1": MetaLlama2ChatV1BaseRequest,
+    "mistral.mistral-7b-instruct-v0:2": MistralBaseRequest,
+    "mistral.mixtral-8x7b-instruct-v0:1": MistralBaseRequest,
+    "mistral.mistral-large-2402-v1:0": MistralBaseRequest
 }
 
 model_response_mapping = {
-    "ai21.j2-ultra-v1": AI21Jurassic2UltraV1Response,
-    "ai21.j2-mid-v1": AI21Jurassic2MidV1Response,
+    "ai21.j2-ultra-v1": AI21Jurassic2BaseResponse,
+    "ai21.j2-mid-v1": AI21Jurassic2BaseResponse,
     "amazon.titan-embed-text-v1": AmazonTitanEmbedTextV1Response,
-    "amazon.titan-text-lite-v1": AmazonTitanTextLiteV1Response,
-    "amazon.titan-text-express-v1": AmazonTitanTextExpressV1Response,
-    "anthropic.claude-instant-v1": AnthropicClaudeInstantV1Response,
-    "anthropic.claude-v2": AnthropicClaudeV2Response,
-    "anthropic.claude-v2:1": AnthropicClaudeV2_1Response,
-    "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3Sonnet20240229V1_0Response,
-    "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3Haiku20240307V1_0Response,
-    "cohere.command-text-v14": CohereCommandTextV14Response,
-    "cohere.command-light-text-v14": CohereCommandLightTextV14Response,
-    "cohere.embed-english-v3": CohereEmbedEnglishV3Response,
-    "cohere.embed-multilingual-v3": CohereEmbedMultilingualV3Response,
-    "meta.llama2-13b-chat-v1": MetaLlama213bChatV1Response,
-    "meta.llama2-70b-chat-v1": MetaLlama270bChatV1Response,
-    "mistral.mistral-7b-instruct-v0:2": MistralMistral7bInstructV0_2Response,
-    "mistral.mixtral-8x7b-instruct-v0:1": MistralMistral8x7bInstructV0_1Response,
-    "mistral.mistral-large-2402-v1:0": MistralMistralLarge2402V1_0Response
+    "amazon.titan-text-lite-v1": AmazonTitanTextV1Response,
+    "amazon.titan-text-express-v1": AmazonTitanTextV1Response,
+    "anthropic.claude-instant-v1": AnthropicClaudeV1V2BaseResponse,
+    "anthropic.claude-v2": AnthropicClaudeV1V2BaseResponse,
+    "anthropic.claude-v2:1": AnthropicClaudeV1V2BaseResponse,
+    "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3BaseResponse,
+    "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3BaseResponse,
+    #  unavailable "anthropic.claude-3-opus-20240229-v1:0": AnthropicClaude3BaseResponse,
+    "cohere.command-text-v14": CohereCommandTextBaseResponse,
+    "cohere.command-light-text-v14": CohereCommandTextBaseResponse,
+    "cohere.embed-english-v3": CohereEmbedBaseResponse,
+    "cohere.embed-multilingual-v3": CohereEmbedBaseResponse,
+    "meta.llama2-13b-chat-v1": MetaLlama2ChatV1BaseResponse,
+    "meta.llama2-70b-chat-v1": MetaLlama2ChatV1BaseResponse,
+    "mistral.mistral-7b-instruct-v0:2": MistralBaseResponse,
+    "mistral.mixtral-8x7b-instruct-v0:1": MistralBaseResponse,
+    "mistral.mistral-large-2402-v1:0": MistralBaseResponse
 }
```

### Comparing `basicbedrock-0.1.3/src/basicbedrock/models/ai21.py` & `basicbedrock-0.1.4/src/basicbedrock/models/ai21.py`

 * *Files 22% similar despite different names*

```diff
@@ -82,46 +82,15 @@
         set the maximum tokens parameter.
         :param max_tokens:
         :return:
         """
         self.maxTokens = max_tokens
 
 
-class AI21Jurassic2UltraV1Request(AI21Jurassic2BaseRequest):
-    """
-    Request format for  AI21 Jurassic 2 Ultra request.
-    this model supports max_token, temperature and top_p.
-    It does not support top_k
-    This class is implemented in AI21Jurassic2BaseRequest.
-    """
-
-
-class AI21Jurassic2MidV1Request(AI21Jurassic2BaseRequest):
-    """
-    Request format for AI21 Jurassic 2 Mid request.
-    this model supports max_token, temperature and top_p.
-    It does not support top_k
-    This class is implemented in MetaLlama2ChatV1BaseRequest.
-    """
-
-
 class AI21Jurassic2BaseResponse(BaseAbstractResponse):
     """
     All AI21 Jurassic 2 models use the same response format.
     """
 
     def get_answer(self) -> List[float]:
         return self.result_raw['completions'][0]['data']['text']
 
-
-class AI21Jurassic2UltraV1Response(AI21Jurassic2BaseResponse):
-    """
-    Response format for AI21 Jurassic 2 Ultra response.
-    It is implemented in AI21Jurassic2BaseResponse
-    """
-
-
-class AI21Jurassic2MidV1Response(AI21Jurassic2BaseResponse):
-    """
-    Response format for AI21 Jurassic 2 Mid response.
-    It is implemented in AI21Jurassic2BaseResponse
-    """
```

### Comparing `basicbedrock-0.1.3/src/basicbedrock/models/amazon.py` & `basicbedrock-0.1.4/src/basicbedrock/models/amazon.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     maxTokenCount: int = 250
     stopSequences: List[Optional[str]] = []
     temperature: float = 0.5
     topP: float = 0.5
 
 
-class AmazonTitanBaseModelRequest(BaseAbstractRequest):
+class AmazonTitanTextV1Request(BaseAbstractRequest):
     """
     All current Amazon Titan family models use the same request schema.
     This base class is used by both Amazon Titan Text G1 Express and Titan Text v1 Lite
     This model does not support top_k parameter.
     """
     inputText: str = "{PROMPT}"
     textGenerationConfig: AmazonTitanTextGenerationConfig = AmazonTitanTextGenerationConfig()
@@ -88,56 +88,24 @@
         Sets top p of Amazon Titan model family
         :param top_p: float
         :return:
         """
         self.textGenerationConfig.topP = top_p
 
 
-class AmazonTitanTextExpressV1Request(AmazonTitanBaseModelRequest):
-    """
-    Request structure for Amazon Titan Text Express V1 API.
-    This model accepts text and returns text.
-    This model does not support K parameter.
-
-    Please see AmazonTitanBaseModelRequest for the implementation of all methods
-    """
-
-
-class AmazonTitanTextLiteV1Request(AmazonTitanBaseModelRequest):
-    """
-    Request structure for Amazon Titan Text Lite V1 API
-    This model accepts text and returns text.
-    This model does not support K parameter.
-
-    Please see AmazonTitanBaseModelRequest for the implementation of all methods
-    """
-
 
 class AmazonTitanTextV1Response(BaseAbstractResponse):
     """
     Response structure for Amazon Titan Text V1 API both Express and Lite
     """
 
     def get_answer(self) -> List[float]:
         return self.result_raw['results'][0]['outputText']
 
 
-class AmazonTitanTextExpressV1Response(AmazonTitanTextV1Response):
-    """
-    Response structure for Amazon Titan Text Express V1 API.
-    Implemented in AmazonTitanTextV1Response
-    """
-
-
-class AmazonTitanTextLiteV1Response(AmazonTitanTextV1Response):
-    """
-    Response structure for Amazon Titan Text Lite V1 API.
-    Implemented in AmazonTitanTextV1Response
-    """
-
 
 class AmazonTitanEmbedTextV1Request(BaseAbstractRequest):
     """
     Request structure for Amazon Titan Embedding V1 API
     This model accepts text and returns a list of floats, representing Amazon Titan embedding vectors.
     """
     inputText: str = "{PROMPT}"
```

### Comparing `basicbedrock-0.1.3/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.1.4/src/basicbedrock/models/baseclasses.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.3/src/basicbedrock/models/meta.py` & `basicbedrock-0.1.4/src/basicbedrock/models/meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -76,46 +76,16 @@
         set the maximum tokens parameter.
         :param max_tokens:
         :return:
         """
         self.max_gen_len = max_tokens
 
 
-class MetaLlama213bChatV1Request(MetaLlama2ChatV1BaseRequest):
-    """
-    Request format for Meta Llama 2 13b chat.
-    this model supports max_token, temperature and top_p.
-    It does not support top_k
-    This class is implemented in MetaLlama2ChatV1BaseRequest.
-    """
-
-
-class MetaLlama270bChatV1Request(MetaLlama2ChatV1BaseRequest):
-    """
-    Request format for Meta Llama 2 70b chat.
-    this model supports max_token, temperature and top_p.
-    It does not support top_k
-    This class is implemented in MetaLlama2ChatV1BaseRequest.
-    """
-
-
-class MetaLlama2V1BaseResponse(BaseAbstractResponse):
+class MetaLlama2ChatV1BaseResponse(BaseAbstractResponse):
     """
     Response format of Meta Llama 2 V1 family chat response.
     """
 
     def get_answer(self) -> str:
         return self.result_raw['generation']
 
 
-class MetaLlama213bChatV1Response(MetaLlama2V1BaseResponse):
-    """
-    Response format of Meta Llama 2 13b chat response.
-    Implemented in MetaLlama2V1BaseResponse.
-    """
-
-
-class MetaLlama270bChatV1Response(MetaLlama2V1BaseResponse):
-    """
-    Response format of Meta Llama 2 70b chat response.
-    Implemented in MetaLlama2V1BaseResponse.
-    """
```

### Comparing `basicbedrock-0.1.3/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.1.4/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.3
+Version: 0.1.4
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.3/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.1.4/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.3/test/tests.py` & `basicbedrock-0.1.4/test/tests.py`

 * *Files identical despite different names*

