# Comparing `tmp/openinference_instrumentation_llama_index-1.2.1.tar.gz` & `tmp/openinference_instrumentation_llama_index-1.2.2.tar.gz`

## Comparing `openinference_instrumentation_llama_index-1.2.1.tar` & `openinference_instrumentation_llama_index-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/src/openinference/instrumentation/llama_index/__init__.py
--rw-r--r--   0        0        0    31099 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/src/openinference/instrumentation/llama_index/_callback.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/src/openinference/instrumentation/llama_index/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/src/openinference/instrumentation/llama_index/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/src/openinference/instrumentation/llama_index/version.py
--rw-r--r--   0        0        0    15132 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/tests/openinference/instrumentation/llama_index/test_callback.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/LICENSE
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/README.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/__init__.py
+-rw-r--r--   0        0        0    31646 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/_callback.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/version.py
+-rw-r--r--   0        0        0    15132 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/tests/openinference/instrumentation/llama_index/test_callback.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/README.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.2.2/PKG-INFO
```

### Comparing `openinference_instrumentation_llama_index-1.2.1/src/openinference/instrumentation/llama_index/__init__.py` & `openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.1/src/openinference/instrumentation/llama_index/_callback.py` & `openinference_instrumentation_llama_index-1.2.2/src/openinference/instrumentation/llama_index/_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Dict,
     Iterable,
     Iterator,
     List,
     Mapping,
     Optional,
     OrderedDict,
+    SupportsFloat,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 from uuid import uuid4
 
@@ -667,14 +668,23 @@
         elif isinstance(value, List) and any(isinstance(item, Mapping) for item in value):
             for index, sub_mapping in enumerate(value):
                 for sub_key, sub_value in _flatten(sub_mapping):
                     yield f"{key}.{index}.{sub_key}", sub_value
         else:
             if isinstance(value, Enum):
                 value = value.value
+            elif isinstance(value, SupportsFloat) and not isinstance(
+                value,
+                (int, float, Iterable),
+            ):
+                # This is for when there are numpy values, which will be rejected by protobuf.
+                # We convert all of them to float, so we don't need a dependency on numpy.
+                # The check on Iterable is to avoid converting numpy arrays to float,
+                # because numpy arrays are instances of SupportsFloat.
+                value = float(value)
             yield key, value
 
 
 _BILLION = 1_000_000_000
 
 _SPAN_KINDS = MappingProxyType(
     {
```

### Comparing `openinference_instrumentation_llama_index-1.2.1/tests/openinference/instrumentation/llama_index/test_callback.py` & `openinference_instrumentation_llama_index-1.2.2/tests/openinference/instrumentation/llama_index/test_callback.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.1/LICENSE` & `openinference_instrumentation_llama_index-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.1/README.md` & `openinference_instrumentation_llama_index-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.1/pyproject.toml` & `openinference_instrumentation_llama_index-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.2.1/PKG-INFO` & `openinference_instrumentation_llama_index-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-llama-index
-Version: 1.2.1
+Version: 1.2.2
 Summary: OpenInference LlamaIndex Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-llama-index
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

