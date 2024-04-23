# Comparing `tmp/doctran_openai-0.0.1.tar.gz` & `tmp/doctran_openai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran_openai-0.0.1.tar", max compression
+gzip compressed data, was "doctran_openai-0.0.2.tar", max compression
```

## Comparing `doctran_openai-0.0.1.tar` & `doctran_openai-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.1/LICENSE
--rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.1/README.md
--rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.1/doctran_openai/__init__.py
--rw-r--r--   0        0        0     9117 2024-04-23 03:01:41.032045 doctran_openai-0.0.1/doctran_openai/doctran_openai.py
--rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.1/doctran_openai/transformers/__init__.py
--rw-r--r--   0        0        0    15480 2024-04-23 03:01:49.279092 doctran_openai-0.0.1/doctran_openai/transformers/transformers.py
--rw-r--r--   0        0        0      550 2024-04-23 04:57:01.976321 doctran_openai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.2/README.md
+-rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.2/doctran_openai/__init__.py
+-rw-r--r--   0        0        0     9117 2024-04-23 03:01:41.032045 doctran_openai-0.0.2/doctran_openai/doctran_openai.py
+-rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.2/doctran_openai/transformers/__init__.py
+-rw-r--r--   0        0        0    15953 2024-04-23 05:05:55.006326 doctran_openai-0.0.2/doctran_openai/transformers/transformers.py
+-rw-r--r--   0        0        0      550 2024-04-23 05:07:06.569953 doctran_openai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.2/PKG-INFO
```

### Comparing `doctran_openai-0.0.1/LICENSE` & `doctran_openai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.1/README.md` & `doctran_openai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.1/doctran_openai/doctran_openai.py` & `doctran_openai-0.0.2/doctran_openai/doctran_openai.py`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.1/doctran_openai/transformers/transformers.py` & `doctran_openai-0.0.2/doctran_openai/transformers/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,29 +60,37 @@
             print(e)
             return document
         return self.executeOpenAICall(document)
 
     def executeOpenAICall(self, document: Document) -> Document:
         try:
             function_call = OpenAIFunctionCall(
-                seed=self.config.openai_deployment_id,
+                # seed=self.config.openai_deployment_id,
                 model=self.config.openai_model,
                 messages=[{"role": "user", "content": document.transformed_content}],
-                tools=[{
-                    "type": "function",
-                    "function": {
-                        "name": self.function_name,
-                        "description": self.function_description,
-                        "parameters": self.function_parameters,
-                    }
+                functions=[{
+                    "name": self.function_name,
+                    "description": self.function_description,
+                    "parameters": self.function_parameters,
                 }],
-                tool_choice={"type": "function", "function": {"name": self.function_name}}
+                function_call={"name": self.function_name},
+                # tools=[{
+                #     "type": "function",
+                #     "function": {
+                #         "name": self.function_name,
+                #         "description": self.function_description,
+                #         "parameters": self.function_parameters,
+                #     }
+                # }],
+                # tool_choice={"type": "function", "function": {"name": self.function_name}}
             )
+            # completion = self.config.openai.chat.completions.create(**function_call.dict())
+            # arguments = completion.choices[0].message.tool_calls[0].function.arguments
             completion = self.config.openai.chat.completions.create(**function_call.dict())
-            arguments = completion.choices[0].message.tool_calls[0].function.arguments
+            arguments = completion.choices[0].message.function_call.arguments
             try:
                 arguments = json.loads(arguments)
             except Exception as e:
                 raise Exception("OpenAI returned malformatted JSON" +
                                 "This is likely due to the completion running out of tokens. " +
                                 f"Setting a higher token limit may fix this error. JSON returned: {arguments}")
             first_value = next(iter(arguments.values()))
```

### Comparing `doctran_openai-0.0.1/pyproject.toml` & `doctran_openai-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran_openai"
-version = "0.0.1"
+version = "0.0.2"
 description = "Document transformation framework for vector based retrieval"
 authors = ["William Yang <yangfei86@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 pydantic = "^1.10.9"
```

### Comparing `doctran_openai-0.0.1/PKG-INFO` & `doctran_openai-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doctran_openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Document transformation framework for vector based retrieval
 Author: William Yang
 Author-email: yangfei86@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.1 Summary: Document
+Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.2 Summary: Document
 transformation framework for vector based retrieval Author: William Yang
 Author-email: yangfei86@gmail.com Requires-Python: >=3.10.0,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=1.23.2,<2.0.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
```

