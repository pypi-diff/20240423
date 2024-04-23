# Comparing `tmp/mypy-boto3-bedrock-1.34.0.tar.gz` & `tmp/mypy_boto3_bedrock-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-bedrock-1.34.0.tar", last modified: Wed Dec 13 21:22:03 2023, max compression
+gzip compressed data, was "mypy_boto3_bedrock-1.34.90.tar", last modified: Tue Apr 23 19:34:19 2024, max compression
```

## Comparing `mypy-boto3-bedrock-1.34.0.tar` & `mypy_boto3_bedrock-1.34.90.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:03.295138 mypy-boto3-bedrock-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13042 2023-12-13 21:22:03.295138 mypy-boto3-bedrock-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:03.295138 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18436 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2023-12-13 21:06:14.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2023-12-13 21:06:14.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19918 2023-12-13 21:06:14.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:03.295138 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13042 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 21:22:03.000000 mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:03.295138 mypy-boto3-bedrock-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-13 21:06:13.000000 mypy-boto3-bedrock-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.980563 mypy_boto3_bedrock-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-23 19:34:19.980563 mypy_boto3_bedrock-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.976563 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26759 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26756 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-23 19:33:08.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-23 19:33:08.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36525 2024-04-23 19:33:08.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36525 2024-04-23 19:33:08.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.980563 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-23 19:34:19.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-23 19:34:19.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:19.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 19:34:19.000000 mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:19.980563 mypy_boto3_bedrock-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-23 19:33:07.000000 mypy_boto3_bedrock-1.34.90/setup.py
```

### Comparing `mypy-boto3-bedrock-1.34.0/LICENSE` & `mypy_boto3_bedrock-1.34.90/LICENSE`

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

### Comparing `mypy-boto3-bedrock-1.34.0/PKG-INFO` & `mypy_boto3_bedrock-1.34.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock
-Version: 1.34.0
-Summary: Type annotations for boto3.Bedrock 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.90
+Summary: Type annotations for boto3.Bedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/
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
 
 <a id="mypy-boto3-bedrock"></a>
 
 # mypy-boto3-bedrock
 
 [![PyPI - mypy-boto3-bedrock](https://img.shields.io/pypi/v/mypy-boto3-bedrock.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock)](https://pepy.tech/project/mypy-boto3-bedrock)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Bedrock 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
+[boto3.Bedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
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
 [mypy-boto3-bedrock docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,23 +281,29 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_bedrock import BedrockClient
 from mypy_boto3_bedrock.paginator import (
     ListCustomModelsPaginator,
+    ListEvaluationJobsPaginator,
+    ListGuardrailsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 
 client: BedrockClient = Session().client("bedrock")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_custom_models_paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")
+list_evaluation_jobs_paginator: ListEvaluationJobsPaginator = client.get_paginator(
+    "list_evaluation_jobs"
+)
+list_guardrails_paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")
 list_model_customization_jobs_paginator: ListModelCustomizationJobsPaginator = client.get_paginator(
     "list_model_customization_jobs"
 )
 list_provisioned_model_throughputs_paginator: ListProvisionedModelThroughputsPaginator = (
     client.get_paginator("list_provisioned_model_throughputs")
 )
 ```
```

### Comparing `mypy-boto3-bedrock-1.34.0/README.md` & `mypy_boto3_bedrock-1.34.90/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock)](https://pepy.tech/project/mypy-boto3-bedrock)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Bedrock 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
+[boto3.Bedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
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
 [mypy-boto3-bedrock docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/).
 
 See how it helps to find and fix potential bugs:
 
@@ -248,23 +248,29 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_bedrock import BedrockClient
 from mypy_boto3_bedrock.paginator import (
     ListCustomModelsPaginator,
+    ListEvaluationJobsPaginator,
+    ListGuardrailsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 
 client: BedrockClient = Session().client("bedrock")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_custom_models_paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")
+list_evaluation_jobs_paginator: ListEvaluationJobsPaginator = client.get_paginator(
+    "list_evaluation_jobs"
+)
+list_guardrails_paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")
 list_model_customization_jobs_paginator: ListModelCustomizationJobsPaginator = client.get_paginator(
     "list_model_customization_jobs"
 )
 list_provisioned_model_throughputs_paginator: ListProvisionedModelThroughputsPaginator = (
     client.get_paginator("list_provisioned_model_throughputs")
 )
 ```
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/__init__.py` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,37 +5,44 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_bedrock import (
         BedrockClient,
         Client,
         ListCustomModelsPaginator,
+        ListEvaluationJobsPaginator,
+        ListGuardrailsPaginator,
         ListModelCustomizationJobsPaginator,
         ListProvisionedModelThroughputsPaginator,
     )
 
     session = Session()
     client: BedrockClient = session.client("bedrock")
 
     list_custom_models_paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")
+    list_evaluation_jobs_paginator: ListEvaluationJobsPaginator = client.get_paginator("list_evaluation_jobs")
+    list_guardrails_paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")
     list_model_customization_jobs_paginator: ListModelCustomizationJobsPaginator = client.get_paginator("list_model_customization_jobs")
     list_provisioned_model_throughputs_paginator: ListProvisionedModelThroughputsPaginator = client.get_paginator("list_provisioned_model_throughputs")
     ```
 """
 
 from .client import BedrockClient
 from .paginator import (
     ListCustomModelsPaginator,
+    ListEvaluationJobsPaginator,
+    ListGuardrailsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 
 Client = BedrockClient
 
-
 __all__ = (
     "BedrockClient",
     "Client",
     "ListCustomModelsPaginator",
+    "ListEvaluationJobsPaginator",
+    "ListGuardrailsPaginator",
     "ListModelCustomizationJobsPaginator",
     "ListProvisionedModelThroughputsPaginator",
 )
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/__init__.pyi` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -5,36 +5,44 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_bedrock import (
         BedrockClient,
         Client,
         ListCustomModelsPaginator,
+        ListEvaluationJobsPaginator,
+        ListGuardrailsPaginator,
         ListModelCustomizationJobsPaginator,
         ListProvisionedModelThroughputsPaginator,
     )
 
     session = Session()
     client: BedrockClient = session.client("bedrock")
 
     list_custom_models_paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")
+    list_evaluation_jobs_paginator: ListEvaluationJobsPaginator = client.get_paginator("list_evaluation_jobs")
+    list_guardrails_paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")
     list_model_customization_jobs_paginator: ListModelCustomizationJobsPaginator = client.get_paginator("list_model_customization_jobs")
     list_provisioned_model_throughputs_paginator: ListProvisionedModelThroughputsPaginator = client.get_paginator("list_provisioned_model_throughputs")
     ```
 """
 
 from .client import BedrockClient
 from .paginator import (
     ListCustomModelsPaginator,
+    ListEvaluationJobsPaginator,
+    ListGuardrailsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 
 Client = BedrockClient
 
 __all__ = (
     "BedrockClient",
     "Client",
     "ListCustomModelsPaginator",
+    "ListEvaluationJobsPaginator",
+    "ListGuardrailsPaginator",
     "ListModelCustomizationJobsPaginator",
     "ListProvisionedModelThroughputsPaginator",
 )
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/__main__.py` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Bedrock 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Bedrock 1.34.90\n"
+        "Version:         1.34.90\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock\n"
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

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/client.py` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,54 +18,71 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CommitmentDurationType,
     CustomizationTypeType,
+    EvaluationJobStatusType,
     FineTuningJobStatusType,
     InferenceTypeType,
     ModelCustomizationType,
     ModelModalityType,
     ProvisionedModelStatusType,
     SortOrderType,
 )
 from .paginator import (
     ListCustomModelsPaginator,
+    ListEvaluationJobsPaginator,
+    ListGuardrailsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 from .type_defs import (
+    CreateEvaluationJobResponseTypeDef,
+    CreateGuardrailResponseTypeDef,
+    CreateGuardrailVersionResponseTypeDef,
     CreateModelCustomizationJobResponseTypeDef,
     CreateProvisionedModelThroughputResponseTypeDef,
+    EvaluationConfigTypeDef,
+    EvaluationInferenceConfigTypeDef,
+    EvaluationOutputDataConfigTypeDef,
     GetCustomModelResponseTypeDef,
+    GetEvaluationJobResponseTypeDef,
     GetFoundationModelResponseTypeDef,
+    GetGuardrailResponseTypeDef,
     GetModelCustomizationJobResponseTypeDef,
     GetModelInvocationLoggingConfigurationResponseTypeDef,
     GetProvisionedModelThroughputResponseTypeDef,
+    GuardrailContentPolicyConfigTypeDef,
+    GuardrailSensitiveInformationPolicyConfigTypeDef,
+    GuardrailTopicPolicyConfigTypeDef,
+    GuardrailWordPolicyConfigTypeDef,
     ListCustomModelsResponseTypeDef,
+    ListEvaluationJobsResponseTypeDef,
     ListFoundationModelsResponseTypeDef,
+    ListGuardrailsResponseTypeDef,
     ListModelCustomizationJobsResponseTypeDef,
     ListProvisionedModelThroughputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingConfigTypeDef,
     OutputDataConfigTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TrainingDataConfigTypeDef,
+    UpdateGuardrailResponseTypeDef,
     ValidationDataConfigTypeDef,
     VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BedrockClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -114,14 +131,68 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#close)
         """
 
+    def create_evaluation_job(
+        self,
+        *,
+        jobName: str,
+        roleArn: str,
+        evaluationConfig: EvaluationConfigTypeDef,
+        inferenceConfig: EvaluationInferenceConfigTypeDef,
+        outputDataConfig: EvaluationOutputDataConfigTypeDef,
+        jobDescription: str = ...,
+        clientRequestToken: str = ...,
+        customerEncryptionKeyId: str = ...,
+        jobTags: Sequence[TagTypeDef] = ...,
+    ) -> CreateEvaluationJobResponseTypeDef:
+        """
+        API operation for creating and managing Amazon Bedrock automatic model
+        evaluation jobs and model evaluation jobs that use human
+        workers.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_evaluation_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_evaluation_job)
+        """
+
+    def create_guardrail(
+        self,
+        *,
+        name: str,
+        blockedInputMessaging: str,
+        blockedOutputsMessaging: str,
+        description: str = ...,
+        topicPolicyConfig: GuardrailTopicPolicyConfigTypeDef = ...,
+        contentPolicyConfig: GuardrailContentPolicyConfigTypeDef = ...,
+        wordPolicyConfig: GuardrailWordPolicyConfigTypeDef = ...,
+        sensitiveInformationPolicyConfig: GuardrailSensitiveInformationPolicyConfigTypeDef = ...,
+        kmsKeyId: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+        clientRequestToken: str = ...,
+    ) -> CreateGuardrailResponseTypeDef:
+        """
+        Creates a guardrail to block topics and to filter out harmful content.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_guardrail)
+        """
+
+    def create_guardrail_version(
+        self, *, guardrailIdentifier: str, description: str = ..., clientRequestToken: str = ...
+    ) -> CreateGuardrailVersionResponseTypeDef:
+        """
+        Creates a version of the guardrail.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_guardrail_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_guardrail_version)
+        """
+
     def create_model_customization_job(
         self,
         *,
         jobName: str,
         customModelName: str,
         roleArn: str,
         baseModelIdentifier: str,
@@ -130,15 +201,15 @@
         hyperParameters: Mapping[str, str],
         clientRequestToken: str = ...,
         customizationType: CustomizationTypeType = ...,
         customModelKmsKeyId: str = ...,
         jobTags: Sequence[TagTypeDef] = ...,
         customModelTags: Sequence[TagTypeDef] = ...,
         validationDataConfig: ValidationDataConfigTypeDef = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...,
     ) -> CreateModelCustomizationJobResponseTypeDef:
         """
         Creates a fine-tuning job to customize a base model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_model_customization_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_model_customization_job)
         """
@@ -147,44 +218,54 @@
         self,
         *,
         modelUnits: int,
         provisionedModelName: str,
         modelId: str,
         clientRequestToken: str = ...,
         commitmentDuration: CommitmentDurationType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProvisionedModelThroughputResponseTypeDef:
         """
-        Creates a provisioned throughput with dedicated capacity for a foundation model
-        or a fine-tuned
-        model.
+        Creates dedicated throughput for a base or custom model with the model units
+        and for the duration that you
+        specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_provisioned_model_throughput)
         """
 
     def delete_custom_model(self, *, modelIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a custom model that you created earlier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_custom_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_custom_model)
         """
 
+    def delete_guardrail(
+        self, *, guardrailIdentifier: str, guardrailVersion: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Deletes a guardrail.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_guardrail)
+        """
+
     def delete_model_invocation_logging_configuration(self) -> Dict[str, Any]:
         """
         Delete the invocation logging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_model_invocation_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_model_invocation_logging_configuration)
         """
 
     def delete_provisioned_model_throughput(self, *, provisionedModelId: str) -> Dict[str, Any]:
         """
-        Deletes a provisioned throughput.
+        Deletes a Provisioned Throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_provisioned_model_throughput)
         """
 
     def generate_presigned_url(
         self,
@@ -201,29 +282,49 @@
         """
 
     def get_custom_model(self, *, modelIdentifier: str) -> GetCustomModelResponseTypeDef:
         """
         Get the properties associated with a Amazon Bedrock custom model that you have
         created.For more information, see [Custom
         models](https://docs.aws.amazon.com/bedrock/latest/userguide/custom-models.html)
-        in the Bedrock User
+        in the Amazon Bedrock User
         Guide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_custom_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_custom_model)
         """
 
+    def get_evaluation_job(self, *, jobIdentifier: str) -> GetEvaluationJobResponseTypeDef:
+        """
+        Retrieves the properties associated with a model evaluation job, including the
+        status of the
+        job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_evaluation_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_evaluation_job)
+        """
+
     def get_foundation_model(self, *, modelIdentifier: str) -> GetFoundationModelResponseTypeDef:
         """
         Get details about a Amazon Bedrock foundation model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_foundation_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_foundation_model)
         """
 
+    def get_guardrail(
+        self, *, guardrailIdentifier: str, guardrailVersion: str = ...
+    ) -> GetGuardrailResponseTypeDef:
+        """
+        Gets details about a guardrail.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_guardrail)
+        """
+
     def get_model_customization_job(
         self, *, jobIdentifier: str
     ) -> GetModelCustomizationJobResponseTypeDef:
         """
         Retrieves the properties associated with a model-customization job, including
         the status of the
         job.
@@ -242,15 +343,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_model_invocation_logging_configuration)
         """
 
     def get_provisioned_model_throughput(
         self, *, provisionedModelId: str
     ) -> GetProvisionedModelThroughputResponseTypeDef:
         """
-        Get details for a provisioned throughput.
+        Returns details for a Provisioned Throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_provisioned_model_throughput)
         """
 
     def list_custom_models(
         self,
@@ -259,51 +360,80 @@
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListCustomModelsResponseTypeDef:
         """
         Returns a list of the custom models that you have created with the
         `CreateModelCustomizationJob`
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_custom_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_custom_models)
         """
 
+    def list_evaluation_jobs(
+        self,
+        *,
+        creationTimeAfter: TimestampTypeDef = ...,
+        creationTimeBefore: TimestampTypeDef = ...,
+        statusEquals: EvaluationJobStatusType = ...,
+        nameContains: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        sortBy: Literal["CreationTime"] = ...,
+        sortOrder: SortOrderType = ...,
+    ) -> ListEvaluationJobsResponseTypeDef:
+        """
+        Lists model evaluation jobs.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_evaluation_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_evaluation_jobs)
+        """
+
     def list_foundation_models(
         self,
         *,
         byProvider: str = ...,
         byCustomizationType: ModelCustomizationType = ...,
         byOutputModality: ModelModalityType = ...,
-        byInferenceType: InferenceTypeType = ...
+        byInferenceType: InferenceTypeType = ...,
     ) -> ListFoundationModelsResponseTypeDef:
         """
-        List of Amazon Bedrock foundation models that you can use.
+        Lists Amazon Bedrock foundation models that you can use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_foundation_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_foundation_models)
         """
 
+    def list_guardrails(
+        self, *, guardrailIdentifier: str = ..., maxResults: int = ..., nextToken: str = ...
+    ) -> ListGuardrailsResponseTypeDef:
+        """
+        Lists details about all the guardrails in an account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_guardrails)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_guardrails)
+        """
+
     def list_model_customization_jobs(
         self,
         *,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListModelCustomizationJobsResponseTypeDef:
         """
         Returns a list of model customization jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_model_customization_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_model_customization_jobs)
         """
@@ -315,18 +445,18 @@
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListProvisionedModelThroughputsResponseTypeDef:
         """
-        List the provisioned capacities.
+        Lists the Provisioned Throughputs in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_provisioned_model_throughputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_provisioned_model_throughputs)
         """
 
     def list_tags_for_resource(self, *, resourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -342,14 +472,22 @@
         """
         Set the configuration values for model invocation logging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.put_model_invocation_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#put_model_invocation_logging_configuration)
         """
 
+    def stop_evaluation_job(self, *, jobIdentifier: str) -> Dict[str, Any]:
+        """
+        Stops an in progress model evaluation job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.stop_evaluation_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#stop_evaluation_job)
+        """
+
     def stop_model_customization_job(self, *, jobIdentifier: str) -> Dict[str, Any]:
         """
         Stops an active model customization job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.stop_model_customization_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#stop_model_customization_job)
         """
@@ -366,23 +504,44 @@
         """
         Remove one or more tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#untag_resource)
         """
 
+    def update_guardrail(
+        self,
+        *,
+        guardrailIdentifier: str,
+        name: str,
+        blockedInputMessaging: str,
+        blockedOutputsMessaging: str,
+        description: str = ...,
+        topicPolicyConfig: GuardrailTopicPolicyConfigTypeDef = ...,
+        contentPolicyConfig: GuardrailContentPolicyConfigTypeDef = ...,
+        wordPolicyConfig: GuardrailWordPolicyConfigTypeDef = ...,
+        sensitiveInformationPolicyConfig: GuardrailSensitiveInformationPolicyConfigTypeDef = ...,
+        kmsKeyId: str = ...,
+    ) -> UpdateGuardrailResponseTypeDef:
+        """
+        Updates a guardrail with the values you specify.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.update_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#update_guardrail)
+        """
+
     def update_provisioned_model_throughput(
         self,
         *,
         provisionedModelId: str,
         desiredProvisionedModelName: str = ...,
-        desiredModelId: str = ...
+        desiredModelId: str = ...,
     ) -> Dict[str, Any]:
         """
-        Update a provisioned throughput.
+        Updates the name or associated model for a Provisioned Throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.update_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#update_provisioned_model_throughput)
         """
 
     @overload
     def get_paginator(
@@ -391,14 +550,30 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_evaluation_jobs"]
+    ) -> ListEvaluationJobsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_guardrails"]) -> ListGuardrailsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_model_customization_jobs"]
     ) -> ListModelCustomizationJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/client.pyi` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/client.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -18,44 +18,62 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CommitmentDurationType,
     CustomizationTypeType,
+    EvaluationJobStatusType,
     FineTuningJobStatusType,
     InferenceTypeType,
     ModelCustomizationType,
     ModelModalityType,
     ProvisionedModelStatusType,
     SortOrderType,
 )
 from .paginator import (
     ListCustomModelsPaginator,
+    ListEvaluationJobsPaginator,
+    ListGuardrailsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 from .type_defs import (
+    CreateEvaluationJobResponseTypeDef,
+    CreateGuardrailResponseTypeDef,
+    CreateGuardrailVersionResponseTypeDef,
     CreateModelCustomizationJobResponseTypeDef,
     CreateProvisionedModelThroughputResponseTypeDef,
+    EvaluationConfigTypeDef,
+    EvaluationInferenceConfigTypeDef,
+    EvaluationOutputDataConfigTypeDef,
     GetCustomModelResponseTypeDef,
+    GetEvaluationJobResponseTypeDef,
     GetFoundationModelResponseTypeDef,
+    GetGuardrailResponseTypeDef,
     GetModelCustomizationJobResponseTypeDef,
     GetModelInvocationLoggingConfigurationResponseTypeDef,
     GetProvisionedModelThroughputResponseTypeDef,
+    GuardrailContentPolicyConfigTypeDef,
+    GuardrailSensitiveInformationPolicyConfigTypeDef,
+    GuardrailTopicPolicyConfigTypeDef,
+    GuardrailWordPolicyConfigTypeDef,
     ListCustomModelsResponseTypeDef,
+    ListEvaluationJobsResponseTypeDef,
     ListFoundationModelsResponseTypeDef,
+    ListGuardrailsResponseTypeDef,
     ListModelCustomizationJobsResponseTypeDef,
     ListProvisionedModelThroughputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingConfigTypeDef,
     OutputDataConfigTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TrainingDataConfigTypeDef,
+    UpdateGuardrailResponseTypeDef,
     ValidationDataConfigTypeDef,
     VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -110,14 +128,68 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#close)
         """
 
+    def create_evaluation_job(
+        self,
+        *,
+        jobName: str,
+        roleArn: str,
+        evaluationConfig: EvaluationConfigTypeDef,
+        inferenceConfig: EvaluationInferenceConfigTypeDef,
+        outputDataConfig: EvaluationOutputDataConfigTypeDef,
+        jobDescription: str = ...,
+        clientRequestToken: str = ...,
+        customerEncryptionKeyId: str = ...,
+        jobTags: Sequence[TagTypeDef] = ...,
+    ) -> CreateEvaluationJobResponseTypeDef:
+        """
+        API operation for creating and managing Amazon Bedrock automatic model
+        evaluation jobs and model evaluation jobs that use human
+        workers.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_evaluation_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_evaluation_job)
+        """
+
+    def create_guardrail(
+        self,
+        *,
+        name: str,
+        blockedInputMessaging: str,
+        blockedOutputsMessaging: str,
+        description: str = ...,
+        topicPolicyConfig: GuardrailTopicPolicyConfigTypeDef = ...,
+        contentPolicyConfig: GuardrailContentPolicyConfigTypeDef = ...,
+        wordPolicyConfig: GuardrailWordPolicyConfigTypeDef = ...,
+        sensitiveInformationPolicyConfig: GuardrailSensitiveInformationPolicyConfigTypeDef = ...,
+        kmsKeyId: str = ...,
+        tags: Sequence[TagTypeDef] = ...,
+        clientRequestToken: str = ...,
+    ) -> CreateGuardrailResponseTypeDef:
+        """
+        Creates a guardrail to block topics and to filter out harmful content.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_guardrail)
+        """
+
+    def create_guardrail_version(
+        self, *, guardrailIdentifier: str, description: str = ..., clientRequestToken: str = ...
+    ) -> CreateGuardrailVersionResponseTypeDef:
+        """
+        Creates a version of the guardrail.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_guardrail_version)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_guardrail_version)
+        """
+
     def create_model_customization_job(
         self,
         *,
         jobName: str,
         customModelName: str,
         roleArn: str,
         baseModelIdentifier: str,
@@ -126,15 +198,15 @@
         hyperParameters: Mapping[str, str],
         clientRequestToken: str = ...,
         customizationType: CustomizationTypeType = ...,
         customModelKmsKeyId: str = ...,
         jobTags: Sequence[TagTypeDef] = ...,
         customModelTags: Sequence[TagTypeDef] = ...,
         validationDataConfig: ValidationDataConfigTypeDef = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...,
     ) -> CreateModelCustomizationJobResponseTypeDef:
         """
         Creates a fine-tuning job to customize a base model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_model_customization_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_model_customization_job)
         """
@@ -143,44 +215,54 @@
         self,
         *,
         modelUnits: int,
         provisionedModelName: str,
         modelId: str,
         clientRequestToken: str = ...,
         commitmentDuration: CommitmentDurationType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProvisionedModelThroughputResponseTypeDef:
         """
-        Creates a provisioned throughput with dedicated capacity for a foundation model
-        or a fine-tuned
-        model.
+        Creates dedicated throughput for a base or custom model with the model units
+        and for the duration that you
+        specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#create_provisioned_model_throughput)
         """
 
     def delete_custom_model(self, *, modelIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a custom model that you created earlier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_custom_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_custom_model)
         """
 
+    def delete_guardrail(
+        self, *, guardrailIdentifier: str, guardrailVersion: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Deletes a guardrail.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_guardrail)
+        """
+
     def delete_model_invocation_logging_configuration(self) -> Dict[str, Any]:
         """
         Delete the invocation logging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_model_invocation_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_model_invocation_logging_configuration)
         """
 
     def delete_provisioned_model_throughput(self, *, provisionedModelId: str) -> Dict[str, Any]:
         """
-        Deletes a provisioned throughput.
+        Deletes a Provisioned Throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#delete_provisioned_model_throughput)
         """
 
     def generate_presigned_url(
         self,
@@ -197,29 +279,49 @@
         """
 
     def get_custom_model(self, *, modelIdentifier: str) -> GetCustomModelResponseTypeDef:
         """
         Get the properties associated with a Amazon Bedrock custom model that you have
         created.For more information, see [Custom
         models](https://docs.aws.amazon.com/bedrock/latest/userguide/custom-models.html)
-        in the Bedrock User
+        in the Amazon Bedrock User
         Guide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_custom_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_custom_model)
         """
 
+    def get_evaluation_job(self, *, jobIdentifier: str) -> GetEvaluationJobResponseTypeDef:
+        """
+        Retrieves the properties associated with a model evaluation job, including the
+        status of the
+        job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_evaluation_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_evaluation_job)
+        """
+
     def get_foundation_model(self, *, modelIdentifier: str) -> GetFoundationModelResponseTypeDef:
         """
         Get details about a Amazon Bedrock foundation model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_foundation_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_foundation_model)
         """
 
+    def get_guardrail(
+        self, *, guardrailIdentifier: str, guardrailVersion: str = ...
+    ) -> GetGuardrailResponseTypeDef:
+        """
+        Gets details about a guardrail.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_guardrail)
+        """
+
     def get_model_customization_job(
         self, *, jobIdentifier: str
     ) -> GetModelCustomizationJobResponseTypeDef:
         """
         Retrieves the properties associated with a model-customization job, including
         the status of the
         job.
@@ -238,15 +340,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_model_invocation_logging_configuration)
         """
 
     def get_provisioned_model_throughput(
         self, *, provisionedModelId: str
     ) -> GetProvisionedModelThroughputResponseTypeDef:
         """
-        Get details for a provisioned throughput.
+        Returns details for a Provisioned Throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_provisioned_model_throughput)
         """
 
     def list_custom_models(
         self,
@@ -255,51 +357,80 @@
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListCustomModelsResponseTypeDef:
         """
         Returns a list of the custom models that you have created with the
         `CreateModelCustomizationJob`
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_custom_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_custom_models)
         """
 
+    def list_evaluation_jobs(
+        self,
+        *,
+        creationTimeAfter: TimestampTypeDef = ...,
+        creationTimeBefore: TimestampTypeDef = ...,
+        statusEquals: EvaluationJobStatusType = ...,
+        nameContains: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        sortBy: Literal["CreationTime"] = ...,
+        sortOrder: SortOrderType = ...,
+    ) -> ListEvaluationJobsResponseTypeDef:
+        """
+        Lists model evaluation jobs.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_evaluation_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_evaluation_jobs)
+        """
+
     def list_foundation_models(
         self,
         *,
         byProvider: str = ...,
         byCustomizationType: ModelCustomizationType = ...,
         byOutputModality: ModelModalityType = ...,
-        byInferenceType: InferenceTypeType = ...
+        byInferenceType: InferenceTypeType = ...,
     ) -> ListFoundationModelsResponseTypeDef:
         """
-        List of Amazon Bedrock foundation models that you can use.
+        Lists Amazon Bedrock foundation models that you can use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_foundation_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_foundation_models)
         """
 
+    def list_guardrails(
+        self, *, guardrailIdentifier: str = ..., maxResults: int = ..., nextToken: str = ...
+    ) -> ListGuardrailsResponseTypeDef:
+        """
+        Lists details about all the guardrails in an account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_guardrails)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_guardrails)
+        """
+
     def list_model_customization_jobs(
         self,
         *,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListModelCustomizationJobsResponseTypeDef:
         """
         Returns a list of model customization jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_model_customization_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_model_customization_jobs)
         """
@@ -311,18 +442,18 @@
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: Literal["CreationTime"] = ...,
-        sortOrder: SortOrderType = ...
+        sortOrder: SortOrderType = ...,
     ) -> ListProvisionedModelThroughputsResponseTypeDef:
         """
-        List the provisioned capacities.
+        Lists the Provisioned Throughputs in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_provisioned_model_throughputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#list_provisioned_model_throughputs)
         """
 
     def list_tags_for_resource(self, *, resourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -338,14 +469,22 @@
         """
         Set the configuration values for model invocation logging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.put_model_invocation_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#put_model_invocation_logging_configuration)
         """
 
+    def stop_evaluation_job(self, *, jobIdentifier: str) -> Dict[str, Any]:
+        """
+        Stops an in progress model evaluation job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.stop_evaluation_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#stop_evaluation_job)
+        """
+
     def stop_model_customization_job(self, *, jobIdentifier: str) -> Dict[str, Any]:
         """
         Stops an active model customization job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.stop_model_customization_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#stop_model_customization_job)
         """
@@ -362,23 +501,44 @@
         """
         Remove one or more tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#untag_resource)
         """
 
+    def update_guardrail(
+        self,
+        *,
+        guardrailIdentifier: str,
+        name: str,
+        blockedInputMessaging: str,
+        blockedOutputsMessaging: str,
+        description: str = ...,
+        topicPolicyConfig: GuardrailTopicPolicyConfigTypeDef = ...,
+        contentPolicyConfig: GuardrailContentPolicyConfigTypeDef = ...,
+        wordPolicyConfig: GuardrailWordPolicyConfigTypeDef = ...,
+        sensitiveInformationPolicyConfig: GuardrailSensitiveInformationPolicyConfigTypeDef = ...,
+        kmsKeyId: str = ...,
+    ) -> UpdateGuardrailResponseTypeDef:
+        """
+        Updates a guardrail with the values you specify.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.update_guardrail)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#update_guardrail)
+        """
+
     def update_provisioned_model_throughput(
         self,
         *,
         provisionedModelId: str,
         desiredProvisionedModelName: str = ...,
-        desiredModelId: str = ...
+        desiredModelId: str = ...,
     ) -> Dict[str, Any]:
         """
-        Update a provisioned throughput.
+        Updates the name or associated model for a Provisioned Throughput.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.update_provisioned_model_throughput)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#update_provisioned_model_throughput)
         """
 
     @overload
     def get_paginator(
@@ -387,14 +547,30 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_evaluation_jobs"]
+    ) -> ListEvaluationJobsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_guardrails"]) -> ListGuardrailsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_model_customization_jobs"]
     ) -> ListModelCustomizationJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/paginator.py` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/paginator.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -7,64 +7,73 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_bedrock.client import BedrockClient
     from mypy_boto3_bedrock.paginator import (
         ListCustomModelsPaginator,
+        ListEvaluationJobsPaginator,
+        ListGuardrailsPaginator,
         ListModelCustomizationJobsPaginator,
         ListProvisionedModelThroughputsPaginator,
     )
 
     session = Session()
     client: BedrockClient = session.client("bedrock")
 
     list_custom_models_paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")
+    list_evaluation_jobs_paginator: ListEvaluationJobsPaginator = client.get_paginator("list_evaluation_jobs")
+    list_guardrails_paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")
     list_model_customization_jobs_paginator: ListModelCustomizationJobsPaginator = client.get_paginator("list_model_customization_jobs")
     list_provisioned_model_throughputs_paginator: ListProvisionedModelThroughputsPaginator = client.get_paginator("list_provisioned_model_throughputs")
     ```
 """
 
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import FineTuningJobStatusType, ProvisionedModelStatusType, SortOrderType
+from .literals import (
+    EvaluationJobStatusType,
+    FineTuningJobStatusType,
+    ProvisionedModelStatusType,
+    SortOrderType,
+)
 from .type_defs import (
     ListCustomModelsResponseTypeDef,
+    ListEvaluationJobsResponseTypeDef,
+    ListGuardrailsResponseTypeDef,
     ListModelCustomizationJobsResponseTypeDef,
     ListProvisionedModelThroughputsResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListCustomModelsPaginator",
+    "ListEvaluationJobsPaginator",
+    "ListGuardrailsPaginator",
     "ListModelCustomizationJobsPaginator",
     "ListProvisionedModelThroughputsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListCustomModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListCustomModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listcustommodelspaginator)
     """
 
     def paginate(
@@ -73,21 +82,56 @@
         creationTimeBefore: TimestampTypeDef = ...,
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListCustomModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListCustomModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listcustommodelspaginator)
         """
 
+class ListEvaluationJobsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListEvaluationJobs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listevaluationjobspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        creationTimeAfter: TimestampTypeDef = ...,
+        creationTimeBefore: TimestampTypeDef = ...,
+        statusEquals: EvaluationJobStatusType = ...,
+        nameContains: str = ...,
+        sortBy: Literal["CreationTime"] = ...,
+        sortOrder: SortOrderType = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListEvaluationJobsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListEvaluationJobs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listevaluationjobspaginator)
+        """
+
+class ListGuardrailsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListGuardrails)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listguardrailspaginator)
+    """
+
+    def paginate(
+        self, *, guardrailIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListGuardrailsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListGuardrails.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listguardrailspaginator)
+        """
 
 class ListModelCustomizationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListModelCustomizationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listmodelcustomizationjobspaginator)
     """
 
@@ -96,22 +140,21 @@
         *,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListModelCustomizationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListModelCustomizationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listmodelcustomizationjobspaginator)
         """
 
