# Comparing `tmp/llama_index_llms_nvidia_triton-0.1.3.tar.gz` & `tmp/llama_index_llms_nvidia_triton-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_nvidia_triton-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_llms_nvidia_triton-0.1.4.tar", max compression
```

## Comparing `llama_index_llms_nvidia_triton-0.1.3.tar` & `llama_index_llms_nvidia_triton-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       45 2024-02-13 13:53:01.676587 llama_index_llms_nvidia_triton-0.1.3/README.md
--rw-r--r--   0        0        0       89 2024-02-13 13:53:01.676780 llama_index_llms_nvidia_triton-0.1.3/llama_index/llms/nvidia_triton/__init__.py
--rw-r--r--   0        0        0     8408 2024-02-20 22:37:41.316799 llama_index_llms_nvidia_triton-0.1.3/llama_index/llms/nvidia_triton/base.py
--rw-r--r--   0        0        0    12063 2024-02-13 13:53:01.676968 llama_index_llms_nvidia_triton-0.1.3/llama_index/llms/nvidia_triton/utils.py
--rw-r--r--   0        0        0     1526 2024-02-21 17:53:26.276462 llama_index_llms_nvidia_triton-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 llama_index_llms_nvidia_triton-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/README.md
+-rw-r--r--   0        0        0     1637 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/__init__.py
+-rw-r--r--   0        0        0    10865 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/base.py
+-rw-r--r--   0        0        0    13918 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/utils.py
+-rw-r--r--   0        0        0     1526 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 llama_index_llms_nvidia_triton-0.1.4/PKG-INFO
```

### Comparing `llama_index_llms_nvidia_triton-0.1.3/llama_index/llms/nvidia_triton/base.py` & `llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+# Copyright 2023-2024, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions
+# are met:
+#  * Redistributions of source code must retain the above copyright
+#    notice, this list of conditions and the following disclaimer.
+#  * Redistributions in binary form must reproduce the above copyright
+#    notice, this list of conditions and the following disclaimer in the
+#    documentation and/or other materials provided with the distribution.
+#  * Neither the name of NVIDIA CORPORATION nor the names of its
+#    contributors may be used to endorse or promote products derived
+#    from this software without specific prior written permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS ``AS IS'' AND ANY
+# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+# PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT OWNER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
+# OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 import random
 from typing import (
     Any,
     Dict,
     Optional,
     Sequence,
 )
@@ -32,19 +58,44 @@
 DEFAULT_TEMPERATURE = 1.0
 DEFAULT_TOP_P = 0
 DEFAULT_TOP_K = 1.0
 DEFAULT_MAX_TOKENS = 100
 DEFAULT_BEAM_WIDTH = 1
 DEFAULT_REPTITION_PENALTY = 1.0
 DEFAULT_LENGTH_PENALTY = 1.0
-DEFAULT_REUSE_CLIENT = True
-DEFAULT_TRITON_LOAD_MODEL = True
+DEFAULT_REUSE_CLIENT = False
+DEFAULT_TRITON_LOAD_MODEL = False
 
 
 class NvidiaTriton(LLM):
