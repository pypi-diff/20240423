# Comparing `tmp/badam-1.0.1.tar.gz` & `tmp/badam-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badam-1.0.1.tar", last modified: Mon Apr 15 12:20:22 2024, max compression
+gzip compressed data, was "badam-1.0.2.tar", last modified: Tue Apr 23 16:11:43 2024, max compression
```

## Comparing `badam-1.0.1.tar` & `badam-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-15 12:20:22.685787 badam-1.0.1/
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)     1065 2024-04-15 08:00:12.000000 badam-1.0.1/LICENSE.txt
--rw-r--r--   0 luoqijun  (1001) luoqijun  (1001)     1718 2024-04-15 12:20:22.685787 badam-1.0.1/PKG-INFO
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)       84 2024-04-15 08:04:52.000000 badam-1.0.1/pyproject.toml
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)      775 2024-04-15 12:20:22.685787 badam-1.0.1/setup.cfg
-drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-15 12:20:22.685787 badam-1.0.1/src/
-drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-15 12:20:22.685787 badam-1.0.1/src/badam/
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)       94 2024-04-15 08:08:59.000000 badam-1.0.1/src/badam/__init__.py
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)    29188 2024-04-15 07:53:11.000000 badam-1.0.1/src/badam/block_optim.py
-drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-15 12:20:22.685787 badam-1.0.1/src/badam.egg-info/
--rw-r--r--   0 luoqijun  (1001) luoqijun  (1001)     1718 2024-04-15 12:20:22.000000 badam-1.0.1/src/badam.egg-info/PKG-INFO
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)      215 2024-04-15 12:20:22.000000 badam-1.0.1/src/badam.egg-info/SOURCES.txt
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)        1 2024-04-15 12:20:22.000000 badam-1.0.1/src/badam.egg-info/dependency_links.txt
--rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)        6 2024-04-15 12:20:22.000000 badam-1.0.1/src/badam.egg-info/top_level.txt
+drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-23 16:11:43.161464 badam-1.0.2/
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)     1065 2024-04-15 08:00:12.000000 badam-1.0.2/LICENSE.txt
+-rw-r--r--   0 luoqijun  (1001) luoqijun  (1001)     1718 2024-04-23 16:11:43.161464 badam-1.0.2/PKG-INFO
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)       84 2024-04-15 08:04:52.000000 badam-1.0.2/pyproject.toml
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)      775 2024-04-23 16:11:43.161464 badam-1.0.2/setup.cfg
+drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-23 16:11:43.157464 badam-1.0.2/src/
+drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-23 16:11:43.157464 badam-1.0.2/src/badam/
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)       94 2024-04-15 08:08:59.000000 badam-1.0.2/src/badam/__init__.py
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)    32005 2024-04-23 13:53:59.000000 badam-1.0.2/src/badam/block_optim.py
+drwxrwxr-x   0 luoqijun  (1001) luoqijun  (1001)        0 2024-04-23 16:11:43.161464 badam-1.0.2/src/badam.egg-info/
+-rw-r--r--   0 luoqijun  (1001) luoqijun  (1001)     1718 2024-04-23 16:11:43.000000 badam-1.0.2/src/badam.egg-info/PKG-INFO
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)      215 2024-04-23 16:11:43.000000 badam-1.0.2/src/badam.egg-info/SOURCES.txt
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)        1 2024-04-23 16:11:43.000000 badam-1.0.2/src/badam.egg-info/dependency_links.txt
+-rw-rw-r--   0 luoqijun  (1001) luoqijun  (1001)        6 2024-04-23 16:11:43.000000 badam-1.0.2/src/badam.egg-info/top_level.txt
```

### Comparing `badam-1.0.1/LICENSE.txt` & `badam-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `badam-1.0.1/PKG-INFO` & `badam-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badam
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package which implements the algorithm proposed by "BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models".
 Home-page: https://github.com/Ledzy/BAdam
 Author: Qijun Luo
 Author-email: qijunluo@link.cuhk.edu.cn
 Project-URL: Bug Tracker, https://github.com/Ledzy/BAdam/issues
 Project-URL: Source Code, https://github.com/Ledzy/BAdam
 Classifier: Programming Language :: Python :: 3
```

