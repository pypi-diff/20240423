# Comparing `tmp/keras_generators-1.4.0-py3-none-any.whl.zip` & `tmp/keras_generators-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 28299 bytes, number of entries: 16
+Zip file size: 29156 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 examples/__init__.py
 -rw-rw-rw-  2.0 fat     6233 b- defN 23-Apr-13 14:38 examples/predict_stock_price.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/__init__.py
--rw-rw-rw-  2.0 fat     7068 b- defN 23-Mar-08 16:27 keras_generators/callbacks.py
--rw-rw-rw-  2.0 fat      520 b- defN 23-Apr-13 14:20 keras_generators/common.py
+-rw-rw-rw-  2.0 fat     4313 b- defN 24-Apr-22 22:07 keras_generators/callbacks.py
+-rw-rw-rw-  2.0 fat      803 b- defN 24-Apr-22 16:08 keras_generators/common.py
 -rw-rw-rw-  2.0 fat    10842 b- defN 23-Mar-08 16:27 keras_generators/encoders.py
--rw-rw-rw-  2.0 fat    36106 b- defN 24-Apr-16 20:19 keras_generators/generators.py
+-rw-rw-rw-  2.0 fat    36073 b- defN 24-Apr-22 16:04 keras_generators/generators.py
 -rw-rw-rw-  2.0 fat     4139 b- defN 23-Mar-08 19:39 keras_generators/splitters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/model_abstractions/__init__.py
 -rw-rw-rw-  2.0 fat     8063 b- defN 23-Dec-01 13:36 keras_generators/model_abstractions/model_object.py
--rw-rw-rw-  2.0 fat     3263 b- defN 24-Apr-16 20:19 keras_generators/model_abstractions/model_params.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9821 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1421 b- defN 24-Apr-16 20:27 keras_generators-1.4.0.dist-info/RECORD
-16 files, 99152 bytes uncompressed, 25913 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat     3263 b- defN 24-Apr-22 14:58 keras_generators/model_abstractions/model_params.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-22 22:08 keras_generators-1.4.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13529 b- defN 24-Apr-22 22:08 keras_generators-1.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 22:08 keras_generators-1.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-22 22:08 keras_generators-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1422 b- defN 24-Apr-22 22:08 keras_generators-1.4.1.dist-info/RECORD
+16 files, 100356 bytes uncompressed, 26770 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: keras_generators/model_abstractions/model_object.py
 Comment: 
 
 Filename: keras_generators/model_abstractions/model_params.py
 Comment: 
 
-Filename: keras_generators-1.4.0.dist-info/LICENSE
+Filename: keras_generators-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: keras_generators-1.4.0.dist-info/METADATA
+Filename: keras_generators-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: keras_generators-1.4.0.dist-info/WHEEL
+Filename: keras_generators-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: keras_generators-1.4.0.dist-info/top_level.txt
+Filename: keras_generators-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: keras_generators-1.4.0.dist-info/RECORD
+Filename: keras_generators-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keras_generators/callbacks.py

