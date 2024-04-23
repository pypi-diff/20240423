# Comparing `tmp/doctran_openai-0.0.5.tar.gz` & `tmp/doctran_openai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran_openai-0.0.5.tar", max compression
+gzip compressed data, was "doctran_openai-0.0.6.tar", max compression
```

## Comparing `doctran_openai-0.0.5.tar` & `doctran_openai-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.5/LICENSE
--rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.5/README.md
--rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.5/doctran_openai/__init__.py
--rw-r--r--   0        0        0     8326 2024-04-23 05:30:16.776253 doctran_openai-0.0.5/doctran_openai/doctran_openai.py
--rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.5/doctran_openai/transformers/__init__.py
--rw-r--r--   0        0        0    15260 2024-04-23 05:24:50.304996 doctran_openai-0.0.5/doctran_openai/transformers/transformers.py
--rw-r--r--   0        0        0      550 2024-04-23 05:30:59.636618 doctran_openai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.6/README.md
+-rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.6/doctran_openai/__init__.py
+-rw-r--r--   0        0        0     8333 2024-04-23 05:41:44.412555 doctran_openai-0.0.6/doctran_openai/doctran_openai.py
+-rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.6/doctran_openai/transformers/__init__.py
+-rw-r--r--   0        0        0    15260 2024-04-23 05:24:50.304996 doctran_openai-0.0.6/doctran_openai/transformers/transformers.py
+-rw-r--r--   0        0        0      550 2024-04-23 05:42:36.615654 doctran_openai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.6/PKG-INFO
```

### Comparing `doctran_openai-0.0.5/LICENSE` & `doctran_openai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.5/README.md` & `doctran_openai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.5/doctran_openai/doctran_openai.py` & `doctran_openai-0.0.6/doctran_openai/doctran_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     '''
 
     def __init__(self, document: Document) -> None:
         self.document = document
         self.transformations = []
 
     def execute(self) -> Document:
-        module_name = "doctran.transformers"
+        module_name = "doctran_openai.transformers"
         module = importlib.import_module(module_name)
         try:
             transformed_document = self.document.copy()
             for transformation in self.transformations:
                 transformer = getattr(module, transformation[0].value)(config=transformed_document.config,
                                                                        **transformation[1])
                 transformed_document = transformer.transform(transformed_document)
```

### Comparing `doctran_openai-0.0.5/doctran_openai/transformers/transformers.py` & `doctran_openai-0.0.6/doctran_openai/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.5/pyproject.toml` & `doctran_openai-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran_openai"
-version = "0.0.5"
+version = "0.0.6"
 description = "Document transformation framework for vector based retrieval"
 authors = ["William Yang <yangfei86@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 pydantic = "^1.10.9"
```

### Comparing `doctran_openai-0.0.5/PKG-INFO` & `doctran_openai-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doctran_openai
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.5 Summary: Document
+Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.6 Summary: Document
 transformation framework for vector based retrieval Author: William Yang
 Author-email: yangfei86@gmail.com Requires-Python: >=3.10.0,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=1.23.2,<2.0.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
```

