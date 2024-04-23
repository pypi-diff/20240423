# Comparing `tmp/hypothesis_torch-0.1.8.tar.gz` & `tmp/hypothesis_torch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.1.8.tar", last modified: Mon Apr 22 03:10:18 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.1.9.tar", last modified: Mon Apr 22 17:23:53 2024, max compression
```

## Comparing `hypothesis_torch-0.1.8.tar` & `hypothesis_torch-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 03:10:18.032761 hypothesis_torch-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8085 2024-04-22 03:10:18.032761 hypothesis_torch-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5272 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 03:10:18.028761 hypothesis_torch-0.1.8/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)      523 2024-04-22 03:10:15.000000 hypothesis_torch-0.1.8/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1454 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2262 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)     8347 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 03:10:18.032761 hypothesis_torch-0.1.8/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8085 2024-04-22 03:10:18.000000 hypothesis_torch-0.1.8/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2024-04-22 03:10:18.000000 hypothesis_torch-0.1.8/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 03:10:18.000000 hypothesis_torch-0.1.8/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-22 03:10:18.000000 hypothesis_torch-0.1.8/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-22 03:10:18.000000 hypothesis_torch-0.1.8/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2090 2024-04-22 03:09:45.000000 hypothesis_torch-0.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 03:10:18.032761 hypothesis_torch-0.1.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8097 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5285 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:23:53.227512 hypothesis_torch-0.1.9/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)      523 2024-04-22 17:23:49.000000 hypothesis_torch-0.1.9/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)     9278 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8097 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/setup.cfg
```

### Comparing `hypothesis_torch-0.1.8/LICENSE` & `hypothesis_torch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.8/PKG-INFO` & `hypothesis_torch-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -162,15 +162,15 @@
 optional arguments for the input size, output size, and number of hidden layers. Each of these arguments can be 
 specified as a fixed value or as a strategy. For example, to generate a fully-connected neural network with an input
 size of 10, an output size of 5, and 3 hidden layers with sizes between 5 and 10:
 
 ```python
 import hypothesis_torch
 from hypothesis import strategies as st
-hypothesis_torch.linear_network_strategy(input_shape=(1,10), output_shape=(1,5), hidden_layer_size=st.integers(5, 10), depth=3)
+hypothesis_torch.linear_network_strategy(input_shape=(1,10), output_shape=(1,5), hidden_layer_size=st.integers(5, 10), num_hidden_layers=3)
 ```
 
 #### Hugging Face Transformer Models
 
 Hugging Face transformer models can be generated with the `transformer_strategy` function. This function takes in any
 Hugging Face `PreTrainedModel` subclass (or a strategy that generates references `PreTrainedModel` subclasses) and 
 returns an instance of that model. For example, to generate an arbitrary Llama2 model:
```

### Comparing `hypothesis_torch-0.1.8/README.md` & `hypothesis_torch-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 optional arguments for the input size, output size, and number of hidden layers. Each of these arguments can be 
 specified as a fixed value or as a strategy. For example, to generate a fully-connected neural network with an input
 size of 10, an output size of 5, and 3 hidden layers with sizes between 5 and 10:
 
 ```python
 import hypothesis_torch
 from hypothesis import strategies as st
-hypothesis_torch.linear_network_strategy(input_shape=(1,10), output_shape=(1,5), hidden_layer_size=st.integers(5, 10), depth=3)
+hypothesis_torch.linear_network_strategy(input_shape=(1,10), output_shape=(1,5), hidden_layer_size=st.integers(5, 10), num_hidden_layers=3)
 ```
 
 #### Hugging Face Transformer Models
 
 Hugging Face transformer models can be generated with the `transformer_strategy` function. This function takes in any
 Hugging Face `PreTrainedModel` subclass (or a strategy that generates references `PreTrainedModel` subclasses) and 
 returns an instance of that model. For example, to generate an arbitrary Llama2 model:
