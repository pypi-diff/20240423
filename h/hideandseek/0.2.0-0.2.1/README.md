# Comparing `tmp/hideandseek-0.2.0.tar.gz` & `tmp/hideandseek-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hideandseek-0.2.0.tar", last modified: Wed Apr  3 19:23:06 2024, max compression
+gzip compressed data, was "hideandseek-0.2.1.tar", last modified: Mon Apr 22 19:51:15 2024, max compression
```

## Comparing `hideandseek-0.2.0.tar` & `hideandseek-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:23:06.936522 hideandseek-0.2.0/
--rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2757 2024-04-03 19:23:06.935528 hideandseek-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2024-01-25 04:08:16.000000 hideandseek-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 19:23:06.900141 hideandseek-0.2.0/hideandseek/
--rw-rw-rw-   0        0        0      375 2024-04-03 19:20:38.000000 hideandseek-0.2.0/hideandseek/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.2.0/hideandseek/dataset.py
--rw-rw-rw-   0        0        0    16568 2024-03-18 18:58:07.000000 hideandseek-0.2.0/hideandseek/eval.py
--rw-rw-rw-   0        0        0     7428 2022-06-27 08:00:35.000000 hideandseek-0.2.0/hideandseek/fv.py
--rw-rw-rw-   0        0        0     2354 2024-03-04 21:20:35.000000 hideandseek-0.2.0/hideandseek/loss.py
--rw-rw-rw-   0        0        0     3187 2024-01-25 21:40:22.000000 hideandseek-0.2.0/hideandseek/model.py
--rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.2.0/hideandseek/plot.py
--rw-rw-rw-   0        0        0    24677 2024-04-03 19:22:41.000000 hideandseek-0.2.0/hideandseek/trainer.py
--rw-rw-rw-   0        0        0     4761 2024-01-26 19:12:55.000000 hideandseek-0.2.0/hideandseek/utils.py
--rw-rw-rw-   0        0        0    11727 2024-01-25 21:35:05.000000 hideandseek-0.2.0/hideandseek/validation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:23:06.933528 hideandseek-0.2.0/hideandseek.egg-info/
--rw-rw-rw-   0        0        0     2757 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 19:23:06.936522 hideandseek-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 19:51:15.136883 hideandseek-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2757 2024-04-22 19:51:15.135888 hideandseek-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2024-01-25 04:08:16.000000 hideandseek-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 19:51:15.083213 hideandseek-0.2.1/hideandseek/
+-rw-rw-rw-   0        0        0      330 2024-04-22 19:37:08.000000 hideandseek-0.2.1/hideandseek/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.2.1/hideandseek/dataset.py
+-rw-rw-rw-   0        0        0    16568 2024-03-18 18:58:07.000000 hideandseek-0.2.1/hideandseek/evaluation.py
+-rw-rw-rw-   0        0        0     9959 2024-04-22 19:50:56.000000 hideandseek-0.2.1/hideandseek/fv.py
+-rw-rw-rw-   0        0        0     2354 2024-03-04 21:20:35.000000 hideandseek-0.2.1/hideandseek/loss.py
+-rw-rw-rw-   0        0        0     3187 2024-01-25 21:40:22.000000 hideandseek-0.2.1/hideandseek/model.py
+-rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.2.1/hideandseek/plot.py
+-rw-rw-rw-   0        0        0    24904 2024-04-22 19:50:06.000000 hideandseek-0.2.1/hideandseek/trainer.py
+-rw-rw-rw-   0        0        0     4757 2024-04-22 19:32:15.000000 hideandseek-0.2.1/hideandseek/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 19:51:15.133881 hideandseek-0.2.1/hideandseek.egg-info/
+-rw-rw-rw-   0        0        0     2757 2024-04-22 19:51:13.000000 hideandseek-0.2.1/hideandseek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-22 19:51:14.000000 hideandseek-0.2.1/hideandseek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 19:51:13.000000 hideandseek-0.2.1/hideandseek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-22 19:51:14.000000 hideandseek-0.2.1/hideandseek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 19:51:14.000000 hideandseek-0.2.1/hideandseek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 19:51:15.137882 hideandseek-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.2.1/setup.py
```

### Comparing `hideandseek-0.2.0/LICENSE` & `hideandseek-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.0/PKG-INFO` & `hideandseek-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.2.0
+Version: 0.2.1
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.2.0/README.md` & `hideandseek-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.0/hideandseek/dataset.py` & `hideandseek-0.2.1/hideandseek/dataset.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.0/hideandseek/eval.py` & `hideandseek-0.2.1/hideandseek/evaluation.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.0/hideandseek/loss.py` & `hideandseek-0.2.1/hideandseek/loss.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.0/hideandseek/model.py` & `hideandseek-0.2.1/hideandseek/model.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.0/hideandseek/plot.py` & `hideandseek-0.2.1/hideandseek/plot.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.2.0/hideandseek/trainer.py` & `hideandseek-0.2.1/hideandseek/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 import torch.optim as optim
 import torch.utils.data as D
 
 import tools # since T is used as a variable in this module, refrain from "import tools as T"
 import tools.torch
 import tools.modules
 
