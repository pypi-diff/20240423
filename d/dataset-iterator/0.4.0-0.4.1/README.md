# Comparing `tmp/dataset_iterator-0.4.0.tar.gz` & `tmp/dataset_iterator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.4.0.tar", last modified: Fri Apr 12 15:30:01 2024, max compression
+gzip compressed data, was "dataset_iterator-0.4.1.tar", last modified: Tue Apr 23 08:09:09 2024, max compression
```

## Comparing `dataset_iterator-0.4.0.tar` & `dataset_iterator-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:01.872205 dataset_iterator-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-12 15:30:01.872205 dataset_iterator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:01.868205 dataset_iterator-0.4.0/dataset_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/concat_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:01.872205 dataset_iterator-0.4.0/dataset_iterator/datasetIO/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/group_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/h5pyIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/memoryIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/hard_sample_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/image_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/index_array_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57974 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/multichannel_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19770 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/tile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/tracking_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/dataset_iterator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:01.872205 dataset_iterator-0.4.0/dataset_iterator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-12 15:30:01.000000 dataset_iterator-0.4.0/dataset_iterator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 15:30:01.000000 dataset_iterator-0.4.0/dataset_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:30:01.000000 dataset_iterator-0.4.0/dataset_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 15:30:01.000000 dataset_iterator-0.4.0/dataset_iterator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 15:30:01.000000 dataset_iterator-0.4.0/dataset_iterator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:30:01.872205 dataset_iterator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-12 15:29:58.000000 dataset_iterator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.088481 dataset_iterator-0.4.1/dataset_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/concat_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/dataset_iterator/datasetIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/h5pyIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/memoryIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/hard_sample_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/image_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/index_array_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57974 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/multichannel_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/ordered_enqueuer_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/tracking_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/dataset_iterator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/dataset_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 08:09:09.000000 dataset_iterator-0.4.1/dataset_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:09:09.092481 dataset_iterator-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-23 08:09:05.000000 dataset_iterator-0.4.1/setup.py
```

### Comparing `dataset_iterator-0.4.0/LICENSE.txt` & `dataset_iterator-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/PKG-INFO` & `dataset_iterator-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.0/dataset_iterator-0.4.0.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.1/dataset_iterator-0.4.1.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.0/README.md` & `dataset_iterator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/__init__.py` & `dataset_iterator-0.4.1/dataset_iterator/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 name = "dataset_iterator"
 
 from .index_array_iterator import IndexArrayIterator
 from .multichannel_iterator import MultiChannelIterator
 from .tracking_iterator import TrackingIterator
-from .tile_utils import extract_tiles, augment_tiles, extract_tile_function, extract_tile_random_zoom_function, augment_tiles_inplace
+from .tile_utils import extract_tile_function, extract_tile_random_zoom_function, extract_single_tile
 from .image_data_generator import get_image_data_generator
 
 from .datasetIO import DatasetIO, H5pyIO, MultipleFileIO, MultipleDatasetIO, ConcatenateDatasetIO, MemoryIO
 from .hard_sample_mining import HardSampleMiningCallback
 from .concat_iterator import ConcatIterator
+from .utils import get_tf_version
```

### Comparing `dataset_iterator-0.4.0/dataset_iterator/concat_iterator.py` & `dataset_iterator-0.4.1/dataset_iterator/concat_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.4.1/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.4.1/dataset_iterator/datasetIO/datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.4.1/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.4.1/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/datasetIO/memoryIO.py` & `dataset_iterator-0.4.1/dataset_iterator/datasetIO/memoryIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.4.1/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/hard_sample_mining.py` & `dataset_iterator-0.4.1/dataset_iterator/hard_sample_mining.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import warnings
 import os
 import numpy as np
 import tensorflow as tf
 from .index_array_iterator import IndexArrayIterator, INCOMPLETE_LAST_BATCH_MODE
+from dataset_iterator.ordered_enqueuer_cf import OrderedEnqueuerCF
+import threading
 
 class HardSampleMiningCallback(tf.keras.callbacks.Callback):