@@ -134,8 +134,8 @@
 import transformers
 from hypothesis import strategies as st
 hypothesis_torch.transformer_strategy(transformers.LlamaForCausalLM, hidden_size=st.integers(64, 128), vocab_size=1000)
 ```
 
 [! Note]
     Currently, the `transformer_strategy` only accepts `kwargs` that can be passed to the constructor of the model's 
-    config class. Thus, it cannot currently replicate all of the behavior of calling `from_pretrained` on a model class.
+    config class. Thus, it cannot currently replicate all of the behavior of calling `from_pretrained` on a model class.
```

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/__init__.py` & `hypothesis_torch-0.1.9/hypothesis_torch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Root imports for hypothesis-torch."""
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 import importlib.util
 
 from hypothesis_torch.device import device_strategy
 from hypothesis_torch.dtype import dtype_strategy
 from hypothesis_torch.module import linear_network_strategy, same_shape_activation_strategy
 from hypothesis_torch.tensor import tensor_strategy
```

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/device.py` & `hypothesis_torch-0.1.9/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/dtype.py` & `hypothesis_torch-0.1.9/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.1.9/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.1.9/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/module.py` & `hypothesis_torch-0.1.9/hypothesis_torch/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,48 @@
     allow_infinity=False,
     allow_subnormal=False,
 )
 POSITIVE_INTS = st.integers(min_value=1)
 
 
 @st.composite
+def lower_upper_strategy(draw: st.DrawFn) -> tuple[float, float]:
+    """Strategy for generating a pair of floats where the first is less than the second.
+
+    Args:
+        draw: The draw function provided by `hypothesis`.
+
+    Returns:
+        A pair of floats where the first is less than the second.
+
+    """
+    lower = draw(SENSIBLE_FLOATS)
+    upper = draw(SENSIBLE_FLOATS.filter(lambda x: x > lower))
+    return lower, upper
+
+
+@st.composite
+def rrelu_strategy(draw: st.DrawFn) -> nn.RReLU:
+    lower, upper = draw(lower_upper_strategy())
+    inplace = draw(st.booleans())
+    return nn.RReLU(lower, upper, inplace)
+
+
+@st.composite
 def signature_to_strategy(draw: st.DrawFn, constructor: type[T], *args, **kwargs) -> T:
     """Strategy for generating instances of a class by drawing values for its constructor.
 
     Args:
-    ----
         draw: The draw function provided by `hypothesis`.
         constructor: The class to generate an instance of.
         args: Positional arguments to pass to the constructor. If an argument is a strategy, it will be drawn from.
         kwargs: Keyword arguments to pass to the constructor. If a keyword argument is a strategy, it will be drawn
             from.
 
     Returns:
