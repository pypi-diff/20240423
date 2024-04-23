# Comparing `tmp/f3dasm_optimize-1.4.0.tar.gz` & `tmp/f3dasm_optimize-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm_optimize-1.4.0.tar", last modified: Thu Nov 30 15:23:51 2023, max compression
+gzip compressed data, was "f3dasm_optimize-1.5.1.tar", last modified: Tue Apr 23 11:21:07 2024, max compression
```

## Comparing `f3dasm_optimize-1.4.0.tar` & `f3dasm_optimize-1.5.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-11-30 15:23:51.420753 f3dasm_optimize-1.4.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1511 2023-06-14 13:02:10.000000 f3dasm_optimize-1.4.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-14 13:00:50.000000 f3dasm_optimize-1.4.0/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     4150 2023-11-30 15:23:51.420753 f3dasm_optimize-1.4.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2912 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/VERSION
--rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-14 13:00:50.000000 f3dasm_optimize-1.4.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       68 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/requirements_all.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1185 2023-11-30 15:23:51.420753 f3dasm_optimize-1.4.0/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-11-30 15:23:51.412753 f3dasm_optimize-1.4.0/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-11-30 15:23:51.416753 f3dasm_optimize-1.4.0/src/f3dasm_optimize/
--rw-rw-r--   0 martin    (1000) martin    (1000)      716 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-11-30 15:23:51.416753 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2344 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4197 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/_imports.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1331 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/_protocol.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-11-30 15:23:51.416753 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-02 02:36:58.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2495 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/evosax_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1631 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3722 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/optuna_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4509 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3900 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2517 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/evosax_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2899 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/nevergrad_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6934 2023-11-30 15:22:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      896 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/optuna_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9064 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/pygmo_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6303 2023-11-17 22:45:34.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/tensorflow_optimizers.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-11-30 15:23:51.416753 f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     4150 2023-11-30 15:23:51.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1084 2023-11-30 15:23:51.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-11-30 15:23:51.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       96 2023-11-30 15:23:51.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       16 2023-11-30 15:23:51.000000 f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1511 2023-06-14 13:02:10.000000 f3dasm_optimize-1.5.1/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-14 13:00:50.000000 f3dasm_optimize-1.5.1/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     4187 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2912 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/VERSION
+-rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-14 13:00:50.000000 f3dasm_optimize-1.5.1/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/requirements_all.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1185 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/f3dasm_optimize/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      716 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2572 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4197 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_imports.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1331 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_protocol.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-02 02:36:58.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2495 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/evosax_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1631 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1648 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/optax_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3893 2024-02-07 15:48:24.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/optuna_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4509 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4056 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2661 2024-02-23 19:54:12.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/evosax_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3024 2024-02-23 19:54:30.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/nevergrad_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2263 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optax_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5783 2024-02-23 20:03:23.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      932 2024-02-23 19:59:00.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optuna_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9380 2024-02-23 20:03:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/pygmo_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6548 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/tensorflow_optimizers.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     4187 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1188 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      102 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       16 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/top_level.txt
```

### Comparing `f3dasm_optimize-1.4.0/LICENSE` & `f3dasm_optimize-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/PKG-INFO` & `f3dasm_optimize-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm_optimize
-Version: 1.4.0
+Version: 1.5.1
 Summary: f3dasm_optimize: Your one line description of the package
 Home-page: https://github.com/bessagroup/f3dasm_optimize
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD-3-Clause License
 Keywords: keyword1,keyword2,keyword3
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,15 @@
 Requires-Dist: f3dasm>=1.4.5
 Provides-Extra: all
 Requires-Dist: tensorflow; extra == "all"
 Requires-Dist: pygmo; platform_system == "Linux" and extra == "all"
 Requires-Dist: nevergrad; extra == "all"
 Requires-Dist: evosax; extra == "all"
 Requires-Dist: optuna; extra == "all"
+Requires-Dist: optax; extra == "all"
 
 f3dasm_optimize
 ---------------
 *Optimization extension package for the framework for data-driven design \& analysis of structures and materials*
 
 ***
