# Comparing `tmp/llama_index_llms_nvidia_tensorrt-0.1.4.tar.gz` & `tmp/llama_index_llms_nvidia_tensorrt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_nvidia_tensorrt-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_nvidia_tensorrt-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_nvidia_tensorrt-0.1.4.tar` & `llama_index_llms_nvidia_tensorrt-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-02-13 13:53:01.675336 llama_index_llms_nvidia_tensorrt-0.1.4/README.md
--rw-r--r--   0        0        0       99 2024-02-13 13:53:01.675586 llama_index_llms_nvidia_tensorrt-0.1.4/llama_index/llms/nvidia_tensorrt/__init__.py
--rw-r--r--   0        0        0    10710 2024-02-20 22:37:41.312625 llama_index_llms_nvidia_tensorrt-0.1.4/llama_index/llms/nvidia_tensorrt/base.py
--rw-r--r--   0        0        0     2575 2024-02-13 13:53:01.675754 llama_index_llms_nvidia_tensorrt-0.1.4/llama_index/llms/nvidia_tensorrt/utils.py
--rw-r--r--   0        0        0     1500 2024-02-21 17:52:21.978740 llama_index_llms_nvidia_tensorrt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 llama_index_llms_nvidia_tensorrt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_tensorrt-0.1.5/README.md
+-rw-r--r--   0        0        0     1647 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_tensorrt-0.1.5/llama_index/llms/nvidia_tensorrt/__init__.py
+-rw-r--r--   0        0        0    14855 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_tensorrt-0.1.5/llama_index/llms/nvidia_tensorrt/base.py
+-rw-r--r--   0        0        0     4123 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_tensorrt-0.1.5/llama_index/llms/nvidia_tensorrt/utils.py
+-rw-r--r--   0        0        0     1500 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_tensorrt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 llama_index_llms_nvidia_tensorrt-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_nvidia_tensorrt-0.1.4/llama_index/llms/nvidia_tensorrt/base.py` & `llama_index_llms_nvidia_tensorrt-0.1.5/llama_index/llms/nvidia_tensorrt/base.py`

 * *Files 27% similar despite different names*

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
 import gc
 import json
 import os
 import time
 from pathlib import Path
 from typing import Any, Callable, Dict, Optional, Sequence
 
@@ -31,14 +57,61 @@
 from transformers import AutoTokenizer
 
 EOS_TOKEN = 2
 PAD_TOKEN = 2
 
 
 class LocalTensorRTLLM(CustomLLM):
+    r"""Local TensorRT LLM.
+
+    [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) provides users with an easy-to-use Python API to define Large Language Models (LLMs) and build TensorRT engines that contain state-of-the-art optimizations to perform inference
+    efficiently on NVIDIA GPUs.
+
+    Since TensorRT-LLM is a SDK for interacting with local models in process there are a few environment steps that must be followed to ensure that the TensorRT-LLM setup can be used.
+
+    1. Nvidia Cuda 12.2 or higher is currently required to run TensorRT-LLM
+    2. Install `tensorrt_llm` via pip with `pip3 install tensorrt_llm -U --extra-index-url https://pypi.nvidia.com`
+    3. For this example we will use Llama2. The Llama2 model files need to be created via scripts following the instructions
+    (https://github.com/NVIDIA/trt-llm-rag-windows/blob/release/1.0/README.md#building-trt-engine)
+        * The following files will be created from following the stop above
+        * `Llama_float16_tp1_rank0.engine`: The main output of the build script, containing the executable graph of operations with the model weights embedded.
+        * `config.json`: Includes detailed information about the model, like its general structure and precision, as well as information about which plug-ins were incorporated into the engine.
+        * `model.cache`: Caches some of the timing and optimization information from model compilation, making successive builds quicker.
+    4. `mkdir model`
+    5. Move all of the files mentioned above to the model directory.
+
+    Examples:
+        `pip install llama-index-llms-nvidia-tensorrt`
+
+        ```python
+        from llama_index.llms.nvidia_tensorrt import LocalTensorRTLLM
+
+
+        def completion_to_prompt(completion):
+            return f"<s> [INST] {completion} [/INST] "
+
+        def messages_to_prompt(messages):
+            content = ""
+            for message in messages:
+                content += str(message) + "\n"
+            return f"<s> [INST] {content} [/INST] "
+
+        llm = LocalTensorRTLLM(
+            model_path="./model",
+            engine_name="llama_float16_tp1_rank0.engine",
+            tokenizer_dir="meta-llama/Llama-2-13b-chat",
+            completion_to_prompt=completion_to_prompt,
+            messages_to_prompt=messages_to_prompt,
+        )
+
+        resp = llm.complete("Who is Paul Graham?")
+        print(str(resp))
+        ```
+    """
+
     model_path: Optional[str] = Field(description="The path to the trt engine.")
     temperature: float = Field(description="The temperature to use for sampling.")
     max_new_tokens: int = Field(description="The maximum number of tokens to generate.")
     context_window: int = Field(
         description="The maximum number of context tokens for the model."
     )
     messages_to_prompt: Callable = Field(
@@ -107,15 +180,17 @@
                 with open(config_path) as f:
                     config = json.load(f)
                 use_gpt_attention_plugin = config["plugin_config"][
                     "gpt_attention_plugin"
                 ]
                 remove_input_padding = config["plugin_config"]["remove_input_padding"]
                 tp_size = config["builder_config"]["tensor_parallel"]
-                pp_size = config["builder_config"]["pipeline_parallel"]
+                pp_size = 1
+                if "pipeline_parallel" in config["builder_config"]:
+                    pp_size = config["builder_config"]["pipeline_parallel"]
                 world_size = tp_size * pp_size
                 assert (
                     world_size == tensorrt_llm.mpi_world_size()
                 ), f"Engine world size ({world_size}) != Runtime world size ({tensorrt_llm.mpi_world_size()})"
                 num_heads = config["builder_config"]["num_heads"] // tp_size
                 hidden_size = config["builder_config"]["hidden_size"] // tp_size
                 vocab_size = config["builder_config"]["vocab_size"]
@@ -134,14 +209,15 @@
                     num_kv_heads=num_kv_heads,
                     hidden_size=hidden_size,
                     vocab_size=vocab_size,
                     num_layers=num_layers,
                     gpt_attention_plugin=use_gpt_attention_plugin,
                     paged_kv_cache=paged_kv_cache,
                     remove_input_padding=remove_input_padding,
+                    max_batch_size=config["builder_config"]["max_batch_size"],
                 )
 
                 assert (
                     pp_size == 1
                 ), "Python runtime does not support pipeline parallelism"
                 world_size = tp_size * pp_size
```

### Comparing `llama_index_llms_nvidia_tensorrt-0.1.4/pyproject.toml` & `llama_index_llms_nvidia_tensorrt-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms nvidia tensorrt integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-nvidia-tensorrt"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 torch = "^2.1.2"
 transformers = "^4.37.0"
```

### Comparing `llama_index_llms_nvidia_tensorrt-0.1.4/PKG-INFO` & `llama_index_llms_nvidia_tensorrt-0.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-nvidia-tensorrt
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index llms nvidia tensorrt integration
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
 Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: transformers (>=4.37.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Nvidia Tensorrt
```

