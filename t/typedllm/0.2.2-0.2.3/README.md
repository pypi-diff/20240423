# Comparing `tmp/typedllm-0.2.2.tar.gz` & `tmp/typedllm-0.2.3.tar.gz`

## Comparing `typedllm-0.2.2.tar` & `typedllm-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.2/HISTORY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 typedllm-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 typedllm-0.2.2/tests/test_client.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.2.2/tests/test_interop.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedllm-0.2.2/tests/test_tool.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.2.2/LICENSE
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.2.2/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 typedllm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 typedllm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.3/HISTORY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_client.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_interop.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_prompt.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedllm-0.2.3/tests/test_tool.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.2.3/LICENSE
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.2.3/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 typedllm-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 typedllm-0.2.3/PKG-INFO
```

### Comparing `typedllm-0.2.2/tests/conftest.py` & `typedllm-0.2.3/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import ClassVar
+
 import os
 import pytest
 
 from typedllm import LLMModel, TypedPrompt, LLMSession, LLMRequest, Tool, create_tool_from_function
-from typedtemplate import JinjaTemplateEngine
+from typedtemplate import JinjaTemplateEngine, TypedTemplate
 from pydantic import Field
 
 
 @pytest.fixture(name="openai_key")
 def get_openai_key() -> str:
     return os.getenv("OPENAI_API_KEY")
 
@@ -35,22 +37,39 @@
 @pytest.fixture(name="jinja_engine")
 def get_template_engine():
     return JinjaTemplateEngine()
 
 
 @pytest.fixture(name="llmprompt")
 def get_prompt(jinja_engine: JinjaTemplateEngine):
-    class PromptTemplate(TypedPrompt):
+    class PromptTemplate(TypedTemplate):
         template_engine = jinja_engine
         template_string = "What year was {{ city }} founded?"
         city: str = Field(description="The city to use in the prompt")
 
     return PromptTemplate
 
 
+@pytest.fixture(name="instruction_template")
+def get_instruction_template(jinja_engine: JinjaTemplateEngine):
+    class InstructionTemplate(TypedTemplate):
+        template_engine = jinja_engine
+        template_string = "What year was {{ city }} founded?"
+        city: str = Field(description="City name")
+    return InstructionTemplate
+
+
+@pytest.fixture(name="context_template")
+def get_context_template(jinja_engine: JinjaTemplateEngine):
+    class ContextTemplate(TypedTemplate):
+        template_engine = jinja_engine
+        template_string = "User Name: {{ username }}"
+        username: str = Field(description="User's name")
+    return ContextTemplate
+
 @pytest.fixture(name="llmsession")
 def get_session(model: LLMModel) -> LLMSession:
     return LLMSession(
         model=model,
         verbose=True,
     )
```

### Comparing `typedllm-0.2.2/tests/test_client.py` & `typedllm-0.2.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.2/tests/test_interop.py` & `typedllm-0.2.3/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.2/tests/test_tool.py` & `typedllm-0.2.3/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.2/.gitignore` & `typedllm-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.2/LICENSE` & `typedllm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `typedllm-0.2.2/pyproject.toml` & `typedllm-0.2.3/pyproject.toml`

 * *Files identical despite different names*