```diff
@@ -1,21 +1,22 @@
 import json
 import logging
 import math
-import pickle
 from json import JSONEncoder
 from pathlib import Path
 from typing import Optional
 
 import numpy as np
-from keras.callbacks import Callback, ReduceLROnPlateau, CSVLogger, TensorBoard
 from tensorflow.python.util.tf_export import keras_export
+from tf_keras.callbacks import Callback, CSVLogger, ReduceLROnPlateau, TensorBoard
 
+from keras_generators.common import SerializableKerasObject
 
-class EarlyStoppingAtMinLoss(Callback):
+
+class EarlyStoppingAtMinLoss(Callback, SerializableKerasObject):
     """Stop training when the loss is at its min, i.e. the loss stops decreasing.
 
     Arguments:
         patience: Number of epochs to wait after min has been hit. After this
         number of no improvement, training stops.
     """
 
@@ -41,31 +42,27 @@
         self.stopped_epoch = 0
         # Initialize the best as infinity.
         self.best = np.Inf
 
     def _stop_train(self, epoch, message: str = ""):
         self.stopped_epoch = epoch
         self.model.stop_training = True
-        logging.info(
-            "Restoring model weights from the end of the best epoch. %s", message
-        )
+        logging.info("Restoring model weights from the end of the best epoch. %s", message)
         logging.warning(message)
         if self.best_weights is not None:
             self.model.set_weights(self.best_weights)
 
     def on_epoch_end(self, epoch, logs=None):
         current = logs.get(self.monitor)
         train_loss = logs.get("loss")
         if current is None:
             print(f"No val_loss yet: {logs!s}")
             return
         if current - train_loss > self.loss_max_diff:
-            self._stop_train(
-                epoch, f"Stopping because loss difference {current - train_loss}"
-            )
+            self._stop_train(epoch, f"Stopping because loss difference {current - train_loss}")
         if math.isnan(current):
             self._stop_train(epoch)
         if np.less(current, self.best):
             # Record the best weights if current results is better (less).
             self._improved()
         if np.less(current, self.best - self.min_delta):
             self.best = current
@@ -76,129 +73,53 @@
                 self._stop_train(epoch)
 
     def _improved(self):
         self.best_weights = self.model.get_weights()
 
     def on_train_end(self, *_a, **_k):
         if self.stopped_epoch > 0:
-            print("Epoch %05d: early stopping" % (self.stopped_epoch + 1))
+            logging.warning("Epoch %05d: early stopping", self.stopped_epoch + 1)
 
 
-class MetricCheckpoint(Callback):
+class MetricCheckpoint(Callback, SerializableKerasObject):
     FNAME = "metrics.jsonl"
 
     def on_train_begin(self, *_args, **_kwargs):
-        self._f = open(
-            self._dir / self.FNAME, "at"
-        )  # pylint: disable=consider-using-with
+        self._f = open(self._dir / self.FNAME, "at", encoding="utf-8")  # pylint: disable=consider-using-with
 
     def __init__(self, model_dir: Path):
         super().__init__()
         self._f = None
         self._dir: Path = model_dir
         self._je = JSONEncoder()
 
     def to_json_obj(self, obj):
         try:
             self._je.encode(obj)
         except TypeError:
             return float(obj)
-        else:
-            return obj
+        return obj
 
     def on_epoch_end(self, epoch, logs=None):
         if logs is not None:
             log = {k: self.to_json_obj(v) for k, v in logs.items()}
             log["_epoch"] = epoch
             self._f.write(json.dumps(log) + "\n")
             self._f.flush()
 
     def on_train_end(self, *_args, **_kwargs):
         self._f.close()
 
 
 @keras_export("keras.callbacks.SerializableReduceLROnPlateau")
-class SerializableReduceLROnPlateau(ReduceLROnPlateau):
-    def serialize(self) -> bytes:
-        kwargs = {
-            "monitor": self.monitor,
-            "factor": self.factor,
-            "patience": self.patience,
-            "verbose": self.verbose,
-            "mode": self.mode,
-            "min_delta": self.min_delta,
-            "cooldown": self.cooldown,
-            "min_lr": self.min_lr,
-        }
-        state_attrs = {
-            "_chief_worker_only": self._chief_worker_only,
-            "_keras_api_names": self._keras_api_names,
-            "_keras_api_names_v1": self._keras_api_names_v1,
-            "_supports_tf_logs": self._supports_tf_logs,
-            "wait": self.wait,
-            "cooldown_counter": self.cooldown_counter,
-            "best": self.best,
-            "params": self.params,
-            "validation_data": self.validation_data,
-        }
-
-        return pickle.dumps((kwargs, state_attrs))
-
-    @classmethod
-    def deserialize(cls, buffer: bytes) -> "SerializableReduceLROnPlateau":
-        kwargs, state_attrs = pickle.loads(buffer)
-        instance = cls(**kwargs)
-        for attr, val in state_attrs.items():
-            setattr(instance, attr, val)
-        return instance
+class SerializableKerasReduceLROnPlateau(ReduceLROnPlateau, SerializableKerasObject):
+    pass
 
 
 @keras_export("keras.callbacks.SerializableTensorBoard")
-class SerializableTensorBoard(TensorBoard):
-    def serialize(self) -> bytes:
-        kwargs = {
-            "log_dir": self.log_dir,
-            "histogram_freq": self.histogram_freq,
-            "write_graph": self.write_graph,
-            "write_images": self.write_images,
-            "update_freq": self.update_freq,
-            "embeddings_freq": self.embeddings_freq,
-            "embeddings_metadata": self.embeddings_metadata,
-        }
-
-        all_state_attrs = self.__dict__.copy()
-        excepted_attrs = set(kwargs.keys()) | {"_writers", "model"}
-        for attr in excepted_attrs:
-            del all_state_attrs[attr]
-
-        return pickle.dumps((kwargs, all_state_attrs))
-
-    @classmethod
-    def deserialize(cls, buffer: bytes) -> "SerializableTensorBoard":
-        kwargs, state_attrs = pickle.loads(buffer)
-        instance = cls(**kwargs)
-        for attr, val in state_attrs.items():
-            setattr(instance, attr, val)
-        return instance
+class SerializableKerasTensorBoard(TensorBoard, SerializableKerasObject):
+    pass
 
 
 @keras_export("keras.callbacks.SerializableCSVLogger")
-class SerializableCSVLogger(CSVLogger):
-    def serialize(self) -> bytes:
-        kwargs = {"filename": self.filename}
-
-        all_state_attrs = self.__dict__.copy()
-        # writer and csv_file are layzily initialized by object
-        # model is set before training, AFAIK
-        excepted_attrs = set(kwargs.keys()) | {"model", "writer", "csv_file"}
-        for attr in excepted_attrs:
-            del all_state_attrs[attr]
-
-        return pickle.dumps((kwargs, all_state_attrs))
-
-    @classmethod
-    def deserialize(cls, buffer: bytes) -> "SerializableCSVLogger":
-        kwargs, state_attrs = pickle.loads(buffer)
-        instance = cls(**kwargs)
-        for attr, val in state_attrs.items():
-            setattr(instance, attr, val)
-        return instance
+class SerializableKerasCSVLogger(CSVLogger, SerializableKerasObject):
+    pass
```