### Comparing `badam-1.0.1/setup.cfg` & `badam-1.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = badam
-version = 1.0.1
+version = 1.0.2
 author = Qijun Luo
 author_email = qijunluo@link.cuhk.edu.cn
 description = Package which implements the algorithm proposed by "BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models".
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/Ledzy/BAdam
 project_urls =
```

### Comparing `badam-1.0.1/src/badam/block_optim.py` & `badam-1.0.2/src/badam/block_optim.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import random
 from torch.optim import Optimizer
 from torch import Tensor
 from collections import defaultdict
 from typing import List, Optional, Dict, Union, Iterable
 import time
 import math
+import warnings
 from transformers.pytorch_utils import ALL_LAYERNORM_LAYERS
 
 # Optional [0, 1, 2]. 
     # 0: no print
     # 1: print the relative time whenever a parameter's grad is ready
     # 2: for debug usage only. Will set all the parameters trainable, print the grad ready time for each parameter. 
     #     In this case, all the grad except the "specified" trainable parameters will be set to None after being calculated.
@@ -23,14 +24,16 @@
         base_optimizer: Optimizer,
         named_parameters_list,
         block_prefix_list: List[str],
         switch_block_every: int = 10,
         start_block: Optional[int] = None,
         switch_mode: str = "descending",
         active_modules: List[str] = [],
+        include_embedding=False,
+        include_lm_head=False,
         verbose: int = 1,
         log_fn = None,
     ):
         """
         Args:
             base_optimizer (Optimizer): The base optimizer being wrapped by the BlockOptimizer.
             named_parameters_list: A function that generates the named parameters of the model.
@@ -39,15 +42,15 @@
             start_block (Optional[int], optional): The index of the block to start with. Defaults to None.
             switch_mode (str, optional): The mode for switching between different blocks of parameters. Defaults to "descending".
             active_modules (List[str]): The list of modules that are always active during optimization. Defaults to None.
             verbose (int, optional): The verbosity level for printing information during optimization. Defaults to 1.
             log_fn: A logging function for recording information during optimization. Defaults to None.
         """
         if block_prefix_list is None:
-            block_prefix_list = self.infer_param_groups([n for n, _ in named_parameters_list])
+            block_prefix_list = self.infer_param_groups([n for n, _ in named_parameters_list], include_embedding, include_lm_head)
 
         assert switch_mode in ["random", "descending", "ascending", "fixed"]
         assert isinstance(block_prefix_list, list)
 
         self.verbose = verbose
         self.switch_mode = switch_mode
         self.switch_block_every = switch_block_every
@@ -75,15 +78,19 @@
             print("next block epoch's update order:", self.block_order[::-1])
             self.current_block_idx = self.block_order.pop()
 
         # detect if in lora mode or not
         self.lora_mode = False
         if any("lora" in n for n, _ in named_parameters_list):
             self.lora_mode = True
-            print("Lora mode detected. Will only train the lora parameters.")
+            print("LoRA mode detected. Will only train the lora parameters.")
+            
+        if any(isinstance(p, torch.FloatTensor) for _, p in named_parameters_list):
+            warnings.warn("BAdam expect model to be loaded in fp16 precision while detect fp32 weight. \
+                This will cause additional memory usage and lose the benefit of mixed precision training.")
             
         super().__init__(self.param_groups, base_optimizer.defaults)
         
         if BACKWARD_VERBOSE:
             self.record_mark = True
             self.ordered_named_params = []
             self.param_num = len(named_parameters_list)
@@ -91,41 +98,54 @@
                 p.register_post_accumulate_grad_hook(self.test_hook(n))
 
         self.update_trainable_params()
 
         if BACKWARD_VERBOSE == 2:
             for name, param in self.named_parameters_list:
                 param.requires_grad_(True)
-                
-    def infer_param_groups(self, param_names):
+    
+    @property
+    def embedding_layer(self):
+        for n, p in self.named_parameters_list:
+            if "embed" in n:
+                return p
+    
+    @property
+    def lm_head_layer(self):
+        for n, p in self.named_parameters_list:
+            if "lm_head" in n:
+                return p
+
+    def infer_param_groups(self, param_names, include_embedding, include_lm_head):
         """automatic inference of the parameter groups based on the parameter names.
         divide groups into:
             * embedding
             * transformer layers
             * lm_head and others
         """
         import re
         
         block_prefix_list = []