-    def __init__(self, iterator, target_iterator, predict_fun, metrics_fun, period:int=10, start_epoch:int=0, skip_first:bool=False, enrich_factor:float=10., quantile_max:float=0.99, quantile_min:float=None, disable_channel_postprocessing:bool=False, workers=None, verbose:int=1):
+    def __init__(self, iterator, target_iterator, predict_fun, metrics_fun, period:int=10, start_epoch:int=0, skip_first:bool=False, start_from_epoch:int=0, enrich_factor:float=10., quantile_max:float=0.99, quantile_min:float=None, disable_channel_postprocessing:bool=False, workers=None, verbose:int=1):
         super().__init__()
         self.period = period
         self.start_epoch = start_epoch
+        self.start_from_epoch = start_from_epoch
         self.skip_first = skip_first
         self.iterator = iterator
         self.target_iterator = target_iterator
         self.predict_fun = predict_fun
         self.metrics_fun = metrics_fun
         self.enrich_factor = enrich_factor
         self.quantile_max = quantile_max
@@ -23,62 +26,77 @@
         self.metric_idx = -1
         self.proba_per_metric = None
         self.n_metrics = 0
         self.data_aug_param = self.iterator.disable_random_transforms(True, self.disable_channel_postprocessing)
         simple_iterator = SimpleIterator(self.iterator)
         self.batch_size = self.iterator.get_batch_size()
         self.n_batches = len(simple_iterator)
-        self.enq = tf.keras.utils.OrderedEnqueuer(simple_iterator, use_multiprocessing=True, shuffle=False)
+        self.enq = OrderedEnqueuerCF(simple_iterator, single_epoch=True, shuffle=False)
+        self.wait_for_me = threading.Event()
 
     def close(self):
         self.enq.stop()
         if self.data_aug_param is not None:
             self.iterator.enable_random_transforms(self.data_aug_param)
         self.iterator.close()
 
     def on_epoch_begin(self, epoch, logs=None):
-        if self.period==1 or (epoch + self.start_epoch) % self.period == 0:
-            if epoch == 0 and self.skip_first:
-                return
-            metrics = self.compute_metrics()
-            first = self.proba_per_metric is None
-            self.proba_per_metric = get_index_probability(metrics, enrich_factor=self.enrich_factor, quantile_max=self.quantile_max, quantile_min=self.quantile_min, verbose=self.verbose)
-            self.n_metrics = self.proba_per_metric.shape[0] if len(self.proba_per_metric.shape) == 2 else 1
-            if first and self.n_metrics > self.period:
-                warnings.warn(f"Hard sample mining period = {self.period} should be greater than metric number = {self.n_metrics}")
+        self.wait_for_me.clear() # will block
+
+    def on_epoch_end(self, epoch, logs=None):
+        if self.period==1 or (epoch + 1 + self.start_epoch) % self.period == 0:
+            if (epoch > 0 or not self.skip_first) and epoch + self.start_epoch >= self.start_from_epoch:
+                metrics = self.compute_metrics()
+                first = self.proba_per_metric is None
+                self.proba_per_metric = get_index_probability(metrics, enrich_factor=self.enrich_factor, quantile_max=self.quantile_max, quantile_min=self.quantile_min, verbose=self.verbose)
+                self.n_metrics = self.proba_per_metric.shape[0] if len(self.proba_per_metric.shape) == 2 else 1
+                if first and self.n_metrics > self.period:
+                    warnings.warn(f"Hard sample mining period = {self.period} should be greater than metric number = {self.n_metrics}")
         if self.proba_per_metric is not None:
             if len(self.proba_per_metric.shape) == 2:
                 self.metric_idx = (self.metric_idx + 1) % self.n_metrics
                 proba = self.proba_per_metric[self.metric_idx]
             else:
                 proba = self.proba_per_metric
             # set probability to iterator in case of multiprocessing iwth OrderedEnqueeur this will be taken into account only a next epoch has iterator has already been sent to processes at this stage
             self.target_iterator.set_index_probability(proba)
+        self.wait_for_me.set() # release block
 
     def on_train_end(self, logs=None):
         self.close()
 
     def compute_metrics(self):
         workers = os.cpu_count() if self.workers is None else self.workers