```

### Comparing `f3dasm_optimize-1.4.0/README.md` & `f3dasm_optimize-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/setup.cfg` & `f3dasm_optimize-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/__init__.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/__init__.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,19 @@
                                    DifferentialEvolution, PygmoPSO,
                                    SimulatedAnnealing)
 
 with try_import() as _optuna_imports:
     from .optuna_optimizers import TPESampler
 
 with try_import() as _tensorflow_imports:
-    from .tensorflow_optimizers import SGD, Adam, Adamax, Ftrl, Nadam, RMSprop
+    from .tensorflow_optimizers import (SGD, Adamax, AdamTensorflow, Ftrl,
+                                        Nadam, RMSprop)
+
+with try_import() as _optax_imports:
+    from .optax_optimizers import Adam
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
@@ -39,25 +43,28 @@
     _OPTIMIZERS.extend([CMAES, PygmoPSO, SADE, SEA, SGA, XNES,
                         DifferentialEvolution, SimulatedAnnealing])
 
 if _optuna_imports.is_successful():
     _OPTIMIZERS.extend([TPESampler])
 
 if _tensorflow_imports.is_successful():
-    _OPTIMIZERS.extend([SGD, Adam, Adamax, Ftrl, Nadam, RMSprop])
+    _OPTIMIZERS.extend([SGD, AdamTensorflow, Adamax, Ftrl, Nadam, RMSprop])
 
 if _evosax_imports.is_successful():
     _OPTIMIZERS.extend([EvoSaxPSO, EvoSaxSimAnneal, EvoSaxDE,
                         EvoSaxCMAES])
 
 if _nevergrad_imports.is_successful():
     _OPTIMIZERS.extend([NevergradDE, PSO])
 
+if _optax_imports.is_successful():
+    _OPTIMIZERS.extend([Adam])
+
 __all__ = [
-    'Adam',
+    'AdamTensorflow',
     'Adamax',
     'CMAES',
     'DifferentialEvolution',
     'EvoSaxCMAES',
     'EvoSaxDE',
     'EvoSaxPSO',
     'EvoSaxSimAnneal',
@@ -72,9 +79,10 @@
     'SADE',
     'SEA',
     'SGA',
     'SGD',
     'SimulatedAnnealing',
     'XNES',
     'TPESampler',
+    'Adam',
     '__version__',
 ]
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/_imports.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_imports.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/_protocol.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_protocol.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/evosax_implementations.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/evosax_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/optuna_implementations.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/optuna_implementations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #                                                                       Modules
 # =============================================================================
 
-from typing import Dict
+from typing import Dict, Tuple
 
+import numpy as np
 # Third party
 import optuna
 
 # Local
 from .._protocol import DataGenerator, Domain
 from ..optimizer import Optimizer
 