+    """Nvidia Triton LLM.
+
+    Nvidia's Triton is an inference server that provides API access to hosted LLM models. This connector allows for llama_index to remotely interact with a Triton inference server over GRPC to
+    accelerate inference operations.
+
+    [Triton Inference Server Github](https://github.com/triton-inference-server/server)
+
+    Examples:
+        `pip install llama-index-llms-nvidia-triton`
+
+        ```python
+        from llama_index.llms.nvidia_triton import NvidiaTriton
+
+        # Ensure a Triton server instance is running and provide the correct URL for your Triton server instance
+        triton_url = "localhost:8001"
+
+        # Instantiate the NvidiaTriton class
+        triton_client = NvidiaTriton()
+
+        # Call the complete method with a prompt
+        resp = triton_client.complete("The tallest mountain in North America is ")
+        print(resp)
+        ```
+    """
+
     server_url: str = Field(
         default=DEFAULT_SERVER_URL,
         description="The URL of the Triton inference server to use.",
     )
     model_name: str = Field(
         default=DEFAULT_MODEL,
         description="The name of the Triton hosted model this client should use",
@@ -206,15 +257,14 @@
 
         if self.triton_load_model_call:
             client.load_model(model_params["model_name"])
 
         result_queue = client.request_streaming(
             model_params["model_name"], request_id, **invocation_params
         )
-
         response = ""
         for token in result_queue:
             if isinstance(token, InferenceServerException):
                 client.stop_stream(model_params["model_name"], request_id)
                 raise token
             response = response + token
```

### Comparing `llama_index_llms_nvidia_triton-0.1.3/llama_index/llms/nvidia_triton/utils.py` & `llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+# Copyright 2023-2024, NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions
+# are met:
+#  * Redistributions of source code must retain the above copyright
+#    notice, this list of conditions and the following disclaimer.
+#  * Redistributions in binary form must reproduce the above copyright
+#    notice, this list of conditions and the following disclaimer in the
+#    documentation and/or other materials provided with the distribution.
+#  * Neither the name of NVIDIA CORPORATION nor the names of its
+#    contributors may be used to endorse or promote products derived
+#    from this software without specific prior written permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS ``AS IS'' AND ANY
+# EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+# PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT OWNER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+# EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+# PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+# PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
+# OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 import abc
 import json
 import random
 import time
 from functools import partial
 from queue import Queue
 from typing import (
@@ -21,38 +47,47 @@
 RANDOM_SEED = 0
 
 
 class StreamingResponseGenerator(Queue):
     """A Generator that provides the inference results from an LLM."""
 
     def __init__(
-        self, client: "GrpcTritonClient", request_id: str, force_batch: bool
+        self,
+        client: "GrpcTritonClient",
+        request_id: str,
+        force_batch: bool,
+        model_name: str,
+        max_tokens: int,
     ) -> None:
         """Instantiate the generator class."""
         super().__init__()
         self._client = client
         self.request_id = request_id
         self._batch = force_batch
+        self._model_name = model_name
+        self._max_tokens = max_tokens
+        self._counter = 0
 
     def __iter__(self) -> "StreamingResponseGenerator":
         """Return self as a generator."""
         return self
 
     def __next__(self) -> str:
         """Return the next retrieved token."""
         val = self.get()
-        if val is None or val in STOP_WORDS:
+        if val is None or val in STOP_WORDS or self._counter == self._max_tokens - 1:
             self._stop_stream()
             raise StopIteration
+        self._counter += 1
         return val
 
     def _stop_stream(self) -> None:
         """Drain and shutdown the Triton stream."""
         self._client.stop_stream(
-            "tensorrt_llm", self.request_id, signal=not self._batch
+            self._model_name, self.request_id, signal=not self._batch
         )
 
 
 class _BaseTritonClient(abc.ABC):
     """An abstraction of the connection to a triton inference server."""
 
     def __init__(self, server_url: str) -> None:
@@ -159,24 +194,24 @@
         beam_width: int = 1,
         repetition_penalty: float = 1,
         length_penalty: float = 1.0,
         stream: bool = True,
     ) -> List[Union["grpcclient.InferInput", "httpclient.InferInput"]]:
         """Create the input for the triton inference server."""
         query = np.array(prompt).astype(object)
-        request_output_len = np.array([tokens]).astype(np.uint32).reshape((1, -1))
-        runtime_top_k = np.array([top_k]).astype(np.uint32).reshape((1, -1))
+        request_output_len = np.array([tokens]).astype(np.int32).reshape((1, -1))
+        runtime_top_k = np.array([top_k]).astype(np.int32).reshape((1, -1))
         runtime_top_p = np.array([top_p]).astype(np.float32).reshape((1, -1))
         temperature_array = np.array([temperature]).astype(np.float32).reshape((1, -1))
         len_penalty = np.array([length_penalty]).astype(np.float32).reshape((1, -1))
         repetition_penalty_array = (
             np.array([repetition_penalty]).astype(np.float32).reshape((1, -1))
         )
         random_seed = np.array([RANDOM_SEED]).astype(np.uint64).reshape((1, -1))
-        beam_width_array = np.array([beam_width]).astype(np.uint32).reshape((1, -1))
+        beam_width_array = np.array([beam_width]).astype(np.int32).reshape((1, -1))
         streaming_data = np.array([[stream]], dtype=bool)
 
         return [
             self._prepare_tensor("text_input", query),
             self._prepare_tensor("max_tokens", request_output_len),
             self._prepare_tensor("top_k", runtime_top_k),
             self._prepare_tensor("top_p", runtime_top_p),
@@ -314,16 +349,18 @@
         """Request a streaming connection."""
         if not self._client.is_model_ready(model_name):
             raise RuntimeError("Cannot request streaming, model is not loaded")
 
         if not request_id:
             request_id = str(random.randint(1, 9999999))  # nosec
 
-        result_queue = StreamingResponseGenerator(self, request_id, force_batch)
         inputs = self._generate_inputs(stream=not force_batch, **params)
+        result_queue = StreamingResponseGenerator(
+            self, request_id, force_batch, model_name, max_tokens=params["tokens"]
+        )
         outputs = self._generate_outputs()
         self._send_prompt_streaming(
             model_name,
             inputs,
             outputs,
             request_id,
             result_queue,
```

### Comparing `llama_index_llms_nvidia_triton-0.1.3/pyproject.toml` & `llama_index_llms_nvidia_triton-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms nvidia triton integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-nvidia-triton"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.dependencies.tritonclient]
 extras = ["all"]
```

### Comparing `llama_index_llms_nvidia_triton-0.1.3/PKG-INFO` & `llama_index_llms_nvidia_triton-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-nvidia-triton
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index llms nvidia triton integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: tritonclient[all] (>=2.41.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Nvidia Triton
```