-        self.enq.start(workers=workers, max_queue_size=max(3, min(self.n_batches, workers)))
+        self.enq.start(workers=workers, max_queue_size=max(2, min(self.n_batches, workers)))
         gen = self.enq.get()
         compute_metrics_fun = get_compute_metrics_fun(self.predict_fun, self.metrics_fun, self.batch_size)
-        metrics = compute_metrics_loop(compute_metrics_fun, gen, self.batch_size, self.n_batches, self.verbose)
+        computed = False
+        metrics = None
+        while not computed:
+            try:
+                metrics = compute_metrics_loop(compute_metrics_fun, gen, self.batch_size, self.n_batches, self.verbose)
+            except BrokenPipeError as e:
+                print("broken pipe error, will re-try metric computation")
+                self.enq.stop()
+                self.enq.start(workers=workers, max_queue_size=max(2, min(self.n_batches, workers)))
+                gen = self.enq.get()
+            else:
+                computed = True
         self.enq.stop()
+        #self.iterator.close()
         return metrics
 
 
 def get_index_probability_1d(metric, enrich_factor:float=10., quantile_min:float=0.01, quantile_max:float=None, max_power:int=10, power_accuracy:float=0.1, verbose:int=1):
     assert 0.5 > quantile_min >= 0, f"invalid min quantile: {quantile_min}"
+    if 1. / enrich_factor < quantile_min: # incompatible enrich factor and quantile
+        quantile_min = 1. / enrich_factor
+        #print(f"modified quantile_min to : {quantile_min}")
     if quantile_max is None:
         quantile_max = 1 - quantile_min
-    assert 1 >= quantile_max > 0.5, f"invalid max quantile: {quantile_max}"
-    if 1. / enrich_factor < (1 - quantile_max): # incompatible enrich factor and quantile
-        quantile_max = 1. - 1 / enrich_factor
-        #print(f"modified quantile_max to : {quantile_max}")
     metric_quantiles = np.quantile(metric, [quantile_min, quantile_max])
 
     Nh = metric[metric <= metric_quantiles[0]].shape[0] # hard examples (low metric)
     Ne = metric[metric >= metric_quantiles[1]].shape[0] # easy examples (high metric)
     metric_sub = metric[(metric < metric_quantiles[1]) & (metric > metric_quantiles[0])]
     Nm = metric_sub.shape[0]
     S = np.sum( ((metric_sub - metric_quantiles[1]) / (metric_quantiles[0] - metric_quantiles[1])) )
@@ -110,16 +128,16 @@
         else:
             return p_min + (p_max - p_min) * ((value - metric_quantiles[1]) / (metric_quantiles[0] - metric_quantiles[1]))**power
 
     vget_proba = np.vectorize(get_proba)
     proba = vget_proba(metric)
     p_sum = float(np.sum(proba))
     proba /= p_sum
-    if verbose > 1:
-        print(f"metric proba range: [{np.min(proba) * metric.shape[0]}, {np.max(proba) * metric.shape[0]}] (target range: [{p_min}; {p_max}]) power: {power} sum: {p_sum} quantiles: [{quantile_min}; {quantile_max}]", flush=True)
+    #if verbose > 1:
+    #    print(f"metric proba range: [{np.min(proba) * metric.shape[0]}, {np.max(proba) * metric.shape[0]}] (target range: [{p_min}; {p_max}]) power: {power} sum: {p_sum} quantiles: [{quantile_min}; {quantile_max}]", flush=True)
     return proba
 
 def get_index_probability(metrics, enrich_factor:float=10., quantile_max:float=0.99, quantile_min:float=None, verbose:int=1):
     if len(metrics.shape) == 1:
         return get_index_probability_1d(metrics, enrich_factor=enrich_factor, quantile_max=quantile_max, quantile_min=quantile_min, verbose=verbose)
     probas_per_metric = [get_index_probability_1d(metrics[:, i], enrich_factor=enrich_factor, quantile_max=quantile_max, quantile_min=quantile_min, verbose=verbose) for i in range(metrics.shape[1])]
     probas_per_metric = np.stack(probas_per_metric, axis=0)