## keras_generators/common.py

```diff
@@ -1,24 +1,35 @@
 #!/usr/bin/env python
 # Author: ASU --<andrei.suiu@gmail.com>
 
 from json import JSONEncoder
 
+import cloudpickle
 import numpy as np
 from pydantic import Extra
 
 
 class NumpyArrayEncoder(JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, np.ndarray):
-            return obj.tolist()
-        return JSONEncoder.default(self, obj)
+    def default(self, o):
+        if isinstance(o, np.ndarray):
+            return o.tolist()
+        return JSONEncoder.default(self, o)
 
 
 class ImmutableConfig:
     allow_mutation = False
     arbitrary_types_allowed = True
     extra = Extra.forbid
 
 
 class ArbitraryTypes:
     arbitrary_types_allowed = True
+
+
+class SerializableKerasObject:
+    def serialize(self) -> bytes:
+        pickled = cloudpickle.dumps(self)
+        return pickled
+
+    @classmethod
+    def deserialize(cls, buffer: bytes) -> "SerializableKerasObject":
+        return cloudpickle.loads(buffer)
```

## keras_generators/generators.py

```diff
@@ -6,17 +6,17 @@
 import json
 import math
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Collection, Dict, ForwardRef, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
+import tf_keras
 from pydantic import PositiveInt, conint, validate_arguments
 from pydantic.dataclasses import dataclass
-from tensorflow.python.keras.utils import data_utils
 
 from .common import ArbitraryTypes, ImmutableConfig, NumpyArrayEncoder
 from .encoders import ChainedDataEncoder, CompoundDataEncoder, DataEncoder
 from .splitters import OrderedSplitter, TrainValTestSpliter
 
 
 class DataSource(ABC):
@@ -636,15 +636,15 @@
 
     def get_encoders(self) -> Dict[str, List[DataEncoder]]:
         both_sources = (self.input_sources, self.target_sources)
         all_encoders = {name: source.get_encoders() for sources in both_sources for name, source in sources.items()}
         return all_encoders
 
 
-class XBatchGenerator(data_utils.Sequence):
+class XBatchGenerator(tf_keras.utils.Sequence):
     @validate_arguments(config=ArbitraryTypes)
     def __init__(self, inputs_map: Dict[str, DataSource], batch_size: PositiveInt = 128):
         self.inputs = inputs_map
         first_ds = inputs_map[list(inputs_map.keys())[0]]
         self.n_instances = len(first_ds)
         self.n_batches = math.ceil(self.n_instances / batch_size)
         for k, input_seq in inputs_map.items():
```

