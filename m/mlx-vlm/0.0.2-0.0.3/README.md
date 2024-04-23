# Comparing `tmp/mlx_vlm-0.0.2.tar.gz` & `tmp/mlx_vlm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_vlm-0.0.2.tar", last modified: Tue Apr 23 00:48:08 2024, max compression
+gzip compressed data, was "mlx_vlm-0.0.3.tar", last modified: Tue Apr 23 14:10:54 2024, max compression
```

## Comparing `mlx_vlm-0.0.2.tar` & `mlx_vlm-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.615497 mlx_vlm-0.0.2/mlx_vlm/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.615497 mlx_vlm-0.0.2/mlx_vlm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.615497 mlx_vlm-0.0.2/mlx_vlm/models/llava/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/llava/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/nanoLlava.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/sample_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/tokenizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24904 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/mlx_vlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/mlx_vlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 00:48:08.000000 mlx_vlm-0.0.2/mlx_vlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 00:48:08.619497 mlx_vlm-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 00:48:00.000000 mlx_vlm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.566111 mlx_vlm-0.0.3/mlx_vlm/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm/models/llava/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/llava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/nanoLlava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/sample_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/tokenizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/mlx_vlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/mlx_vlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 14:10:54.000000 mlx_vlm-0.0.3/mlx_vlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:10:54.570111 mlx_vlm-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 14:10:45.000000 mlx_vlm-0.0.3/setup.py
```

### Comparing `mlx_vlm-0.0.2/LICENSE` & `mlx_vlm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/PKG-INFO` & `mlx_vlm-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_vlm-0.0.2/mlx_vlm/convert.py` & `mlx_vlm-0.0.3/mlx_vlm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/generate.py` & `mlx_vlm-0.0.3/mlx_vlm/generate.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/models/base.py` & `mlx_vlm-0.0.3/mlx_vlm/models/base.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/models/llava/language.py` & `mlx_vlm-0.0.3/mlx_vlm/models/llava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/models/llava/llava.py` & `mlx_vlm-0.0.3/mlx_vlm/models/llava/llava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/models/llava/vision.py` & `mlx_vlm-0.0.3/mlx_vlm/models/llava/vision.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,28 @@
             **{
                 k: v
                 for k, v in params.items()
                 if k in inspect.signature(cls).parameters
             }
         )
 
+def check_array_shape(arr):
+    shape = arr.shape
+
+    # Check if the shape has 4 dimensions
+    if len(shape) != 4:
+        return False
+
+    out_channels, kH, KW, _ = shape
+
+    # Check if out_channels is the largest, and kH and KW are the same
+    if (out_channels >= kH) and (out_channels >= KW) and (kH == KW):
+        return True
+    else:
+        return False
 
 class Attention(nn.Module):
     def __init__(
         self,
         dims: int,
         num_heads: int,
         query_input_dims: Optional[int] = None,
@@ -213,12 +227,15 @@
                 # Remove unused position_ids
                 continue
             elif "patch_embedding.weight" in k:
                 # PyTorch conv2d weight tensors have shape:
                 #   [out_channels, in_channels, kH, KW]
                 # MLX conv2d expects the weight be of shape:
                 #   [out_channels, kH, KW, in_channels]
-                sanitized_weights[k] = v.transpose(0, 2, 3, 1)
+                if check_array_shape(v):
+                    sanitized_weights[k] = v
+                else:
+                    sanitized_weights[k] = v.transpose(0, 2, 3, 1)
             else:
                 sanitized_weights[k] = v
 
         return sanitized_weights
```

### Comparing `mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/language.py` & `mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/nanoLlava.py` & `mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/nanoLlava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/models/nanoLlava/vision.py` & `mlx_vlm-0.0.3/mlx_vlm/models/nanoLlava/vision.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,28 @@
             **{
                 k: v
                 for k, v in params.items()
                 if k in inspect.signature(cls).parameters
             }
         )
 