@@ -133,56 +151,47 @@
     batch_size = iterator.get_batch_size()
     n_batches = len(simple_iterator)
 
     compute_metrics_fun = get_compute_metrics_fun(predict_function, metrics_function, batch_size)
 
     if workers is None:
         workers = os.cpu_count()
-    enq = tf.keras.utils.OrderedEnqueuer(simple_iterator, use_multiprocessing=True, shuffle=False)
+    #enq = tf.keras.utils.OrderedEnqueuer(simple_iterator, use_multiprocessing=True, shuffle=False)
+    enq = OrderedEnqueuerCF(simple_iterator, single_epoch=True, shuffle=False)
     enq.start(workers=workers, max_queue_size=max(3, min(n_batches, workers)))
     gen = enq.get()
     metrics = compute_metrics_loop(compute_metrics_fun, gen, batch_size, n_batches, verbose)
     enq.stop()
     if data_aug_param is not None:
         iterator.enable_random_transforms(data_aug_param)
     iterator.close()
     return metrics
 
 def compute_metrics_loop(compute_metrics_fun, gen, batch_size, n_batches, verbose):
     metrics = []
-    indices = []
     if verbose>=1:
-        print(f"Hard Sample Mining: computing metrics...")
+        print(f"Hard Sample Mining: computing metrics...", flush=True)
         progbar = tf.keras.utils.Progbar(n_batches)
     n_tiles = None
     for i in range(n_batches):
-        current_indices, x, y_true = next(gen)
+        x, y_true = next(gen)
         batch_metrics = compute_metrics_fun(x, y_true)
         if x.shape[0] > batch_size or n_tiles is not None:  # tiling: keep hardest tile per sample
             if n_tiles is None:  # record n_tile which is constant but last batch may have fewer elements
                 n_tiles = x.shape[0] // batch_size
             batch_metrics = tf.reshape(batch_metrics, shape=(n_tiles, -1, batch_metrics.shape[1]))
             batch_metrics = tf.reduce_max(batch_metrics, axis=0, keepdims=False)  # record hardest tile per sample
         metrics.append(batch_metrics)
-        indices.append(current_indices)
         if verbose >= 1:
             progbar.update(i + 1)
-    if verbose >= 1:
-        print("metrics computed", flush=True)
-    indices = tf.concat(indices, axis=0).numpy()
     metrics = tf.concat(metrics, axis=0).numpy()
-    if len(metrics.shape) == 1:
-        metrics = indices[:, np.newaxis]
     # metrics = tf.concat([indices[:, np.newaxis].astype(metrics.dtype), metrics], axis=1)
-    if not np.all(indices[1:] - indices[:-1] == 1):
-        indices = np.argsort(indices)
-        metrics = metrics[indices, :]
-        if verbose >= 1:
-            print("some indices where not in order!!", flush=True)
     return metrics
+
+
 def get_compute_metrics_fun(predict_function, metrics_function, batch_size):
     @tf.function
     def compute_metrics(x, y_true):
         y_pred = predict_function(x)
         n_samples = tf.shape(x)[0]
         def metrics_fun(j): # compute metric per batch item in case metric is reduced along batch size
             y_t = [y_true[k][j:j+1] for k in range(len(y_true))]
@@ -201,19 +210,19 @@
         self.iterator = iterator
         self.input_scaling_function = batchwise_inplace(input_scaling_function) if input_scaling_function is not None else None
 
     def _get_batches_of_transformed_samples(self, index_array):
         batch = self.iterator._get_batches_of_transformed_samples(index_array)
         if isinstance(batch, (list, tuple)):
             x, y = batch
-            batch = index_array, x, y
+            batch = x, y
         else:
             if self.input_scaling_function is not None:
                 x = self.input_scaling_function(batch)
-            batch = index_array, x
+            batch = x
         return batch
 
 def batchwise_inplace(function):
     def fun(batch):
         for i in range(batch.shape[0]):
             batch[i] = function(batch[i])
         return batch
```

### Comparing `dataset_iterator-0.4.0/dataset_iterator/helpers.py` & `dataset_iterator-0.4.1/dataset_iterator/helpers.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/image_data_generator.py` & `dataset_iterator-0.4.1/dataset_iterator/image_data_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 import numpy as np
 from random import uniform, random, getrandbits