@@ -15,14 +16,16 @@
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
+optuna.logging.set_verbosity(optuna.logging.WARNING)
+
 
 class OptunaOptimizer(Optimizer):
     def _construct_model(self, data_generator: DataGenerator):
 
         for i in range(len(self.data)):
             experiment_sample = self.data.get_experiment_sample(i)
             self.algorithm.add_trial(
@@ -54,23 +57,27 @@
                 optuna_dict[name] = self.trial.suggest_categorical(
                     name=name, choices=[parameter.value])
 
         return optuna_dict
         # return ExperimentSample(dict_input=optuna_dict,
         # dict_output = {}, jobnumber = 0)
 
-    def update_step(self, data_generator: DataGenerator):
+    def update_step(
+            self, data_generator: DataGenerator
+    ) -> Tuple[np.ndarray, np.ndarray]:
         self.trial = self.algorithm.ask()
         experiment_sample = data_generator._run(
             self._create_trial(), domain=self.domain)
-        self.algorithm.tell(self.trial, experiment_sample.to_numpy()[1])
-        return experiment_sample
+
+        x, y = experiment_sample.to_numpy()
+        self.algorithm.tell(self.trial, y)
+        return np.atleast_2d(x), np.atleast_2d(y)
 
 
-def domain_to_optuna_distributions(domain: Domain):
+def domain_to_optuna_distributions(domain: Domain) -> dict:
     optuna_distributions = {}
     for name, parameter in domain.items():
         if parameter._type == 'float':
             optuna_distributions[
                 name] = optuna.distributions.FloatDistribution(
                 low=parameter.lower_bound,
                 high=parameter.upper_bound, log=parameter.log)
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,18 @@
             logits = 0.0 + tf.cast(self.args["model"](None), tf.float64)
             loss = self.args["func"](tf.reshape(
                 logits, (len(self.domain))))
 
         grads = tape.gradient(loss, self.args["tvars"])
         self.algorithm.apply_gradients(zip(grads, self.args["tvars"]))
 
+        logits = 0.0 + tf.cast(self.args["model"](None), tf.float64)
+        loss = self.args["func"](tf.reshape(
+            logits, (len(self.domain))))
+
         x = logits.numpy().copy()
         y = loss.numpy().copy()
 
         # return the data
         return x, np.atleast_2d(np.array(y))
 
     def _construct_model(self, data_generator: DataGenerator):
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/evosax_optimizers.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/evosax_optimizers.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,51 +39,55 @@
 class PSO_Parameters(OptimizerParameters):
     """Hyperparameters for EvoSaxPSO optimizer"""
 
     population: int = 30
 
 
 class EvoSaxPSO(EvoSaxOptimizer):
+    require_gradients: bool = False
     hyperparameters: PSO_Parameters = PSO_Parameters()
     evosax_algorithm = PSO
 
 # =============================================================================
 
 
 @dataclass
 class SimAnneal_Parameters(OptimizerParameters):
     """Hyperparameters for EvoSaxSimAnneal optimizer"""
 
     population: int = 30
 
 
 class EvoSaxSimAnneal(EvoSaxOptimizer):
+    require_gradients: bool = False
     hyperparameters: SimAnneal_Parameters = SimAnneal_Parameters()
     evosax_algorithm = SimAnneal
 
 # =============================================================================
 
 
 @dataclass
 class DE_Parameters(OptimizerParameters):
     """Hyperparameters for EvoSaxDE optimizer"""
 
     population: int = 30
 
 
 class EvoSaxDE(EvoSaxOptimizer):
+    require_gradients: bool = False
     hyperparameters: DE_Parameters = DE_Parameters()
     evosax_algorithm = DE
 
 # =============================================================================
 
 
 @dataclass
 class BIPOPCMAES_Parameters(OptimizerParameters):
     """Hyperparameters for EvoSaxBIPOP_CMAES optimizer"""
 
     population: int = 30
 
 
 class EvoSaxBIPOPCMAES(EvoSaxOptimizer):
+    require_gradients: bool = False
     hyperparameters: BIPOPCMAES_Parameters = BIPOPCMAES_Parameters()
     evosax_algorithm = BIPOP_CMA_ES
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/nevergrad_optimizers.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/nevergrad_optimizers.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     recommendation: str = 'optimistic'
     crossover: float = 0.5
     F1: float = 0.8
     F2: float = 0.8
 
 
 class NevergradDE(NeverGradOptimizer):
-
+    require_gradients: bool = False
     hyperparameters: NevergradDE_Parameters = NevergradDE_Parameters()
 
     def set_algorithm(self):
         p = ng.p.Array(shape=(len(self.domain),),
                        lower=self.domain.get_bounds()[:, 0],
                        upper=self.domain.get_bounds()[:, 1])
         self.algorithm = ng.optimizers.DifferentialEvolution(
@@ -50,34 +50,35 @@
             F2=self.hyperparameters.F2)(p, budget=1e8)
 
 # =============================================================================
 
 
 @dataclass
 class NevergradPSO_Parameters(OptimizerParameters):
-    population: int = 40
+    population: int = 30
     transform: str = 'identity'
     omega: float = 0.7213475204444817
     phip: float = 1.1931471805599454
     phig: float = 1.1931471805599454
     qo: bool = False
     sqo: bool = False
     so: bool = False
 
 
 class PSO(NeverGradOptimizer):
 
-    parameter: NevergradPSO_Parameters = NevergradPSO_Parameters()
+    require_gradients: bool = False
+    hyperparameters: NevergradPSO_Parameters = NevergradPSO_Parameters()
 
     def set_algorithm(self):
         p = ng.p.Array(shape=(len(self.domain),),
                        lower=self.domain.get_bounds()[:, 0],
                        upper=self.domain.get_bounds()[:, 1])
         self.algorithm = ng.optimizers.ConfPSO(
-            transform=self.parameter.transform,
-            popsize=self.parameter.population,
-            omega=self.parameter.omega,
-            phip=self.parameter.phip,
-            phig=self.parameter.phig,
-            qo=self.parameter.qo,
-            sqo=self.parameter.sqo,
-            so=self.parameter.so)(p, budget=1e8)
+            transform=self.hyperparameters.transform,
+            popsize=self.hyperparameters.population,
+            omega=self.hyperparameters.omega,
+            phip=self.hyperparameters.phip,
+            phig=self.hyperparameters.phig,
+            qo=self.hyperparameters.qo,
+            sqo=self.hyperparameters.sqo,
+            so=self.hyperparameters.so)(p, budget=1e8)
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/optimizer.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 # =============================================================================
 
 from __future__ import annotations
 
 # Standard
 import sys
 from dataclasses import dataclass
