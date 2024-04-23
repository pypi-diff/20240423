# Comparing `tmp/xtrain-0.2.1.tar.gz` & `tmp/xtrain-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtrain-0.2.1.tar", max compression
+gzip compressed data, was "xtrain-0.2.2.tar", max compression
```

## Comparing `xtrain-0.2.1.tar` & `xtrain-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-04-14 14:01:13.686413 xtrain-0.2.1/LICENSE
--rw-r--r--   0        0        0     1231 2024-04-14 14:01:13.686413 xtrain-0.2.1/README.md
--rw-r--r--   0        0        0      833 2024-04-14 14:01:29.298452 xtrain-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      160 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/__init__.py
--rw-r--r--   0        0        0    10659 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/base_trainer.py
--rw-r--r--   0        0        0     1399 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/loss.py
--rw-r--r--   0        0        0     4564 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/strategy.py
--rw-r--r--   0        0        0     5517 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/utils.py
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-23 13:38:19.629050 xtrain-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1231 2024-04-23 13:38:19.629050 xtrain-0.2.2/README.md
+-rw-r--r--   0        0        0      833 2024-04-23 13:38:39.005170 xtrain-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/__init__.py
+-rw-r--r--   0        0        0    10925 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/base_trainer.py
+-rw-r--r--   0        0        0     1464 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/loss.py
+-rw-r--r--   0        0        0     4564 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/strategy.py
+-rw-r--r--   0        0        0     5517 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/utils.py
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.2/PKG-INFO
```

### Comparing `xtrain-0.2.1/LICENSE` & `xtrain-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.1/README.md` & `xtrain-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.1/pyproject.toml` & `xtrain-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtrain"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Flax trainer"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flax = "^0.8"
```

### Comparing `xtrain-0.2.1/xtrain/base_trainer.py` & `xtrain-0.2.2/xtrain/base_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,21 @@
 
     def _compute_loss_log(self) -> dict:
         return {
             _get_name(loss_log.loss_fn): loss_log.compute()
             for loss_log in self.loss_logs
         }
 
+    def reset(self):
+        """ Restart the dataset iteration and reset loss metrics
+        """
+        self.data = Peekable(iter(self.ctx.dataset))
+        self.reset_loss_logs()
+
+
     def reset_loss_logs(self):
         """Reset internal loss value tracking.
 
         Args:
             loss_weights: Optional weights of individual loss functions. If not None, the
                 total loss is weighted sum.
         """
@@ -191,39 +198,42 @@
         inputs, _, _ = unpack_x_y_sample_weight(peek)
 
         return self.strategy.init_fn(rng, self.model, inputs)
 
     def train(
         self,
         dataset: Iterable,
+        *,
         strategy: type | None = None,
         rng_cols: Sequence[str] = ["dropout"],
         init_vars: dict | None = None,
         frozen: dict | None = None,
         **kwargs,
     ) -> TrainIterator:
         """Create the training iterator
 
         Args:
             dataset: An iterator or iterable to supply the training data.
                 The dataset should produce ```(inputs, labels, sample_weight)```, however
-                both the labels and the sample_weight are optional. The inputs is either a tuple
-                or a dict. If the inputs is a dict, the keys are interpreted as the names for
-                keyword args of the model's __call__ function.
+                both the labels and the sample_weight are optional. The inputs is either a list 
+                (not tuple) or a dict. If latter, the keys are interpreted as the names for
+                keyword args of the model's __call__ function. 
             strategy: Optionally override the default strategy.
             rng_cols: Names of any RNG used by the model. Should be a list of strings.
             init_vars: optional variables to initialize model
-            frozen: a pytree indicating frozen parameters
+            frozen: a bool pytree (matching model parameter tree) indicating frozen parameters.
             **kwargs: Additional keyward args passed to the model. E.g. "training=True"
 
         Returns:
             TrainIterator. Stepping through the iterator will train the model.
 
         """
         config = dataclasses.replace(self, strategy=strategy or self.strategy)
+        config.dataset = dataset
+
         assert config.strategy is not None
 
         dataset_iter = Peekable(iter(dataset))
 
         seed = (
             self.seed
             if isinstance(self.seed, jnp.ndarray)
```

### Comparing `xtrain-0.2.1/xtrain/loss.py` & `xtrain-0.2.2/xtrain/loss.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,18 @@
         loss *= self.weight
         self.cnt += 1
         self.sum += loss
 
         return loss, self
 
     def compute(self):
-        return self.sum / self.cnt
+        if self.cnt == 0:
+            return 0
+        else:
+            return self.sum / self.cnt
 
     def reset(self):
         self.cnt = 0.0
         self.sum = 0.0
 
     def __repr__(self) -> str:
         return self.__name__ + f": {float(self.compute()):.4f}"
```

### Comparing `xtrain-0.2.1/xtrain/strategy.py` & `xtrain-0.2.2/xtrain/strategy.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.1/xtrain/utils.py` & `xtrain-0.2.2/xtrain/utils.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.1/PKG-INFO` & `xtrain-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtrain
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Flax trainer
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