-from .utils import is_list, ensure_multiplicity
+from .utils import is_list, ensure_multiplicity, get_tf_version
 from .pre_processing import get_center_scale_range, compute_histogram_range, adjust_histogram_range, add_poisson_noise, add_speckle_noise, add_gaussian_noise, gaussian_blur, get_histogram_elasticdeform_target_points_delta, histogram_elasticdeform, get_illumination_variation_target_points, illumination_variation
 
 def get_image_data_generator(scaling_parameters=None, illumination_parameters=None, affine_transform_parameters=None):
     generators = []
     if scaling_parameters is not None:
         if isinstance(scaling_parameters, dict):
             generators.append(ScalingImageGenerator(**scaling_parameters))
@@ -356,15 +356,15 @@
 
     def standardize(self, img):
         return img
 
 class KerasImageDataGenerator(tf.keras.preprocessing.image.ImageDataGenerator):
     def __init__(self, **kwargs):
         if "interpolation_order" in kwargs: # interpolation_order was introduced at version 2.9.0
-            tf_version = tuple(map(int, (tf.__version__.split("."))))
+            tf_version = get_tf_version()
             if tf_version < (2,9,0):
                 kwargs.pop("interpolation_order")
         super().__init__(**kwargs)
 
     def transfer_parameters(self, source, destination):
         destination['flip_vertical'] = source.get('flip_vertical', False)
         destination['flip_horizontal'] = source.get('flip_horizontal', False)
```

### Comparing `dataset_iterator-0.4.0/dataset_iterator/index_array_iterator.py` & `dataset_iterator-0.4.1/dataset_iterator/index_array_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.4.1/dataset_iterator/multichannel_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/pre_processing.py` & `dataset_iterator-0.4.1/dataset_iterator/pre_processing.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/tile_utils.py` & `dataset_iterator-0.4.1/dataset_iterator/tile_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,42 @@
 import numpy as np
 from numpy.random import randint, random
 from .utils import ensure_multiplicity, is_null
 from scipy.ndimage import zoom
 
 OVERLAP_MODE = ["NO_OVERLAP", "ALLOW", "FORCE"]
 
+
+def extract_single_tile(tensor_slice=None, tile_shape=None, contraction_factor=None, return_none_for_identity:bool=True):
+    if tensor_slice is not None:
+        def extract_tiles_fun(batch, is_mask: bool, allow_random: bool = False):
+            if isinstance(batch, (list, tuple)):
+                return [b[tensor_slice] for b in batch]
+            else:
+                return batch[tensor_slice]
+    elif tile_shape is not None: # fixed patch shape
+        def extract_tiles_fun(batch, is_mask: bool, allow_random: bool = False):
+            if isinstance(batch, (list, tuple)):
+                return [crop(b, tile_shape) for b in batch]
+            else:
+                return crop(batch, tile_shape)
+    elif contraction_factor is not None: # honor contraction factor
+        assert contraction_factor is not None, "either tensor_slice, tile_shape or contraction factor must be provided"
+        def extract_tiles_fun(batch, is_mask:bool, allow_random:bool=False):
+            if isinstance(batch, (list, tuple)):
+                return [crop_to_contraction(b, contraction_factor) for b in batch]
+            else:
+                return crop_to_contraction(batch, contraction_factor)
+    else: # identity
+        if return_none_for_identity:
+            return None
+        def extract_tiles_fun(batch, is_mask: bool, allow_random: bool = False):
+            return batch
+    return extract_tiles_fun
+
 def extract_tile_function(tile_shape, perform_augmentation=True, overlap_mode=OVERLAP_MODE[1], min_overlap=1, n_tiles=None, random_stride=False, augmentation_rotate=True):
     def func(batch, is_mask:bool, allow_random:bool=True):
         tiles = extract_tiles(batch, tile_shape=tile_shape, overlap_mode=overlap_mode, min_overlap=min_overlap, n_tiles=n_tiles, random_stride=random_stride if allow_random else False, return_coords=False)
         if perform_augmentation and allow_random:
             tiles = augment_tiles_inplace(tiles, rotate=augmentation_rotate and all([s==tile_shape[0] for s in tile_shape]), n_dims=len(tile_shape))
         return tiles
     return func