-from typing import ClassVar, List, Optional, Tuple
+from typing import ClassVar, Iterable, List, Optional, Tuple
 
 if sys.version_info < (3, 8):  # NOQA
     from typing_extensions import Protocol  # NOQA
 else:
     from typing import Protocol
 
 # Third-party core
 import numpy as np
+import pandas as pd
 
 # Locals
 from ._protocol import DataGenerator, Domain
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
@@ -32,23 +33,30 @@
 #
 # =============================================================================
 
 
 class ExperimentData(Protocol):
     domain: Domain
 
+    @property
+    def index(self, index) -> pd.Index:
+        ...
+
     def get_n_best_output(self, n_samples: int) -> ExperimentData:
         ...
 
     def _reset_index() -> None:
         ...
 
     def to_numpy() -> Tuple[np.ndarray, np.ndarray]:
         ...
 
+    def select(self, indices: int | slice | Iterable[int]) -> ExperimentData:
+        ...
+
 
 @dataclass
 class OptimizerParameters:
     """Interface of a continuous benchmark function
 
     Parameters
     ----------
@@ -60,19 +68,20 @@
 
     population: int = 1
     force_bounds: bool = True
 
 
 class Optimizer:
     type: ClassVar[str] = 'any'
+    require_gradients: ClassVar[bool] = False
     hyperparameters: OptimizerParameters = OptimizerParameters()
 
-    def __init__(self, domain: Domain,
-                 seed: Optional[int] = None,
-                 name: Optional[str] = None, **hyperparameters):
+    def __init__(
+            self, domain: Domain, seed: Optional[int] = None,
+            name: Optional[str] = None, **hyperparameters):
         """Optimizer class for the optimization of a data-driven process
 
         Parameters
         ----------
         domain : Domain
             Domain indicating the search-space of the optimization parameters
         seed : Optional[int], optional
@@ -82,16 +91,16 @@
             Name of the optimization object, by default None,
             it will use the name of the class
 
 
         Note
         ----
 
-        Any additional keyword arguments will be used to overwrite the default
-        hyperparameters of the optimizer.
+        Any additional keyword arguments will be used to overwrite
+        the default hyperparameters of the optimizer.
         """
 
         # Check if **hyperparameters is empty
         if not hyperparameters:
             hyperparameters = {}
 
         # Overwrite the default hyperparameters with the given hyperparameters
@@ -119,84 +128,41 @@
         ...
 
     def _construct_model(self, data_generator: DataGenerator):
         ...
 
     def _check_number_of_datapoints(self):
         """Check if the number of datapoints is sufficient