-    -------
         An instance of the class.
 
     """
     args_drawn = [draw(strategy) for strategy in args]
     kwargs_drawn = {k: draw(strategy) for k, strategy in kwargs.items()}
     return constructor(*args_drawn, **kwargs_drawn)
 
@@ -95,27 +116,22 @@
         # TODO: nn.PReLU(num_parameters=1, init=0.25, device=None, dtype=None)
         # TODO: PReLU might depend on the input shape
         # TODO: num_parameters (int) – number of a to learn. Although it takes an int as input, there is only two
         #  values are legitimate: 1, or the number of channels at input. Default: 1
         signature_to_strategy(nn.PReLU, num_parameters=st.just(1), init=SENSIBLE_FLOATS),
         signature_to_strategy(nn.ReLU, inplace=st.booleans()),
         signature_to_strategy(nn.ReLU6, inplace=st.booleans()),
-        signature_to_strategy(
-            nn.RReLU,
-            lower=SENSIBLE_FLOATS,
-            upper=SENSIBLE_FLOATS,
-            inplace=st.booleans(),
-        ),
+        rrelu_strategy(),
         signature_to_strategy(nn.SELU, inplace=st.booleans()),
-        signature_to_strategy(nn.CELU, alpha=SENSIBLE_FLOATS, inplace=st.booleans()),
+        signature_to_strategy(nn.CELU, alpha=SENSIBLE_FLOATS.filter(lambda x: abs(x) > 1e-5), inplace=st.booleans()),
         signature_to_strategy(nn.GELU, approximate=st.sampled_from(["none", "tanh"])),
         signature_to_strategy(nn.Sigmoid),
         signature_to_strategy(nn.SiLU, inplace=st.booleans()),
         signature_to_strategy(nn.Mish, inplace=st.booleans()),
-        signature_to_strategy(nn.Softplus, beta=SENSIBLE_FLOATS, threshold=POSITIVE_INTS),
+        signature_to_strategy(nn.Softplus, beta=SENSIBLE_FLOATS, threshold=SENSIBLE_POSITIVE_FLOATS),
         signature_to_strategy(nn.Softshrink, lambd=SENSIBLE_POSITIVE_FLOATS),
         signature_to_strategy(nn.Softsign),
         signature_to_strategy(nn.Tanh),
         signature_to_strategy(nn.Tanhshrink),
         signature_to_strategy(
             nn.Threshold,
             threshold=SENSIBLE_FLOATS,
@@ -129,26 +145,26 @@
 @st.composite
 def linear_network_strategy(
     draw: st.DrawFn,
     input_shape: tuple[int, ...] | torch.Size | st.SearchStrategy[tuple[int, ...]] | st.SearchStrategy[torch.Size],
     output_shape: tuple[int, ...] | torch.Size | st.SearchStrategy[tuple[int, ...]] | st.SearchStrategy[torch.Size],
     activation_layer: nn.Module | st.SearchStrategy[nn.Module],
     hidden_layer_size: int | st.SearchStrategy[int],
-    depth: int | st.SearchStrategy[int],
+    num_hidden_layers: int | st.SearchStrategy[int],
     device: torch.device | st.SearchStrategy[torch.device],
 ) -> nn.Module:
     """Strategy for generating random Torch sequential networks of linear layers with activation functions.
 
     Args:
         draw: The draw function provided by `hypothesis`.
         input_shape: The shape of the input tensor. If a strategy is provided, it will be drawn from.
         output_shape: The shape of the output tensor. If a strategy is provided, it will be drawn from.
         activation_layer: Activation layer to use. If a strategy is provided, it will be drawn from.
         hidden_layer_size: The size of the hidden layers. If a strategy is provided, it will be drawn from.
