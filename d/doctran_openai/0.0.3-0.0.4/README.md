# Comparing `tmp/doctran_openai-0.0.3.tar.gz` & `tmp/doctran_openai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran_openai-0.0.3.tar", max compression
+gzip compressed data, was "doctran_openai-0.0.4.tar", max compression
```

## Comparing `doctran_openai-0.0.3.tar` & `doctran_openai-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.3/LICENSE
--rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.3/README.md
--rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.3/doctran_openai/__init__.py
--rw-r--r--   0        0        0     9117 2024-04-23 03:01:41.032045 doctran_openai-0.0.3/doctran_openai/doctran_openai.py
--rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.3/doctran_openai/transformers/__init__.py
--rw-r--r--   0        0        0    15960 2024-04-23 05:12:48.919822 doctran_openai-0.0.3/doctran_openai/transformers/transformers.py
--rw-r--r--   0        0        0      550 2024-04-23 05:13:18.655151 doctran_openai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.4/README.md
+-rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.4/doctran_openai/__init__.py
+-rw-r--r--   0        0        0     8323 2024-04-23 05:23:04.044400 doctran_openai-0.0.4/doctran_openai/doctran_openai.py
+-rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.4/doctran_openai/transformers/__init__.py
+-rw-r--r--   0        0        0    15260 2024-04-23 05:24:50.304996 doctran_openai-0.0.4/doctran_openai/transformers/transformers.py
+-rw-r--r--   0        0        0      550 2024-04-23 05:25:43.687739 doctran_openai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.4/PKG-INFO
```

### Comparing `doctran_openai-0.0.3/LICENSE` & `doctran_openai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.3/README.md` & `doctran_openai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.3/doctran_openai/doctran_openai.py` & `doctran_openai-0.0.4/doctran_openai/doctran_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 class OpenAIConfig(BaseModel):
     api_key: str
     base_url: Optional[str]
 
 
 class DoctranConfig(BaseModel):
-    openai_deployment_id: Optional[str]
     openai_model: str
     openai: Any
     openai_token_limit: int
 
 
 class ContentType(Enum):
     text = "text"
@@ -182,42 +181,30 @@
 
     def process_template(self, *, template_regex: str) -> 'DocumentTransformationBuilder':
         self.transformations.append((Transformation.process_template, {"template_regex": template_regex}))
         return self
 
 
 class Doctran:
-    def __init__(self, openai_api_key: str = None, openai_model: str = "gpt-4", openai_token_limit: int = 8000,
-                 openai_deployment_id: Optional[str] = None):
+    def __init__(self, openai_api_key: str = None, openai_model: str = "gpt-4", openai_token_limit: int = 8000):
         self.config = DoctranConfig(
             openai_model=openai_model,
             openai=None,
             openai_token_limit=openai_token_limit
         )
         if openai_api_key:
-            # self.config.openai.api_key = openai_api_key
             openai_config = OpenAIConfig(api_key=openai_api_key)
         elif os.environ.get("OPENAI_API_KEY"):
-            # self.config.openai.api_key = os.environ["OPENAI_API_KEY"]
             openai_config = OpenAIConfig(api_key=os.environ["OPENAI_API_KEY"])
         else:
             raise Exception("No OpenAI API Key provided")
 
-        if openai_deployment_id:
-            self.config.openai_deployment_id = openai_deployment_id
-        elif os.environ.get("OPENAI_DEPLOYMENT_ID"):
-            self.config.openai_deployment_id = os.environ["OPENAI_DEPLOYMENT_ID"]
-
-        # if os.environ.get('OPENAI_API_TYPE'):
-        #     self.config.openai.api_type = os.environ['OPENAI_API_TYPE']
         if os.environ.get('OPENAI_API_BASE'):
             openai_config.base_url = os.environ['OPENAI_API_BASE']
-        #     self.config.openai.api_base = os.environ['OPENAI_API_BASE']
-        # if os.environ.get('OPENAI_API_VERSION'):
-        #     self.config.openai.api_version = os.environ['OPENAI_API_VERSION']
+
         self.config.openai = OpenAI(**openai_config.dict())
 
     def parse(self, *, content: str, content_type: ContentType = "text", uri: str = None,
               metadata: dict = None) -> Document:
         '''
         Parse raw text and apply different chunking schemes based on the content type.
```

### Comparing `doctran_openai-0.0.3/doctran_openai/transformers/transformers.py` & `doctran_openai-0.0.4/doctran_openai/transformers/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,43 +60,31 @@
             print(e)
             return document
         return self.executeOpenAICall(document)
 
     def executeOpenAICall(self, document: Document) -> Document:
         try:
             function_call = OpenAIFunctionCall(
-                # seed=self.config.openai_deployment_id,
                 model=self.config.openai_model,
                 messages=[{"role": "user", "content": document.transformed_content}],
                 functions=[{
                     "name": self.function_name,
                     "description": self.function_description,
                     "parameters": self.function_parameters,
                 }],
-                function_call={"name": self.function_name},
-                # tools=[{
-                #     "type": "function",
-                #     "function": {
-                #         "name": self.function_name,
-                #         "description": self.function_description,
-                #         "parameters": self.function_parameters,
-                #     }
-                # }],
-                # tool_choice={"type": "function", "function": {"name": self.function_name}}
+                function_call={"name": self.function_name}
             )
-            # completion = self.config.openai.chat.completions.create(**function_call.dict())
-            # arguments = completion.choices[0].message.tool_calls[0].function.arguments
             completion = self.config.openai.chat.completions.create(**function_call.dict())
             arguments = completion.choices[0].message.function_call.arguments
             try:
                 arguments = json.loads(arguments)
             except Exception as e:
-                raise Exception("OpenAI returned malformatted JSON" +
-                                "This is likely due to the completion running out of tokens. " +
-                                f"Setting a higher token limit may fix this error. JSON returned: {arguments}")
+                raise Exception(
+                    "OpenAI returned malformatted JSON This is likely due to the completion running out of tokens. " +
+                    f"Setting a higher token limit may fix this error. JSON returned: {arguments}")
             first_value = next(iter(arguments.values()))
             if len(arguments) > 1 or not isinstance(first_value, str):
                 # If multiple arguments or a dict/list is returned, treat arguments as extracted values
                 document.extracted_properties = document.extracted_properties or arguments
             else:
                 # If there is only one argument and it's a string, treat arguments as transformed content
                 document.transformed_content = first_value
```

### Comparing `doctran_openai-0.0.3/pyproject.toml` & `doctran_openai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran_openai"
-version = "0.0.3"
+version = "0.0.4"
 description = "Document transformation framework for vector based retrieval"
 authors = ["William Yang <yangfei86@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 pydantic = "^1.10.9"
```

### Comparing `doctran_openai-0.0.3/PKG-INFO` & `doctran_openai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doctran_openai
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.3 Summary: Document
+Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.4 Summary: Document
 transformation framework for vector based retrieval Author: William Yang
 Author-email: yangfei86@gmail.com Requires-Python: >=3.10.0,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=1.23.2,<2.0.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
```