-        for the initial population
+         for the initial population
 
         Raises
         ------
         ValueError
             Raises then the number of datapoints is insufficient
         """
         if len(self.data) < self.hyperparameters.population:
             raise ValueError(
                 f'There are {len(self.data)} datapoints available, \
-                     need {self.hyperparameters.population} for \
-                         initial population!'
+                     need {self.hyperparameters.population} for initial \
+                         population!'
             )
 
     def set_seed(self):
         """Set the seed of the random number generator"""
         ...
 
     def reset(self, data: ExperimentData):
         """Reset the optimizer to its initial state"""
-        self.data = data
+        self.set_data(data)
         self.__post_init__()
 
     def set_data(self, data: ExperimentData):
         """Set the data attribute to the given data"""
         self.data = data
 
-    def set_x0(self, experiment_data: ExperimentData, mode: str):
-        """Set the initial population to the best n samples of the given data
-
-        Parameters
-        ----------
-        experiment_data : ExperimentData
-            Data to be used for the initial population
-        mode : str
-            Mode of selecting the initial population, by default 'best'
-
-        Raises
-        ------
-        ValueError
-            Raises when the mode is not recognized
-
-        Notes
-        -----
-        The following modes are available:
-            - best: select the best n samples
-            - random: select n random samples
-            - last: select the last n samples
-        """
-        if mode.lower() == 'best':
-            x0 = experiment_data.get_n_best_output(
-                self.hyperparameters.population)
-
-        elif mode.lower() == 'random':
-            x0 = experiment_data.select(
-                np.random.choice(
-                    experiment_data.index,
-                    self.hyperparameters.population, replace=False))
-
-        elif mode.lower() == 'last':
-            x0 = experiment_data.select(
-                experiment_data.index[-self.hyperparameters.population:])
-
-        else:
-            raise ValueError(
-                f'Unknown selection mode {mode}, use best, random or last')
-
-        x0._reset_index()
-        self.data = x0
-
     def get_name(self) -> str:
         """Get the name of the optimizer
 
         Returns
         -------
         str
             name of the optimizer
@@ -209,16 +175,16 @@
         Returns
         -------
             List of strings denoting the characteristics of this optimizer
         """
         return []
 
     def update_step(self, data_generator: DataGenerator) -> ExperimentData:
-        """Update step of the optimizer. Needs to be
-        implemented by the child class
+        """Update step of the optimizer. Needs to be implemented
+         by the child class
 
         Parameters
         ----------
         data_generator : DataGenerator
             data generator object to calculate the objective value
 
         Returns
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/optuna_optimizers.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optuna_optimizers.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,10 +14,11 @@
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
 class TPESampler(OptunaOptimizer):
+    require_gradients: bool = False
     def set_algorithm(self):
         self.algorithm = optuna.create_study(
             sampler=optuna.samplers.TPESampler(seed=self.seed))
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/pygmo_optimizers.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/pygmo_optimizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 class CMAES(PygmoAlgorithm):
     """Covariance Matrix Adaptation Evolution Strategy optimizer
     implemented from pygmo"""
 
     hyperparameters: CMAES_Parameters = CMAES_Parameters()
+    require_gradients: bool = False
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.cmaes(
                 gen=1,
                 memory=True,
                 seed=self.seed,
@@ -70,15 +71,15 @@
     variant: int = 2
     ftol: float = 0.0
     xtol: float = 0.0
 
 
 class DifferentialEvolution(PygmoAlgorithm):
     "DifferentialEvolution optimizer implemented from pygmo"
-
+    require_gradients: bool = False
     hyperparameters: DifferentialEvolution_Parameters = \
         DifferentialEvolution_Parameters()
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.de(
                 gen=1,
@@ -109,15 +110,15 @@
 
 
 class PygmoPSO(PygmoAlgorithm):
     """
     Particle Swarm Optimization (Generational) optimizer
     implemented from pygmo
     """
-
+    require_gradients: bool = False
     hyperparameters: PSO_Parameters = PSO_Parameters()
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.pso_gen(
                 gen=1,
                 memory=True,
@@ -143,15 +144,15 @@
     variant_adptv: int = 1
     ftol: float = 0.0
     xtol: float = 0.0
 
 
 class SADE(PygmoAlgorithm):
     "Self-adaptive Differential Evolution optimizer implemented from pygmo"
-
+    require_gradients: bool = False
     hyperparameters: SADE_Parameters = SADE_Parameters()
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.sade(
                 gen=1,
                 variant=self.hyperparameters.variant,
@@ -168,21 +169,21 @@
 
 
 # =============================================================================
 
 @dataclass
 class SEA_Parameters(OptimizerParameters):
     """Hyperparameters for SEA optimizer"""
-
+    require_gradients: bool = False
     population: int = 30
 
 
 class SEA(PygmoAlgorithm):
     """Simple Evolutionary Algorithm optimizer implemented from pygmo"""
-
+    require_gradients: bool = False
     hyperparameters: SEA_Parameters = SEA_Parameters()
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.sea(
                 gen=1,
                 seed=self.seed,
@@ -208,15 +209,15 @@
     mutation: str = "polynomial"
     selection: str = "tournament"
     population: int = 30
 
 
 class SGA(PygmoAlgorithm):
     """Simple Genetic Algorithm optimizer implemented from pygmo"""
-
+    require_gradients: bool = False
     hyperparameters: SGA_Parameters = SGA_Parameters()
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.sga(
                 gen=1,
                 cr=self.hyperparameters.cr,
@@ -248,15 +249,15 @@
     n_range_adj: int = 10
     bin_size: int = 10
     start_range: float = 1.0
 
 
 class SimulatedAnnealing(PygmoAlgorithm):
     "DifferentialEvolution optimizer implemented from pygmo"
-
+    require_gradients: bool = False
     hyperparameters: SimulatedAnnealing_Parameters = \
         SimulatedAnnealing_Parameters()
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.simulated_annealing(
                 Ts=self.hyperparameters.Ts,
@@ -289,15 +290,15 @@
     sigma0: float = -1.0
     ftol: float = 1e-06
     xtol: float = 1e-06
 
 
 class XNES(PygmoAlgorithm):
     """XNES optimizer implemented from pygmo"""
-
+    require_gradients: bool = False
     hyperparameters: XNES_Parameters = XNES_Parameters()
 
     def set_algorithm(self):
         self.algorithm = pg.algorithm(
             pg.xnes(
                 gen=1,
                 eta_mu=self.hyperparameters.eta_mu,
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize/_src/tensorflow_optimizers.py` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/tensorflow_optimizers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Information on the Adam optimizer
 """
 #                                                                       Modules
 # =============================================================================
 
