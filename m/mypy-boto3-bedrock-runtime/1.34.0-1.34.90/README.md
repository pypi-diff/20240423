# Comparing `tmp/mypy-boto3-bedrock-runtime-1.34.0.tar.gz` & `tmp/mypy_boto3_bedrock_runtime-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-bedrock-runtime-1.34.0.tar", last modified: Wed Dec 13 21:22:03 2023, max compression
+gzip compressed data, was "mypy_boto3_bedrock_runtime-1.34.90.tar", last modified: Tue Apr 23 19:34:20 2024, max compression
```

## Comparing `mypy-boto3-bedrock-runtime-1.34.0.tar` & `mypy_boto3_bedrock_runtime-1.34.90.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:03.663139 mypy-boto3-bedrock-runtime-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2023-12-13 21:22:03.663139 mypy-boto3-bedrock-runtime-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10884 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:03.663139 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:03.663139 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:03.663139 mypy-boto3-bedrock-runtime-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-12-13 21:06:17.000000 mypy-boto3-bedrock-runtime-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:34:20.000000 mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:20.312567 mypy_boto3_bedrock_runtime-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_runtime-1.34.90/setup.py
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/LICENSE` & `mypy_boto3_bedrock_runtime-1.34.90/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/PKG-INFO` & `mypy_boto3_bedrock_runtime-1.34.90/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-runtime
-Version: 1.34.0
-Summary: Type annotations for boto3.BedrockRuntime 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.90
+Summary: Type annotations for boto3.BedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-bedrock-runtime"></a>
 
 # mypy-boto3-bedrock-runtime
 
 [![PyPI - mypy-boto3-bedrock-runtime](https://img.shields.io/pypi/v/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BedrockRuntime 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
+[boto3.BedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-bedrock-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,18 +280,18 @@
 `mypy_boto3_bedrock_runtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `BedrockRuntime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/).
 
 ```python
-from mypy_boto3_bedrock_runtime.literals import BedrockRuntimeServiceName
+from mypy_boto3_bedrock_runtime.literals import TraceType
 
 
-def check_value(value: BedrockRuntimeServiceName) -> bool: ...
+def check_value(value: TraceType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_bedrock_runtime.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/README.md` & `mypy_boto3_bedrock_runtime-1.34.90/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BedrockRuntime 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
+[boto3.BedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-bedrock-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -247,18 +247,18 @@
 `mypy_boto3_bedrock_runtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `BedrockRuntime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/).
 
 ```python
-from mypy_boto3_bedrock_runtime.literals import BedrockRuntimeServiceName
+from mypy_boto3_bedrock_runtime.literals import TraceType
 
 
-def check_value(value: BedrockRuntimeServiceName) -> bool: ...
+def check_value(value: TraceType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_bedrock_runtime.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/__main__.py` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BedrockRuntime 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.BedrockRuntime 1.34.90\n"
+        "Version:         1.34.90\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/client.py` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ```
 """
 
 from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import TraceType
 from .type_defs import (
     BlobTypeDef,
     InvokeModelResponseTypeDef,
     InvokeModelWithResponseStreamResponseTypeDef,
 )
 
 __all__ = ("BedrockRuntimeClient",)
@@ -93,27 +94,45 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#generate_presigned_url)
         """
 
     def invoke_model(
-        self, *, body: BlobTypeDef, modelId: str, contentType: str = ..., accept: str = ...
+        self,
+        *,
+        body: BlobTypeDef,
+        modelId: str,
+        contentType: str = ...,
+        accept: str = ...,
+        trace: TraceType = ...,
+        guardrailIdentifier: str = ...,
+        guardrailVersion: str = ...,
     ) -> InvokeModelResponseTypeDef:
         """
-        Invokes the specified Bedrock model to run inference using the input provided
-        in the request
+        Invokes the specified Amazon Bedrock model to run inference using the prompt
+        and inference parameters provided in the request
         body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.invoke_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#invoke_model)
         """
 
     def invoke_model_with_response_stream(
-        self, *, body: BlobTypeDef, modelId: str, contentType: str = ..., accept: str = ...
+        self,
+        *,
+        body: BlobTypeDef,
+        modelId: str,
+        contentType: str = ...,
+        accept: str = ...,
+        trace: TraceType = ...,
+        guardrailIdentifier: str = ...,
+        guardrailVersion: str = ...,
     ) -> InvokeModelWithResponseStreamResponseTypeDef:
         """
-        Invoke the specified Bedrock model to run inference using the input provided.
+        Invoke the specified Amazon Bedrock model to run inference using the prompt and
+        inference parameters provided in the request
+        body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.invoke_model_with_response_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#invoke_model_with_response_stream)
         """
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/client.pyi` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ```
 """
 
 from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import TraceType
 from .type_defs import (
     BlobTypeDef,
     InvokeModelResponseTypeDef,
     InvokeModelWithResponseStreamResponseTypeDef,
 )
 
 __all__ = ("BedrockRuntimeClient",)
@@ -90,27 +91,45 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#generate_presigned_url)
         """
 
     def invoke_model(
-        self, *, body: BlobTypeDef, modelId: str, contentType: str = ..., accept: str = ...
+        self,
+        *,
+        body: BlobTypeDef,
+        modelId: str,
+        contentType: str = ...,
+        accept: str = ...,
+        trace: TraceType = ...,
+        guardrailIdentifier: str = ...,
+        guardrailVersion: str = ...,
     ) -> InvokeModelResponseTypeDef:
         """
-        Invokes the specified Bedrock model to run inference using the input provided
-        in the request
+        Invokes the specified Amazon Bedrock model to run inference using the prompt
+        and inference parameters provided in the request
         body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.invoke_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#invoke_model)
         """
 
     def invoke_model_with_response_stream(
-        self, *, body: BlobTypeDef, modelId: str, contentType: str = ..., accept: str = ...
+        self,
+        *,
+        body: BlobTypeDef,
+        modelId: str,
+        contentType: str = ...,
+        accept: str = ...,
+        trace: TraceType = ...,
+        guardrailIdentifier: str = ...,
+        guardrailVersion: str = ...,
     ) -> InvokeModelWithResponseStreamResponseTypeDef:
         """
-        Invoke the specified Bedrock model to run inference using the input provided.
+        Invoke the specified Amazon Bedrock model to run inference using the prompt and
+        inference parameters provided in the request
+        body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client.invoke_model_with_response_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/client/#invoke_model_with_response_stream)
         """
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/literals.py` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 Type annotations for bedrock-runtime service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_bedrock_runtime.literals import BedrockRuntimeServiceName
+    from mypy_boto3_bedrock_runtime.literals import TraceType
 
-    data: BedrockRuntimeServiceName = "bedrock-runtime"
+    data: TraceType = "DISABLED"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+__all__ = ("TraceType", "BedrockRuntimeServiceName", "ServiceName", "ResourceServiceName")
 
-__all__ = ("BedrockRuntimeServiceName", "ServiceName", "ResourceServiceName")
-
-
+TraceType = Literal["DISABLED", "ENABLED"]
 BedrockRuntimeServiceName = Literal["bedrock-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -46,14 +45,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -64,14 +64,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -89,14 +90,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -109,24 +111,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -187,15 +191,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -267,17 +270,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -322,14 +327,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -367,19 +373,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/literals.pyi` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 Type annotations for bedrock-runtime service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_bedrock_runtime.literals import BedrockRuntimeServiceName
+    from mypy_boto3_bedrock_runtime.literals import TraceType
 
-    data: BedrockRuntimeServiceName = "bedrock-runtime"
+    data: TraceType = "DISABLED"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = ("BedrockRuntimeServiceName", "ServiceName", "ResourceServiceName")
+__all__ = ("TraceType", "BedrockRuntimeServiceName", "ServiceName", "ResourceServiceName")
 
+TraceType = Literal["DISABLED", "ENABLED"]
 BedrockRuntimeServiceName = Literal["bedrock-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -44,14 +45,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -62,14 +64,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -87,14 +90,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -107,24 +111,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -185,15 +191,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -265,17 +270,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -320,14 +327,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -365,19 +373,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/type_defs.py` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 
 import sys
 from typing import IO, Any, Dict, Union
 
 from botocore.eventstream import EventStream
 from botocore.response import StreamingBody
 
+from .literals import TraceType
+
 if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "InternalServerExceptionTypeDef",
     "ResponseMetadataTypeDef",
     "ModelStreamErrorExceptionTypeDef",
     "ModelTimeoutExceptionTypeDef",
     "PayloadPartTypeDef",
@@ -51,18 +52,18 @@
         "message": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ModelStreamErrorExceptionTypeDef = TypedDict(
     "ModelStreamErrorExceptionTypeDef",
     {
         "message": NotRequired[str],
         "originalStatusCode": NotRequired[int],
@@ -96,23 +97,29 @@
 InvokeModelRequestRequestTypeDef = TypedDict(
     "InvokeModelRequestRequestTypeDef",
     {
         "body": BlobTypeDef,
         "modelId": str,
         "contentType": NotRequired[str],
         "accept": NotRequired[str],
+        "trace": NotRequired[TraceType],
+        "guardrailIdentifier": NotRequired[str],
+        "guardrailVersion": NotRequired[str],
     },
 )
 InvokeModelWithResponseStreamRequestRequestTypeDef = TypedDict(
     "InvokeModelWithResponseStreamRequestRequestTypeDef",
     {
         "body": BlobTypeDef,
         "modelId": str,
         "contentType": NotRequired[str],
         "accept": NotRequired[str],
+        "trace": NotRequired[TraceType],
+        "guardrailIdentifier": NotRequired[str],
+        "guardrailVersion": NotRequired[str],
     },
 )
 InvokeModelResponseTypeDef = TypedDict(
     "InvokeModelResponseTypeDef",
     {
         "body": StreamingBody,
         "contentType": str,
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime/type_defs.pyi` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 import sys
 from typing import IO, Any, Dict, Union
 
 from botocore.eventstream import EventStream
 from botocore.response import StreamingBody
 
+from .literals import TraceType
+
 if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
@@ -50,18 +52,18 @@
         "message": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ModelStreamErrorExceptionTypeDef = TypedDict(
     "ModelStreamErrorExceptionTypeDef",
     {
         "message": NotRequired[str],
         "originalStatusCode": NotRequired[int],
@@ -95,23 +97,29 @@
 InvokeModelRequestRequestTypeDef = TypedDict(
     "InvokeModelRequestRequestTypeDef",
     {
         "body": BlobTypeDef,
         "modelId": str,
         "contentType": NotRequired[str],
         "accept": NotRequired[str],
+        "trace": NotRequired[TraceType],
+        "guardrailIdentifier": NotRequired[str],
+        "guardrailVersion": NotRequired[str],
     },
 )
 InvokeModelWithResponseStreamRequestRequestTypeDef = TypedDict(
     "InvokeModelWithResponseStreamRequestRequestTypeDef",
     {
         "body": BlobTypeDef,
         "modelId": str,
         "contentType": NotRequired[str],
         "accept": NotRequired[str],
+        "trace": NotRequired[TraceType],
+        "guardrailIdentifier": NotRequired[str],
+        "guardrailVersion": NotRequired[str],
     },
 )
 InvokeModelResponseTypeDef = TypedDict(
     "InvokeModelResponseTypeDef",
     {
         "body": StreamingBody,
         "contentType": str,
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-runtime
-Version: 1.34.0
-Summary: Type annotations for boto3.BedrockRuntime 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.90
+Summary: Type annotations for boto3.BedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-bedrock-runtime"></a>
 
 # mypy-boto3-bedrock-runtime
 
 [![PyPI - mypy-boto3-bedrock-runtime](https://img.shields.io/pypi/v/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BedrockRuntime 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
+[boto3.BedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-bedrock-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,18 +280,18 @@
 `mypy_boto3_bedrock_runtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `BedrockRuntime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/literals/).
 
 ```python
-from mypy_boto3_bedrock_runtime.literals import BedrockRuntimeServiceName
+from mypy_boto3_bedrock_runtime.literals import TraceType
 
 
-def check_value(value: BedrockRuntimeServiceName) -> bool: ...
+def check_value(value: TraceType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_bedrock_runtime.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt` & `mypy_boto3_bedrock_runtime-1.34.90/mypy_boto3_bedrock_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-runtime-1.34.0/setup.py` & `mypy_boto3_bedrock_runtime-1.34.90/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock-runtime",
-    version="1.34.0",
+    version="1.34.90",
     packages=["mypy_boto3_bedrock_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.BedrockRuntime 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.BedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 bedrock-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_bedrock_runtime": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_runtime/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