+def check_array_shape(arr):
+    shape = arr.shape
+
+    # Check if the shape has 4 dimensions
+    if len(shape) != 4:
+        return False
+
+    out_channels, kH, KW, _ = shape
+
+    # Check if out_channels is the largest, and kH and KW are the same
+    if (out_channels >= kH) and (out_channels >= KW) and (kH == KW):
+        return True
+    else:
+        return False
 
 class Attention(nn.Module):
     def __init__(
         self,
         dims: int,
         num_heads: int,
         query_input_dims: Optional[int] = None,
@@ -274,12 +288,15 @@
                 # Remove unused position_ids
                 continue
             elif "patch_embedding.weight" in k:
                 # PyTorch conv2d weight tensors have shape:
                 #   [out_channels, in_channels, kH, KW]
                 # MLX conv2d expects the weight be of shape:
                 #   [out_channels, kH, KW, in_channels]
-                sanitized_weights[k] = v.transpose(0, 2, 3, 1)
+                if check_array_shape(v):
+                    sanitized_weights[k] = v
+                else:
+                    sanitized_weights[k] = v.transpose(0, 2, 3, 1)
             else:
                 sanitized_weights[k] = v
 
         return sanitized_weights
```

### Comparing `mlx_vlm-0.0.2/mlx_vlm/sample_utils.py` & `mlx_vlm-0.0.3/mlx_vlm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/tokenizer_utils.py` & `mlx_vlm-0.0.3/mlx_vlm/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/mlx_vlm/utils.py` & `mlx_vlm-0.0.3/mlx_vlm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,34 +142,25 @@
 
     if hasattr(model, "sanitize"):
         weights = model.sanitize(weights)
 
     weights = model_class.VisionModel(model_config.vision_config).sanitize(weights=weights)
     weights = model_class.LanguageModel(model_config.text_config).sanitize(weights=weights)
 
-    if quantization is not None:
-        # for legacy models that don't have lm_head quant due to non-32 dims
-        if "lm_head.scales" not in weights.keys():
-            vocab_size = config["vocab_size"]
-            extended_linear_class_predicate = (
-                lambda layer: linear_class_predicate(layer)
-                and layer.weight.shape[0] != vocab_size
-            )
-            nn.QuantizedLinear.quantize_module(
-                model,
-                **quantization,
-                linear_class_predicate=extended_linear_class_predicate,
-            )
-        # for models that have lm_head quant
-        else:
-            nn.QuantizedLinear.quantize_module(
-                model,
-                **quantization,
-                linear_class_predicate=linear_class_predicate,
-            )
+    if (quantization := config.get("quantization", None)) is not None:
+        # Handle legacy models which may not have everything quantized
+        class_predicate = (
+            lambda p, m: isinstance(m, (nn.Linear, nn.Embedding))
+            and f"{p}.scales" in weights
+        )
+        nn.quantize(
+            model,
+            **quantization,
+            class_predicate=class_predicate,
+        )
 
     model.load_weights(list(weights.items()))
     if not lazy:
         mx.eval(model.parameters())
 
     model.eval()
     return model
@@ -275,31 +266,31 @@
         path (str): Local path to the model.
         upload_repo (str): Name of the HF repo to upload to.
         hf_path (str): Path to the original Hugging Face model.
     """
     import os
 
     from huggingface_hub import HfApi, ModelCard, logging
+    from . import __version__
 
     card = ModelCard.load(hf_path)
     card.data.tags = ["mlx"] if card.data.tags is None else card.data.tags + ["mlx"]
     card.text = dedent(
         f"""
         # {upload_repo}
-        This model was converted to MLX format from [`{hf_path}`]() using mlx-vllm version **0.0.0**.
+        This model was converted to MLX format from [`{hf_path}`]() using mlx-vllm version **{__version__}**.
         Refer to the [original model card](https://huggingface.co/{hf_path}) for more details on the model.
         ## Use with mlx
 
         ```bash
-        git clone https://github.com/ml-explore/mlx-examples.git
+        pip install -U mlx-vlm
         ```
 
         ```bash
-        cd mlx-lm/vllms
-        python -m generate --model {path} --max-tokens 10 --temp 0.0
+        python -m mlx_vlm.generate --model {upload_repo} --max-tokens 100 --temp 0.0
         ```
         """
     )
     card.save(os.path.join(path, "README.md"))
 
     logging.set_verbosity_info()
 
@@ -413,14 +404,16 @@
     with open(save_path / "model.safetensors.index.json", "w") as f:
         json.dump(
             index_data,
             f,
             indent=4,
         )
 
+def class_predicate(path, m):
+    return isinstance(m, nn.Linear) and not isinstance(m, nn.Embedding)
 
 def quantize_model(
     model: nn.Module, config: dict, q_group_size: int, q_bits: int
 ) -> Tuple:
     """
     Applies quantization to the model weights.
 
@@ -430,15 +423,15 @@
         q_group_size (int): Group size for quantization.
         q_bits (int): Bits per weight for quantization.
 
     Returns:
         Tuple: Tuple containing quantized weights and config.
     """
     quantized_config = copy.deepcopy(config)
-    nn.quantize(model, q_group_size, q_bits)
+    nn.quantize(model, q_group_size, q_bits, class_predicate=class_predicate)
     quantized_config["quantization"] = {"group_size": q_group_size, "bits": q_bits}
     quantized_weights = dict(tree_flatten(model.parameters()))
 
     return quantized_weights, quantized_config
 
 
 def save_config(
@@ -504,15 +497,15 @@
     dtype: str = "float16",
     upload_repo: str = None,
     revision: Optional[str] = None,
     dequantize: bool = False,
 ):
     print("[INFO] Loading")
     model_path = get_model_path(hf_path, revision=revision)
-    model, config, tokenizer = fetch_from_hub(model_path, lazy=True)
+    model, config, tokenizer = fetch_from_hub(model_path, lazy=False)
 
     weights = dict(tree_flatten(model.parameters()))
     dtype = mx.float16 if quantize else getattr(mx, dtype)
     weights = {k: v.astype(dtype) for k, v in weights.items()}
 
     if quantize and dequantize:
         raise ValueError("Choose either quantize or dequantize, not both.")
@@ -533,22 +526,21 @@
     del model
     save_weights(mlx_path, weights, donate_weights=True)
 
     py_files = glob.glob(str(model_path / "*.py"))
     for file in py_files:
         shutil.copy(file, mlx_path)
 
-    if "tokenizer" in tokenizer.__dict__.keys():
-        tokenizer.tokenizer.save_pretrained(mlx_path)
-    else:
-        tokenizer.save_pretrained(mlx_path)
+
+    tokenizer.save_pretrained(mlx_path)
 
 
     save_config(config, config_path=mlx_path / "config.json")
 
+
     if upload_repo is not None:
         upload_to_hub(mlx_path, upload_repo, hf_path)
 
 def load_image(image_source):
     """
     Helper function to load an image from either a URL or file.
     """
```

### Comparing `mlx_vlm-0.0.2/mlx_vlm.egg-info/PKG-INFO` & `mlx_vlm-0.0.3/mlx_vlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_vlm-0.0.2/mlx_vlm.egg-info/SOURCES.txt` & `mlx_vlm-0.0.3/mlx_vlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.2/setup.py` & `mlx_vlm-0.0.3/setup.py`

 * *Files identical despite different names*