+
 # Standard
 from dataclasses import dataclass
 from typing import List
 
 # Third-party
 import tensorflow as tf
 
@@ -22,28 +23,28 @@
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
 @dataclass
-class Adam_Parameters(OptimizerParameters):
+class AdamTensorflow_Parameters(OptimizerParameters):
     """Hyperparameters for Adam optimizer"""
 
     learning_rate: float = 0.001
     beta_1: float = 0.9
     beta_2: float = 0.999
     epsilon: float = 1e-07
     amsgrad: bool = False
 
 
-class Adam(TensorflowOptimizer):
+class AdamTensorflow(TensorflowOptimizer):
     """Adam"""
-
-    hyperparameters: Adam_Parameters = Adam_Parameters()
+    require_gradients: bool = True
+    hyperparameters: AdamTensorflow_Parameters = AdamTensorflow_Parameters()
 
     def set_algorithm(self):
         self.algorithm = tf.keras.optimizers.Adam(
             learning_rate=self.hyperparameters.learning_rate,
             beta_1=self.hyperparameters.beta_1,
             beta_2=self.hyperparameters.beta_2,
             epsilon=self.hyperparameters.epsilon,
@@ -64,15 +65,15 @@
     beta_1: float = 0.9
     beta_2: float = 0.999
     epsilon: float = 1e-07
 
 
 class Adamax(TensorflowOptimizer):
     """Adamax"""
-
+    require_gradients: bool = True
     hyperparameters: Adamax_Parameters = Adamax_Parameters()
 
     def set_algorithm(self):
         self.algorithm = tf.keras.optimizers.Adamax(
             learning_rate=self.hyperparameters.learning_rate,
             beta_1=self.hyperparameters.beta_1,
             beta_2=self.hyperparameters.beta_2,
@@ -96,15 +97,15 @@
     l2_regularization_strength: float = 0.0
     l2_shrinkage_regularization_strength: float = 0.0
     beta: float = 0.0
 
 
 class Ftrl(TensorflowOptimizer):
     """Ftrl"""
-
+    require_gradients: bool = True
     hyperparameters: Ftrl_Parameters = Ftrl_Parameters()
 
     def set_algorithm(self):
         self.algorithm = tf.keras.optimizers.Ftrl(
             learning_rate=self.
             hyperparameters.learning_rate,
             learning_rate_power=self.
@@ -136,15 +137,15 @@
     beta_1: float = 0.9
     beta_2: float = 0.999
     epsilon: float = 1e-07
 
 
 class Nadam(TensorflowOptimizer):
     """Nadam"""
-
+    require_gradients: bool = True
     hyperparameters: Nadam_Parameters = Nadam_Parameters()
 
     def set_algorithm(self):
         self.algorithm = tf.keras.optimizers.Nadam(
             learning_rate=self.hyperparameters.learning_rate,
             beta_1=self.hyperparameters.beta_1,
             beta_2=self.hyperparameters.beta_2,
@@ -166,15 +167,15 @@
     momentum: float = 0.0
     epsilon: float = 1e-07
     centered: bool = False
 
 
 class RMSprop(TensorflowOptimizer):
     """RMSprop"""
-
+    require_gradients: bool = True
     hyperparameters: RMSprop_Parameters = RMSprop_Parameters()
 
     def set_algorithm(self):
         self.algorithm = tf.keras.optimizers.RMSprop(
             learning_rate=self.hyperparameters.learning_rate,
             rho=self.hyperparameters.rho,
             momentum=self.hyperparameters.momentum,
@@ -195,15 +196,15 @@
     learning_rate: float = 0.01
     momentum: float = 0.0
     nesterov: bool = False
 
 
 class SGD(TensorflowOptimizer):
     """SGD"""
-
+    require_gradients: bool = True
     hyperparameters: SGD_Parameters = SGD_Parameters()
 
     def set_algorithm(self):
         self.algorithm = tf.keras.optimizers.SGD(
             learning_rate=self.hyperparameters.learning_rate,
             momentum=self.hyperparameters.momentum,
             nesterov=self.hyperparameters.nesterov,
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/PKG-INFO` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: f3dasm-optimize
-Version: 1.4.0
+Name: f3dasm_optimize
+Version: 1.5.1
 Summary: f3dasm_optimize: Your one line description of the package
 Home-page: https://github.com/bessagroup/f3dasm_optimize
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD-3-Clause License
 Keywords: keyword1,keyword2,keyword3
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,15 @@
 Requires-Dist: f3dasm>=1.4.5
 Provides-Extra: all
 Requires-Dist: tensorflow; extra == "all"
 Requires-Dist: pygmo; platform_system == "Linux" and extra == "all"
 Requires-Dist: nevergrad; extra == "all"
 Requires-Dist: evosax; extra == "all"
 Requires-Dist: optuna; extra == "all"
+Requires-Dist: optax; extra == "all"
 
 f3dasm_optimize
 ---------------
 *Optimization extension package for the framework for data-driven design \& analysis of structures and materials*
 
 ***
```

### Comparing `f3dasm_optimize-1.4.0/src/f3dasm_optimize.egg-info/SOURCES.txt` & `f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 src/f3dasm_optimize.egg-info/requires.txt
 src/f3dasm_optimize.egg-info/top_level.txt
 src/f3dasm_optimize/_src/__init__.py
 src/f3dasm_optimize/_src/_imports.py
 src/f3dasm_optimize/_src/_protocol.py
 src/f3dasm_optimize/_src/evosax_optimizers.py
 src/f3dasm_optimize/_src/nevergrad_optimizers.py
+src/f3dasm_optimize/_src/optax_optimizers.py
 src/f3dasm_optimize/_src/optimizer.py
 src/f3dasm_optimize/_src/optuna_optimizers.py
 src/f3dasm_optimize/_src/pygmo_optimizers.py
 src/f3dasm_optimize/_src/tensorflow_optimizers.py
 src/f3dasm_optimize/_src/adapters/__init__.py
 src/f3dasm_optimize/_src/adapters/evosax_implementations.py
 src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py
+src/f3dasm_optimize/_src/adapters/optax_implementations.py
 src/f3dasm_optimize/_src/adapters/optuna_implementations.py
 src/f3dasm_optimize/_src/adapters/pygmo_implementations.py
 src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py
```

