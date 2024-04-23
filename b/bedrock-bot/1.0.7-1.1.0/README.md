# Comparing `tmp/bedrock_bot-1.0.7.tar.gz` & `tmp/bedrock_bot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.0.7.tar", max compression
+gzip compressed data, was "bedrock_bot-1.1.0.tar", max compression
```

## Comparing `bedrock_bot-1.0.7.tar` & `bedrock_bot-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/README.md
--rw-r--r--   0        0        0       91 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     2817 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/cli.py
--rw-r--r--   0        0        0     3173 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/model.py
--rw-r--r--   0        0        0      175 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-23 00:36:06.049515 bedrock_bot-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-23 02:19:22.616756 bedrock_bot-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-23 02:19:22.616756 bedrock_bot-1.1.0/README.md
+-rw-r--r--   0        0        0      119 2024-04-23 02:19:22.616756 bedrock_bot-1.1.0/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     3531 2024-04-23 02:19:22.616756 bedrock_bot-1.1.0/bedrock_bot/cli.py
+-rw-r--r--   0        0        0     4559 2024-04-23 02:19:22.616756 bedrock_bot-1.1.0/bedrock_bot/model.py
+-rw-r--r--   0        0        0      175 2024-04-23 02:19:22.616756 bedrock_bot-1.1.0/bedrock_bot/util.py
+-rw-r--r--   0        0        0      448 2024-04-23 02:19:22.616756 bedrock_bot-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.1.0/PKG-INFO
```

### Comparing `bedrock_bot-1.0.7/LICENSE` & `bedrock_bot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.7/README.md` & `bedrock_bot-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.7/bedrock_bot/model.py` & `bedrock_bot-1.1.0/bedrock_bot/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
+import logging
 from enum import Enum
 
 import boto3
 from botocore.config import Config
 from rich.console import Console
 
+logger = logging.getLogger()
+
 console = Console()
 
 
 class ConversationRole(Enum):
     USER = "user"
     ASSISTANT = "assistant"
 
@@ -45,46 +48,58 @@
         self.messages = []
 
     def append_message(self, role: ConversationRole, message: str):
         self.messages.append({"role": role.value, "content": message})
 
     def invoke(self, message: str):
         self.append_message(ConversationRole.USER, message)
+
+        logger.info(f"Sending current messages to AI: {self.messages}")
         response = self._invoke()
         self.append_message(ConversationRole.ASSISTANT, response)
         return response
 
     def _create_invoke_body(self) -> dict:
-        body = {
-            "messages": self.messages,
-        }
+        raise NotImplementedError
 
-        return body
+    def _handle_response(self, body) -> str:
+        raise NotImplementedError
 
     def _invoke(self):
         body = self._create_invoke_body() | self._model_params
 
         with console.status("[bold green]Waiting for response..."):
             response = self._bedrock.invoke_model(
                 modelId=self._model_id, body=json.dumps(body)
             )
             body = json.loads(response["body"].read())
-            response_message = body["content"][0]
 
-            if response_message["type"] != "text":
-                raise RuntimeError(
-                    "Unexpected response type to prompt: " + response_message["type"]
-                )
-
-            output = response_message["text"]
+            output = self._handle_response(body)
 
         return output
 
 
 class _Claude3(_BedrockModel):
+    def _create_invoke_body(self) -> dict:
+        body = {
+            "messages": self.messages,
+        }
+
+        return body
+
+    def _handle_response(self, body) -> str:
+        response_message = body["content"][0]
+
+        if response_message["type"] != "text":
+            raise RuntimeError(
+                "Unexpected response type to prompt: " + response_message["type"]
+            )
+
+        return response_message["text"]
+
     def __init__(self, model_id: str, boto_config=None):
         self._model_params = {
             "max_tokens": 2000,
             "temperature": 1,
             "top_k": 250,
             "top_p": 0.999,
             "stop_sequences": ["\n\nHuman:"],
@@ -111,7 +126,42 @@
     name = "Claude-3-Haiku"
 
     def __init__(self, boto_config=None):
         super().__init__(
             model_id="anthropic.claude-3-haiku-20240307-v1:0",
             boto_config=boto_config,
         )
+
+
+class MistralLarge(_BedrockModel):
+    name = "Mistral-Large"
+
+    def __init__(self, boto_config=None):
+        self._model_params = {
+            "max_tokens": 200,
+            "temperature": 0.5,
+            "top_p": 0.9,
+            "top_k": 50,
+        }
+        super().__init__(
+            model_id="mistral.mistral-large-2402-v1:0", boto_config=boto_config
+        )
+
+    def _format_messages(self):
+        formatted_messages = ["<s>[INST]"]
+        for message in self.messages:
+            role = message["role"]
+            content = message["content"]
+            formatted_message = f"{role}: {content}"
+            formatted_messages.append(formatted_message)
+        formatted_messages.append("[/INST]")
+        return "\n".join(formatted_messages)
+
+    def _create_invoke_body(self) -> dict:
+        prompt = self._format_messages()
+        body = {"prompt": prompt}
+        return body
+
+    def _handle_response(self, body) -> str:
+        response_message = body["outputs"][0]
+
+        return response_message["text"]
```

### Comparing `bedrock_bot-1.0.7/PKG-INFO` & `bedrock_bot-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.0.7
+Version: 1.1.0
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

