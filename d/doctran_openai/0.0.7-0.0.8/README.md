# Comparing `tmp/doctran_openai-0.0.7.tar.gz` & `tmp/doctran_openai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran_openai-0.0.7.tar", max compression
+gzip compressed data, was "doctran_openai-0.0.8.tar", max compression
```

## Comparing `doctran_openai-0.0.7.tar` & `doctran_openai-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.7/LICENSE
--rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.7/README.md
--rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.7/doctran_openai/__init__.py
--rw-r--r--   0        0        0     8299 2024-04-23 07:04:55.674764 doctran_openai-0.0.7/doctran_openai/doctran_openai.py
--rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.7/doctran_openai/transformers/__init__.py
--rw-r--r--   0        0        0    15260 2024-04-23 05:24:50.304996 doctran_openai-0.0.7/doctran_openai/transformers/transformers.py
--rw-r--r--   0        0        0      550 2024-04-23 07:05:14.225241 doctran_openai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.8/LICENSE
+-rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.8/README.md
+-rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.8/doctran_openai/__init__.py
+-rw-r--r--   0        0        0     8396 2024-04-23 10:37:28.266936 doctran_openai-0.0.8/doctran_openai/doctran_openai.py
+-rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.8/doctran_openai/transformers/__init__.py
+-rw-r--r--   0        0        0    15249 2024-04-23 10:44:06.378621 doctran_openai-0.0.8/doctran_openai/transformers/transformers.py
+-rw-r--r--   0        0        0      550 2024-04-23 10:46:04.216865 doctran_openai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.8/PKG-INFO
```

### Comparing `doctran_openai-0.0.7/LICENSE` & `doctran_openai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.7/README.md` & `doctran_openai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.7/doctran_openai/doctran_openai.py` & `doctran_openai-0.0.8/doctran_openai/doctran_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,29 +181,31 @@
 
     def process_template(self, *, template_regex: str) -> 'DocumentTransformationBuilder':
         self.transformations.append((Transformation.process_template, {"template_regex": template_regex}))
         return self
 
 
 class Doctran:
-    def __init__(self, openai_api_key: str = None, openai_model: str = "gpt-4", openai_token_limit: int = 8000):
+    def __init__(self, openai_api_key: str = None, openai_model: str = "gpt-4", openai_token_limit: int = 8000, openai_api_base: str = None):
         if openai_api_key:
             openai_config = OpenAIConfig(api_key=openai_api_key)
         elif os.environ.get("OPENAI_API_KEY"):
             openai_config = OpenAIConfig(api_key=os.environ["OPENAI_API_KEY"])
         else:
             raise Exception("No OpenAI API Key provided")
 
-        if os.environ.get('OPENAI_API_BASE'):
+        if openai_api_base:
+            openai_config.base_url = openai_api_base
+        elif os.environ.get('OPENAI_API_BASE'):
             openai_config.base_url = os.environ['OPENAI_API_BASE']
 
         self.config = DoctranConfig(
             openai_model=openai_model,
-            openai=OpenAI(**openai_config.dict()),
-            openai_token_limit=openai_token_limit
+            openai_token_limit=openai_token_limit,
+            **openai_config.dict()
         )
 
     def parse(self, *, content: str, content_type: ContentType = "text", uri: str = None,
               metadata: dict = None) -> Document:
         '''
         Parse raw text and apply different chunking schemes based on the content type.
```

### Comparing `doctran_openai-0.0.7/doctran_openai/transformers/transformers.py` & `doctran_openai-0.0.8/doctran_openai/transformers/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,22 @@
         return self.executeOpenAICall(document)
 
     def executeOpenAICall(self, document: Document) -> Document:
         try:
             function_call = OpenAIFunctionCall(
                 model=self.config.openai_model,
                 messages=[{"role": "user", "content": document.transformed_content}],
-                functions=[{
+                tools=[{
                     "name": self.function_name,
                     "description": self.function_description,
                     "parameters": self.function_parameters,
                 }],
-                function_call={"name": self.function_name}
+                tool_choice={"name": self.function_name}
             )
-            completion = self.config.openai.chat.completions.create(**function_call.dict())
+            completion = self.config.openai.completions.create(**function_call.dict())
             arguments = completion.choices[0].message.function_call.arguments
             try:
                 arguments = json.loads(arguments)
             except Exception as e:
                 raise Exception(
                     "OpenAI returned malformatted JSON This is likely due to the completion running out of tokens. " +
                     f"Setting a higher token limit may fix this error. JSON returned: {arguments}")
```

### Comparing `doctran_openai-0.0.7/pyproject.toml` & `doctran_openai-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran_openai"
-version = "0.0.7"
+version = "0.0.8"
 description = "Document transformation framework for vector based retrieval"
 authors = ["William Yang <yangfei86@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 pydantic = "^1.10.9"
```

### Comparing `doctran_openai-0.0.7/PKG-INFO` & `doctran_openai-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doctran_openai
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.7 Summary: Document
+Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.8 Summary: Document
 transformation framework for vector based retrieval Author: William Yang
 Author-email: yangfei86@gmail.com Requires-Python: >=3.10.0,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=1.23.2,<2.0.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
```