-# from . import validation as V
 from . import utils as U
-from . import eval as E
+from . import evaluation as E
 from . import model as M
 
 # __all__ = [
 # 'Trainer'
 # ]
 
 # %%
@@ -45,14 +44,15 @@
 
         :param validation: dict of Validation objects
 
         :param cfg_train: dict-like object which contains:
             lr
             batch_size
             weight_decay (optional)
+            cv_step (optional)
         
         :param cfg_val (optional): dict-like object which contains:
             increase_better
             patience
             batch_size
             target_dataset (optional, if val_dataset is dict for multiple datasets)
             criterion (optional, if val_metrics is dict for multiple metrics) 
@@ -319,15 +319,15 @@
 
         except Exception as e:
             log.warning(e)
             import pdb; pdb.set_trace()
 
     def _forward(self, data):
         '''
-        Pseudo function to support amp (automatic mixed precision)
+        Pseudo function to support passing tuple or dict from a batch from dataloader to forward()
         '''
         datatype = type(data)
         # When data is given as a tuple/list
         if datatype is tuple or datatype is list:
             data = [x.to(self._device) for x in data]
             N = len(data[0]) # number of data in batch
             outputs = self.forward(*data)
@@ -340,32 +340,36 @@
 
         else:
             raise Exception(f'return type from dataset must be one of [tuple, list, dict], received: {datatype}')
         return outputs, N
 
     def forward(self, x, y):
         """
-        Forward pass. Receive data and return the loss function.
-        Inherit Node and define new forward() function to build custom forward pass.
+        Forward pass: Receive data and pass values to criterion.
+        Define forward for custom trainers.
 
         May return tuple or dictionary, whichever will be feeded to criterion.
-        """
 
+        Defaults to args[0] feeding to self.network (assuming x), and args[1] feeding to self.criterion (assuming y)
+        """
+        
         y_hat = self.network(x)
 
         return y_hat, y
 
     def _criterion(self, outputs):
         outputstype = type(outputs)
         if outputstype is tuple or outputstype is list:
             loss = self.criterion(*outputs)
         elif outputstype==dict:
             loss = self.criterion(**outputs)
+        elif outputstype==torch.Tensor:
+            loss = self.criterion(outputs)
         else:
-            raise Exception(f'return type from forward must be one of [tuple, list, dict], received: {type(outputs)}')
+            raise Exception(f'return type from forward must be one of [tuple, list, dict, torch.Tensor], received: {type(outputs)}')
         return loss
 
     def epoch_f(self):
         # TODO: rename to forward hook? epoch_hook?
         '''function to call every other epoch. May be used in child class'''
         pass
 
@@ -447,15 +451,15 @@
 
     def save(self, path=None, best=True):
         '''
         Save the following:
         state_dict() -> path/state_dict.p
         network.state_dict() -> path/network.pt
         '''
-        path = self.model_dir if path is None else path
+        path = self.network_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
         state_dict_path = os.path.join(path, 'node.p')
         self.print(f'[save] Saving node info to: {state_dict_path}')
         state_dict = self.state_dict()
         self.print(f'[save] state_dict: {list(state_dict.keys())}')
         tools.save_pickle(state_dict, state_dict_path)
@@ -478,15 +482,15 @@
 
     def load(self, path=None):
         '''
         load state_dict() and network:
         path/node.p -> state_dict
         path/network.pt -> network.state_dict
         '''
-        path = self.model_dir if path is None else path
+        path = self.network_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
         state_dict_path = os.path.join(path, 'node.p')
         self.print(f'[load] Loading from path: {state_dict_path}')
         state_dict = tools.load_pickle(state_dict_path)
         self.print(f'[load] Updating: {list(state_dict.keys())}')
         self.load_state_dict(state_dict)
```

### Comparing `hideandseek-0.2.0/hideandseek/utils.py` & `hideandseek-0.2.1/hideandseek/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     '''
     d = {}
     for cfg in listconfig:
         key, value = cfg.split('=')
         d[key]=value
     return d
 
-
 def load_cfg(subdir):
     cfg = OmegaConf.load(os.path.join(subdir, '.hydra/config.yaml'))
     overrides = overrides_to_dict(OmegaConf.load(os.path.join(subdir, '.hydra/overrides.yaml')))
     return cfg, overrides
 
 def load_cfg_sweep(l_subdir):
     '''
@@ -125,15 +124,14 @@
     else:
         return 'unknown'
 
 def extract_dataset(dataset):
     if hasattr(dataset, 'get_x_all'):
         x = dataset.get_x_all()
 
-
     return {'x': x, 'y': y}
 
 def add_batch_dim(data):
     """
     adds batch dimension (axis=0)
 
     Parameters
```

### Comparing `hideandseek-0.2.0/hideandseek.egg-info/PKG-INFO` & `hideandseek-0.2.1/hideandseek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.2.0
+Version: 0.2.1
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.2.0/setup.py` & `hideandseek-0.2.1/setup.py`

 * *Files identical despite different names*