-        depth: The maximum depth of the network. If a strategy is provided, it will be drawn from.
+        num_hidden_layers: The maximum depth of the network. If a strategy is provided, it will be drawn from.
         device: The device on which to place the network. If a strategy is provided, it will be drawn from.
 
     Returns:
         A strategy for generating random linear networks.
 
     """
     if isinstance(input_shape, st.SearchStrategy):
@@ -167,33 +183,41 @@
         device = draw(device)
 
     if isinstance(activation_layer, nn.Module):
         activation_layer_strategy = st.just(activation_layer)
     else:
         activation_layer_strategy = activation_layer
 
+    # Several activation functions are not supported on MPS devices
+    if device.type == "mps":
+        unsupported_mps_activations = [nn.Hardshrink, nn.RReLU]
+
+        activation_layer_strategy = activation_layer_strategy.filter(
+            lambda x: not isinstance(x, tuple(unsupported_mps_activations))
+        )
+
     if not isinstance(hidden_layer_size, st.SearchStrategy):
         hidden_layer_size = st.just(hidden_layer_size)
-    if isinstance(depth, st.SearchStrategy):
-        depth = draw(depth)
+    if isinstance(num_hidden_layers, st.SearchStrategy):
+        num_hidden_layers = draw(num_hidden_layers)
 
     with device:
         interior_layer_sizes = draw(
             st.lists(
                 hidden_layer_size,
-                min_size=depth,
-                max_size=depth,
-            ),
+                min_size=num_hidden_layers,
+                max_size=num_hidden_layers,
+            )
         )
         layer_sizes = [input_size, *interior_layer_sizes, output_size]
         layers: list[nn.Module] = [nn.Linear(a, b) for a, b in utils.pairwise(layer_sizes)]
         activations: list[nn.Module] = draw(
             st.lists(activation_layer_strategy, min_size=len(layers), max_size=len(layers)),
         )
-        return nn.Sequential(*utils.alternate(layers, activations))
+        return nn.Sequential(*utils.alternate(layers, activations)).to(device)
 
 
 def convolution_output_shape(
     input_shape: tuple[int, ...] | torch.Tensor,
     kernel_size: tuple[int, ...] | torch.Tensor,
     stride: tuple[int, ...] | torch.Tensor,
     padding: tuple[int, ...] | torch.Tensor,
```

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/tensor.py` & `hypothesis_torch-0.1.9/hypothesis_torch/tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from collections.abc import Mapping
 from typing import Any
 
 import hypothesis.extra.numpy as numpy_st
 import torch
 from hypothesis import strategies as st
+import hypothesis
 
 from hypothesis_torch import dtype as dtype_module
 
 
 @st.composite
 def tensor_strategy(
     draw: st.DrawFn,
@@ -44,24 +45,27 @@
 
     """
     # We will pre-sample the dtype so that we can cast it to a concrete numpy dtype
     if isinstance(dtype, st.SearchStrategy):
         dtype = draw(dtype)
     numpy_dtype = dtype_module.numpy_dtype_map[dtype]
 
+    # We will pre-sample the device so that we can cast it to a concrete torch device
+    if isinstance(device, st.SearchStrategy):
+        device = draw(device)
+
+    # MPS devices do not support tensors with dtype torch.float64 and bfloat16
+    hypothesis.assume(not (device is not None and device.type == "mps" and dtype in (torch.float64, torch.bfloat16)))
+
     if isinstance(unique, st.SearchStrategy):
         unique = draw(unique)
 
     ndarray_strategy = numpy_st.arrays(numpy_dtype, shape, elements=elements, fill=fill, unique=unique)
     tensor = draw(ndarray_strategy.map(torch.from_numpy))
 
-    # We will pre-sample the device so that we can cast it to a concrete torch device
-    if isinstance(device, st.SearchStrategy):
-        device = draw(device)
-
     return tensor.to(dtype=dtype, device=device)  # Final casting to the desired dtype and device
 
 
 st.register_type_strategy(
     torch.Tensor,
     tensor_strategy(
         dtype=dtype_module.dtype_strategy(),
```

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch/utils.py` & `hypothesis_torch-0.1.9/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.8/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.1.9/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -162,15 +162,15 @@
 optional arguments for the input size, output size, and number of hidden layers. Each of these arguments can be 
 specified as a fixed value or as a strategy. For example, to generate a fully-connected neural network with an input
 size of 10, an output size of 5, and 3 hidden layers with sizes between 5 and 10:
 
 ```python
 import hypothesis_torch
 from hypothesis import strategies as st
-hypothesis_torch.linear_network_strategy(input_shape=(1,10), output_shape=(1,5), hidden_layer_size=st.integers(5, 10), depth=3)
+hypothesis_torch.linear_network_strategy(input_shape=(1,10), output_shape=(1,5), hidden_layer_size=st.integers(5, 10), num_hidden_layers=3)
 ```
 
 #### Hugging Face Transformer Models
 
 Hugging Face transformer models can be generated with the `transformer_strategy` function. This function takes in any
 Hugging Face `PreTrainedModel` subclass (or a strategy that generates references `PreTrainedModel` subclasses) and 
 returns an instance of that model. For example, to generate an arbitrary Llama2 model:
```

### Comparing `hypothesis_torch-0.1.8/pyproject.toml` & `hypothesis_torch-0.1.9/pyproject.toml`

 * *Files identical despite different names*