## Comparing `keras_generators-1.4.0.dist-info/LICENSE` & `keras_generators-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keras_generators-1.4.0.dist-info/RECORD` & `keras_generators-1.4.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 examples/predict_stock_price.py,sha256=OLhlvKkctYf12kGk7QgxSWKVWM61EI6r0NzXwSKOuAY,6233
 keras_generators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-keras_generators/callbacks.py,sha256=fGCSRg13d7oPutoXVnSA2R72ri9kGcZnj47LdNCCcvs,7068
-keras_generators/common.py,sha256=sFcCpVV8dJBrWG3Ry9MhpNZC0l-MZAMBdUBJNwlZYs4,520
+keras_generators/callbacks.py,sha256=Y2Ddnl2RIoHOBpdoTfyfgea-IvdeTdl9EJ0Vi0Z95so,4313
+keras_generators/common.py,sha256=dD1g27em-9aBGpjxlepTLN7rLxBDytXnVB-n1UrnOQw,803
 keras_generators/encoders.py,sha256=WwviJAdT_mYwjSIn9wqzt3-DEjLNl7jbliKC2jjlYik,10842
-keras_generators/generators.py,sha256=DGdpqFQ5DngMqGWLRzE4UBrfriQnF7_qHF4aZ9YG14E,36106
+keras_generators/generators.py,sha256=ZZXh0c4RPzKui0n-VVvvJQesmhc4ZRu3KIo_MqK0NMU,36073
 keras_generators/splitters.py,sha256=O7AKehcoPiQNjv1kuZWOoax-yvnjTFPuOkwLjox-qMw,4139
 keras_generators/model_abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keras_generators/model_abstractions/model_object.py,sha256=TkkAcMJQ6S9Onzueret5xNwMZN0eLqqtocbpZEkUZxs,8063
 keras_generators/model_abstractions/model_params.py,sha256=114iJ1gi15XEUhhU5vZnBgvfL1GY2ozhEsIiXf7rwTE,3263
-keras_generators-1.4.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-keras_generators-1.4.0.dist-info/METADATA,sha256=Fx1195gHaQBTtfL-czLzltBMITN4opxGXNDEG5g_LwA,9821
-keras_generators-1.4.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-keras_generators-1.4.0.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
-keras_generators-1.4.0.dist-info/RECORD,,
+keras_generators-1.4.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+keras_generators-1.4.1.dist-info/METADATA,sha256=Jehl7hzT1gIi6ZR4IFjqK6Vs4byoAzmWnI9eKb8sM6E,13529
+keras_generators-1.4.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+keras_generators-1.4.1.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
+keras_generators-1.4.1.dist-info/RECORD,,
```

