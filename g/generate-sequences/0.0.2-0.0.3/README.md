# Comparing `tmp/generate_sequences-0.0.2.tar.gz` & `tmp/generate_sequences-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_sequences-0.0.2.tar", last modified: Sun Apr 21 10:07:17 2024, max compression
+gzip compressed data, was "generate_sequences-0.0.3.tar", last modified: Tue Apr 23 06:23:22 2024, max compression
```

## Comparing `generate_sequences-0.0.2.tar` & `generate_sequences-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:07:17.954053 generate_sequences-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-21 10:07:17.954053 generate_sequences-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:07:17.950053 generate_sequences-0.0.2/generate_sequences/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/generate_sequences/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:07:17.950053 generate_sequences-0.0.2/generate_sequences.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-21 10:07:17.000000 generate_sequences-0.0.2/generate_sequences.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-21 10:03:34.000000 generate_sequences-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:07:17.954053 generate_sequences-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:23:22.921271 generate_sequences-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-23 06:23:22.921271 generate_sequences-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:23:22.913272 generate_sequences-0.0.3/generate_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/generate_sequences/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:23:22.917271 generate_sequences-0.0.3/generate_sequences.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 06:23:22.000000 generate_sequences-0.0.3/generate_sequences.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-23 06:21:05.000000 generate_sequences-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:23:22.921271 generate_sequences-0.0.3/setup.cfg
```

### Comparing `generate_sequences-0.0.2/LICENSE` & `generate_sequences-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_sequences-0.0.2/PKG-INFO` & `generate_sequences-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.2
+Version: 0.0.3
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `generate_sequences-0.0.2/generate_sequences/generate.py` & `generate_sequences-0.0.3/generate_sequences/generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import heapq
+import warnings
 from typing import Callable, Iterator, List, Union
 
 import torch
 import torch.nn.functional as F
 import torch.utils
 from tqdm.auto import tqdm
 
@@ -15,48 +16,44 @@
         generate_fn: Callable[
             [Union[List[torch.Tensor], List[str]], torch.Tensor],
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
         device: str = "cuda",
+        temperature: float = 1.0,
         use_tqdm: bool = True,
     ) -> None:
         self.device = device
         self.use_tqdm = use_tqdm
         self.max_length = max_length
         self.batch_size = batch_size
         self.generate_fn = generate_fn
         self.eos_token_id = eos_token_id
         self.decoder_start_token_id = decoder_start_token_id
+        self.temperature = temperature
 
     def get_batches(self, inputs: Union[List[torch.Tensor], List[str]]) -> Iterator[List[str]]:
         for i in tqdm(
             range(0, len(inputs), self.batch_size),
             disable=not self.use_tqdm,
             desc="Generating Sequences",
             total=len(inputs) // self.batch_size,
         ):
             yield inputs[i : i + self.batch_size]
 
-    def sample_tokens_probs(
-        self,
-        outputs: torch.Tensor,
-    ) -> torch.Tensor:
-        raise NotImplementedError
-
 
 class GreedyGenerator(BaseGenerator):
-    def sample_tokens_probs(self, outputs: torch.Tensor) -> torch.Tensor:
-        next_tokens = torch.argmax(outputs, dim=-1)
-        return next_tokens
-
     @torch.no_grad()
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
         outputs = []
+        # add user warning if temperature is not 1.0 that greedy search is not appropriate
+        if self.temperature != 1.0:
+            warnings.warn("Temperature does not have an affect on Greedy search!")
+
         for batch_inputs in self.get_batches(inputs):
             batch_size = len(batch_inputs)
             decoder_inputs = torch.full(
                 (batch_size, self.max_length),
                 self.eos_token_id,  # Pre-fill with EOS; only overwrite if generating
                 dtype=torch.long,
                 device=self.device,
@@ -65,164 +62,166 @@
             finished_mask = torch.zeros(batch_size, dtype=torch.bool, device=self.device)
 
             for step in range(1, self.max_length):
                 if finished_mask.all():
                     break  # Stop if all sequences are finished
                 batch_outputs = self.generate_fn(batch_inputs, decoder_inputs[:, :step])
                 batch_outputs = batch_outputs[:, -1, :]  # Get last tokens' outputs for the batch
-                next_tokens = self.sample_tokens_probs(batch_outputs)
+                next_tokens = batch_outputs / self.temperature
+                next_tokens = F.softmax(next_tokens, dim=-1)
+                next_tokens = torch.argmax(next_tokens, dim=-1)
                 not_finished = ~finished_mask
                 decoder_inputs[not_finished, step] = next_tokens[not_finished]
                 finished_mask |= next_tokens == self.eos_token_id  # Update finished sequences
-            outputs.extend(decoder_inputs)
+            outputs += decoder_inputs
         return outputs
 
 
 class BeamNode:
+    """Represents a node in a beam search. Stores token sequences and their associated score."""
+
     def __init__(self, tokens: List[int], score: float) -> None:
         self.tokens = tokens
         self.score = score
 
 
 def default_beam_nodes_ordering_fn(
     node: BeamNode,
     eos_token_id: int,
-    length_penalty_alpha: float = 1.0,
-    minimum_penalty_tokens_length: int = 0,
+    length_penalty: float = 1.0,
 ) -> float:
+    """Calculates the adjusted score of a node for beam sorting. Applies length penalty to score."""
     tokens = node.tokens
     if eos_token_id in tokens:
         tokens = tokens[1 : tokens.index(eos_token_id) + 1]
-    return node.score / ((len(tokens) + minimum_penalty_tokens_length) ** length_penalty_alpha)
+    return node.score / (len(tokens) ** length_penalty)
 
 
 class Beam:
+    """Manages a list of BeamNodes for the beam search algorithm with a fixed beam width."""
+
     def __init__(
         self,
         eos_token_id: int,
         beam_width: int = 4,
-        length_penalty_alpha: float = 1,
-        minimum_penalty_tokens_length: int = 0,
+        length_penalty: float = 1.0,
         beam_nodes_ordering_function: Callable[
-            [BeamNode, int, float, int], float
+            [BeamNode, int, float], float
         ] = default_beam_nodes_ordering_fn,
     ):
         self.nodes: List[BeamNode] = []
         self.beam_width = beam_width
         self.eos_token_id = eos_token_id
-        self.length_penalty_alpha = length_penalty_alpha
-        self.minimum_penalty_tokens_length = minimum_penalty_tokens_length
+        self.length_penalty = length_penalty
         self.beam_nodes_ordering_function = beam_nodes_ordering_function
 
-    def add(self, node):
+    def add(self, node: BeamNode) -> None:
+        """Adds a new node to the beam."""
         self.nodes.append(node)
 
-    def get_topk(self):
+    def get_topk(self) -> List[BeamNode]:
+        """Returns the top k nodes in the beam according to the ordering function."""
         return heapq.nlargest(
             self.beam_width,
             self.nodes,
             key=lambda node: self.beam_nodes_ordering_function(
                 node,
                 self.eos_token_id,
-                self.length_penalty_alpha,
-                self.minimum_penalty_tokens_length,
+                self.length_penalty,
             ),
         )
 
-    def has_finished(self):
-        return all([node.tokens[-1] == self.eos_token_id for node in self.nodes])
+    def has_finished(self) -> bool:
+        """Checks if all nodes in the beam have reached the end of sequence token."""
+        return all(node.tokens[-1] == self.eos_token_id for node in self.nodes)
 
 
 class BeamSearchGenerator(BaseGenerator):
     def __init__(
         self,
         decoder_start_token_id: int,
         eos_token_id: int,
         generate_fn: Callable[
             [Union[List[torch.Tensor], List[str]], torch.Tensor],
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
         device: str = "cuda",
+        temperature: float = 1.0,
         use_tqdm: bool = True,
         beam_width: int = 4,
-        length_penalty_alpha: float = 1.0,
-        minimum_penalty_tokens_length: int = 0,
+        length_penalty: float = 1.0,
         beam_nodes_ordering_function: Callable[
-            [BeamNode, int, float, int], float
+            [BeamNode, int, float], float
         ] = default_beam_nodes_ordering_fn,
     ) -> None:
         super().__init__(
             decoder_start_token_id,
             eos_token_id,
             generate_fn,
             max_length,
             batch_size,
             device,
+            temperature,
             use_tqdm,
         )
         self.beam_width = beam_width
-        self.length_penalty_alpha = length_penalty_alpha
-        self.minimum_penalty_tokens_length = minimum_penalty_tokens_length
+        self.length_penalty = length_penalty
         self.beam_nodes_ordering_function = beam_nodes_ordering_function
 
-    def sample_tokens_probs(self, outputs: torch.Tensor) -> torch.Tensor:
-        outputs = F.log_softmax(outputs[:, -1, :], dim=-1)
-        return outputs
-
     @torch.no_grad
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
         predictions = []
         for batch in self.get_batches(inputs):
             beams = []
             for _ in range(len(batch)):
                 beam = Beam(
                     beam_width=self.beam_width,
                     eos_token_id=self.eos_token_id,
-                    length_penalty_alpha=self.length_penalty_alpha,
-                    minimum_penalty_tokens_length=self.minimum_penalty_tokens_length,
+                    length_penalty=self.length_penalty,
                     beam_nodes_ordering_function=self.beam_nodes_ordering_function,
                 )
                 beam.add(
                     BeamNode(
                         tokens=[self.decoder_start_token_id],
                         score=0.0,
                     )
                 )
                 beams.append(beam)
             for t in range(self.max_length):
                 next_beams = [
                     Beam(
                         beam_width=self.beam_width,
                         eos_token_id=self.eos_token_id,
-                        length_penalty_alpha=self.length_penalty_alpha,
-                        minimum_penalty_tokens_length=self.minimum_penalty_tokens_length,
+                        length_penalty=self.length_penalty,
                         beam_nodes_ordering_function=self.beam_nodes_ordering_function,
                     )
                     for _ in range(len(batch))
                 ]
                 best_beams_nodes = [beam.get_topk() for beam in beams]
                 for k in range(
                     len(best_beams_nodes[0])
                 ):  # beam width, taking the case where k < len(best_beams_nodes[0])
                     decoder_input_ids = torch.LongTensor(
                         [topk_nodes[k].tokens for topk_nodes in best_beams_nodes]
                     ).to(self.device)
-                    outputs = self.generate_fn(batch, decoder_input_ids)
-                    outputs = self.sample_tokens_probs(outputs)
-                    topk_scores, topk_indices = torch.topk(outputs, self.beam_width)
+                    batch_outputs = self.generate_fn(batch, decoder_input_ids)
+                    batch_outputs = batch_outputs[:, -1, :]
+                    batch_outputs = batch_outputs / self.temperature
+                    batch_outputs = F.log_softmax(batch_outputs, dim=-1)
+                    topk_scores, topk_indices = torch.topk(batch_outputs, self.beam_width)
                     for beam_index, beam in enumerate(next_beams):
                         # Check if this sequence has already reached eos token
                         if best_beams_nodes[beam_index][k].tokens[-1] == self.eos_token_id:
                             beam.add(
                                 BeamNode(
                                     tokens=best_beams_nodes[beam_index][k].tokens
                                     + [self.eos_token_id],
-                                    score=best_beams_nodes[beam_index][k].score,
+                                    score=0,
                                 )
                             )
                         else:
                             for k2 in range(self.beam_width):
                                 beam.add(
                                     BeamNode(
                                         tokens=best_beams_nodes[beam_index][k].tokens
@@ -238,14 +237,13 @@
             batch_predictions = []
             for beam in beams:
                 best_node = max(
                     beam.nodes,
                     key=lambda node: self.beam_nodes_ordering_function(
                         node,
                         self.eos_token_id,
-                        self.length_penalty_alpha,
-                        self.minimum_penalty_tokens_length,
+                        self.length_penalty,
                     ),
                 )
                 batch_predictions.append(best_node.tokens)
             predictions += batch_predictions
         return predictions
```

### Comparing `generate_sequences-0.0.2/generate_sequences.egg-info/PKG-INFO` & `generate_sequences-0.0.3/generate_sequences.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.2
+Version: 0.0.3
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `generate_sequences-0.0.2/pyproject.toml` & `generate_sequences-0.0.3/pyproject.toml`

 * *Files identical despite different names*