-
 class ListProvisionedModelThroughputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListProvisionedModelThroughputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listprovisionedmodelthroughputspaginator)
     """
 
     def paginate(
@@ -120,13 +163,13 @@
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListProvisionedModelThroughputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListProvisionedModelThroughputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listprovisionedmodelthroughputspaginator)
         """
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock/paginator.pyi` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock/paginator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,60 +7,75 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_bedrock.client import BedrockClient
     from mypy_boto3_bedrock.paginator import (
         ListCustomModelsPaginator,
+        ListEvaluationJobsPaginator,
+        ListGuardrailsPaginator,
         ListModelCustomizationJobsPaginator,
         ListProvisionedModelThroughputsPaginator,
     )
 
     session = Session()
     client: BedrockClient = session.client("bedrock")
 
     list_custom_models_paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")
+    list_evaluation_jobs_paginator: ListEvaluationJobsPaginator = client.get_paginator("list_evaluation_jobs")
+    list_guardrails_paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")
     list_model_customization_jobs_paginator: ListModelCustomizationJobsPaginator = client.get_paginator("list_model_customization_jobs")
     list_provisioned_model_throughputs_paginator: ListProvisionedModelThroughputsPaginator = client.get_paginator("list_provisioned_model_throughputs")
     ```
 """
 
 import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import FineTuningJobStatusType, ProvisionedModelStatusType, SortOrderType
+from .literals import (
+    EvaluationJobStatusType,
+    FineTuningJobStatusType,
+    ProvisionedModelStatusType,
+    SortOrderType,
+)
 from .type_defs import (
     ListCustomModelsResponseTypeDef,
+    ListEvaluationJobsResponseTypeDef,
+    ListGuardrailsResponseTypeDef,
     ListModelCustomizationJobsResponseTypeDef,
     ListProvisionedModelThroughputsResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ListCustomModelsPaginator",
+    "ListEvaluationJobsPaginator",
+    "ListGuardrailsPaginator",
     "ListModelCustomizationJobsPaginator",
     "ListProvisionedModelThroughputsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListCustomModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListCustomModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listcustommodelspaginator)
     """
 
     def paginate(
@@ -69,21 +84,60 @@
         creationTimeBefore: TimestampTypeDef = ...,
         creationTimeAfter: TimestampTypeDef = ...,
         nameContains: str = ...,
         baseModelArnEquals: str = ...,
         foundationModelArnEquals: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListCustomModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListCustomModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listcustommodelspaginator)
         """
 
+
+class ListEvaluationJobsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListEvaluationJobs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listevaluationjobspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        creationTimeAfter: TimestampTypeDef = ...,
+        creationTimeBefore: TimestampTypeDef = ...,
+        statusEquals: EvaluationJobStatusType = ...,
+        nameContains: str = ...,
+        sortBy: Literal["CreationTime"] = ...,
+        sortOrder: SortOrderType = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListEvaluationJobsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListEvaluationJobs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listevaluationjobspaginator)
+        """
+
+
+class ListGuardrailsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListGuardrails)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listguardrailspaginator)
+    """
+
+    def paginate(
+        self, *, guardrailIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListGuardrailsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListGuardrails.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listguardrailspaginator)
+        """
+
+
 class ListModelCustomizationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListModelCustomizationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listmodelcustomizationjobspaginator)
     """
 
     def paginate(
@@ -91,21 +145,22 @@
         *,
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: FineTuningJobStatusType = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListModelCustomizationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListModelCustomizationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listmodelcustomizationjobspaginator)
         """
 