-        non_embed_layer_params = []
-        
+        lm_head_and_other_params = []
         embed_pattern = r'.*embed[^.]*\.'
         layer_pattern = r'.*layers.[^.]*\.'
 
         for name in param_names:
             if any(prefix[0] in name for prefix in block_prefix_list):
                 continue
             
-            prefix = re.findall(embed_pattern + '|' + layer_pattern, name)
-            if prefix:
-                block_prefix_list.append(prefix)
+            if re.findall(layer_pattern, name):
+                block_prefix_list.append(re.findall(layer_pattern, name))
+            elif re.findall(embed_pattern, name) and include_embedding:
+                block_prefix_list.append(re.findall(embed_pattern, name))
             else:
-                non_embed_layer_params.append(name)
+                lm_head_and_other_params.append(name)
         
-        block_prefix_list.append(non_embed_layer_params)
+        if include_lm_head:
+            block_prefix_list.append(lm_head_and_other_params)
         
         return block_prefix_list
                 
     def test_hook(self, name):
         """hook used for recording the time of gradient calculation, see comments on BACKWARD_VERBOSE for more details."""
         
         def func(x):
@@ -287,50 +307,64 @@
         elif self.switch_mode == "ascending":
             self.current_block_idx = (self.current_block_idx + 1) % self.block_num
         elif self.switch_mode == "descending":
             self.current_block_idx = (self.current_block_idx - 1) % self.block_num
         elif self.switch_mode == "fixed":
             pass
             
-# In BlockOptimizerRatio, each block contains a part of trainable weights
 class BlockOptimizerRatio(Optimizer):
+    """
+    BlockOptimizerRatio is an extension of BlockOptimizer, where each block contains a part of trainable weights
+    Args:
+        param_groups (list): List of parameter groups.
+        named_parameters_list (list): List of named parameters.
+        update_ratio (float, optional): The update ratio for sparsification. Defaults to 0.1.
+        switch_every (int, optional): Number of steps before switching to new parameter groups. Defaults to 100.
+        preserve_threshold (int, optional): Threshold for preserving the whole gradient when parameter is too small. Defaults to 100.
+        param_update_ratios (defaultdict, optional): Dictionary of parameter update ratios for specific parameter heads. Defaults to defaultdict(lambda: None).
+        mask_mode (str, optional): Choices: ("adjacent", "scatter"). "adjacent" mode selects a group of adjacent entries in the matrix, while "scatter" selects random entries in the matrix.
+        keep_mask (bool, optional): Flag to keep the mask. Defaults to True.
+        include_embedding (bool, optional): Flag to include the embedding layer in optimization. Defaults to False.
+    """
+
     def __init__(self, param_groups, 
                  named_parameters_list,
                  update_ratio=0.1, 
                  verbose=1, 
                  switch_every=100, 
                  preserve_threshold=100, 
                  param_update_ratios=defaultdict(lambda: None),
                  mask_mode = "adjacent",
                  lr=1e-5,
                  betas=(0.9, 0.999), 
                  eps=1e-8,
                  optimizer_defaults=None,
                  keep_mask=True,
-                 include_embedding=True,
-                #  maximize: bool = False
+                 include_embedding=False,
+                 include_lm_head=False
                  ):
         self.update_ratio = update_ratio
         self.verbose = verbose
         self.sparse_hook = self.sparse_update_hook()
         self.param_groups = param_groups
         self.named_parameters_list = named_parameters_list
         self.sparse_dict = defaultdict(lambda: {})
         self.switch_every = switch_every
         self.preserve_threshold = preserve_threshold
         self.global_step = 0
         self.current_block_index = 0
-        self.embedding_layer = self._get_embedding_layer()
         self.include_embedding = include_embedding
         
         self.param_num = len(named_parameters_list)
         self.ordered_named_params = []
         
         if not include_embedding:
             self.embedding_layer.requires_grad_(False)
+        if not include_lm_head:
+            self.lm_head_layer.requires_grad_(False)
         
         # mask
         self.mask_mode = mask_mode
         self.keep_mask = keep_mask
         self.mask_dict = {}
         
         for n, p in named_parameters_list:
@@ -343,34 +377,53 @@
                 if param_head in n:
                     self.sparse_dict[p]["update_ratio"] = param_update_ratios[param_head]
                     continue
                     
         defaults = dict(lr=lr, betas=betas, eps=eps) if optimizer_defaults is None else optimizer_defaults
         super().__init__(self.param_groups, defaults)
 
