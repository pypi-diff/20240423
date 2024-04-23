# Comparing `tmp/ragas_haystack-0.1.3.tar.gz` & `tmp/ragas_haystack-0.2.0.tar.gz`

## Comparing `ragas_haystack-0.1.3.tar` & `ragas_haystack-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/example/example.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/pydoc/config.yml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/evaluator.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/metrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0    13780 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/tests/test_evaluator.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/tests/test_metrics.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/README.md
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/example/example.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/pydoc/config.yml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/src/haystack_integrations/components/evaluators/ragas/__init__.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/src/haystack_integrations/components/evaluators/ragas/evaluator.py
+-rw-r--r--   0        0        0    12683 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/src/haystack_integrations/components/evaluators/ragas/metrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    13780 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/tests/test_evaluator.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/tests/test_metrics.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/README.md
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 ragas_haystack-0.2.0/PKG-INFO
```

### Comparing `ragas_haystack-0.1.3/example/example.py` & `ragas_haystack-0.2.0/example/example.py`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.3/pydoc/config.yml` & `ragas_haystack-0.2.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/evaluator.py` & `ragas_haystack-0.2.0/src/haystack_integrations/components/evaluators/ragas/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from typing import Any, Callable, Dict, List, Optional, Union
 
-from datasets import Dataset  # type: ignore
+from datasets import Dataset
 from haystack import DeserializationError, component, default_from_dict, default_to_dict
 
 from ragas import evaluate  # type: ignore
-from ragas.evaluation import Result  # type: ignore
-from ragas.metrics.base import Metric  # type: ignore
+from ragas.evaluation import Result
+from ragas.metrics.base import Metric
 
 from .metrics import (
     METRIC_DESCRIPTORS,
     InputConverters,
     OutputConverters,
     RagasMetric,
 )
```

### Comparing `ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/metrics.py` & `ragas_haystack-0.2.0/src/haystack_integrations/components/evaluators/ragas/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     AspectCritique,  # type: ignore
     ContextPrecision,  # type: ignore
     ContextRecall,  # type: ignore
     ContextRelevancy,  # type: ignore
     ContextUtilization,  # type: ignore
     Faithfulness,  # type: ignore
 )
-from ragas.metrics.base import Metric  # type: ignore
+from ragas.metrics.base import Metric
 
 
 class RagasBaseEnum(Enum):
     """
     Base functionality for a Ragas enum.
     """
```

### Comparing `ragas_haystack-0.1.3/tests/test_evaluator.py` & `ragas_haystack-0.2.0/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.3/.gitignore` & `ragas_haystack-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.3/LICENSE.txt` & `ragas_haystack-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.3/README.md` & `ragas_haystack-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.3/pyproject.toml` & `ragas_haystack-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["haystack-ai", "ragas==0.1.1"]
+dependencies = ["haystack-ai", "ragas"]
 
 [project.urls]
 Source = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ragas"
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/ragas/README.md"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 
 [tool.hatch.build.targets.wheel]
@@ -148,12 +148,13 @@
 
 
 [[tool.mypy.overrides]]
 module = [
   "haystack.*",
   "pytest.*",
   "ragas.*",
+  "datasets.*",
   "numpy",
   "grpc",
   "haystack_integrations.*",
 ]
 ignore_missing_imports = true
```

### Comparing `ragas_haystack-0.1.3/PKG-INFO` & `ragas_haystack-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragas-haystack
-Version: 0.1.3
+Version: 0.2.0
 Summary: An integration of Ragas LLM evaluation framework with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ragas
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/ragas/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: haystack-ai
-Requires-Dist: ragas==0.1.1
+Requires-Dist: ragas
 Description-Content-Type: text/markdown
 
 # ragas-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ragas-haystack.svg)](https://pypi.org/project/ragas-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ragas-haystack.svg)](https://pypi.org/project/ragas-haystack)
```