+
 class ListProvisionedModelThroughputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListProvisionedModelThroughputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listprovisionedmodelthroughputspaginator)
     """
 
     def paginate(
@@ -114,13 +169,13 @@
         creationTimeAfter: TimestampTypeDef = ...,
         creationTimeBefore: TimestampTypeDef = ...,
         statusEquals: ProvisionedModelStatusType = ...,
         modelArnEquals: str = ...,
         nameContains: str = ...,
         sortBy: Literal["CreationTime"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListProvisionedModelThroughputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Paginator.ListProvisionedModelThroughputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/paginators/#listprovisionedmodelthroughputspaginator)
         """
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/PKG-INFO` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock
-Version: 1.34.0
-Summary: Type annotations for boto3.Bedrock 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.90
+Summary: Type annotations for boto3.Bedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/
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
 
 <a id="mypy-boto3-bedrock"></a>
 
 # mypy-boto3-bedrock
 
 [![PyPI - mypy-boto3-bedrock](https://img.shields.io/pypi/v/mypy-boto3-bedrock.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock)](https://pepy.tech/project/mypy-boto3-bedrock)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Bedrock 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
+[boto3.Bedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
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
 [mypy-boto3-bedrock docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,23 +281,29 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_bedrock import BedrockClient
 from mypy_boto3_bedrock.paginator import (
     ListCustomModelsPaginator,
+    ListEvaluationJobsPaginator,
+    ListGuardrailsPaginator,
     ListModelCustomizationJobsPaginator,
     ListProvisionedModelThroughputsPaginator,
 )
 
 client: BedrockClient = Session().client("bedrock")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_custom_models_paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")
+list_evaluation_jobs_paginator: ListEvaluationJobsPaginator = client.get_paginator(
+    "list_evaluation_jobs"
+)
+list_guardrails_paginator: ListGuardrailsPaginator = client.get_paginator("list_guardrails")
 list_model_customization_jobs_paginator: ListModelCustomizationJobsPaginator = client.get_paginator(
     "list_model_customization_jobs"
 )
 list_provisioned_model_throughputs_paginator: ListProvisionedModelThroughputsPaginator = (
     client.get_paginator("list_provisioned_model_throughputs")
 )
 ```
```

### Comparing `mypy-boto3-bedrock-1.34.0/mypy_boto3_bedrock.egg-info/SOURCES.txt` & `mypy_boto3_bedrock-1.34.90/mypy_boto3_bedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-bedrock-1.34.0/setup.py` & `mypy_boto3_bedrock-1.34.90/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock",
-    version="1.34.0",
+    version="1.34.90",
     packages=["mypy_boto3_bedrock"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Bedrock 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.Bedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 bedrock type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_bedrock": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