-    def _get_embedding_layer(self):
+    @property
+    def embedding_layer(self):
         for n, p in self.named_parameters_list:
             if "embed" in n:
                 return p
+            
+    @property
+    def lm_head_layer(self):
+        for n, p in self.named_parameters_list:
+            if "lm_head" in n:
+                return p
     
     def _sparse_adam(self,
                     params: List[Tensor],
                     grads: List[Tensor],
                     exp_avgs: List[Tensor],
                     exp_avg_sqs: List[Tensor],
                     state_steps: List[int],
                     *,
                     eps: float,
                     beta1: float,
                     beta2: float,
                     lr: float,
                     maximize: bool):
-        r"""Functional API that performs Sparse Adam algorithm computation.
+        """
+        Functional API that performs Sparse Adam algorithm computation.
+
+        Args:
+            params (List[Tensor]): List of parameters.
+            grads (List[Tensor]): List of gradients.
+            exp_avgs (List[Tensor]): List of exponential moving average of gradients.
+            exp_avg_sqs (List[Tensor]): List of exponential moving average of squared gradients.
+            state_steps (List[int]): List of steps for each parameter group update.
+            eps (float): Term added to the denominator to improve numerical stability.
+            beta1 (float): Coefficient used for computing running averages of gradient.
+            beta2 (float): Coefficient used for computing running averages of squared gradient.
+            lr (float): Learning rate.
+            maximize (bool): Flag to indicate if maximizing the objective function.
 
-        See :class:`~torch.optim.SparseAdam` for details.
         """
         for i, param in enumerate(params):
             grad = grads[i]
             grad = grad if not maximize else -grad
             grad = grad.coalesce()  # the update is non-linear so indices must be unique
             grad_indices = grad._indices()
             grad_values = grad._values()
@@ -476,15 +529,14 @@
 
         return loss
     
     def _reset_state_dict(self):
         for group in self.param_groups:
             for p in group["params"]:
                 self.state[p] = defaultdict()
-        print("switch to new parameter groups, set the state dictionary to be zero")
     
     def _generate_mask_adjacent(self, param, ratio, offset):
         """select a group of adjacent entries in the matrix, starting from the offset. If the end of the matrix is reached, continue from the beginning."""
         num_elements = param.numel()
         num_ones = int(num_elements * ratio)
         
         if offset + num_ones > num_elements:
@@ -528,16 +580,14 @@
                 iterator = self.ordered_named_params[self.current_block_index:]
             
             for n, p in iterator:
                 
                 if p.requires_grad and p.grad is not None:
                     if p.grad.is_sparse:
                         continue
-                    if p is self.embedding_layer and not self.include_embedding:
-                        p.grad = None
                     num_elements = p.numel()
                     offset = self.sparse_dict[p]["offset"]
                     update_ratio = self.sparse_dict[p]["update_ratio"] if "update_ratio" in self.sparse_dict[p] else self.update_ratio
                     
                     # when the parameter is too small, we simply sparsify the whole gradient
                     if num_elements < self.preserve_threshold:
                         p.grad = p.grad.add_(1e-9).to_sparse()
@@ -554,14 +604,15 @@
                         else:
                             if self.mask_mode == "adjacent":
                                 mask = self._generate_mask_adjacent(p, update_ratio, offset)
                             elif self.mask_mode == "scatter":
                                 mask = self._generate_mask_scatter(p, update_ratio, offset)
                             else:
                                 raise NotImplementedError
+                            # We save the same mask for all the parameters with the same shape, this treats memory for time.
                             if self.keep_mask:
                                 self.mask_dict[p.shape] = mask
                         
                         p.grad = p.grad.sparse_mask(mask)
                             
                         if (self.global_step + 1) % self.switch_every == 0:
                             self.sparse_dict[p]["offset"] = (offset + int(num_elements * update_ratio)) % num_elements
```

### Comparing `badam-1.0.1/src/badam.egg-info/PKG-INFO` & `badam-1.0.2/src/badam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badam
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package which implements the algorithm proposed by "BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models".
 Home-page: https://github.com/Ledzy/BAdam
 Author: Qijun Luo
 Author-email: qijunluo@link.cuhk.edu.cn
 Project-URL: Bug Tracker, https://github.com/Ledzy/BAdam/issues
 Project-URL: Source Code, https://github.com/Ledzy/BAdam
 Classifier: Programming Language :: Python :: 3
```