@@ -353,7 +381,33 @@
                     tiles[bidx][b] = aug_fun[aug[b]](tiles[bidx][b])
     else:
         for b in range(n_tiles):
             if aug[b]>0: # 0 is identity
                 tiles[b] = aug_fun[aug[b]](tiles[b])
     return tiles
 
+def crop_to_contraction(batch, contraction_factor):
+    if len(batch.shape) == 4:
+        contraction_factor = ensure_multiplicity(2, contraction_factor)
+        _, Y, X, _ = batch.shape
+        newY = contraction_factor[0] * int(Y / contraction_factor[0])
+        newX = contraction_factor[1] * int(X / contraction_factor[1])
+        return batch if newY==Y and newX==X else batch[:, :newY, :newX]
+    elif len(batch.shape) == 5:
+        contraction_factor = ensure_multiplicity(3, contraction_factor)
+        _, Z, Y, X, _ = batch.shape
+        newZ = contraction_factor[0] * int(Z / contraction_factor[0])
+        newY = contraction_factor[1] * int(Y / contraction_factor[1])
+        newX = contraction_factor[2] * int(X / contraction_factor[2])
+        return batch if newZ == Z and newY == Y and newX == X else batch[:, :newZ, newY, :newX]
+
+def crop(batch, target_shape=None):
+    if len(batch.shape) == 4:
+        target_shape = ensure_multiplicity(2, target_shape)
+        _, Y, X, _ = batch.shape
+        assert target_shape[0] <= Y and target_shape[1] <= X, "target shape is larger than tensor to crop"
+        return batch if target_shape[0]==Y and target_shape[1]==X else batch[:, :target_shape[0], :target_shape[1]]
+    elif len(batch.shape) == 5:
+        target_shape = ensure_multiplicity(3, target_shape)
+        _, Z, Y, X, _ = batch.shape
+        assert target_shape[0] <= Z and target_shape[1] <= Y and target_shape[0] <= X, "target shape is larger than tensor to crop"
+        return batch if target_shape[0] == Z and target_shape[1] == Y and target_shape[2] == X else batch[:, :target_shape[0], :target_shape[1], :target_shape[2]]
```

### Comparing `dataset_iterator-0.4.0/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.4.1/dataset_iterator/tracking_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.0/dataset_iterator/utils.py` & `dataset_iterator-0.4.1/dataset_iterator/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import tensorflow as tf
 import numpy as np
 from math import ceil
 
+def get_tf_version():
+    return tuple(map(int, (tf.__version__.split("."))))
+
 def replace_last(s, old, new):
     # return (s[::-1].replace(old[::-1], new[::-1], 1))[::-1]
     return new.join(s.rsplit(old, 1))
 
 def remove_duplicates(seq):
     seen = set()
     seen_add = seen.add
```

### Comparing `dataset_iterator-0.4.0/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.4.1/dataset_iterator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.0/dataset_iterator-0.4.0.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.1/dataset_iterator-0.4.1.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.0/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.4.1/dataset_iterator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 dataset_iterator/__init__.py
 dataset_iterator/concat_iterator.py
 dataset_iterator/hard_sample_mining.py
 dataset_iterator/helpers.py
 dataset_iterator/image_data_generator.py
 dataset_iterator/index_array_iterator.py
 dataset_iterator/multichannel_iterator.py
+dataset_iterator/ordered_enqueuer_cf.py
 dataset_iterator/pre_processing.py
 dataset_iterator/tile_utils.py
 dataset_iterator/tracking_iterator.py
 dataset_iterator/utils.py
 dataset_iterator.egg-info/PKG-INFO
 dataset_iterator.egg-info/SOURCES.txt
 dataset_iterator.egg-info/dependency_links.txt
```

### Comparing `dataset_iterator-0.4.0/setup.py` & `dataset_iterator-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.4.0",
+    version="0.4.1",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.0/dataset_iterator-0.4.0.tar.gz',
+    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.1/dataset_iterator-0.4.1.tar.gz',
     keywords=['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

